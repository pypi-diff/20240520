# Comparing `tmp/authentik_client-2024.4.2.post1715271061.tar.gz` & `tmp/authentik_client-2024.4.2.post1716209289.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authentik_client-2024.4.2.post1715271061.tar", max compression
+gzip compressed data, was "authentik_client-2024.4.2.post1716209289.tar", max compression
```

## Comparing `authentik_client-2024.4.2.post1715271061.tar` & `authentik_client-2024.4.2.post1716209289.tar`

### file list

```diff
@@ -1,628 +1,628 @@
--rw-r--r--   0        0        0   157746 2024-05-09 16:11:14.194467 authentik_client-2024.4.2.post1715271061/README.md
--rw-r--r--   0        0        0    52131 2024-05-09 16:11:14.202468 authentik_client-2024.4.2.post1715271061/authentik_client/__init__.py
--rw-r--r--   0        0        0     1170 2024-05-09 16:11:14.206468 authentik_client-2024.4.2.post1715271061/authentik_client/api/__init__.py
--rw-r--r--   0        0        0    97518 2024-05-09 16:11:13.930465 authentik_client-2024.4.2.post1715271061/authentik_client/api/admin_api.py
--rw-r--r--   0        0        0   700271 2024-05-09 16:11:13.946465 authentik_client-2024.4.2.post1715271061/authentik_client/api/authenticators_api.py
--rw-r--r--   0        0        0   701197 2024-05-09 16:11:13.970465 authentik_client-2024.4.2.post1715271061/authentik_client/api/core_api.py
--rw-r--r--   0        0        0   116805 2024-05-09 16:11:13.982465 authentik_client-2024.4.2.post1715271061/authentik_client/api/crypto_api.py
--rw-r--r--   0        0        0   107946 2024-05-09 16:11:13.990465 authentik_client-2024.4.2.post1715271061/authentik_client/api/enterprise_api.py
--rw-r--r--   0        0        0   408008 2024-05-09 16:11:14.002466 authentik_client-2024.4.2.post1715271061/authentik_client/api/events_api.py
--rw-r--r--   0        0        0   280806 2024-05-09 16:11:14.010466 authentik_client-2024.4.2.post1715271061/authentik_client/api/flows_api.py
--rw-r--r--   0        0        0   101134 2024-05-09 16:11:14.018466 authentik_client-2024.4.2.post1715271061/authentik_client/api/managed_api.py
--rw-r--r--   0        0        0   135649 2024-05-09 16:11:14.026466 authentik_client-2024.4.2.post1715271061/authentik_client/api/oauth2_api.py
--rw-r--r--   0        0        0   413301 2024-05-09 16:11:14.038466 authentik_client-2024.4.2.post1715271061/authentik_client/api/outposts_api.py
--rw-r--r--   0        0        0   725201 2024-05-09 16:11:14.054466 authentik_client-2024.4.2.post1715271061/authentik_client/api/policies_api.py
--rw-r--r--   0        0        0   721674 2024-05-09 16:11:14.070466 authentik_client-2024.4.2.post1715271061/authentik_client/api/propertymappings_api.py
--rw-r--r--   0        0        0  1235079 2024-05-09 16:11:14.090467 authentik_client-2024.4.2.post1715271061/authentik_client/api/providers_api.py
--rw-r--r--   0        0        0   150485 2024-05-09 16:11:14.106467 authentik_client-2024.4.2.post1715271061/authentik_client/api/rac_api.py
--rw-r--r--   0        0        0   207550 2024-05-09 16:11:14.114467 authentik_client-2024.4.2.post1715271061/authentik_client/api/rbac_api.py
--rw-r--r--   0        0        0    10391 2024-05-09 16:11:14.118467 authentik_client-2024.4.2.post1715271061/authentik_client/api/root_api.py
--rw-r--r--   0        0        0    11845 2024-05-09 16:11:14.122467 authentik_client-2024.4.2.post1715271061/authentik_client/api/schema_api.py
--rw-r--r--   0        0        0  1037196 2024-05-09 16:11:14.138467 authentik_client-2024.4.2.post1715271061/authentik_client/api/sources_api.py
--rw-r--r--   0        0        0  1945986 2024-05-09 16:11:14.166467 authentik_client-2024.4.2.post1715271061/authentik_client/api/stages_api.py
--rw-r--r--   0        0        0   157909 2024-05-09 16:11:14.182467 authentik_client-2024.4.2.post1715271061/authentik_client/api/tenants_api.py
--rw-r--r--   0        0        0    25779 2024-05-09 16:11:14.206468 authentik_client-2024.4.2.post1715271061/authentik_client/api_client.py
--rw-r--r--   0        0        0      652 2024-05-09 16:11:14.206468 authentik_client-2024.4.2.post1715271061/authentik_client/api_response.py
--rw-r--r--   0        0        0    14724 2024-05-09 16:11:14.202468 authentik_client-2024.4.2.post1715271061/authentik_client/configuration.py
--rw-r--r--   0        0        0     5934 2024-05-09 16:11:14.206468 authentik_client-2024.4.2.post1715271061/authentik_client/exceptions.py
--rw-r--r--   0        0        0    50433 2024-05-09 16:11:14.202468 authentik_client-2024.4.2.post1715271061/authentik_client/models/__init__.py
--rw-r--r--   0        0        0     4513 2024-05-09 16:11:11.114437 authentik_client-2024.4.2.post1715271061/authentik_client/models/access_denied_challenge.py
--rw-r--r--   0        0        0      688 2024-05-09 16:11:11.126438 authentik_client-2024.4.2.post1715271061/authentik_client/models/alg_enum.py
--rw-r--r--   0        0        0     2482 2024-05-09 16:11:11.134437 authentik_client-2024.4.2.post1715271061/authentik_client/models/app.py
--rw-r--r--   0        0        0     4460 2024-05-09 16:11:11.142438 authentik_client-2024.4.2.post1715271061/authentik_client/models/app_enum.py
--rw-r--r--   0        0        0     2702 2024-05-09 16:11:11.150438 authentik_client-2024.4.2.post1715271061/authentik_client/models/apple_challenge_response_request.py
--rw-r--r--   0        0        0     4508 2024-05-09 16:11:11.162438 authentik_client-2024.4.2.post1715271061/authentik_client/models/apple_login_challenge.py
--rw-r--r--   0        0        0     6686 2024-05-09 16:11:11.174438 authentik_client-2024.4.2.post1715271061/authentik_client/models/application.py
--rw-r--r--   0        0        0     4473 2024-05-09 16:11:11.186438 authentik_client-2024.4.2.post1715271061/authentik_client/models/application_request.py
--rw-r--r--   0        0        0      711 2024-05-09 16:11:11.190438 authentik_client-2024.4.2.post1715271061/authentik_client/models/auth_mode_enum.py
--rw-r--r--   0        0        0      709 2024-05-09 16:11:11.194438 authentik_client-2024.4.2.post1715271061/authentik_client/models/auth_type_enum.py
--rw-r--r--   0        0        0     5195 2024-05-09 16:11:11.198438 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticated_session.py
--rw-r--r--   0        0        0     3064 2024-05-09 16:11:11.206438 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticated_session_asn.py
--rw-r--r--   0        0        0     2826 2024-05-09 16:11:11.214438 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticated_session_geo_ip.py
--rw-r--r--   0        0        0     3865 2024-05-09 16:11:11.218438 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticated_session_user_agent.py
--rw-r--r--   0        0        0     2646 2024-05-09 16:11:11.226438 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticated_session_user_agent_device.py
--rw-r--r--   0        0        0     2792 2024-05-09 16:11:11.230438 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticated_session_user_agent_os.py
--rw-r--r--   0        0        0     2725 2024-05-09 16:11:11.238438 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticated_session_user_agent_user_agent.py
--rw-r--r--   0        0        0      895 2024-05-09 16:11:11.242439 authentik_client-2024.4.2.post1715271061/authentik_client/models/authentication_enum.py
--rw-r--r--   0        0        0      782 2024-05-09 16:11:11.242439 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_attachment_enum.py
--rw-r--r--   0        0        0     4686 2024-05-09 16:11:11.250439 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_duo_challenge.py
--rw-r--r--   0        0        0     2743 2024-05-09 16:11:11.258439 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_duo_challenge_response_request.py
--rw-r--r--   0        0        0     5327 2024-05-09 16:11:11.266439 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_duo_stage.py
--rw-r--r--   0        0        0     2768 2024-05-09 16:11:11.270439 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_duo_stage_device_import_response.py
--rw-r--r--   0        0        0     2785 2024-05-09 16:11:11.278439 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py
--rw-r--r--   0        0        0     4744 2024-05-09 16:11:11.282439 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_duo_stage_request.py
--rw-r--r--   0        0        0     4594 2024-05-09 16:11:11.290439 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_sms_challenge.py
--rw-r--r--   0        0        0     3022 2024-05-09 16:11:11.294439 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_sms_challenge_response_request.py
--rw-r--r--   0        0        0     6409 2024-05-09 16:11:11.298439 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_sms_stage.py
--rw-r--r--   0        0        0     5595 2024-05-09 16:11:11.306439 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_sms_stage_request.py
--rw-r--r--   0        0        0     4474 2024-05-09 16:11:11.310439 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_static_challenge.py
--rw-r--r--   0        0        0     2761 2024-05-09 16:11:11.314439 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_static_challenge_response_request.py
--rw-r--r--   0        0        0     5363 2024-05-09 16:11:11.322439 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_static_stage.py
--rw-r--r--   0        0        0     4392 2024-05-09 16:11:11.326439 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_static_stage_request.py
--rw-r--r--   0        0        0     4468 2024-05-09 16:11:11.334439 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_totp_challenge.py
--rw-r--r--   0        0        0     2858 2024-05-09 16:11:11.338440 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_totp_challenge_response_request.py
--rw-r--r--   0        0        0     5132 2024-05-09 16:11:11.346439 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_totp_stage.py
--rw-r--r--   0        0        0     4201 2024-05-09 16:11:11.354440 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_totp_stage_request.py
--rw-r--r--   0        0        0     6722 2024-05-09 16:11:11.358440 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_validate_stage.py
--rw-r--r--   0        0        0     4893 2024-05-09 16:11:11.362440 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_validate_stage_request.py
--rw-r--r--   0        0        0     5717 2024-05-09 16:11:11.370440 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_validation_challenge.py
--rw-r--r--   0        0        0     3805 2024-05-09 16:11:11.378440 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_validation_challenge_response_request.py
--rw-r--r--   0        0        0     4499 2024-05-09 16:11:11.386440 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_web_authn_challenge.py
--rw-r--r--   0        0        0     2852 2024-05-09 16:11:11.390440 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_web_authn_challenge_response_request.py
--rw-r--r--   0        0        0     7081 2024-05-09 16:11:11.398440 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_web_authn_stage.py
--rw-r--r--   0        0        0     5302 2024-05-09 16:11:11.402440 authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_web_authn_stage_request.py
--rw-r--r--   0        0        0     2718 2024-05-09 16:11:11.406440 authentik_client-2024.4.2.post1715271061/authentik_client/models/auto_submit_challenge_response_request.py
--rw-r--r--   0        0        0     4388 2024-05-09 16:11:11.410440 authentik_client-2024.4.2.post1715271061/authentik_client/models/autosubmit_challenge.py
--rw-r--r--   0        0        0      950 2024-05-09 16:11:11.414440 authentik_client-2024.4.2.post1715271061/authentik_client/models/backends_enum.py
--rw-r--r--   0        0        0      748 2024-05-09 16:11:11.414440 authentik_client-2024.4.2.post1715271061/authentik_client/models/binding_type_enum.py
--rw-r--r--   0        0        0     2995 2024-05-09 16:11:11.418440 authentik_client-2024.4.2.post1715271061/authentik_client/models/blueprint_file.py
--rw-r--r--   0        0        0     4453 2024-05-09 16:11:11.422440 authentik_client-2024.4.2.post1715271061/authentik_client/models/blueprint_instance.py
--rw-r--r--   0        0        0     3208 2024-05-09 16:11:11.426440 authentik_client-2024.4.2.post1715271061/authentik_client/models/blueprint_instance_request.py
--rw-r--r--   0        0        0      836 2024-05-09 16:11:11.430440 authentik_client-2024.4.2.post1715271061/authentik_client/models/blueprint_instance_status_enum.py
--rw-r--r--   0        0        0     6255 2024-05-09 16:11:11.434440 authentik_client-2024.4.2.post1715271061/authentik_client/models/brand.py
--rw-r--r--   0        0        0     6307 2024-05-09 16:11:11.438440 authentik_client-2024.4.2.post1715271061/authentik_client/models/brand_request.py
--rw-r--r--   0        0        0     2501 2024-05-09 16:11:11.442441 authentik_client-2024.4.2.post1715271061/authentik_client/models/cache.py
--rw-r--r--   0        0        0      875 2024-05-09 16:11:11.442441 authentik_client-2024.4.2.post1715271061/authentik_client/models/capabilities_enum.py
--rw-r--r--   0        0        0     4476 2024-05-09 16:11:11.450441 authentik_client-2024.4.2.post1715271061/authentik_client/models/captcha_challenge.py
--rw-r--r--   0        0        0     2797 2024-05-09 16:11:11.450441 authentik_client-2024.4.2.post1715271061/authentik_client/models/captcha_challenge_response_request.py
--rw-r--r--   0        0        0     4438 2024-05-09 16:11:11.454441 authentik_client-2024.4.2.post1715271061/authentik_client/models/captcha_stage.py
--rw-r--r--   0        0        0     3774 2024-05-09 16:11:11.462441 authentik_client-2024.4.2.post1715271061/authentik_client/models/captcha_stage_request.py
--rw-r--r--   0        0        0     2522 2024-05-09 16:11:11.466441 authentik_client-2024.4.2.post1715271061/authentik_client/models/certificate_data.py
--rw-r--r--   0        0        0     2990 2024-05-09 16:11:11.470441 authentik_client-2024.4.2.post1715271061/authentik_client/models/certificate_generation_request.py
--rw-r--r--   0        0        0     6655 2024-05-09 16:11:11.482441 authentik_client-2024.4.2.post1715271061/authentik_client/models/certificate_key_pair.py
--rw-r--r--   0        0        0     2989 2024-05-09 16:11:11.486441 authentik_client-2024.4.2.post1715271061/authentik_client/models/certificate_key_pair_request.py
--rw-r--r--   0        0        0      747 2024-05-09 16:11:11.490441 authentik_client-2024.4.2.post1715271061/authentik_client/models/challenge_choices.py
--rw-r--r--   0        0        0    24236 2024-05-09 16:11:11.494441 authentik_client-2024.4.2.post1715271061/authentik_client/models/challenge_types.py
--rw-r--r--   0        0        0      729 2024-05-09 16:11:11.498441 authentik_client-2024.4.2.post1715271061/authentik_client/models/client_type_enum.py
--rw-r--r--   0        0        0     3539 2024-05-09 16:11:11.502441 authentik_client-2024.4.2.post1715271061/authentik_client/models/config.py
--rw-r--r--   0        0        0     4021 2024-05-09 16:11:11.506441 authentik_client-2024.4.2.post1715271061/authentik_client/models/connection_token.py
--rw-r--r--   0        0        0     2662 2024-05-09 16:11:11.506441 authentik_client-2024.4.2.post1715271061/authentik_client/models/connection_token_request.py
--rw-r--r--   0        0        0     5736 2024-05-09 16:11:11.514441 authentik_client-2024.4.2.post1715271061/authentik_client/models/consent_challenge.py
--rw-r--r--   0        0        0     2838 2024-05-09 16:11:11.518441 authentik_client-2024.4.2.post1715271061/authentik_client/models/consent_challenge_response_request.py
--rw-r--r--   0        0        0     2513 2024-05-09 16:11:11.522441 authentik_client-2024.4.2.post1715271061/authentik_client/models/consent_permission.py
--rw-r--r--   0        0        0     4511 2024-05-09 16:11:11.526441 authentik_client-2024.4.2.post1715271061/authentik_client/models/consent_stage.py
--rw-r--r--   0        0        0      783 2024-05-09 16:11:11.526441 authentik_client-2024.4.2.post1715271061/authentik_client/models/consent_stage_mode_enum.py
--rw-r--r--   0        0        0     3569 2024-05-09 16:11:11.530441 authentik_client-2024.4.2.post1715271061/authentik_client/models/consent_stage_request.py
--rw-r--r--   0        0        0     2891 2024-05-09 16:11:11.534441 authentik_client-2024.4.2.post1715271061/authentik_client/models/contextual_flow_info.py
--rw-r--r--   0        0        0      879 2024-05-09 16:11:11.538442 authentik_client-2024.4.2.post1715271061/authentik_client/models/contextual_flow_info_layout_enum.py
--rw-r--r--   0        0        0     2657 2024-05-09 16:11:11.542441 authentik_client-2024.4.2.post1715271061/authentik_client/models/coordinate.py
--rw-r--r--   0        0        0     4704 2024-05-09 16:11:11.546442 authentik_client-2024.4.2.post1715271061/authentik_client/models/current_brand.py
--rw-r--r--   0        0        0      771 2024-05-09 16:11:11.546442 authentik_client-2024.4.2.post1715271061/authentik_client/models/denied_action_enum.py
--rw-r--r--   0        0        0     4200 2024-05-09 16:11:11.550442 authentik_client-2024.4.2.post1715271061/authentik_client/models/deny_stage.py
--rw-r--r--   0        0        0     3230 2024-05-09 16:11:11.558442 authentik_client-2024.4.2.post1715271061/authentik_client/models/deny_stage_request.py
--rw-r--r--   0        0        0     3522 2024-05-09 16:11:11.562442 authentik_client-2024.4.2.post1715271061/authentik_client/models/device.py
--rw-r--r--   0        0        0     2657 2024-05-09 16:11:11.566442 authentik_client-2024.4.2.post1715271061/authentik_client/models/device_challenge.py
--rw-r--r--   0        0        0     2792 2024-05-09 16:11:11.570442 authentik_client-2024.4.2.post1715271061/authentik_client/models/device_challenge_request.py
--rw-r--r--   0        0        0      780 2024-05-09 16:11:11.574442 authentik_client-2024.4.2.post1715271061/authentik_client/models/device_classes_enum.py
--rw-r--r--   0        0        0     1244 2024-05-09 16:11:11.578442 authentik_client-2024.4.2.post1715271061/authentik_client/models/digest_algorithm_enum.py
--rw-r--r--   0        0        0      695 2024-05-09 16:11:11.578442 authentik_client-2024.4.2.post1715271061/authentik_client/models/digits_enum.py
--rw-r--r--   0        0        0     4969 2024-05-09 16:11:11.582442 authentik_client-2024.4.2.post1715271061/authentik_client/models/docker_service_connection.py
--rw-r--r--   0        0        0     4087 2024-05-09 16:11:11.586442 authentik_client-2024.4.2.post1715271061/authentik_client/models/docker_service_connection_request.py
--rw-r--r--   0        0        0     2847 2024-05-09 16:11:11.590442 authentik_client-2024.4.2.post1715271061/authentik_client/models/domain.py
--rw-r--r--   0        0        0     2746 2024-05-09 16:11:11.594442 authentik_client-2024.4.2.post1715271061/authentik_client/models/domain_request.py
--rw-r--r--   0        0        0     4155 2024-05-09 16:11:11.598442 authentik_client-2024.4.2.post1715271061/authentik_client/models/dummy_challenge.py
--rw-r--r--   0        0        0     2681 2024-05-09 16:11:11.598442 authentik_client-2024.4.2.post1715271061/authentik_client/models/dummy_challenge_response_request.py
--rw-r--r--   0        0        0     4515 2024-05-09 16:11:11.602442 authentik_client-2024.4.2.post1715271061/authentik_client/models/dummy_policy.py
--rw-r--r--   0        0        0     3237 2024-05-09 16:11:11.606442 authentik_client-2024.4.2.post1715271061/authentik_client/models/dummy_policy_request.py
--rw-r--r--   0        0        0     4213 2024-05-09 16:11:11.610442 authentik_client-2024.4.2.post1715271061/authentik_client/models/dummy_stage.py
--rw-r--r--   0        0        0     3232 2024-05-09 16:11:11.614442 authentik_client-2024.4.2.post1715271061/authentik_client/models/dummy_stage_request.py
--rw-r--r--   0        0        0     2720 2024-05-09 16:11:11.618442 authentik_client-2024.4.2.post1715271061/authentik_client/models/duo_device.py
--rw-r--r--   0        0        0     2575 2024-05-09 16:11:11.622442 authentik_client-2024.4.2.post1715271061/authentik_client/models/duo_device_enrollment_status.py
--rw-r--r--   0        0        0     2619 2024-05-09 16:11:11.622442 authentik_client-2024.4.2.post1715271061/authentik_client/models/duo_device_request.py
--rw-r--r--   0        0        0      748 2024-05-09 16:11:11.626442 authentik_client-2024.4.2.post1715271061/authentik_client/models/duo_response_enum.py
--rw-r--r--   0        0        0     4090 2024-05-09 16:11:11.630442 authentik_client-2024.4.2.post1715271061/authentik_client/models/email_challenge.py
--rw-r--r--   0        0        0     2770 2024-05-09 16:11:11.634442 authentik_client-2024.4.2.post1715271061/authentik_client/models/email_challenge_response_request.py
--rw-r--r--   0        0        0     5902 2024-05-09 16:11:11.638442 authentik_client-2024.4.2.post1715271061/authentik_client/models/email_stage.py
--rw-r--r--   0        0        0     5121 2024-05-09 16:11:11.642443 authentik_client-2024.4.2.post1715271061/authentik_client/models/email_stage_request.py
--rw-r--r--   0        0        0     4707 2024-05-09 16:11:11.650442 authentik_client-2024.4.2.post1715271061/authentik_client/models/endpoint.py
--rw-r--r--   0        0        0     3678 2024-05-09 16:11:11.654443 authentik_client-2024.4.2.post1715271061/authentik_client/models/endpoint_request.py
--rw-r--r--   0        0        0     2530 2024-05-09 16:11:11.658443 authentik_client-2024.4.2.post1715271061/authentik_client/models/error_detail.py
--rw-r--r--   0        0        0     3309 2024-05-09 16:11:11.662443 authentik_client-2024.4.2.post1715271061/authentik_client/models/error_reporting_config.py
--rw-r--r--   0        0        0     4129 2024-05-09 16:11:11.666443 authentik_client-2024.4.2.post1715271061/authentik_client/models/event.py
--rw-r--r--   0        0        0     1730 2024-05-09 16:11:11.666443 authentik_client-2024.4.2.post1715271061/authentik_client/models/event_actions.py
--rw-r--r--   0        0        0     6006 2024-05-09 16:11:11.670443 authentik_client-2024.4.2.post1715271061/authentik_client/models/event_matcher_policy.py
--rw-r--r--   0        0        0     4807 2024-05-09 16:11:11.674443 authentik_client-2024.4.2.post1715271061/authentik_client/models/event_matcher_policy_request.py
--rw-r--r--   0        0        0     3990 2024-05-09 16:11:11.678443 authentik_client-2024.4.2.post1715271061/authentik_client/models/event_request.py
--rw-r--r--   0        0        0     2697 2024-05-09 16:11:11.678443 authentik_client-2024.4.2.post1715271061/authentik_client/models/event_top_per_user.py
--rw-r--r--   0        0        0     3926 2024-05-09 16:11:11.682443 authentik_client-2024.4.2.post1715271061/authentik_client/models/expiring_base_grant_model.py
--rw-r--r--   0        0        0     4191 2024-05-09 16:11:11.686443 authentik_client-2024.4.2.post1715271061/authentik_client/models/expression_policy.py
--rw-r--r--   0        0        0     2992 2024-05-09 16:11:11.690443 authentik_client-2024.4.2.post1715271061/authentik_client/models/expression_policy_request.py
--rw-r--r--   0        0        0     4524 2024-05-09 16:11:11.698443 authentik_client-2024.4.2.post1715271061/authentik_client/models/extra_role_object_permission.py
--rw-r--r--   0        0        0     4524 2024-05-09 16:11:11.702443 authentik_client-2024.4.2.post1715271061/authentik_client/models/extra_user_object_permission.py
--rw-r--r--   0        0        0     2519 2024-05-09 16:11:11.706443 authentik_client-2024.4.2.post1715271061/authentik_client/models/file_path_request.py
--rw-r--r--   0        0        0     6047 2024-05-09 16:11:11.710443 authentik_client-2024.4.2.post1715271061/authentik_client/models/flow.py
--rw-r--r--   0        0        0    25850 2024-05-09 16:11:11.714443 authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_challenge_response_request.py
--rw-r--r--   0        0        0      934 2024-05-09 16:11:11.718443 authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_designation_enum.py
--rw-r--r--   0        0        0     2533 2024-05-09 16:11:11.722443 authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_diagram.py
--rw-r--r--   0        0        0     4505 2024-05-09 16:11:11.726443 authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_error_challenge.py
--rw-r--r--   0        0        0     3111 2024-05-09 16:11:11.730443 authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_import_result.py
--rw-r--r--   0        0        0     3418 2024-05-09 16:11:11.734443 authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_inspection.py
--rw-r--r--   0        0        0     3875 2024-05-09 16:11:11.734443 authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_inspector_plan.py
--rw-r--r--   0        0        0      837 2024-05-09 16:11:11.738443 authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_layout_enum.py
--rw-r--r--   0        0        0     4741 2024-05-09 16:11:11.742443 authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_request.py
--rw-r--r--   0        0        0     5223 2024-05-09 16:11:11.746444 authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_set.py
--rw-r--r--   0        0        0     4459 2024-05-09 16:11:11.750444 authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_set_request.py
--rw-r--r--   0        0        0     4763 2024-05-09 16:11:11.750444 authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_stage_binding.py
--rw-r--r--   0        0        0     3983 2024-05-09 16:11:11.754444 authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_stage_binding_request.py
--rw-r--r--   0        0        0     2641 2024-05-09 16:11:11.758444 authentik_client-2024.4.2.post1715271061/authentik_client/models/footer_link.py
--rw-r--r--   0        0        0     2531 2024-05-09 16:11:11.762444 authentik_client-2024.4.2.post1715271061/authentik_client/models/generic_error.py
--rw-r--r--   0        0        0      865 2024-05-09 16:11:11.762444 authentik_client-2024.4.2.post1715271061/authentik_client/models/geoip_binding_enum.py
--rw-r--r--   0        0        0     6418 2024-05-09 16:11:11.766444 authentik_client-2024.4.2.post1715271061/authentik_client/models/google_workspace_provider.py
--rw-r--r--   0        0        0     3083 2024-05-09 16:11:11.770444 authentik_client-2024.4.2.post1715271061/authentik_client/models/google_workspace_provider_group.py
--rw-r--r--   0        0        0     2526 2024-05-09 16:11:11.774444 authentik_client-2024.4.2.post1715271061/authentik_client/models/google_workspace_provider_group_request.py
--rw-r--r--   0        0        0     4324 2024-05-09 16:11:11.774444 authentik_client-2024.4.2.post1715271061/authentik_client/models/google_workspace_provider_mapping.py
--rw-r--r--   0        0        0     3385 2024-05-09 16:11:11.778444 authentik_client-2024.4.2.post1715271061/authentik_client/models/google_workspace_provider_mapping_request.py
--rw-r--r--   0        0        0     4740 2024-05-09 16:11:11.782444 authentik_client-2024.4.2.post1715271061/authentik_client/models/google_workspace_provider_request.py
--rw-r--r--   0        0        0     3084 2024-05-09 16:11:11.786444 authentik_client-2024.4.2.post1715271061/authentik_client/models/google_workspace_provider_user.py
--rw-r--r--   0        0        0     2518 2024-05-09 16:11:11.790444 authentik_client-2024.4.2.post1715271061/authentik_client/models/google_workspace_provider_user_request.py
--rw-r--r--   0        0        0     5445 2024-05-09 16:11:11.794444 authentik_client-2024.4.2.post1715271061/authentik_client/models/group.py
--rw-r--r--   0        0        0     4209 2024-05-09 16:11:11.798444 authentik_client-2024.4.2.post1715271061/authentik_client/models/group_member.py
--rw-r--r--   0        0        0     4006 2024-05-09 16:11:11.802444 authentik_client-2024.4.2.post1715271061/authentik_client/models/group_member_request.py
--rw-r--r--   0        0        0     3347 2024-05-09 16:11:11.806444 authentik_client-2024.4.2.post1715271061/authentik_client/models/group_request.py
--rw-r--r--   0        0        0     6080 2024-05-09 16:11:11.810444 authentik_client-2024.4.2.post1715271061/authentik_client/models/identification_challenge.py
--rw-r--r--   0        0        0     3174 2024-05-09 16:11:11.810444 authentik_client-2024.4.2.post1715271061/authentik_client/models/identification_challenge_response_request.py
--rw-r--r--   0        0        0     7503 2024-05-09 16:11:11.814444 authentik_client-2024.4.2.post1715271061/authentik_client/models/identification_stage.py
--rw-r--r--   0        0        0     6533 2024-05-09 16:11:11.818444 authentik_client-2024.4.2.post1715271061/authentik_client/models/identification_stage_request.py
--rw-r--r--   0        0        0     2438 2024-05-09 16:11:11.822444 authentik_client-2024.4.2.post1715271061/authentik_client/models/install_id.py
--rw-r--r--   0        0        0      771 2024-05-09 16:11:11.822444 authentik_client-2024.4.2.post1715271061/authentik_client/models/intent_enum.py
--rw-r--r--   0        0        0      800 2024-05-09 16:11:11.830444 authentik_client-2024.4.2.post1715271061/authentik_client/models/invalid_response_action_enum.py
--rw-r--r--   0        0        0     4878 2024-05-09 16:11:11.834444 authentik_client-2024.4.2.post1715271061/authentik_client/models/invitation.py
--rw-r--r--   0        0        0     3895 2024-05-09 16:11:11.838444 authentik_client-2024.4.2.post1715271061/authentik_client/models/invitation_request.py
--rw-r--r--   0        0        0     4508 2024-05-09 16:11:11.842445 authentik_client-2024.4.2.post1715271061/authentik_client/models/invitation_stage.py
--rw-r--r--   0        0        0     3527 2024-05-09 16:11:11.846444 authentik_client-2024.4.2.post1715271061/authentik_client/models/invitation_stage_request.py
--rw-r--r--   0        0        0      729 2024-05-09 16:11:11.850444 authentik_client-2024.4.2.post1715271061/authentik_client/models/issuer_mode_enum.py
--rw-r--r--   0        0        0     4386 2024-05-09 16:11:11.854445 authentik_client-2024.4.2.post1715271061/authentik_client/models/kubernetes_service_connection.py
--rw-r--r--   0        0        0     3454 2024-05-09 16:11:11.858445 authentik_client-2024.4.2.post1715271061/authentik_client/models/kubernetes_service_connection_request.py
--rw-r--r--   0        0        0     2811 2024-05-09 16:11:11.862445 authentik_client-2024.4.2.post1715271061/authentik_client/models/ldap_debug.py
--rw-r--r--   0        0        0     5765 2024-05-09 16:11:11.866445 authentik_client-2024.4.2.post1715271061/authentik_client/models/ldap_outpost_config.py
--rw-r--r--   0        0        0     4378 2024-05-09 16:11:11.870445 authentik_client-2024.4.2.post1715271061/authentik_client/models/ldap_property_mapping.py
--rw-r--r--   0        0        0     3478 2024-05-09 16:11:11.870445 authentik_client-2024.4.2.post1715271061/authentik_client/models/ldap_property_mapping_request.py
--rw-r--r--   0        0        0     8694 2024-05-09 16:11:11.874445 authentik_client-2024.4.2.post1715271061/authentik_client/models/ldap_provider.py
--rw-r--r--   0        0        0     6192 2024-05-09 16:11:11.878445 authentik_client-2024.4.2.post1715271061/authentik_client/models/ldap_provider_request.py
--rw-r--r--   0        0        0    11791 2024-05-09 16:11:11.882445 authentik_client-2024.4.2.post1715271061/authentik_client/models/ldap_source.py
--rw-r--r--   0        0        0     9542 2024-05-09 16:11:11.890445 authentik_client-2024.4.2.post1715271061/authentik_client/models/ldap_source_request.py
--rw-r--r--   0        0        0      726 2024-05-09 16:11:11.858445 authentik_client-2024.4.2.post1715271061/authentik_client/models/ldapapi_access_mode.py
--rw-r--r--   0        0        0     3278 2024-05-09 16:11:11.890445 authentik_client-2024.4.2.post1715271061/authentik_client/models/license.py
--rw-r--r--   0        0        0     2897 2024-05-09 16:11:11.894445 authentik_client-2024.4.2.post1715271061/authentik_client/models/license_forecast.py
--rw-r--r--   0        0        0     2509 2024-05-09 16:11:11.898445 authentik_client-2024.4.2.post1715271061/authentik_client/models/license_request.py
--rw-r--r--   0        0        0     3222 2024-05-09 16:11:11.902445 authentik_client-2024.4.2.post1715271061/authentik_client/models/license_summary.py
--rw-r--r--   0        0        0     2411 2024-05-09 16:11:11.906445 authentik_client-2024.4.2.post1715271061/authentik_client/models/link.py
--rw-r--r--   0        0        0     2882 2024-05-09 16:11:11.906445 authentik_client-2024.4.2.post1715271061/authentik_client/models/log_event.py
--rw-r--r--   0        0        0      843 2024-05-09 16:11:11.910445 authentik_client-2024.4.2.post1715271061/authentik_client/models/log_level_enum.py
--rw-r--r--   0        0        0     6520 2024-05-09 16:11:11.914445 authentik_client-2024.4.2.post1715271061/authentik_client/models/login_challenge_types.py
--rw-r--r--   0        0        0     4171 2024-05-09 16:11:11.918445 authentik_client-2024.4.2.post1715271061/authentik_client/models/login_metrics.py
--rw-r--r--   0        0        0     3192 2024-05-09 16:11:11.922445 authentik_client-2024.4.2.post1715271061/authentik_client/models/login_source.py
--rw-r--r--   0        0        0     2513 2024-05-09 16:11:11.926445 authentik_client-2024.4.2.post1715271061/authentik_client/models/metadata.py
--rw-r--r--   0        0        0     5920 2024-05-09 16:11:11.930445 authentik_client-2024.4.2.post1715271061/authentik_client/models/microsoft_entra_provider.py
--rw-r--r--   0        0        0     3079 2024-05-09 16:11:11.934445 authentik_client-2024.4.2.post1715271061/authentik_client/models/microsoft_entra_provider_group.py
--rw-r--r--   0        0        0     2522 2024-05-09 16:11:11.934445 authentik_client-2024.4.2.post1715271061/authentik_client/models/microsoft_entra_provider_group_request.py
--rw-r--r--   0        0        0     4320 2024-05-09 16:11:11.938445 authentik_client-2024.4.2.post1715271061/authentik_client/models/microsoft_entra_provider_mapping.py
--rw-r--r--   0        0        0     3381 2024-05-09 16:11:11.942445 authentik_client-2024.4.2.post1715271061/authentik_client/models/microsoft_entra_provider_mapping_request.py
--rw-r--r--   0        0        0     4307 2024-05-09 16:11:11.946446 authentik_client-2024.4.2.post1715271061/authentik_client/models/microsoft_entra_provider_request.py
--rw-r--r--   0        0        0     3080 2024-05-09 16:11:11.950446 authentik_client-2024.4.2.post1715271061/authentik_client/models/microsoft_entra_provider_user.py
--rw-r--r--   0        0        0     2514 2024-05-09 16:11:11.954445 authentik_client-2024.4.2.post1715271061/authentik_client/models/microsoft_entra_provider_user_request.py
--rw-r--r--   0        0        0     8160 2024-05-09 16:11:11.954445 authentik_client-2024.4.2.post1715271061/authentik_client/models/model_enum.py
--rw-r--r--   0        0        0    11885 2024-05-09 16:11:11.958446 authentik_client-2024.4.2.post1715271061/authentik_client/models/model_request.py
--rw-r--r--   0        0        0     1559 2024-05-09 16:11:11.962446 authentik_client-2024.4.2.post1715271061/authentik_client/models/name_id_policy_enum.py
--rw-r--r--   0        0        0      831 2024-05-09 16:11:11.962446 authentik_client-2024.4.2.post1715271061/authentik_client/models/network_binding_enum.py
--rw-r--r--   0        0        0      764 2024-05-09 16:11:11.966446 authentik_client-2024.4.2.post1715271061/authentik_client/models/not_configured_action_enum.py
--rw-r--r--   0        0        0     3479 2024-05-09 16:11:11.970446 authentik_client-2024.4.2.post1715271061/authentik_client/models/notification.py
--rw-r--r--   0        0        0     2858 2024-05-09 16:11:11.970446 authentik_client-2024.4.2.post1715271061/authentik_client/models/notification_request.py
--rw-r--r--   0        0        0     4010 2024-05-09 16:11:11.974446 authentik_client-2024.4.2.post1715271061/authentik_client/models/notification_rule.py
--rw-r--r--   0        0        0     3549 2024-05-09 16:11:11.978446 authentik_client-2024.4.2.post1715271061/authentik_client/models/notification_rule_request.py
--rw-r--r--   0        0        0     3760 2024-05-09 16:11:11.982446 authentik_client-2024.4.2.post1715271061/authentik_client/models/notification_transport.py
--rw-r--r--   0        0        0      818 2024-05-09 16:11:11.986446 authentik_client-2024.4.2.post1715271061/authentik_client/models/notification_transport_mode_enum.py
--rw-r--r--   0        0        0     3500 2024-05-09 16:11:11.986446 authentik_client-2024.4.2.post1715271061/authentik_client/models/notification_transport_request.py
--rw-r--r--   0        0        0     2503 2024-05-09 16:11:11.990446 authentik_client-2024.4.2.post1715271061/authentik_client/models/notification_transport_test.py
--rw-r--r--   0        0        0     2707 2024-05-09 16:11:11.994446 authentik_client-2024.4.2.post1715271061/authentik_client/models/notification_webhook_mapping.py
--rw-r--r--   0        0        0     2717 2024-05-09 16:11:11.998446 authentik_client-2024.4.2.post1715271061/authentik_client/models/notification_webhook_mapping_request.py
--rw-r--r--   0        0        0     8888 2024-05-09 16:11:12.002446 authentik_client-2024.4.2.post1715271061/authentik_client/models/o_auth2_provider.py
--rw-r--r--   0        0        0     6654 2024-05-09 16:11:12.006446 authentik_client-2024.4.2.post1715271061/authentik_client/models/o_auth2_provider_request.py
--rw-r--r--   0        0        0     3482 2024-05-09 16:11:12.006446 authentik_client-2024.4.2.post1715271061/authentik_client/models/o_auth2_provider_setup_urls.py
--rw-r--r--   0        0        0     4164 2024-05-09 16:11:12.010446 authentik_client-2024.4.2.post1715271061/authentik_client/models/o_auth_device_code_challenge.py
--rw-r--r--   0        0        0     2846 2024-05-09 16:11:12.014446 authentik_client-2024.4.2.post1715271061/authentik_client/models/o_auth_device_code_challenge_response_request.py
--rw-r--r--   0        0        0     4213 2024-05-09 16:11:12.022446 authentik_client-2024.4.2.post1715271061/authentik_client/models/o_auth_device_code_finish_challenge.py
--rw-r--r--   0        0        0     2816 2024-05-09 16:11:12.022446 authentik_client-2024.4.2.post1715271061/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py
--rw-r--r--   0        0        0    10563 2024-05-09 16:11:12.026446 authentik_client-2024.4.2.post1715271061/authentik_client/models/o_auth_source.py
--rw-r--r--   0        0        0     8013 2024-05-09 16:11:12.030446 authentik_client-2024.4.2.post1715271061/authentik_client/models/o_auth_source_request.py
--rw-r--r--   0        0        0     3922 2024-05-09 16:11:12.034446 authentik_client-2024.4.2.post1715271061/authentik_client/models/open_id_connect_configuration.py
--rw-r--r--   0        0        0      779 2024-05-09 16:11:12.034446 authentik_client-2024.4.2.post1715271061/authentik_client/models/outgoing_sync_delete_action.py
--rw-r--r--   0        0        0     5545 2024-05-09 16:11:12.038446 authentik_client-2024.4.2.post1715271061/authentik_client/models/outpost.py
--rw-r--r--   0        0        0     2541 2024-05-09 16:11:12.042446 authentik_client-2024.4.2.post1715271061/authentik_client/models/outpost_default_config.py
--rw-r--r--   0        0        0     3755 2024-05-09 16:11:12.042446 authentik_client-2024.4.2.post1715271061/authentik_client/models/outpost_health.py
--rw-r--r--   0        0        0     4050 2024-05-09 16:11:12.046446 authentik_client-2024.4.2.post1715271061/authentik_client/models/outpost_request.py
--rw-r--r--   0        0        0      752 2024-05-09 16:11:12.050446 authentik_client-2024.4.2.post1715271061/authentik_client/models/outpost_type_enum.py
--rw-r--r--   0        0        0     3322 2024-05-09 16:11:12.050446 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_application_list.py
--rw-r--r--   0        0        0     3395 2024-05-09 16:11:12.054447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_authenticated_session_list.py
--rw-r--r--   0        0        0     3404 2024-05-09 16:11:12.058447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_authenticator_duo_stage_list.py
--rw-r--r--   0        0        0     3404 2024-05-09 16:11:12.058447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_authenticator_sms_stage_list.py
--rw-r--r--   0        0        0     3428 2024-05-09 16:11:12.062447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_authenticator_static_stage_list.py
--rw-r--r--   0        0        0     3412 2024-05-09 16:11:12.066447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_authenticator_totp_stage_list.py
--rw-r--r--   0        0        0     3444 2024-05-09 16:11:12.066447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_authenticator_validate_stage_list.py
--rw-r--r--   0        0        0     3445 2024-05-09 16:11:12.070447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_authenticator_web_authn_stage_list.py
--rw-r--r--   0        0        0     3371 2024-05-09 16:11:12.074447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_blueprint_instance_list.py
--rw-r--r--   0        0        0     3274 2024-05-09 16:11:12.074447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_brand_list.py
--rw-r--r--   0        0        0     3331 2024-05-09 16:11:12.078447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_captcha_stage_list.py
--rw-r--r--   0        0        0     3380 2024-05-09 16:11:12.082447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_certificate_key_pair_list.py
--rw-r--r--   0        0        0     3355 2024-05-09 16:11:12.082447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_connection_token_list.py
--rw-r--r--   0        0        0     3331 2024-05-09 16:11:12.086447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_consent_stage_list.py
--rw-r--r--   0        0        0     3307 2024-05-09 16:11:12.090447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_deny_stage_list.py
--rw-r--r--   0        0        0     3420 2024-05-09 16:11:12.094447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_docker_service_connection_list.py
--rw-r--r--   0        0        0     3282 2024-05-09 16:11:12.102447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_domain_list.py
--rw-r--r--   0        0        0     3323 2024-05-09 16:11:12.102447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_dummy_policy_list.py
--rw-r--r--   0        0        0     3315 2024-05-09 16:11:12.106447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_dummy_stage_list.py
--rw-r--r--   0        0        0     3307 2024-05-09 16:11:12.110447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_duo_device_list.py
--rw-r--r--   0        0        0     3315 2024-05-09 16:11:12.114447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_email_stage_list.py
--rw-r--r--   0        0        0     3298 2024-05-09 16:11:12.114447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_endpoint_list.py
--rw-r--r--   0        0        0     3274 2024-05-09 16:11:12.118447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_event_list.py
--rw-r--r--   0        0        0     3380 2024-05-09 16:11:12.122447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_event_matcher_policy_list.py
--rw-r--r--   0        0        0     3413 2024-05-09 16:11:12.122447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_expiring_base_grant_model_list.py
--rw-r--r--   0        0        0     3363 2024-05-09 16:11:12.126447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_expression_policy_list.py
--rw-r--r--   0        0        0     3437 2024-05-09 16:11:12.130447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_extra_role_object_permission_list.py
--rw-r--r--   0        0        0     3437 2024-05-09 16:11:12.130447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_extra_user_object_permission_list.py
--rw-r--r--   0        0        0     3266 2024-05-09 16:11:12.134447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_flow_list.py
--rw-r--r--   0        0        0     3364 2024-05-09 16:11:12.138447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_flow_stage_binding_list.py
--rw-r--r--   0        0        0     3461 2024-05-09 16:11:12.146448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_google_workspace_provider_group_list.py
--rw-r--r--   0        0        0     3420 2024-05-09 16:11:12.150447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_google_workspace_provider_list.py
--rw-r--r--   0        0        0     3477 2024-05-09 16:11:12.154447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_google_workspace_provider_mapping_list.py
--rw-r--r--   0        0        0     3453 2024-05-09 16:11:12.158448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_google_workspace_provider_user_list.py
--rw-r--r--   0        0        0     3274 2024-05-09 16:11:12.166447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_group_list.py
--rw-r--r--   0        0        0     3387 2024-05-09 16:11:12.166447 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_identification_stage_list.py
--rw-r--r--   0        0        0     3314 2024-05-09 16:11:12.170448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_invitation_list.py
--rw-r--r--   0        0        0     3355 2024-05-09 16:11:12.174448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_invitation_stage_list.py
--rw-r--r--   0        0        0     3452 2024-05-09 16:11:12.174448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_kubernetes_service_connection_list.py
--rw-r--r--   0        0        0     3372 2024-05-09 16:11:12.178448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_ldap_outpost_config_list.py
--rw-r--r--   0        0        0     3388 2024-05-09 16:11:12.182448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_ldap_property_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-05-09 16:11:12.182448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_ldap_provider_list.py
--rw-r--r--   0        0        0     3315 2024-05-09 16:11:12.186448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_ldap_source_list.py
--rw-r--r--   0        0        0     3290 2024-05-09 16:11:12.190448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_license_list.py
--rw-r--r--   0        0        0     3453 2024-05-09 16:11:12.190448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_microsoft_entra_provider_group_list.py
--rw-r--r--   0        0        0     3412 2024-05-09 16:11:12.194448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_microsoft_entra_provider_list.py
--rw-r--r--   0        0        0     3469 2024-05-09 16:11:12.198448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_microsoft_entra_provider_mapping_list.py
--rw-r--r--   0        0        0     3445 2024-05-09 16:11:12.198448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_microsoft_entra_provider_user_list.py
--rw-r--r--   0        0        0     3330 2024-05-09 16:11:12.202448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_notification_list.py
--rw-r--r--   0        0        0     3363 2024-05-09 16:11:12.206448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_notification_rule_list.py
--rw-r--r--   0        0        0     3403 2024-05-09 16:11:12.206448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_notification_transport_list.py
--rw-r--r--   0        0        0     3444 2024-05-09 16:11:12.210448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_notification_webhook_mapping_list.py
--rw-r--r--   0        0        0     3348 2024-05-09 16:11:12.214448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_o_auth2_provider_list.py
--rw-r--r--   0        0        0     3324 2024-05-09 16:11:12.218448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_o_auth_source_list.py
--rw-r--r--   0        0        0     3290 2024-05-09 16:11:12.218448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_outpost_list.py
--rw-r--r--   0        0        0     3396 2024-05-09 16:11:12.222448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_password_expiry_policy_list.py
--rw-r--r--   0        0        0     3347 2024-05-09 16:11:12.226448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_password_policy_list.py
--rw-r--r--   0        0        0     3339 2024-05-09 16:11:12.226448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_password_stage_list.py
--rw-r--r--   0        0        0     3314 2024-05-09 16:11:12.230448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_permission_list.py
--rw-r--r--   0        0        0     3396 2024-05-09 16:11:12.234448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_plex_source_connection_list.py
--rw-r--r--   0        0        0     3315 2024-05-09 16:11:12.234448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_plex_source_list.py
--rw-r--r--   0        0        0     3339 2024-05-09 16:11:12.238448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_policy_binding_list.py
--rw-r--r--   0        0        0     3282 2024-05-09 16:11:12.242448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_policy_list.py
--rw-r--r--   0        0        0     3282 2024-05-09 16:11:12.242448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_prompt_list.py
--rw-r--r--   0        0        0     3323 2024-05-09 16:11:12.246448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_prompt_stage_list.py
--rw-r--r--   0        0        0     3355 2024-05-09 16:11:12.250448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_property_mapping_list.py
--rw-r--r--   0        0        0     3298 2024-05-09 16:11:12.250448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_provider_list.py
--rw-r--r--   0        0        0     3380 2024-05-09 16:11:12.254449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_proxy_outpost_config_list.py
--rw-r--r--   0        0        0     3339 2024-05-09 16:11:12.258448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_proxy_provider_list.py
--rw-r--r--   0        0        0     3380 2024-05-09 16:11:12.258448 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_rac_property_mapping_list.py
--rw-r--r--   0        0        0     3323 2024-05-09 16:11:12.262449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_rac_provider_list.py
--rw-r--r--   0        0        0     3388 2024-05-09 16:11:12.266449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_radius_outpost_config_list.py
--rw-r--r--   0        0        0     3347 2024-05-09 16:11:12.270449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_radius_provider_list.py
--rw-r--r--   0        0        0     3314 2024-05-09 16:11:12.274449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_reputation_list.py
--rw-r--r--   0        0        0     3363 2024-05-09 16:11:12.278449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_reputation_policy_list.py
--rw-r--r--   0        0        0     3461 2024-05-09 16:11:12.282449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_role_assigned_object_permission_list.py
--rw-r--r--   0        0        0     3266 2024-05-09 16:11:12.282449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_role_list.py
--rw-r--r--   0        0        0     3388 2024-05-09 16:11:12.286449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_saml_property_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-05-09 16:11:12.290449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_saml_provider_list.py
--rw-r--r--   0        0        0     3315 2024-05-09 16:11:12.290449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_saml_source_list.py
--rw-r--r--   0        0        0     3323 2024-05-09 16:11:12.294449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_scim_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-05-09 16:11:12.298449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_scim_provider_list.py
--rw-r--r--   0        0        0     3356 2024-05-09 16:11:12.298449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_scim_source_group_list.py
--rw-r--r--   0        0        0     3315 2024-05-09 16:11:12.302449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_scim_source_list.py
--rw-r--r--   0        0        0     3348 2024-05-09 16:11:12.306449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_scim_source_user_list.py
--rw-r--r--   0        0        0     3331 2024-05-09 16:11:12.310449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_scope_mapping_list.py
--rw-r--r--   0        0        0     3371 2024-05-09 16:11:12.314449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_service_connection_list.py
--rw-r--r--   0        0        0     3307 2024-05-09 16:11:12.310449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_sms_device_list.py
--rw-r--r--   0        0        0     3282 2024-05-09 16:11:12.318449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_source_list.py
--rw-r--r--   0        0        0     3323 2024-05-09 16:11:12.318449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_source_stage_list.py
--rw-r--r--   0        0        0     3274 2024-05-09 16:11:12.322449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_stage_list.py
--rw-r--r--   0        0        0     3331 2024-05-09 16:11:12.326449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_static_device_list.py
--rw-r--r--   0        0        0     3315 2024-05-09 16:11:12.330449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_system_task_list.py
--rw-r--r--   0        0        0     3282 2024-05-09 16:11:12.338449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_tenant_list.py
--rw-r--r--   0        0        0     3274 2024-05-09 16:11:12.342449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_token_list.py
--rw-r--r--   0        0        0     3315 2024-05-09 16:11:12.346449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_token_model_list.py
--rw-r--r--   0        0        0     3315 2024-05-09 16:11:12.334449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_totp_device_list.py
--rw-r--r--   0        0        0     3461 2024-05-09 16:11:12.346449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_user_assigned_object_permission_list.py
--rw-r--r--   0        0        0     3323 2024-05-09 16:11:12.350449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_user_consent_list.py
--rw-r--r--   0        0        0     3356 2024-05-09 16:11:12.354449 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_user_delete_stage_list.py
--rw-r--r--   0        0        0     3266 2024-05-09 16:11:12.358450 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_user_list.py
--rw-r--r--   0        0        0     3348 2024-05-09 16:11:12.362450 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_user_login_stage_list.py
--rw-r--r--   0        0        0     3356 2024-05-09 16:11:12.362450 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_user_logout_stage_list.py
--rw-r--r--   0        0        0     3438 2024-05-09 16:11:12.366450 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_user_o_auth_source_connection_list.py
--rw-r--r--   0        0        0     3429 2024-05-09 16:11:12.366450 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_user_saml_source_connection_list.py
--rw-r--r--   0        0        0     3396 2024-05-09 16:11:12.370450 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_user_source_connection_list.py
--rw-r--r--   0        0        0     3348 2024-05-09 16:11:12.374450 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_user_write_stage_list.py
--rw-r--r--   0        0        0     3348 2024-05-09 16:11:12.374450 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_web_authn_device_list.py
--rw-r--r--   0        0        0     3381 2024-05-09 16:11:12.378450 authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_web_authn_device_type_list.py
--rw-r--r--   0        0        0     3076 2024-05-09 16:11:12.378450 authentik_client-2024.4.2.post1715271061/authentik_client/models/pagination.py
--rw-r--r--   0        0        0     4454 2024-05-09 16:11:12.382450 authentik_client-2024.4.2.post1715271061/authentik_client/models/password_challenge.py
--rw-r--r--   0        0        0     2819 2024-05-09 16:11:12.386450 authentik_client-2024.4.2.post1715271061/authentik_client/models/password_challenge_response_request.py
--rw-r--r--   0        0        0     4377 2024-05-09 16:11:12.390450 authentik_client-2024.4.2.post1715271061/authentik_client/models/password_expiry_policy.py
--rw-r--r--   0        0        0     3099 2024-05-09 16:11:12.394450 authentik_client-2024.4.2.post1715271061/authentik_client/models/password_expiry_policy_request.py
--rw-r--r--   0        0        0     6428 2024-05-09 16:11:12.394450 authentik_client-2024.4.2.post1715271061/authentik_client/models/password_policy.py
--rw-r--r--   0        0        0     5239 2024-05-09 16:11:12.398450 authentik_client-2024.4.2.post1715271061/authentik_client/models/password_policy_request.py
--rw-r--r--   0        0        0     5274 2024-05-09 16:11:12.402450 authentik_client-2024.4.2.post1715271061/authentik_client/models/password_stage.py
--rw-r--r--   0        0        0     4264 2024-05-09 16:11:12.406450 authentik_client-2024.4.2.post1715271061/authentik_client/models/password_stage_request.py
--rw-r--r--   0        0        0     4594 2024-05-09 16:11:12.410450 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_application_request.py
--rw-r--r--   0        0        0     4833 2024-05-09 16:11:12.414450 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_authenticator_duo_stage_request.py
--rw-r--r--   0        0        0     5701 2024-05-09 16:11:12.418450 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_authenticator_sms_stage_request.py
--rw-r--r--   0        0        0     4430 2024-05-09 16:11:12.422450 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_authenticator_static_stage_request.py
--rw-r--r--   0        0        0     4256 2024-05-09 16:11:12.422450 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_authenticator_totp_stage_request.py
--rw-r--r--   0        0        0     4931 2024-05-09 16:11:12.426450 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_authenticator_validate_stage_request.py
--rw-r--r--   0        0        0     5340 2024-05-09 16:11:12.430450 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_authenticator_web_authn_stage_request.py
--rw-r--r--   0        0        0     3246 2024-05-09 16:11:12.434450 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_blueprint_instance_request.py
--rw-r--r--   0        0        0     6352 2024-05-09 16:11:12.438450 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_brand_request.py
--rw-r--r--   0        0        0     3860 2024-05-09 16:11:12.442450 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_captcha_stage_request.py
--rw-r--r--   0        0        0     3051 2024-05-09 16:11:12.442450 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_certificate_key_pair_request.py
--rw-r--r--   0        0        0     2717 2024-05-09 16:11:12.446450 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_connection_token_request.py
--rw-r--r--   0        0        0     3607 2024-05-09 16:11:12.450451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_consent_stage_request.py
--rw-r--r--   0        0        0     3268 2024-05-09 16:11:12.454450 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_deny_stage_request.py
--rw-r--r--   0        0        0     4149 2024-05-09 16:11:12.454450 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_docker_service_connection_request.py
--rw-r--r--   0        0        0     2801 2024-05-09 16:11:12.458450 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_domain_request.py
--rw-r--r--   0        0        0     3275 2024-05-09 16:11:12.462451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_dummy_policy_request.py
--rw-r--r--   0        0        0     3270 2024-05-09 16:11:12.470450 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_dummy_stage_request.py
--rw-r--r--   0        0        0     2674 2024-05-09 16:11:12.470450 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_duo_device_request.py
--rw-r--r--   0        0        0     5159 2024-05-09 16:11:12.474451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_email_stage_request.py
--rw-r--r--   0        0        0     3784 2024-05-09 16:11:12.478451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_endpoint_request.py
--rw-r--r--   0        0        0     4845 2024-05-09 16:11:12.482451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_event_matcher_policy_request.py
--rw-r--r--   0        0        0     4045 2024-05-09 16:11:12.482451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_event_request.py
--rw-r--r--   0        0        0     3047 2024-05-09 16:11:12.486451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_expression_policy_request.py
--rw-r--r--   0        0        0     4903 2024-05-09 16:11:12.486451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_flow_request.py
--rw-r--r--   0        0        0     4055 2024-05-09 16:11:12.490451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_flow_stage_binding_request.py
--rw-r--r--   0        0        0     2574 2024-05-09 16:11:12.490451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_google_workspace_provider_group_request.py
--rw-r--r--   0        0        0     3440 2024-05-09 16:11:12.494451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_google_workspace_provider_mapping_request.py
--rw-r--r--   0        0        0     4819 2024-05-09 16:11:12.494451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_google_workspace_provider_request.py
--rw-r--r--   0        0        0     2566 2024-05-09 16:11:12.498451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_google_workspace_provider_user_request.py
--rw-r--r--   0        0        0     3385 2024-05-09 16:11:12.498451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_group_request.py
--rw-r--r--   0        0        0     6571 2024-05-09 16:11:12.502451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_identification_stage_request.py
--rw-r--r--   0        0        0     3985 2024-05-09 16:11:12.506451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_invitation_request.py
--rw-r--r--   0        0        0     3565 2024-05-09 16:11:12.506451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_invitation_stage_request.py
--rw-r--r--   0        0        0     3492 2024-05-09 16:11:12.510451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_kubernetes_service_connection_request.py
--rw-r--r--   0        0        0     3550 2024-05-09 16:11:12.510451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_ldap_property_mapping_request.py
--rw-r--r--   0        0        0     6254 2024-05-09 16:11:12.514451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_ldap_provider_request.py
--rw-r--r--   0        0        0     9697 2024-05-09 16:11:12.518451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_ldap_source_request.py
--rw-r--r--   0        0        0     2557 2024-05-09 16:11:12.518451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_license_request.py
--rw-r--r--   0        0        0     2570 2024-05-09 16:11:12.522451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_microsoft_entra_provider_group_request.py
--rw-r--r--   0        0        0     3436 2024-05-09 16:11:12.522451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_microsoft_entra_provider_mapping_request.py
--rw-r--r--   0        0        0     4396 2024-05-09 16:11:12.526451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_microsoft_entra_provider_request.py
--rw-r--r--   0        0        0     2562 2024-05-09 16:11:12.530451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_microsoft_entra_provider_user_request.py
--rw-r--r--   0        0        0     2879 2024-05-09 16:11:12.534451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_notification_request.py
--rw-r--r--   0        0        0     3587 2024-05-09 16:11:12.538451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_notification_rule_request.py
--rw-r--r--   0        0        0     3538 2024-05-09 16:11:12.538451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_notification_transport_request.py
--rw-r--r--   0        0        0     2782 2024-05-09 16:11:12.542451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_notification_webhook_mapping_request.py
--rw-r--r--   0        0        0     6716 2024-05-09 16:11:12.546451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_o_auth2_provider_request.py
--rw-r--r--   0        0        0     8185 2024-05-09 16:11:12.550451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_o_auth_source_request.py
--rw-r--r--   0        0        0     4139 2024-05-09 16:11:12.554451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_outpost_request.py
--rw-r--r--   0        0        0     3154 2024-05-09 16:11:12.558452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_password_expiry_policy_request.py
--rw-r--r--   0        0        0     5277 2024-05-09 16:11:12.558452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_password_policy_request.py
--rw-r--r--   0        0        0     4326 2024-05-09 16:11:12.562451 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_password_stage_request.py
--rw-r--r--   0        0        0     2922 2024-05-09 16:11:12.566452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_permission_assign_request.py
--rw-r--r--   0        0        0     2784 2024-05-09 16:11:12.570452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_plex_source_connection_request.py
--rw-r--r--   0        0        0     5905 2024-05-09 16:11:12.570452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_plex_source_request.py
--rw-r--r--   0        0        0     4286 2024-05-09 16:11:12.574452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_policy_binding_request.py
--rw-r--r--   0        0        0     5023 2024-05-09 16:11:12.578452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_prompt_request.py
--rw-r--r--   0        0        0     3406 2024-05-09 16:11:12.582452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_prompt_stage_request.py
--rw-r--r--   0        0        0     6907 2024-05-09 16:11:12.586452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_proxy_provider_request.py
--rw-r--r--   0        0        0     3495 2024-05-09 16:11:12.586452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_rac_property_mapping_request.py
--rw-r--r--   0        0        0     4413 2024-05-09 16:11:12.590452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_rac_provider_request.py
--rw-r--r--   0        0        0     4563 2024-05-09 16:11:12.594452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_radius_provider_request.py
--rw-r--r--   0        0        0     3276 2024-05-09 16:11:12.598452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_reputation_policy_request.py
--rw-r--r--   0        0        0     2565 2024-05-09 16:11:12.602452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_role_request.py
--rw-r--r--   0        0        0     3901 2024-05-09 16:11:12.602452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_saml_property_mapping_request.py
--rw-r--r--   0        0        0     7539 2024-05-09 16:11:12.606452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_saml_provider_request.py
--rw-r--r--   0        0        0     8676 2024-05-09 16:11:12.610452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_saml_source_request.py
--rw-r--r--   0        0        0     3364 2024-05-09 16:11:12.610452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_scim_mapping_request.py
--rw-r--r--   0        0        0     3888 2024-05-09 16:11:12.614452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_scim_provider_request.py
--rw-r--r--   0        0        0     3095 2024-05-09 16:11:12.618452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_scim_source_group_request.py
--rw-r--r--   0        0        0     3829 2024-05-09 16:11:12.622452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_scim_source_request.py
--rw-r--r--   0        0        0     3098 2024-05-09 16:11:12.622452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_scim_source_user_request.py
--rw-r--r--   0        0        0     3819 2024-05-09 16:11:12.626452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_scope_mapping_request.py
--rw-r--r--   0        0        0     5079 2024-05-09 16:11:12.630452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_settings_request.py
--rw-r--r--   0        0        0     2674 2024-05-09 16:11:12.626452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_sms_device_request.py
--rw-r--r--   0        0        0     3562 2024-05-09 16:11:12.634452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_source_stage_request.py
--rw-r--r--   0        0        0     2686 2024-05-09 16:11:12.634452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_static_device_request.py
--rw-r--r--   0        0        0     2820 2024-05-09 16:11:12.642452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_tenant_request.py
--rw-r--r--   0        0        0     4419 2024-05-09 16:11:12.642452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_token_request.py
--rw-r--r--   0        0        0     2678 2024-05-09 16:11:12.638452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_totp_device_request.py
--rw-r--r--   0        0        0     3167 2024-05-09 16:11:12.646452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_user_delete_stage_request.py
--rw-r--r--   0        0        0     4766 2024-05-09 16:11:12.650452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_user_login_stage_request.py
--rw-r--r--   0        0        0     3167 2024-05-09 16:11:12.654452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_user_logout_stage_request.py
--rw-r--r--   0        0        0     3109 2024-05-09 16:11:12.654452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_user_o_auth_source_connection_request.py
--rw-r--r--   0        0        0     3934 2024-05-09 16:11:12.658452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_user_request.py
--rw-r--r--   0        0        0     2733 2024-05-09 16:11:12.658452 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_user_saml_source_connection_request.py
--rw-r--r--   0        0        0     4450 2024-05-09 16:11:12.662453 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_user_write_stage_request.py
--rw-r--r--   0        0        0     2625 2024-05-09 16:11:12.662453 authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_web_authn_device_request.py
--rw-r--r--   0        0        0     3548 2024-05-09 16:11:12.662453 authentik_client-2024.4.2.post1715271061/authentik_client/models/permission.py
--rw-r--r--   0        0        0     2884 2024-05-09 16:11:12.666453 authentik_client-2024.4.2.post1715271061/authentik_client/models/permission_assign_request.py
--rw-r--r--   0        0        0     4315 2024-05-09 16:11:12.666453 authentik_client-2024.4.2.post1715271061/authentik_client/models/plex_authentication_challenge.py
--rw-r--r--   0        0        0     2726 2024-05-09 16:11:12.670452 authentik_client-2024.4.2.post1715271061/authentik_client/models/plex_authentication_challenge_response_request.py
--rw-r--r--   0        0        0     7752 2024-05-09 16:11:12.670452 authentik_client-2024.4.2.post1715271061/authentik_client/models/plex_source.py
--rw-r--r--   0        0        0     3265 2024-05-09 16:11:12.674453 authentik_client-2024.4.2.post1715271061/authentik_client/models/plex_source_connection.py
--rw-r--r--   0        0        0     2719 2024-05-09 16:11:12.674453 authentik_client-2024.4.2.post1715271061/authentik_client/models/plex_source_connection_request.py
--rw-r--r--   0        0        0     5760 2024-05-09 16:11:12.678453 authentik_client-2024.4.2.post1715271061/authentik_client/models/plex_source_request.py
--rw-r--r--   0        0        0     2576 2024-05-09 16:11:12.682453 authentik_client-2024.4.2.post1715271061/authentik_client/models/plex_token_redeem_request.py
--rw-r--r--   0        0        0     4055 2024-05-09 16:11:12.682453 authentik_client-2024.4.2.post1715271061/authentik_client/models/policy.py
--rw-r--r--   0        0        0     5643 2024-05-09 16:11:12.686453 authentik_client-2024.4.2.post1715271061/authentik_client/models/policy_binding.py
--rw-r--r--   0        0        0     4231 2024-05-09 16:11:12.686453 authentik_client-2024.4.2.post1715271061/authentik_client/models/policy_binding_request.py
--rw-r--r--   0        0        0      711 2024-05-09 16:11:12.690453 authentik_client-2024.4.2.post1715271061/authentik_client/models/policy_engine_mode.py
--rw-r--r--   0        0        0     2817 2024-05-09 16:11:12.690453 authentik_client-2024.4.2.post1715271061/authentik_client/models/policy_request.py
--rw-r--r--   0        0        0     2583 2024-05-09 16:11:12.694453 authentik_client-2024.4.2.post1715271061/authentik_client/models/policy_test_request.py
--rw-r--r--   0        0        0     3281 2024-05-09 16:11:12.694453 authentik_client-2024.4.2.post1715271061/authentik_client/models/policy_test_result.py
--rw-r--r--   0        0        0     4885 2024-05-09 16:11:12.698453 authentik_client-2024.4.2.post1715271061/authentik_client/models/prompt.py
--rw-r--r--   0        0        0     4649 2024-05-09 16:11:12.702453 authentik_client-2024.4.2.post1715271061/authentik_client/models/prompt_challenge.py
--rw-r--r--   0        0        0     3325 2024-05-09 16:11:12.702453 authentik_client-2024.4.2.post1715271061/authentik_client/models/prompt_challenge_response_request.py
--rw-r--r--   0        0        0     4927 2024-05-09 16:11:12.706453 authentik_client-2024.4.2.post1715271061/authentik_client/models/prompt_request.py
--rw-r--r--   0        0        0     4321 2024-05-09 16:11:12.710453 authentik_client-2024.4.2.post1715271061/authentik_client/models/prompt_stage.py
--rw-r--r--   0        0        0     3351 2024-05-09 16:11:12.710453 authentik_client-2024.4.2.post1715271061/authentik_client/models/prompt_stage_request.py
--rw-r--r--   0        0        0     1185 2024-05-09 16:11:12.714453 authentik_client-2024.4.2.post1715271061/authentik_client/models/prompt_type_enum.py
--rw-r--r--   0        0        0     4264 2024-05-09 16:11:12.714453 authentik_client-2024.4.2.post1715271061/authentik_client/models/property_mapping.py
--rw-r--r--   0        0        0     2610 2024-05-09 16:11:12.718453 authentik_client-2024.4.2.post1715271061/authentik_client/models/property_mapping_preview.py
--rw-r--r--   0        0        0     2744 2024-05-09 16:11:12.722453 authentik_client-2024.4.2.post1715271061/authentik_client/models/property_mapping_test_result.py
--rw-r--r--   0        0        0      715 2024-05-09 16:11:12.722453 authentik_client-2024.4.2.post1715271061/authentik_client/models/protocol_enum.py
--rw-r--r--   0        0        0     5722 2024-05-09 16:11:12.726453 authentik_client-2024.4.2.post1715271061/authentik_client/models/provider.py
--rw-r--r--   0        0        0      713 2024-05-09 16:11:12.726453 authentik_client-2024.4.2.post1715271061/authentik_client/models/provider_enum.py
--rw-r--r--   0        0        0     1578 2024-05-09 16:11:12.730453 authentik_client-2024.4.2.post1715271061/authentik_client/models/provider_model_enum.py
--rw-r--r--   0        0        0     3397 2024-05-09 16:11:12.730453 authentik_client-2024.4.2.post1715271061/authentik_client/models/provider_request.py
--rw-r--r--   0        0        0     1009 2024-05-09 16:11:12.734453 authentik_client-2024.4.2.post1715271061/authentik_client/models/provider_type_enum.py
--rw-r--r--   0        0        0      754 2024-05-09 16:11:12.734453 authentik_client-2024.4.2.post1715271061/authentik_client/models/proxy_mode.py
--rw-r--r--   0        0        0     7819 2024-05-09 16:11:12.738453 authentik_client-2024.4.2.post1715271061/authentik_client/models/proxy_outpost_config.py
--rw-r--r--   0        0        0     9552 2024-05-09 16:11:12.738453 authentik_client-2024.4.2.post1715271061/authentik_client/models/proxy_provider.py
--rw-r--r--   0        0        0     6828 2024-05-09 16:11:12.742453 authentik_client-2024.4.2.post1715271061/authentik_client/models/proxy_provider_request.py
--rw-r--r--   0        0        0     4407 2024-05-09 16:11:12.742453 authentik_client-2024.4.2.post1715271061/authentik_client/models/rac_property_mapping.py
--rw-r--r--   0        0        0     3440 2024-05-09 16:11:12.746453 authentik_client-2024.4.2.post1715271061/authentik_client/models/rac_property_mapping_request.py
--rw-r--r--   0        0        0     6813 2024-05-09 16:11:12.750453 authentik_client-2024.4.2.post1715271061/authentik_client/models/rac_provider.py
--rw-r--r--   0        0        0     4351 2024-05-09 16:11:12.750453 authentik_client-2024.4.2.post1715271061/authentik_client/models/rac_provider_request.py
--rw-r--r--   0        0        0     3833 2024-05-09 16:11:12.758453 authentik_client-2024.4.2.post1715271061/authentik_client/models/radius_outpost_config.py
--rw-r--r--   0        0        0     6924 2024-05-09 16:11:12.762453 authentik_client-2024.4.2.post1715271061/authentik_client/models/radius_provider.py
--rw-r--r--   0        0        0     4501 2024-05-09 16:11:12.766454 authentik_client-2024.4.2.post1715271061/authentik_client/models/radius_provider_request.py
--rw-r--r--   0        0        0     4184 2024-05-09 16:11:12.770454 authentik_client-2024.4.2.post1715271061/authentik_client/models/redirect_challenge.py
--rw-r--r--   0        0        0     3642 2024-05-09 16:11:12.770454 authentik_client-2024.4.2.post1715271061/authentik_client/models/reputation.py
--rw-r--r--   0        0        0     4516 2024-05-09 16:11:12.774453 authentik_client-2024.4.2.post1715271061/authentik_client/models/reputation_policy.py
--rw-r--r--   0        0        0     3238 2024-05-09 16:11:12.778454 authentik_client-2024.4.2.post1715271061/authentik_client/models/reputation_policy_request.py
--rw-r--r--   0        0        0      795 2024-05-09 16:11:12.778454 authentik_client-2024.4.2.post1715271061/authentik_client/models/resident_key_requirement_enum.py
--rw-r--r--   0        0        0     2618 2024-05-09 16:11:12.782454 authentik_client-2024.4.2.post1715271061/authentik_client/models/role.py
--rw-r--r--   0        0        0     3333 2024-05-09 16:11:12.786454 authentik_client-2024.4.2.post1715271061/authentik_client/models/role_assigned_object_permission.py
--rw-r--r--   0        0        0     3293 2024-05-09 16:11:12.790454 authentik_client-2024.4.2.post1715271061/authentik_client/models/role_object_permission.py
--rw-r--r--   0        0        0     2517 2024-05-09 16:11:12.790454 authentik_client-2024.4.2.post1715271061/authentik_client/models/role_request.py
--rw-r--r--   0        0        0     2712 2024-05-09 16:11:12.794454 authentik_client-2024.4.2.post1715271061/authentik_client/models/saml_metadata.py
--rw-r--r--   0        0        0     4718 2024-05-09 16:11:12.798454 authentik_client-2024.4.2.post1715271061/authentik_client/models/saml_property_mapping.py
--rw-r--r--   0        0        0     3829 2024-05-09 16:11:12.798454 authentik_client-2024.4.2.post1715271061/authentik_client/models/saml_property_mapping_request.py
--rw-r--r--   0        0        0    11056 2024-05-09 16:11:12.802454 authentik_client-2024.4.2.post1715271061/authentik_client/models/saml_provider.py
--rw-r--r--   0        0        0     7460 2024-05-09 16:11:12.806454 authentik_client-2024.4.2.post1715271061/authentik_client/models/saml_provider_request.py
--rw-r--r--   0        0        0    10563 2024-05-09 16:11:12.810454 authentik_client-2024.4.2.post1715271061/authentik_client/models/saml_source.py
--rw-r--r--   0        0        0     8507 2024-05-09 16:11:12.814454 authentik_client-2024.4.2.post1715271061/authentik_client/models/saml_source_request.py
--rw-r--r--   0        0        0     4248 2024-05-09 16:11:12.818454 authentik_client-2024.4.2.post1715271061/authentik_client/models/scim_mapping.py
--rw-r--r--   0        0        0     3309 2024-05-09 16:11:12.818454 authentik_client-2024.4.2.post1715271061/authentik_client/models/scim_mapping_request.py
--rw-r--r--   0        0        0     5454 2024-05-09 16:11:12.822454 authentik_client-2024.4.2.post1715271061/authentik_client/models/scim_provider.py
--rw-r--r--   0        0        0     3802 2024-05-09 16:11:12.826454 authentik_client-2024.4.2.post1715271061/authentik_client/models/scim_provider_request.py
--rw-r--r--   0        0        0     5999 2024-05-09 16:11:12.830454 authentik_client-2024.4.2.post1715271061/authentik_client/models/scim_source.py
--rw-r--r--   0        0        0     3369 2024-05-09 16:11:12.830454 authentik_client-2024.4.2.post1715271061/authentik_client/models/scim_source_group.py
--rw-r--r--   0        0        0     3023 2024-05-09 16:11:12.834454 authentik_client-2024.4.2.post1715271061/authentik_client/models/scim_source_group_request.py
--rw-r--r--   0        0        0     3708 2024-05-09 16:11:12.838454 authentik_client-2024.4.2.post1715271061/authentik_client/models/scim_source_request.py
--rw-r--r--   0        0        0     3370 2024-05-09 16:11:12.842454 authentik_client-2024.4.2.post1715271061/authentik_client/models/scim_source_user.py
--rw-r--r--   0        0        0     3026 2024-05-09 16:11:12.842454 authentik_client-2024.4.2.post1715271061/authentik_client/models/scim_source_user_request.py
--rw-r--r--   0        0        0     4629 2024-05-09 16:11:12.850454 authentik_client-2024.4.2.post1715271061/authentik_client/models/scope_mapping.py
--rw-r--r--   0        0        0     3740 2024-05-09 16:11:12.854454 authentik_client-2024.4.2.post1715271061/authentik_client/models/scope_mapping_request.py
--rw-r--r--   0        0        0     2738 2024-05-09 16:11:12.858454 authentik_client-2024.4.2.post1715271061/authentik_client/models/selectable_stage.py
--rw-r--r--   0        0        0     3773 2024-05-09 16:11:12.858454 authentik_client-2024.4.2.post1715271061/authentik_client/models/service_connection.py
--rw-r--r--   0        0        0     2776 2024-05-09 16:11:12.862455 authentik_client-2024.4.2.post1715271061/authentik_client/models/service_connection_request.py
--rw-r--r--   0        0        0     2731 2024-05-09 16:11:12.866454 authentik_client-2024.4.2.post1715271061/authentik_client/models/service_connection_state.py
--rw-r--r--   0        0        0     3178 2024-05-09 16:11:12.866454 authentik_client-2024.4.2.post1715271061/authentik_client/models/session_user.py
--rw-r--r--   0        0        0     4931 2024-05-09 16:11:12.870454 authentik_client-2024.4.2.post1715271061/authentik_client/models/settings.py
--rw-r--r--   0        0        0     5058 2024-05-09 16:11:12.874455 authentik_client-2024.4.2.post1715271061/authentik_client/models/settings_request.py
--rw-r--r--   0        0        0      733 2024-05-09 16:11:12.874455 authentik_client-2024.4.2.post1715271061/authentik_client/models/severity_enum.py
--rw-r--r--   0        0        0     4175 2024-05-09 16:11:12.878455 authentik_client-2024.4.2.post1715271061/authentik_client/models/shell_challenge.py
--rw-r--r--   0        0        0     2172 2024-05-09 16:11:12.878455 authentik_client-2024.4.2.post1715271061/authentik_client/models/signature_algorithm_enum.py
--rw-r--r--   0        0        0     2906 2024-05-09 16:11:12.846454 authentik_client-2024.4.2.post1715271061/authentik_client/models/sms_device.py
--rw-r--r--   0        0        0     2619 2024-05-09 16:11:12.850454 authentik_client-2024.4.2.post1715271061/authentik_client/models/sms_device_request.py
--rw-r--r--   0        0        0     6945 2024-05-09 16:11:12.882455 authentik_client-2024.4.2.post1715271061/authentik_client/models/source.py
--rw-r--r--   0        0        0     4836 2024-05-09 16:11:12.886455 authentik_client-2024.4.2.post1715271061/authentik_client/models/source_request.py
--rw-r--r--   0        0        0     4438 2024-05-09 16:11:12.890455 authentik_client-2024.4.2.post1715271061/authentik_client/models/source_stage.py
--rw-r--r--   0        0        0     3507 2024-05-09 16:11:12.894455 authentik_client-2024.4.2.post1715271061/authentik_client/models/source_stage_request.py
--rw-r--r--   0        0        0     5355 2024-05-09 16:11:12.894455 authentik_client-2024.4.2.post1715271061/authentik_client/models/source_type.py
--rw-r--r--   0        0        0      714 2024-05-09 16:11:12.898455 authentik_client-2024.4.2.post1715271061/authentik_client/models/sp_binding_enum.py
--rw-r--r--   0        0        0     4070 2024-05-09 16:11:12.902455 authentik_client-2024.4.2.post1715271061/authentik_client/models/stage.py
--rw-r--r--   0        0        0     3437 2024-05-09 16:11:12.902455 authentik_client-2024.4.2.post1715271061/authentik_client/models/stage_prompt.py
--rw-r--r--   0        0        0     3089 2024-05-09 16:11:12.906455 authentik_client-2024.4.2.post1715271061/authentik_client/models/stage_request.py
--rw-r--r--   0        0        0     3385 2024-05-09 16:11:12.906455 authentik_client-2024.4.2.post1715271061/authentik_client/models/static_device.py
--rw-r--r--   0        0        0     2631 2024-05-09 16:11:12.910455 authentik_client-2024.4.2.post1715271061/authentik_client/models/static_device_request.py
--rw-r--r--   0        0        0     2546 2024-05-09 16:11:12.914455 authentik_client-2024.4.2.post1715271061/authentik_client/models/static_device_token.py
--rw-r--r--   0        0        0     2581 2024-05-09 16:11:12.914455 authentik_client-2024.4.2.post1715271061/authentik_client/models/static_device_token_request.py
--rw-r--r--   0        0        0      846 2024-05-09 16:11:12.918455 authentik_client-2024.4.2.post1715271061/authentik_client/models/sub_mode_enum.py
--rw-r--r--   0        0        0     3114 2024-05-09 16:11:12.918455 authentik_client-2024.4.2.post1715271061/authentik_client/models/sync_status.py
--rw-r--r--   0        0        0     4463 2024-05-09 16:11:12.922455 authentik_client-2024.4.2.post1715271061/authentik_client/models/system_info.py
--rw-r--r--   0        0        0     2934 2024-05-09 16:11:12.926455 authentik_client-2024.4.2.post1715271061/authentik_client/models/system_info_runtime.py
--rw-r--r--   0        0        0     4701 2024-05-09 16:11:12.930455 authentik_client-2024.4.2.post1715271061/authentik_client/models/system_task.py
--rw-r--r--   0        0        0      789 2024-05-09 16:11:12.930455 authentik_client-2024.4.2.post1715271061/authentik_client/models/system_task_status_enum.py
--rw-r--r--   0        0        0     2872 2024-05-09 16:11:12.938455 authentik_client-2024.4.2.post1715271061/authentik_client/models/tenant.py
--rw-r--r--   0        0        0     2589 2024-05-09 16:11:12.942455 authentik_client-2024.4.2.post1715271061/authentik_client/models/tenant_admin_group_request_request.py
--rw-r--r--   0        0        0     2705 2024-05-09 16:11:12.946455 authentik_client-2024.4.2.post1715271061/authentik_client/models/tenant_recovery_key_request_request.py
--rw-r--r--   0        0        0     2599 2024-05-09 16:11:12.946455 authentik_client-2024.4.2.post1715271061/authentik_client/models/tenant_recovery_key_response.py
--rw-r--r--   0        0        0     2765 2024-05-09 16:11:12.950455 authentik_client-2024.4.2.post1715271061/authentik_client/models/tenant_request.py
--rw-r--r--   0        0        0     4802 2024-05-09 16:11:12.954455 authentik_client-2024.4.2.post1715271061/authentik_client/models/token.py
--rw-r--r--   0        0        0     4198 2024-05-09 16:11:12.958455 authentik_client-2024.4.2.post1715271061/authentik_client/models/token_model.py
--rw-r--r--   0        0        0     4329 2024-05-09 16:11:12.962455 authentik_client-2024.4.2.post1715271061/authentik_client/models/token_request.py
--rw-r--r--   0        0        0     2521 2024-05-09 16:11:12.962455 authentik_client-2024.4.2.post1715271061/authentik_client/models/token_set_key_request.py
--rw-r--r--   0        0        0     2494 2024-05-09 16:11:12.966456 authentik_client-2024.4.2.post1715271061/authentik_client/models/token_view.py
--rw-r--r--   0        0        0     2724 2024-05-09 16:11:12.934455 authentik_client-2024.4.2.post1715271061/authentik_client/models/totp_device.py
--rw-r--r--   0        0        0     2623 2024-05-09 16:11:12.938455 authentik_client-2024.4.2.post1715271061/authentik_client/models/totp_device_request.py
--rw-r--r--   0        0        0     3389 2024-05-09 16:11:12.970456 authentik_client-2024.4.2.post1715271061/authentik_client/models/transaction_application_request.py
--rw-r--r--   0        0        0     2595 2024-05-09 16:11:12.974455 authentik_client-2024.4.2.post1715271061/authentik_client/models/transaction_application_response.py
--rw-r--r--   0        0        0     2936 2024-05-09 16:11:12.974455 authentik_client-2024.4.2.post1715271061/authentik_client/models/type_create.py
--rw-r--r--   0        0        0      730 2024-05-09 16:11:12.978456 authentik_client-2024.4.2.post1715271061/authentik_client/models/ui_theme_enum.py
--rw-r--r--   0        0        0     2808 2024-05-09 16:11:12.978456 authentik_client-2024.4.2.post1715271061/authentik_client/models/used_by.py
--rw-r--r--   0        0        0      795 2024-05-09 16:11:12.982456 authentik_client-2024.4.2.post1715271061/authentik_client/models/used_by_action_enum.py
--rw-r--r--   0        0        0     5459 2024-05-09 16:11:12.986456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user.py
--rw-r--r--   0        0        0     2458 2024-05-09 16:11:12.990456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_account_request.py
--rw-r--r--   0        0        0     4946 2024-05-09 16:11:12.994456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_assigned_object_permission.py
--rw-r--r--   0        0        0     3828 2024-05-09 16:11:12.998456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_consent.py
--rw-r--r--   0        0        0      811 2024-05-09 16:11:12.998456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_creation_mode_enum.py
--rw-r--r--   0        0        0     4110 2024-05-09 16:11:12.998456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_delete_stage.py
--rw-r--r--   0        0        0     3129 2024-05-09 16:11:13.002456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_delete_stage_request.py
--rw-r--r--   0        0        0      735 2024-05-09 16:11:13.002456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_fields_enum.py
--rw-r--r--   0        0        0     3909 2024-05-09 16:11:13.006456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_group.py
--rw-r--r--   0        0        0     3193 2024-05-09 16:11:13.006456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_group_request.py
--rw-r--r--   0        0        0     4334 2024-05-09 16:11:13.010456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_login_challenge.py
--rw-r--r--   0        0        0     2805 2024-05-09 16:11:13.010456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_login_challenge_response_request.py
--rw-r--r--   0        0        0     5631 2024-05-09 16:11:13.014456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_login_stage.py
--rw-r--r--   0        0        0     4728 2024-05-09 16:11:13.018456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_login_stage_request.py
--rw-r--r--   0        0        0     4110 2024-05-09 16:11:13.018456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_logout_stage.py
--rw-r--r--   0        0        0     3129 2024-05-09 16:11:13.022456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_logout_stage_request.py
--rw-r--r--   0        0        0      853 2024-05-09 16:11:13.022456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_matching_mode_enum.py
--rw-r--r--   0        0        0     4160 2024-05-09 16:11:13.026456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_metrics.py
--rw-r--r--   0        0        0     3188 2024-05-09 16:11:13.026456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_o_auth_source_connection.py
--rw-r--r--   0        0        0     3054 2024-05-09 16:11:13.030456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_o_auth_source_connection_request.py
--rw-r--r--   0        0        0     3293 2024-05-09 16:11:13.030456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_object_permission.py
--rw-r--r--   0        0        0     2557 2024-05-09 16:11:13.034456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_password_set_request.py
--rw-r--r--   0        0        0     2491 2024-05-09 16:11:13.034456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_path.py
--rw-r--r--   0        0        0     3872 2024-05-09 16:11:13.038456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_request.py
--rw-r--r--   0        0        0     3107 2024-05-09 16:11:13.038456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_saml_source_connection.py
--rw-r--r--   0        0        0     2668 2024-05-09 16:11:13.042456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_saml_source_connection_request.py
--rw-r--r--   0        0        0     5465 2024-05-09 16:11:13.042456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_self.py
--rw-r--r--   0        0        0     2629 2024-05-09 16:11:13.046456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_self_groups.py
--rw-r--r--   0        0        0     3074 2024-05-09 16:11:13.046456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_service_account_request.py
--rw-r--r--   0        0        0     2844 2024-05-09 16:11:13.046456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_service_account_response.py
--rw-r--r--   0        0        0     2866 2024-05-09 16:11:13.050456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_setting.py
--rw-r--r--   0        0        0     3245 2024-05-09 16:11:13.050456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_source_connection.py
--rw-r--r--   0        0        0      817 2024-05-09 16:11:13.054456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_type_enum.py
--rw-r--r--   0        0        0      777 2024-05-09 16:11:13.054456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_verification_enum.py
--rw-r--r--   0        0        0     5382 2024-05-09 16:11:13.054456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_write_stage.py
--rw-r--r--   0        0        0     4412 2024-05-09 16:11:13.058456 authentik_client-2024.4.2.post1715271061/authentik_client/models/user_write_stage_request.py
--rw-r--r--   0        0        0     3197 2024-05-09 16:11:13.058456 authentik_client-2024.4.2.post1715271061/authentik_client/models/validation_error.py
--rw-r--r--   0        0        0     3589 2024-05-09 16:11:13.066456 authentik_client-2024.4.2.post1715271061/authentik_client/models/version.py
--rw-r--r--   0        0        0     3786 2024-05-09 16:11:13.066456 authentik_client-2024.4.2.post1715271061/authentik_client/models/web_authn_device.py
--rw-r--r--   0        0        0     2577 2024-05-09 16:11:13.070457 authentik_client-2024.4.2.post1715271061/authentik_client/models/web_authn_device_request.py
--rw-r--r--   0        0        0     2562 2024-05-09 16:11:13.070457 authentik_client-2024.4.2.post1715271061/authentik_client/models/web_authn_device_type.py
--rw-r--r--   0        0        0     2669 2024-05-09 16:11:13.074457 authentik_client-2024.4.2.post1715271061/authentik_client/models/web_authn_device_type_request.py
--rw-r--r--   0        0        0     2410 2024-05-09 16:11:13.074457 authentik_client-2024.4.2.post1715271061/authentik_client/models/workers.py
--rw-r--r--   0        0        0        0 2024-05-09 16:11:14.198468 authentik_client-2024.4.2.post1715271061/authentik_client/py.typed
--rw-r--r--   0        0        0     9196 2024-05-09 16:11:14.206468 authentik_client-2024.4.2.post1715271061/authentik_client/rest.py
--rw-r--r--   0        0        0     1936 2024-05-09 16:11:14.198468 authentik_client-2024.4.2.post1715271061/pyproject.toml
--rw-r--r--   0        0        0   158698 1970-01-01 00:00:00.000000 authentik_client-2024.4.2.post1715271061/PKG-INFO
+-rw-r--r--   0        0        0   157746 2024-05-20 12:48:22.381320 authentik_client-2024.4.2.post1716209289/README.md
+-rw-r--r--   0        0        0    52131 2024-05-20 12:48:22.393320 authentik_client-2024.4.2.post1716209289/authentik_client/__init__.py
+-rw-r--r--   0        0        0     1170 2024-05-20 12:48:22.397320 authentik_client-2024.4.2.post1716209289/authentik_client/api/__init__.py
+-rw-r--r--   0        0        0    97518 2024-05-20 12:48:22.089319 authentik_client-2024.4.2.post1716209289/authentik_client/api/admin_api.py
+-rw-r--r--   0        0        0   700271 2024-05-20 12:48:22.109319 authentik_client-2024.4.2.post1716209289/authentik_client/api/authenticators_api.py
+-rw-r--r--   0        0        0   701822 2024-05-20 12:48:22.137319 authentik_client-2024.4.2.post1716209289/authentik_client/api/core_api.py
+-rw-r--r--   0        0        0   116805 2024-05-20 12:48:22.149319 authentik_client-2024.4.2.post1716209289/authentik_client/api/crypto_api.py
+-rw-r--r--   0        0        0   107946 2024-05-20 12:48:22.157319 authentik_client-2024.4.2.post1716209289/authentik_client/api/enterprise_api.py
+-rw-r--r--   0        0        0   408008 2024-05-20 12:48:22.169319 authentik_client-2024.4.2.post1716209289/authentik_client/api/events_api.py
+-rw-r--r--   0        0        0   280806 2024-05-20 12:48:22.185319 authentik_client-2024.4.2.post1716209289/authentik_client/api/flows_api.py
+-rw-r--r--   0        0        0   101134 2024-05-20 12:48:22.193319 authentik_client-2024.4.2.post1716209289/authentik_client/api/managed_api.py
+-rw-r--r--   0        0        0   135649 2024-05-20 12:48:22.201319 authentik_client-2024.4.2.post1716209289/authentik_client/api/oauth2_api.py
+-rw-r--r--   0        0        0   413301 2024-05-20 12:48:22.213319 authentik_client-2024.4.2.post1716209289/authentik_client/api/outposts_api.py
+-rw-r--r--   0        0        0   725201 2024-05-20 12:48:22.229319 authentik_client-2024.4.2.post1716209289/authentik_client/api/policies_api.py
+-rw-r--r--   0        0        0   721674 2024-05-20 12:48:22.245319 authentik_client-2024.4.2.post1716209289/authentik_client/api/propertymappings_api.py
+-rw-r--r--   0        0        0  1235079 2024-05-20 12:48:22.273319 authentik_client-2024.4.2.post1716209289/authentik_client/api/providers_api.py
+-rw-r--r--   0        0        0   150485 2024-05-20 12:48:22.285319 authentik_client-2024.4.2.post1716209289/authentik_client/api/rac_api.py
+-rw-r--r--   0        0        0   207550 2024-05-20 12:48:22.293320 authentik_client-2024.4.2.post1716209289/authentik_client/api/rbac_api.py
+-rw-r--r--   0        0        0    10391 2024-05-20 12:48:22.301320 authentik_client-2024.4.2.post1716209289/authentik_client/api/root_api.py
+-rw-r--r--   0        0        0    11845 2024-05-20 12:48:22.305320 authentik_client-2024.4.2.post1716209289/authentik_client/api/schema_api.py
+-rw-r--r--   0        0        0  1037196 2024-05-20 12:48:22.325320 authentik_client-2024.4.2.post1716209289/authentik_client/api/sources_api.py
+-rw-r--r--   0        0        0  1945986 2024-05-20 12:48:22.357320 authentik_client-2024.4.2.post1716209289/authentik_client/api/stages_api.py
+-rw-r--r--   0        0        0   157909 2024-05-20 12:48:22.369320 authentik_client-2024.4.2.post1716209289/authentik_client/api/tenants_api.py
+-rw-r--r--   0        0        0    25779 2024-05-20 12:48:22.401320 authentik_client-2024.4.2.post1716209289/authentik_client/api_client.py
+-rw-r--r--   0        0        0      652 2024-05-20 12:48:22.401320 authentik_client-2024.4.2.post1716209289/authentik_client/api_response.py
+-rw-r--r--   0        0        0    14724 2024-05-20 12:48:22.393320 authentik_client-2024.4.2.post1716209289/authentik_client/configuration.py
+-rw-r--r--   0        0        0     5934 2024-05-20 12:48:22.397320 authentik_client-2024.4.2.post1716209289/authentik_client/exceptions.py
+-rw-r--r--   0        0        0    50433 2024-05-20 12:48:22.397320 authentik_client-2024.4.2.post1716209289/authentik_client/models/__init__.py
+-rw-r--r--   0        0        0     4513 2024-05-20 12:48:19.265305 authentik_client-2024.4.2.post1716209289/authentik_client/models/access_denied_challenge.py
+-rw-r--r--   0        0        0      688 2024-05-20 12:48:19.273305 authentik_client-2024.4.2.post1716209289/authentik_client/models/alg_enum.py
+-rw-r--r--   0        0        0     2482 2024-05-20 12:48:19.285305 authentik_client-2024.4.2.post1716209289/authentik_client/models/app.py
+-rw-r--r--   0        0        0     4460 2024-05-20 12:48:19.293305 authentik_client-2024.4.2.post1716209289/authentik_client/models/app_enum.py
+-rw-r--r--   0        0        0     2702 2024-05-20 12:48:19.305305 authentik_client-2024.4.2.post1716209289/authentik_client/models/apple_challenge_response_request.py
+-rw-r--r--   0        0        0     4508 2024-05-20 12:48:19.313305 authentik_client-2024.4.2.post1716209289/authentik_client/models/apple_login_challenge.py
+-rw-r--r--   0        0        0     6686 2024-05-20 12:48:19.325305 authentik_client-2024.4.2.post1716209289/authentik_client/models/application.py
+-rw-r--r--   0        0        0     4473 2024-05-20 12:48:19.333305 authentik_client-2024.4.2.post1716209289/authentik_client/models/application_request.py
+-rw-r--r--   0        0        0      711 2024-05-20 12:48:19.337305 authentik_client-2024.4.2.post1716209289/authentik_client/models/auth_mode_enum.py
+-rw-r--r--   0        0        0      709 2024-05-20 12:48:19.341305 authentik_client-2024.4.2.post1716209289/authentik_client/models/auth_type_enum.py
+-rw-r--r--   0        0        0     5195 2024-05-20 12:48:19.345305 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticated_session.py
+-rw-r--r--   0        0        0     3064 2024-05-20 12:48:19.353305 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticated_session_asn.py
+-rw-r--r--   0        0        0     2826 2024-05-20 12:48:19.357305 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticated_session_geo_ip.py
+-rw-r--r--   0        0        0     3865 2024-05-20 12:48:19.361305 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticated_session_user_agent.py
+-rw-r--r--   0        0        0     2646 2024-05-20 12:48:19.369305 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticated_session_user_agent_device.py
+-rw-r--r--   0        0        0     2792 2024-05-20 12:48:19.373305 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticated_session_user_agent_os.py
+-rw-r--r--   0        0        0     2725 2024-05-20 12:48:19.381305 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticated_session_user_agent_user_agent.py
+-rw-r--r--   0        0        0      895 2024-05-20 12:48:19.385305 authentik_client-2024.4.2.post1716209289/authentik_client/models/authentication_enum.py
+-rw-r--r--   0        0        0      782 2024-05-20 12:48:19.385305 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_attachment_enum.py
+-rw-r--r--   0        0        0     4686 2024-05-20 12:48:19.393305 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_duo_challenge.py
+-rw-r--r--   0        0        0     2743 2024-05-20 12:48:19.397305 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_duo_challenge_response_request.py
+-rw-r--r--   0        0        0     5327 2024-05-20 12:48:19.405305 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_duo_stage.py
+-rw-r--r--   0        0        0     2768 2024-05-20 12:48:19.409305 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_duo_stage_device_import_response.py
+-rw-r--r--   0        0        0     2785 2024-05-20 12:48:19.413305 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py
+-rw-r--r--   0        0        0     4744 2024-05-20 12:48:19.421305 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_duo_stage_request.py
+-rw-r--r--   0        0        0     4594 2024-05-20 12:48:19.425305 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_sms_challenge.py
+-rw-r--r--   0        0        0     3022 2024-05-20 12:48:19.429305 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_sms_challenge_response_request.py
+-rw-r--r--   0        0        0     6409 2024-05-20 12:48:19.437305 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_sms_stage.py
+-rw-r--r--   0        0        0     5595 2024-05-20 12:48:19.441305 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_sms_stage_request.py
+-rw-r--r--   0        0        0     4474 2024-05-20 12:48:19.449305 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_static_challenge.py
+-rw-r--r--   0        0        0     2761 2024-05-20 12:48:19.453306 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_static_challenge_response_request.py
+-rw-r--r--   0        0        0     5363 2024-05-20 12:48:19.457306 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_static_stage.py
+-rw-r--r--   0        0        0     4392 2024-05-20 12:48:19.461305 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_static_stage_request.py
+-rw-r--r--   0        0        0     4468 2024-05-20 12:48:19.465306 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_totp_challenge.py
+-rw-r--r--   0        0        0     2858 2024-05-20 12:48:19.469306 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_totp_challenge_response_request.py
+-rw-r--r--   0        0        0     5132 2024-05-20 12:48:19.477306 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_totp_stage.py
+-rw-r--r--   0        0        0     4201 2024-05-20 12:48:19.481306 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_totp_stage_request.py
+-rw-r--r--   0        0        0     6722 2024-05-20 12:48:19.485306 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_validate_stage.py
+-rw-r--r--   0        0        0     4893 2024-05-20 12:48:19.489306 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_validate_stage_request.py
+-rw-r--r--   0        0        0     5717 2024-05-20 12:48:19.493306 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_validation_challenge.py
+-rw-r--r--   0        0        0     3805 2024-05-20 12:48:19.501306 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_validation_challenge_response_request.py
+-rw-r--r--   0        0        0     4499 2024-05-20 12:48:19.505306 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_web_authn_challenge.py
+-rw-r--r--   0        0        0     2852 2024-05-20 12:48:19.509306 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_web_authn_challenge_response_request.py
+-rw-r--r--   0        0        0     7081 2024-05-20 12:48:19.513306 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_web_authn_stage.py
+-rw-r--r--   0        0        0     5302 2024-05-20 12:48:19.517306 authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_web_authn_stage_request.py
+-rw-r--r--   0        0        0     2718 2024-05-20 12:48:19.521306 authentik_client-2024.4.2.post1716209289/authentik_client/models/auto_submit_challenge_response_request.py
+-rw-r--r--   0        0        0     4388 2024-05-20 12:48:19.529306 authentik_client-2024.4.2.post1716209289/authentik_client/models/autosubmit_challenge.py
+-rw-r--r--   0        0        0      950 2024-05-20 12:48:19.533306 authentik_client-2024.4.2.post1716209289/authentik_client/models/backends_enum.py
+-rw-r--r--   0        0        0      748 2024-05-20 12:48:19.537306 authentik_client-2024.4.2.post1716209289/authentik_client/models/binding_type_enum.py
+-rw-r--r--   0        0        0     2995 2024-05-20 12:48:19.549306 authentik_client-2024.4.2.post1716209289/authentik_client/models/blueprint_file.py
+-rw-r--r--   0        0        0     4453 2024-05-20 12:48:19.553306 authentik_client-2024.4.2.post1716209289/authentik_client/models/blueprint_instance.py
+-rw-r--r--   0        0        0     3208 2024-05-20 12:48:19.557306 authentik_client-2024.4.2.post1716209289/authentik_client/models/blueprint_instance_request.py
+-rw-r--r--   0        0        0      836 2024-05-20 12:48:19.557306 authentik_client-2024.4.2.post1716209289/authentik_client/models/blueprint_instance_status_enum.py
+-rw-r--r--   0        0        0     6255 2024-05-20 12:48:19.561306 authentik_client-2024.4.2.post1716209289/authentik_client/models/brand.py
+-rw-r--r--   0        0        0     6307 2024-05-20 12:48:19.565306 authentik_client-2024.4.2.post1716209289/authentik_client/models/brand_request.py
+-rw-r--r--   0        0        0     2501 2024-05-20 12:48:19.569306 authentik_client-2024.4.2.post1716209289/authentik_client/models/cache.py
+-rw-r--r--   0        0        0      875 2024-05-20 12:48:19.573306 authentik_client-2024.4.2.post1716209289/authentik_client/models/capabilities_enum.py
+-rw-r--r--   0        0        0     4476 2024-05-20 12:48:19.577306 authentik_client-2024.4.2.post1716209289/authentik_client/models/captcha_challenge.py
+-rw-r--r--   0        0        0     2797 2024-05-20 12:48:19.581306 authentik_client-2024.4.2.post1716209289/authentik_client/models/captcha_challenge_response_request.py
+-rw-r--r--   0        0        0     4438 2024-05-20 12:48:19.585306 authentik_client-2024.4.2.post1716209289/authentik_client/models/captcha_stage.py
+-rw-r--r--   0        0        0     3774 2024-05-20 12:48:19.589306 authentik_client-2024.4.2.post1716209289/authentik_client/models/captcha_stage_request.py
+-rw-r--r--   0        0        0     2522 2024-05-20 12:48:19.593306 authentik_client-2024.4.2.post1716209289/authentik_client/models/certificate_data.py
+-rw-r--r--   0        0        0     2990 2024-05-20 12:48:19.597306 authentik_client-2024.4.2.post1716209289/authentik_client/models/certificate_generation_request.py
+-rw-r--r--   0        0        0     6655 2024-05-20 12:48:19.605306 authentik_client-2024.4.2.post1716209289/authentik_client/models/certificate_key_pair.py
+-rw-r--r--   0        0        0     2989 2024-05-20 12:48:19.609306 authentik_client-2024.4.2.post1716209289/authentik_client/models/certificate_key_pair_request.py
+-rw-r--r--   0        0        0      747 2024-05-20 12:48:19.613306 authentik_client-2024.4.2.post1716209289/authentik_client/models/challenge_choices.py
+-rw-r--r--   0        0        0    24236 2024-05-20 12:48:19.617306 authentik_client-2024.4.2.post1716209289/authentik_client/models/challenge_types.py
+-rw-r--r--   0        0        0      729 2024-05-20 12:48:19.621306 authentik_client-2024.4.2.post1716209289/authentik_client/models/client_type_enum.py
+-rw-r--r--   0        0        0     3539 2024-05-20 12:48:19.625306 authentik_client-2024.4.2.post1716209289/authentik_client/models/config.py
+-rw-r--r--   0        0        0     4021 2024-05-20 12:48:19.629306 authentik_client-2024.4.2.post1716209289/authentik_client/models/connection_token.py
+-rw-r--r--   0        0        0     2662 2024-05-20 12:48:19.629306 authentik_client-2024.4.2.post1716209289/authentik_client/models/connection_token_request.py
+-rw-r--r--   0        0        0     5736 2024-05-20 12:48:19.633306 authentik_client-2024.4.2.post1716209289/authentik_client/models/consent_challenge.py
+-rw-r--r--   0        0        0     2838 2024-05-20 12:48:19.637306 authentik_client-2024.4.2.post1716209289/authentik_client/models/consent_challenge_response_request.py
+-rw-r--r--   0        0        0     2513 2024-05-20 12:48:19.641306 authentik_client-2024.4.2.post1716209289/authentik_client/models/consent_permission.py
+-rw-r--r--   0        0        0     4511 2024-05-20 12:48:19.645306 authentik_client-2024.4.2.post1716209289/authentik_client/models/consent_stage.py
+-rw-r--r--   0        0        0      783 2024-05-20 12:48:19.645306 authentik_client-2024.4.2.post1716209289/authentik_client/models/consent_stage_mode_enum.py
+-rw-r--r--   0        0        0     3569 2024-05-20 12:48:19.649306 authentik_client-2024.4.2.post1716209289/authentik_client/models/consent_stage_request.py
+-rw-r--r--   0        0        0     2891 2024-05-20 12:48:19.653307 authentik_client-2024.4.2.post1716209289/authentik_client/models/contextual_flow_info.py
+-rw-r--r--   0        0        0      879 2024-05-20 12:48:19.657307 authentik_client-2024.4.2.post1716209289/authentik_client/models/contextual_flow_info_layout_enum.py
+-rw-r--r--   0        0        0     2657 2024-05-20 12:48:19.657307 authentik_client-2024.4.2.post1716209289/authentik_client/models/coordinate.py
+-rw-r--r--   0        0        0     4704 2024-05-20 12:48:19.661306 authentik_client-2024.4.2.post1716209289/authentik_client/models/current_brand.py
+-rw-r--r--   0        0        0      771 2024-05-20 12:48:19.665307 authentik_client-2024.4.2.post1716209289/authentik_client/models/denied_action_enum.py
+-rw-r--r--   0        0        0     4200 2024-05-20 12:48:19.669307 authentik_client-2024.4.2.post1716209289/authentik_client/models/deny_stage.py
+-rw-r--r--   0        0        0     3230 2024-05-20 12:48:19.673307 authentik_client-2024.4.2.post1716209289/authentik_client/models/deny_stage_request.py
+-rw-r--r--   0        0        0     3522 2024-05-20 12:48:19.677307 authentik_client-2024.4.2.post1716209289/authentik_client/models/device.py
+-rw-r--r--   0        0        0     2657 2024-05-20 12:48:19.681307 authentik_client-2024.4.2.post1716209289/authentik_client/models/device_challenge.py
+-rw-r--r--   0        0        0     2792 2024-05-20 12:48:19.685307 authentik_client-2024.4.2.post1716209289/authentik_client/models/device_challenge_request.py
+-rw-r--r--   0        0        0      780 2024-05-20 12:48:19.689307 authentik_client-2024.4.2.post1716209289/authentik_client/models/device_classes_enum.py
+-rw-r--r--   0        0        0     1244 2024-05-20 12:48:19.689307 authentik_client-2024.4.2.post1716209289/authentik_client/models/digest_algorithm_enum.py
+-rw-r--r--   0        0        0      695 2024-05-20 12:48:19.693307 authentik_client-2024.4.2.post1716209289/authentik_client/models/digits_enum.py
+-rw-r--r--   0        0        0     4969 2024-05-20 12:48:19.697307 authentik_client-2024.4.2.post1716209289/authentik_client/models/docker_service_connection.py
+-rw-r--r--   0        0        0     4087 2024-05-20 12:48:19.697307 authentik_client-2024.4.2.post1716209289/authentik_client/models/docker_service_connection_request.py
+-rw-r--r--   0        0        0     2847 2024-05-20 12:48:19.701307 authentik_client-2024.4.2.post1716209289/authentik_client/models/domain.py
+-rw-r--r--   0        0        0     2746 2024-05-20 12:48:19.705307 authentik_client-2024.4.2.post1716209289/authentik_client/models/domain_request.py
+-rw-r--r--   0        0        0     4155 2024-05-20 12:48:19.709307 authentik_client-2024.4.2.post1716209289/authentik_client/models/dummy_challenge.py
+-rw-r--r--   0        0        0     2681 2024-05-20 12:48:19.713307 authentik_client-2024.4.2.post1716209289/authentik_client/models/dummy_challenge_response_request.py
+-rw-r--r--   0        0        0     4515 2024-05-20 12:48:19.717307 authentik_client-2024.4.2.post1716209289/authentik_client/models/dummy_policy.py
+-rw-r--r--   0        0        0     3237 2024-05-20 12:48:19.721307 authentik_client-2024.4.2.post1716209289/authentik_client/models/dummy_policy_request.py
+-rw-r--r--   0        0        0     4213 2024-05-20 12:48:19.725307 authentik_client-2024.4.2.post1716209289/authentik_client/models/dummy_stage.py
+-rw-r--r--   0        0        0     3232 2024-05-20 12:48:19.729307 authentik_client-2024.4.2.post1716209289/authentik_client/models/dummy_stage_request.py
+-rw-r--r--   0        0        0     2720 2024-05-20 12:48:19.733307 authentik_client-2024.4.2.post1716209289/authentik_client/models/duo_device.py
+-rw-r--r--   0        0        0     2575 2024-05-20 12:48:19.737307 authentik_client-2024.4.2.post1716209289/authentik_client/models/duo_device_enrollment_status.py
+-rw-r--r--   0        0        0     2619 2024-05-20 12:48:19.741307 authentik_client-2024.4.2.post1716209289/authentik_client/models/duo_device_request.py
+-rw-r--r--   0        0        0      748 2024-05-20 12:48:19.745307 authentik_client-2024.4.2.post1716209289/authentik_client/models/duo_response_enum.py
+-rw-r--r--   0        0        0     4090 2024-05-20 12:48:19.753307 authentik_client-2024.4.2.post1716209289/authentik_client/models/email_challenge.py
+-rw-r--r--   0        0        0     2770 2024-05-20 12:48:19.757307 authentik_client-2024.4.2.post1716209289/authentik_client/models/email_challenge_response_request.py
+-rw-r--r--   0        0        0     5902 2024-05-20 12:48:19.761307 authentik_client-2024.4.2.post1716209289/authentik_client/models/email_stage.py
+-rw-r--r--   0        0        0     5121 2024-05-20 12:48:19.765307 authentik_client-2024.4.2.post1716209289/authentik_client/models/email_stage_request.py
+-rw-r--r--   0        0        0     4707 2024-05-20 12:48:19.769307 authentik_client-2024.4.2.post1716209289/authentik_client/models/endpoint.py
+-rw-r--r--   0        0        0     3678 2024-05-20 12:48:19.773307 authentik_client-2024.4.2.post1716209289/authentik_client/models/endpoint_request.py
+-rw-r--r--   0        0        0     2530 2024-05-20 12:48:19.777307 authentik_client-2024.4.2.post1716209289/authentik_client/models/error_detail.py
+-rw-r--r--   0        0        0     3309 2024-05-20 12:48:19.781307 authentik_client-2024.4.2.post1716209289/authentik_client/models/error_reporting_config.py
+-rw-r--r--   0        0        0     4129 2024-05-20 12:48:19.785307 authentik_client-2024.4.2.post1716209289/authentik_client/models/event.py
+-rw-r--r--   0        0        0     1730 2024-05-20 12:48:19.789307 authentik_client-2024.4.2.post1716209289/authentik_client/models/event_actions.py
+-rw-r--r--   0        0        0     6006 2024-05-20 12:48:19.789307 authentik_client-2024.4.2.post1716209289/authentik_client/models/event_matcher_policy.py
+-rw-r--r--   0        0        0     4807 2024-05-20 12:48:19.793307 authentik_client-2024.4.2.post1716209289/authentik_client/models/event_matcher_policy_request.py
+-rw-r--r--   0        0        0     3990 2024-05-20 12:48:19.797307 authentik_client-2024.4.2.post1716209289/authentik_client/models/event_request.py
+-rw-r--r--   0        0        0     2697 2024-05-20 12:48:19.801307 authentik_client-2024.4.2.post1716209289/authentik_client/models/event_top_per_user.py
+-rw-r--r--   0        0        0     3926 2024-05-20 12:48:19.805307 authentik_client-2024.4.2.post1716209289/authentik_client/models/expiring_base_grant_model.py
+-rw-r--r--   0        0        0     4191 2024-05-20 12:48:19.809307 authentik_client-2024.4.2.post1716209289/authentik_client/models/expression_policy.py
+-rw-r--r--   0        0        0     2992 2024-05-20 12:48:19.813307 authentik_client-2024.4.2.post1716209289/authentik_client/models/expression_policy_request.py
+-rw-r--r--   0        0        0     4524 2024-05-20 12:48:19.817307 authentik_client-2024.4.2.post1716209289/authentik_client/models/extra_role_object_permission.py
+-rw-r--r--   0        0        0     4524 2024-05-20 12:48:19.821307 authentik_client-2024.4.2.post1716209289/authentik_client/models/extra_user_object_permission.py
+-rw-r--r--   0        0        0     2519 2024-05-20 12:48:19.825307 authentik_client-2024.4.2.post1716209289/authentik_client/models/file_path_request.py
+-rw-r--r--   0        0        0     6047 2024-05-20 12:48:19.833307 authentik_client-2024.4.2.post1716209289/authentik_client/models/flow.py
+-rw-r--r--   0        0        0    25850 2024-05-20 12:48:19.837307 authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_challenge_response_request.py
+-rw-r--r--   0        0        0      934 2024-05-20 12:48:19.841307 authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_designation_enum.py
+-rw-r--r--   0        0        0     2533 2024-05-20 12:48:19.845307 authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_diagram.py
+-rw-r--r--   0        0        0     4505 2024-05-20 12:48:19.849307 authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_error_challenge.py
+-rw-r--r--   0        0        0     3111 2024-05-20 12:48:19.853308 authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_import_result.py
+-rw-r--r--   0        0        0     3418 2024-05-20 12:48:19.857308 authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_inspection.py
+-rw-r--r--   0        0        0     3875 2024-05-20 12:48:19.861307 authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_inspector_plan.py
+-rw-r--r--   0        0        0      837 2024-05-20 12:48:19.865307 authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_layout_enum.py
+-rw-r--r--   0        0        0     4741 2024-05-20 12:48:19.869308 authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_request.py
+-rw-r--r--   0        0        0     5223 2024-05-20 12:48:19.873308 authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_set.py
+-rw-r--r--   0        0        0     4459 2024-05-20 12:48:19.877308 authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_set_request.py
+-rw-r--r--   0        0        0     4763 2024-05-20 12:48:19.881308 authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_stage_binding.py
+-rw-r--r--   0        0        0     3983 2024-05-20 12:48:19.885308 authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_stage_binding_request.py
+-rw-r--r--   0        0        0     2641 2024-05-20 12:48:19.889308 authentik_client-2024.4.2.post1716209289/authentik_client/models/footer_link.py
+-rw-r--r--   0        0        0     2531 2024-05-20 12:48:19.893308 authentik_client-2024.4.2.post1716209289/authentik_client/models/generic_error.py
+-rw-r--r--   0        0        0      865 2024-05-20 12:48:19.893308 authentik_client-2024.4.2.post1716209289/authentik_client/models/geoip_binding_enum.py
+-rw-r--r--   0        0        0     6418 2024-05-20 12:48:19.901308 authentik_client-2024.4.2.post1716209289/authentik_client/models/google_workspace_provider.py
+-rw-r--r--   0        0        0     3083 2024-05-20 12:48:19.905308 authentik_client-2024.4.2.post1716209289/authentik_client/models/google_workspace_provider_group.py
+-rw-r--r--   0        0        0     2526 2024-05-20 12:48:19.905308 authentik_client-2024.4.2.post1716209289/authentik_client/models/google_workspace_provider_group_request.py
+-rw-r--r--   0        0        0     4324 2024-05-20 12:48:19.917308 authentik_client-2024.4.2.post1716209289/authentik_client/models/google_workspace_provider_mapping.py
+-rw-r--r--   0        0        0     3385 2024-05-20 12:48:19.921308 authentik_client-2024.4.2.post1716209289/authentik_client/models/google_workspace_provider_mapping_request.py
+-rw-r--r--   0        0        0     4740 2024-05-20 12:48:19.925308 authentik_client-2024.4.2.post1716209289/authentik_client/models/google_workspace_provider_request.py
+-rw-r--r--   0        0        0     3084 2024-05-20 12:48:19.929308 authentik_client-2024.4.2.post1716209289/authentik_client/models/google_workspace_provider_user.py
+-rw-r--r--   0        0        0     2518 2024-05-20 12:48:19.933308 authentik_client-2024.4.2.post1716209289/authentik_client/models/google_workspace_provider_user_request.py
+-rw-r--r--   0        0        0     5445 2024-05-20 12:48:19.937308 authentik_client-2024.4.2.post1716209289/authentik_client/models/group.py
+-rw-r--r--   0        0        0     4209 2024-05-20 12:48:19.941308 authentik_client-2024.4.2.post1716209289/authentik_client/models/group_member.py
+-rw-r--r--   0        0        0     4006 2024-05-20 12:48:19.949308 authentik_client-2024.4.2.post1716209289/authentik_client/models/group_member_request.py
+-rw-r--r--   0        0        0     3347 2024-05-20 12:48:19.953308 authentik_client-2024.4.2.post1716209289/authentik_client/models/group_request.py
+-rw-r--r--   0        0        0     6080 2024-05-20 12:48:19.957308 authentik_client-2024.4.2.post1716209289/authentik_client/models/identification_challenge.py
+-rw-r--r--   0        0        0     3174 2024-05-20 12:48:19.961308 authentik_client-2024.4.2.post1716209289/authentik_client/models/identification_challenge_response_request.py
+-rw-r--r--   0        0        0     7503 2024-05-20 12:48:19.965308 authentik_client-2024.4.2.post1716209289/authentik_client/models/identification_stage.py
+-rw-r--r--   0        0        0     6533 2024-05-20 12:48:19.969308 authentik_client-2024.4.2.post1716209289/authentik_client/models/identification_stage_request.py
+-rw-r--r--   0        0        0     2438 2024-05-20 12:48:19.973308 authentik_client-2024.4.2.post1716209289/authentik_client/models/install_id.py
+-rw-r--r--   0        0        0      771 2024-05-20 12:48:19.977308 authentik_client-2024.4.2.post1716209289/authentik_client/models/intent_enum.py
+-rw-r--r--   0        0        0      800 2024-05-20 12:48:19.977308 authentik_client-2024.4.2.post1716209289/authentik_client/models/invalid_response_action_enum.py
+-rw-r--r--   0        0        0     4878 2024-05-20 12:48:19.985308 authentik_client-2024.4.2.post1716209289/authentik_client/models/invitation.py
+-rw-r--r--   0        0        0     3895 2024-05-20 12:48:19.989308 authentik_client-2024.4.2.post1716209289/authentik_client/models/invitation_request.py
+-rw-r--r--   0        0        0     4508 2024-05-20 12:48:19.993308 authentik_client-2024.4.2.post1716209289/authentik_client/models/invitation_stage.py
+-rw-r--r--   0        0        0     3527 2024-05-20 12:48:19.997308 authentik_client-2024.4.2.post1716209289/authentik_client/models/invitation_stage_request.py
+-rw-r--r--   0        0        0      729 2024-05-20 12:48:20.001308 authentik_client-2024.4.2.post1716209289/authentik_client/models/issuer_mode_enum.py
+-rw-r--r--   0        0        0     4386 2024-05-20 12:48:20.005308 authentik_client-2024.4.2.post1716209289/authentik_client/models/kubernetes_service_connection.py
+-rw-r--r--   0        0        0     3454 2024-05-20 12:48:20.009308 authentik_client-2024.4.2.post1716209289/authentik_client/models/kubernetes_service_connection_request.py
+-rw-r--r--   0        0        0     2811 2024-05-20 12:48:20.013308 authentik_client-2024.4.2.post1716209289/authentik_client/models/ldap_debug.py
+-rw-r--r--   0        0        0     5765 2024-05-20 12:48:20.017308 authentik_client-2024.4.2.post1716209289/authentik_client/models/ldap_outpost_config.py
+-rw-r--r--   0        0        0     4378 2024-05-20 12:48:20.021308 authentik_client-2024.4.2.post1716209289/authentik_client/models/ldap_property_mapping.py
+-rw-r--r--   0        0        0     3478 2024-05-20 12:48:20.025308 authentik_client-2024.4.2.post1716209289/authentik_client/models/ldap_property_mapping_request.py
+-rw-r--r--   0        0        0     8694 2024-05-20 12:48:20.033308 authentik_client-2024.4.2.post1716209289/authentik_client/models/ldap_provider.py
+-rw-r--r--   0        0        0     6192 2024-05-20 12:48:20.037308 authentik_client-2024.4.2.post1716209289/authentik_client/models/ldap_provider_request.py
+-rw-r--r--   0        0        0    11791 2024-05-20 12:48:20.041308 authentik_client-2024.4.2.post1716209289/authentik_client/models/ldap_source.py
+-rw-r--r--   0        0        0     9542 2024-05-20 12:48:20.045308 authentik_client-2024.4.2.post1716209289/authentik_client/models/ldap_source_request.py
+-rw-r--r--   0        0        0      726 2024-05-20 12:48:20.009308 authentik_client-2024.4.2.post1716209289/authentik_client/models/ldapapi_access_mode.py
+-rw-r--r--   0        0        0     3278 2024-05-20 12:48:20.049308 authentik_client-2024.4.2.post1716209289/authentik_client/models/license.py
+-rw-r--r--   0        0        0     2897 2024-05-20 12:48:20.053309 authentik_client-2024.4.2.post1716209289/authentik_client/models/license_forecast.py
+-rw-r--r--   0        0        0     2509 2024-05-20 12:48:20.057309 authentik_client-2024.4.2.post1716209289/authentik_client/models/license_request.py
+-rw-r--r--   0        0        0     3222 2024-05-20 12:48:20.061308 authentik_client-2024.4.2.post1716209289/authentik_client/models/license_summary.py
+-rw-r--r--   0        0        0     2411 2024-05-20 12:48:20.065308 authentik_client-2024.4.2.post1716209289/authentik_client/models/link.py
+-rw-r--r--   0        0        0     2882 2024-05-20 12:48:20.069309 authentik_client-2024.4.2.post1716209289/authentik_client/models/log_event.py
+-rw-r--r--   0        0        0      843 2024-05-20 12:48:20.069309 authentik_client-2024.4.2.post1716209289/authentik_client/models/log_level_enum.py
+-rw-r--r--   0        0        0     6520 2024-05-20 12:48:20.073309 authentik_client-2024.4.2.post1716209289/authentik_client/models/login_challenge_types.py
+-rw-r--r--   0        0        0     4171 2024-05-20 12:48:20.077309 authentik_client-2024.4.2.post1716209289/authentik_client/models/login_metrics.py
+-rw-r--r--   0        0        0     3192 2024-05-20 12:48:20.081309 authentik_client-2024.4.2.post1716209289/authentik_client/models/login_source.py
+-rw-r--r--   0        0        0     2513 2024-05-20 12:48:20.085309 authentik_client-2024.4.2.post1716209289/authentik_client/models/metadata.py
+-rw-r--r--   0        0        0     5920 2024-05-20 12:48:20.089309 authentik_client-2024.4.2.post1716209289/authentik_client/models/microsoft_entra_provider.py
+-rw-r--r--   0        0        0     3079 2024-05-20 12:48:20.093309 authentik_client-2024.4.2.post1716209289/authentik_client/models/microsoft_entra_provider_group.py
+-rw-r--r--   0        0        0     2522 2024-05-20 12:48:20.097309 authentik_client-2024.4.2.post1716209289/authentik_client/models/microsoft_entra_provider_group_request.py
+-rw-r--r--   0        0        0     4320 2024-05-20 12:48:20.101309 authentik_client-2024.4.2.post1716209289/authentik_client/models/microsoft_entra_provider_mapping.py
+-rw-r--r--   0        0        0     3381 2024-05-20 12:48:20.105309 authentik_client-2024.4.2.post1716209289/authentik_client/models/microsoft_entra_provider_mapping_request.py
+-rw-r--r--   0        0        0     4307 2024-05-20 12:48:20.109309 authentik_client-2024.4.2.post1716209289/authentik_client/models/microsoft_entra_provider_request.py
+-rw-r--r--   0        0        0     3080 2024-05-20 12:48:20.113309 authentik_client-2024.4.2.post1716209289/authentik_client/models/microsoft_entra_provider_user.py
+-rw-r--r--   0        0        0     2514 2024-05-20 12:48:20.117309 authentik_client-2024.4.2.post1716209289/authentik_client/models/microsoft_entra_provider_user_request.py
+-rw-r--r--   0        0        0     8160 2024-05-20 12:48:20.117309 authentik_client-2024.4.2.post1716209289/authentik_client/models/model_enum.py
+-rw-r--r--   0        0        0    11885 2024-05-20 12:48:20.121309 authentik_client-2024.4.2.post1716209289/authentik_client/models/model_request.py
+-rw-r--r--   0        0        0     1559 2024-05-20 12:48:20.125309 authentik_client-2024.4.2.post1716209289/authentik_client/models/name_id_policy_enum.py
+-rw-r--r--   0        0        0      831 2024-05-20 12:48:20.129309 authentik_client-2024.4.2.post1716209289/authentik_client/models/network_binding_enum.py
+-rw-r--r--   0        0        0      764 2024-05-20 12:48:20.129309 authentik_client-2024.4.2.post1716209289/authentik_client/models/not_configured_action_enum.py
+-rw-r--r--   0        0        0     3479 2024-05-20 12:48:20.133309 authentik_client-2024.4.2.post1716209289/authentik_client/models/notification.py
+-rw-r--r--   0        0        0     2858 2024-05-20 12:48:20.137309 authentik_client-2024.4.2.post1716209289/authentik_client/models/notification_request.py
+-rw-r--r--   0        0        0     4010 2024-05-20 12:48:20.141309 authentik_client-2024.4.2.post1716209289/authentik_client/models/notification_rule.py
+-rw-r--r--   0        0        0     3549 2024-05-20 12:48:20.145309 authentik_client-2024.4.2.post1716209289/authentik_client/models/notification_rule_request.py
+-rw-r--r--   0        0        0     3760 2024-05-20 12:48:20.145309 authentik_client-2024.4.2.post1716209289/authentik_client/models/notification_transport.py
+-rw-r--r--   0        0        0      818 2024-05-20 12:48:20.149309 authentik_client-2024.4.2.post1716209289/authentik_client/models/notification_transport_mode_enum.py
+-rw-r--r--   0        0        0     3500 2024-05-20 12:48:20.153309 authentik_client-2024.4.2.post1716209289/authentik_client/models/notification_transport_request.py
+-rw-r--r--   0        0        0     2503 2024-05-20 12:48:20.157309 authentik_client-2024.4.2.post1716209289/authentik_client/models/notification_transport_test.py
+-rw-r--r--   0        0        0     2707 2024-05-20 12:48:20.161309 authentik_client-2024.4.2.post1716209289/authentik_client/models/notification_webhook_mapping.py
+-rw-r--r--   0        0        0     2717 2024-05-20 12:48:20.161309 authentik_client-2024.4.2.post1716209289/authentik_client/models/notification_webhook_mapping_request.py
+-rw-r--r--   0        0        0     8888 2024-05-20 12:48:20.165309 authentik_client-2024.4.2.post1716209289/authentik_client/models/o_auth2_provider.py
+-rw-r--r--   0        0        0     6654 2024-05-20 12:48:20.169309 authentik_client-2024.4.2.post1716209289/authentik_client/models/o_auth2_provider_request.py
+-rw-r--r--   0        0        0     3482 2024-05-20 12:48:20.173309 authentik_client-2024.4.2.post1716209289/authentik_client/models/o_auth2_provider_setup_urls.py
+-rw-r--r--   0        0        0     4164 2024-05-20 12:48:20.177309 authentik_client-2024.4.2.post1716209289/authentik_client/models/o_auth_device_code_challenge.py
+-rw-r--r--   0        0        0     2846 2024-05-20 12:48:20.181309 authentik_client-2024.4.2.post1716209289/authentik_client/models/o_auth_device_code_challenge_response_request.py
+-rw-r--r--   0        0        0     4213 2024-05-20 12:48:20.185309 authentik_client-2024.4.2.post1716209289/authentik_client/models/o_auth_device_code_finish_challenge.py
+-rw-r--r--   0        0        0     2816 2024-05-20 12:48:20.189309 authentik_client-2024.4.2.post1716209289/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py
+-rw-r--r--   0        0        0    10563 2024-05-20 12:48:20.193309 authentik_client-2024.4.2.post1716209289/authentik_client/models/o_auth_source.py
+-rw-r--r--   0        0        0     8013 2024-05-20 12:48:20.201309 authentik_client-2024.4.2.post1716209289/authentik_client/models/o_auth_source_request.py
+-rw-r--r--   0        0        0     3922 2024-05-20 12:48:20.205309 authentik_client-2024.4.2.post1716209289/authentik_client/models/open_id_connect_configuration.py
+-rw-r--r--   0        0        0      779 2024-05-20 12:48:20.205309 authentik_client-2024.4.2.post1716209289/authentik_client/models/outgoing_sync_delete_action.py
+-rw-r--r--   0        0        0     5545 2024-05-20 12:48:20.209309 authentik_client-2024.4.2.post1716209289/authentik_client/models/outpost.py
+-rw-r--r--   0        0        0     2541 2024-05-20 12:48:20.213309 authentik_client-2024.4.2.post1716209289/authentik_client/models/outpost_default_config.py
+-rw-r--r--   0        0        0     3755 2024-05-20 12:48:20.217309 authentik_client-2024.4.2.post1716209289/authentik_client/models/outpost_health.py
+-rw-r--r--   0        0        0     4050 2024-05-20 12:48:20.221309 authentik_client-2024.4.2.post1716209289/authentik_client/models/outpost_request.py
+-rw-r--r--   0        0        0      752 2024-05-20 12:48:20.221309 authentik_client-2024.4.2.post1716209289/authentik_client/models/outpost_type_enum.py
+-rw-r--r--   0        0        0     3322 2024-05-20 12:48:20.225309 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_application_list.py
+-rw-r--r--   0        0        0     3395 2024-05-20 12:48:20.229309 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_authenticated_session_list.py
+-rw-r--r--   0        0        0     3404 2024-05-20 12:48:20.233309 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_authenticator_duo_stage_list.py
+-rw-r--r--   0        0        0     3404 2024-05-20 12:48:20.237309 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_authenticator_sms_stage_list.py
+-rw-r--r--   0        0        0     3428 2024-05-20 12:48:20.241310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_authenticator_static_stage_list.py
+-rw-r--r--   0        0        0     3412 2024-05-20 12:48:20.245309 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_authenticator_totp_stage_list.py
+-rw-r--r--   0        0        0     3444 2024-05-20 12:48:20.249309 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_authenticator_validate_stage_list.py
+-rw-r--r--   0        0        0     3445 2024-05-20 12:48:20.253309 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_authenticator_web_authn_stage_list.py
+-rw-r--r--   0        0        0     3371 2024-05-20 12:48:20.253309 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_blueprint_instance_list.py
+-rw-r--r--   0        0        0     3274 2024-05-20 12:48:20.257310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_brand_list.py
+-rw-r--r--   0        0        0     3331 2024-05-20 12:48:20.261309 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_captcha_stage_list.py
+-rw-r--r--   0        0        0     3380 2024-05-20 12:48:20.265309 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_certificate_key_pair_list.py
+-rw-r--r--   0        0        0     3355 2024-05-20 12:48:20.269310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_connection_token_list.py
+-rw-r--r--   0        0        0     3331 2024-05-20 12:48:20.277310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_consent_stage_list.py
+-rw-r--r--   0        0        0     3307 2024-05-20 12:48:20.277310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_deny_stage_list.py
+-rw-r--r--   0        0        0     3420 2024-05-20 12:48:20.281310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_docker_service_connection_list.py
+-rw-r--r--   0        0        0     3282 2024-05-20 12:48:20.285310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_domain_list.py
+-rw-r--r--   0        0        0     3323 2024-05-20 12:48:20.289310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_dummy_policy_list.py
+-rw-r--r--   0        0        0     3315 2024-05-20 12:48:20.293310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_dummy_stage_list.py
+-rw-r--r--   0        0        0     3307 2024-05-20 12:48:20.297310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_duo_device_list.py
+-rw-r--r--   0        0        0     3315 2024-05-20 12:48:20.301310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_email_stage_list.py
+-rw-r--r--   0        0        0     3298 2024-05-20 12:48:20.301310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_endpoint_list.py
+-rw-r--r--   0        0        0     3274 2024-05-20 12:48:20.305310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_event_list.py
+-rw-r--r--   0        0        0     3380 2024-05-20 12:48:20.309310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_event_matcher_policy_list.py
+-rw-r--r--   0        0        0     3413 2024-05-20 12:48:20.313310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_expiring_base_grant_model_list.py
+-rw-r--r--   0        0        0     3363 2024-05-20 12:48:20.317310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_expression_policy_list.py
+-rw-r--r--   0        0        0     3437 2024-05-20 12:48:20.317310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_extra_role_object_permission_list.py
+-rw-r--r--   0        0        0     3437 2024-05-20 12:48:20.321310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_extra_user_object_permission_list.py
+-rw-r--r--   0        0        0     3266 2024-05-20 12:48:20.325310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_flow_list.py
+-rw-r--r--   0        0        0     3364 2024-05-20 12:48:20.329310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_flow_stage_binding_list.py
+-rw-r--r--   0        0        0     3461 2024-05-20 12:48:20.333310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_google_workspace_provider_group_list.py
+-rw-r--r--   0        0        0     3420 2024-05-20 12:48:20.337310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_google_workspace_provider_list.py
+-rw-r--r--   0        0        0     3477 2024-05-20 12:48:20.341310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_google_workspace_provider_mapping_list.py
+-rw-r--r--   0        0        0     3453 2024-05-20 12:48:20.345310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_google_workspace_provider_user_list.py
+-rw-r--r--   0        0        0     3274 2024-05-20 12:48:20.345310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_group_list.py
+-rw-r--r--   0        0        0     3387 2024-05-20 12:48:20.349310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_identification_stage_list.py
+-rw-r--r--   0        0        0     3314 2024-05-20 12:48:20.353310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_invitation_list.py
+-rw-r--r--   0        0        0     3355 2024-05-20 12:48:20.357310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_invitation_stage_list.py
+-rw-r--r--   0        0        0     3452 2024-05-20 12:48:20.357310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_kubernetes_service_connection_list.py
+-rw-r--r--   0        0        0     3372 2024-05-20 12:48:20.361310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_ldap_outpost_config_list.py
+-rw-r--r--   0        0        0     3388 2024-05-20 12:48:20.365310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_ldap_property_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-05-20 12:48:20.369310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_ldap_provider_list.py
+-rw-r--r--   0        0        0     3315 2024-05-20 12:48:20.373310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_ldap_source_list.py
+-rw-r--r--   0        0        0     3290 2024-05-20 12:48:20.373310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_license_list.py
+-rw-r--r--   0        0        0     3453 2024-05-20 12:48:20.377310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_microsoft_entra_provider_group_list.py
+-rw-r--r--   0        0        0     3412 2024-05-20 12:48:20.381310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_microsoft_entra_provider_list.py
+-rw-r--r--   0        0        0     3469 2024-05-20 12:48:20.385310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_microsoft_entra_provider_mapping_list.py
+-rw-r--r--   0        0        0     3445 2024-05-20 12:48:20.389310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_microsoft_entra_provider_user_list.py
+-rw-r--r--   0        0        0     3330 2024-05-20 12:48:20.393310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_notification_list.py
+-rw-r--r--   0        0        0     3363 2024-05-20 12:48:20.393310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_notification_rule_list.py
+-rw-r--r--   0        0        0     3403 2024-05-20 12:48:20.397310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_notification_transport_list.py
+-rw-r--r--   0        0        0     3444 2024-05-20 12:48:20.401310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_notification_webhook_mapping_list.py
+-rw-r--r--   0        0        0     3348 2024-05-20 12:48:20.405310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_o_auth2_provider_list.py
+-rw-r--r--   0        0        0     3324 2024-05-20 12:48:20.409310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_o_auth_source_list.py
+-rw-r--r--   0        0        0     3290 2024-05-20 12:48:20.413310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_outpost_list.py
+-rw-r--r--   0        0        0     3396 2024-05-20 12:48:20.413310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_password_expiry_policy_list.py
+-rw-r--r--   0        0        0     3347 2024-05-20 12:48:20.417310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_password_policy_list.py
+-rw-r--r--   0        0        0     3339 2024-05-20 12:48:20.421310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_password_stage_list.py
+-rw-r--r--   0        0        0     3314 2024-05-20 12:48:20.425310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_permission_list.py
+-rw-r--r--   0        0        0     3396 2024-05-20 12:48:20.429310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_plex_source_connection_list.py
+-rw-r--r--   0        0        0     3315 2024-05-20 12:48:20.429310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_plex_source_list.py
+-rw-r--r--   0        0        0     3339 2024-05-20 12:48:20.433310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_policy_binding_list.py
+-rw-r--r--   0        0        0     3282 2024-05-20 12:48:20.437310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_policy_list.py
+-rw-r--r--   0        0        0     3282 2024-05-20 12:48:20.441311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_prompt_list.py
+-rw-r--r--   0        0        0     3323 2024-05-20 12:48:20.445310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_prompt_stage_list.py
+-rw-r--r--   0        0        0     3355 2024-05-20 12:48:20.449310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_property_mapping_list.py
+-rw-r--r--   0        0        0     3298 2024-05-20 12:48:20.449310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_provider_list.py
+-rw-r--r--   0        0        0     3380 2024-05-20 12:48:20.453310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_proxy_outpost_config_list.py
+-rw-r--r--   0        0        0     3339 2024-05-20 12:48:20.457311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_proxy_provider_list.py
+-rw-r--r--   0        0        0     3380 2024-05-20 12:48:20.461310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_rac_property_mapping_list.py
+-rw-r--r--   0        0        0     3323 2024-05-20 12:48:20.465310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_rac_provider_list.py
+-rw-r--r--   0        0        0     3388 2024-05-20 12:48:20.465310 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_radius_outpost_config_list.py
+-rw-r--r--   0        0        0     3347 2024-05-20 12:48:20.469311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_radius_provider_list.py
+-rw-r--r--   0        0        0     3314 2024-05-20 12:48:20.473311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_reputation_list.py
+-rw-r--r--   0        0        0     3363 2024-05-20 12:48:20.477311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_reputation_policy_list.py
+-rw-r--r--   0        0        0     3461 2024-05-20 12:48:20.477311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_role_assigned_object_permission_list.py
+-rw-r--r--   0        0        0     3266 2024-05-20 12:48:20.481311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_role_list.py
+-rw-r--r--   0        0        0     3388 2024-05-20 12:48:20.485311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_saml_property_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-05-20 12:48:20.489311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_saml_provider_list.py
+-rw-r--r--   0        0        0     3315 2024-05-20 12:48:20.489311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_saml_source_list.py
+-rw-r--r--   0        0        0     3323 2024-05-20 12:48:20.493311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_scim_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-05-20 12:48:20.497311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_scim_provider_list.py
+-rw-r--r--   0        0        0     3356 2024-05-20 12:48:20.501311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_scim_source_group_list.py
+-rw-r--r--   0        0        0     3315 2024-05-20 12:48:20.501311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_scim_source_list.py
+-rw-r--r--   0        0        0     3348 2024-05-20 12:48:20.505311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_scim_source_user_list.py
+-rw-r--r--   0        0        0     3331 2024-05-20 12:48:20.513311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_scope_mapping_list.py
+-rw-r--r--   0        0        0     3371 2024-05-20 12:48:20.517311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_service_connection_list.py
+-rw-r--r--   0        0        0     3307 2024-05-20 12:48:20.509311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_sms_device_list.py
+-rw-r--r--   0        0        0     3282 2024-05-20 12:48:20.521311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_source_list.py
+-rw-r--r--   0        0        0     3323 2024-05-20 12:48:20.525311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_source_stage_list.py
+-rw-r--r--   0        0        0     3274 2024-05-20 12:48:20.525311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_stage_list.py
+-rw-r--r--   0        0        0     3331 2024-05-20 12:48:20.533311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_static_device_list.py
+-rw-r--r--   0        0        0     3315 2024-05-20 12:48:20.533311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_system_task_list.py
+-rw-r--r--   0        0        0     3282 2024-05-20 12:48:20.541311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_tenant_list.py
+-rw-r--r--   0        0        0     3274 2024-05-20 12:48:20.545311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_token_list.py
+-rw-r--r--   0        0        0     3315 2024-05-20 12:48:20.549311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_token_model_list.py
+-rw-r--r--   0        0        0     3315 2024-05-20 12:48:20.537311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_totp_device_list.py
+-rw-r--r--   0        0        0     3461 2024-05-20 12:48:20.553311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_user_assigned_object_permission_list.py
+-rw-r--r--   0        0        0     3323 2024-05-20 12:48:20.553311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_user_consent_list.py
+-rw-r--r--   0        0        0     3356 2024-05-20 12:48:20.557311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_user_delete_stage_list.py
+-rw-r--r--   0        0        0     3266 2024-05-20 12:48:20.561311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_user_list.py
+-rw-r--r--   0        0        0     3348 2024-05-20 12:48:20.565311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_user_login_stage_list.py
+-rw-r--r--   0        0        0     3356 2024-05-20 12:48:20.565311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_user_logout_stage_list.py
+-rw-r--r--   0        0        0     3438 2024-05-20 12:48:20.569311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_user_o_auth_source_connection_list.py
+-rw-r--r--   0        0        0     3429 2024-05-20 12:48:20.569311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_user_saml_source_connection_list.py
+-rw-r--r--   0        0        0     3396 2024-05-20 12:48:20.573311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_user_source_connection_list.py
+-rw-r--r--   0        0        0     3348 2024-05-20 12:48:20.577311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_user_write_stage_list.py
+-rw-r--r--   0        0        0     3348 2024-05-20 12:48:20.577311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_web_authn_device_list.py
+-rw-r--r--   0        0        0     3381 2024-05-20 12:48:20.581311 authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_web_authn_device_type_list.py
+-rw-r--r--   0        0        0     3076 2024-05-20 12:48:20.581311 authentik_client-2024.4.2.post1716209289/authentik_client/models/pagination.py
+-rw-r--r--   0        0        0     4454 2024-05-20 12:48:20.585311 authentik_client-2024.4.2.post1716209289/authentik_client/models/password_challenge.py
+-rw-r--r--   0        0        0     2819 2024-05-20 12:48:20.589311 authentik_client-2024.4.2.post1716209289/authentik_client/models/password_challenge_response_request.py
+-rw-r--r--   0        0        0     4377 2024-05-20 12:48:20.593311 authentik_client-2024.4.2.post1716209289/authentik_client/models/password_expiry_policy.py
+-rw-r--r--   0        0        0     3099 2024-05-20 12:48:20.593311 authentik_client-2024.4.2.post1716209289/authentik_client/models/password_expiry_policy_request.py
+-rw-r--r--   0        0        0     6428 2024-05-20 12:48:20.597311 authentik_client-2024.4.2.post1716209289/authentik_client/models/password_policy.py
+-rw-r--r--   0        0        0     5239 2024-05-20 12:48:20.601311 authentik_client-2024.4.2.post1716209289/authentik_client/models/password_policy_request.py
+-rw-r--r--   0        0        0     5274 2024-05-20 12:48:20.609311 authentik_client-2024.4.2.post1716209289/authentik_client/models/password_stage.py
+-rw-r--r--   0        0        0     4264 2024-05-20 12:48:20.613311 authentik_client-2024.4.2.post1716209289/authentik_client/models/password_stage_request.py
+-rw-r--r--   0        0        0     4594 2024-05-20 12:48:20.617311 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_application_request.py
+-rw-r--r--   0        0        0     4833 2024-05-20 12:48:20.621311 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_authenticator_duo_stage_request.py
+-rw-r--r--   0        0        0     5701 2024-05-20 12:48:20.625311 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_authenticator_sms_stage_request.py
+-rw-r--r--   0        0        0     4430 2024-05-20 12:48:20.629311 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_authenticator_static_stage_request.py
+-rw-r--r--   0        0        0     4256 2024-05-20 12:48:20.633311 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_authenticator_totp_stage_request.py
+-rw-r--r--   0        0        0     4931 2024-05-20 12:48:20.633311 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_authenticator_validate_stage_request.py
+-rw-r--r--   0        0        0     5340 2024-05-20 12:48:20.637311 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_authenticator_web_authn_stage_request.py
+-rw-r--r--   0        0        0     3246 2024-05-20 12:48:20.641311 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_blueprint_instance_request.py
+-rw-r--r--   0        0        0     6352 2024-05-20 12:48:20.645311 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_brand_request.py
+-rw-r--r--   0        0        0     3860 2024-05-20 12:48:20.645311 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_captcha_stage_request.py
+-rw-r--r--   0        0        0     3051 2024-05-20 12:48:20.649311 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_certificate_key_pair_request.py
+-rw-r--r--   0        0        0     2717 2024-05-20 12:48:20.653311 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_connection_token_request.py
+-rw-r--r--   0        0        0     3607 2024-05-20 12:48:20.657312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_consent_stage_request.py
+-rw-r--r--   0        0        0     3268 2024-05-20 12:48:20.661311 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_deny_stage_request.py
+-rw-r--r--   0        0        0     4149 2024-05-20 12:48:20.661311 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_docker_service_connection_request.py
+-rw-r--r--   0        0        0     2801 2024-05-20 12:48:20.665311 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_domain_request.py
+-rw-r--r--   0        0        0     3275 2024-05-20 12:48:20.669312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_dummy_policy_request.py
+-rw-r--r--   0        0        0     3270 2024-05-20 12:48:20.669312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_dummy_stage_request.py
+-rw-r--r--   0        0        0     2674 2024-05-20 12:48:20.673312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_duo_device_request.py
+-rw-r--r--   0        0        0     5159 2024-05-20 12:48:20.677312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_email_stage_request.py
+-rw-r--r--   0        0        0     3784 2024-05-20 12:48:20.681311 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_endpoint_request.py
+-rw-r--r--   0        0        0     4845 2024-05-20 12:48:20.685312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_event_matcher_policy_request.py
+-rw-r--r--   0        0        0     4045 2024-05-20 12:48:20.685312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_event_request.py
+-rw-r--r--   0        0        0     3047 2024-05-20 12:48:20.689312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_expression_policy_request.py
+-rw-r--r--   0        0        0     4903 2024-05-20 12:48:20.693312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_flow_request.py
+-rw-r--r--   0        0        0     4055 2024-05-20 12:48:20.693312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_flow_stage_binding_request.py
+-rw-r--r--   0        0        0     2574 2024-05-20 12:48:20.697312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_google_workspace_provider_group_request.py
+-rw-r--r--   0        0        0     3440 2024-05-20 12:48:20.701312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_google_workspace_provider_mapping_request.py
+-rw-r--r--   0        0        0     4819 2024-05-20 12:48:20.701312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_google_workspace_provider_request.py
+-rw-r--r--   0        0        0     2566 2024-05-20 12:48:20.705312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_google_workspace_provider_user_request.py
+-rw-r--r--   0        0        0     3385 2024-05-20 12:48:20.705312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_group_request.py
+-rw-r--r--   0        0        0     6571 2024-05-20 12:48:20.709312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_identification_stage_request.py
+-rw-r--r--   0        0        0     3985 2024-05-20 12:48:20.713312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_invitation_request.py
+-rw-r--r--   0        0        0     3565 2024-05-20 12:48:20.713312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_invitation_stage_request.py
+-rw-r--r--   0        0        0     3492 2024-05-20 12:48:20.717312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_kubernetes_service_connection_request.py
+-rw-r--r--   0        0        0     3550 2024-05-20 12:48:20.721312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_ldap_property_mapping_request.py
+-rw-r--r--   0        0        0     6254 2024-05-20 12:48:20.721312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_ldap_provider_request.py
+-rw-r--r--   0        0        0     9697 2024-05-20 12:48:20.725312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_ldap_source_request.py
+-rw-r--r--   0        0        0     2557 2024-05-20 12:48:20.729312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_license_request.py
+-rw-r--r--   0        0        0     2570 2024-05-20 12:48:20.729312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_microsoft_entra_provider_group_request.py
+-rw-r--r--   0        0        0     3436 2024-05-20 12:48:20.733312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_microsoft_entra_provider_mapping_request.py
+-rw-r--r--   0        0        0     4396 2024-05-20 12:48:20.737312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_microsoft_entra_provider_request.py
+-rw-r--r--   0        0        0     2562 2024-05-20 12:48:20.741312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_microsoft_entra_provider_user_request.py
+-rw-r--r--   0        0        0     2879 2024-05-20 12:48:20.745312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_notification_request.py
+-rw-r--r--   0        0        0     3587 2024-05-20 12:48:20.745312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_notification_rule_request.py
+-rw-r--r--   0        0        0     3538 2024-05-20 12:48:20.749312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_notification_transport_request.py
+-rw-r--r--   0        0        0     2782 2024-05-20 12:48:20.753312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_notification_webhook_mapping_request.py
+-rw-r--r--   0        0        0     6716 2024-05-20 12:48:20.757312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_o_auth2_provider_request.py
+-rw-r--r--   0        0        0     8185 2024-05-20 12:48:20.761312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_o_auth_source_request.py
+-rw-r--r--   0        0        0     4139 2024-05-20 12:48:20.765312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_outpost_request.py
+-rw-r--r--   0        0        0     3154 2024-05-20 12:48:20.765312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_password_expiry_policy_request.py
+-rw-r--r--   0        0        0     5277 2024-05-20 12:48:20.769312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_password_policy_request.py
+-rw-r--r--   0        0        0     4326 2024-05-20 12:48:20.773312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_password_stage_request.py
+-rw-r--r--   0        0        0     2922 2024-05-20 12:48:20.777312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_permission_assign_request.py
+-rw-r--r--   0        0        0     2784 2024-05-20 12:48:20.777312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_plex_source_connection_request.py
+-rw-r--r--   0        0        0     5905 2024-05-20 12:48:20.781312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_plex_source_request.py
+-rw-r--r--   0        0        0     4286 2024-05-20 12:48:20.785312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_policy_binding_request.py
+-rw-r--r--   0        0        0     5023 2024-05-20 12:48:20.785312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_prompt_request.py
+-rw-r--r--   0        0        0     3406 2024-05-20 12:48:20.789312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_prompt_stage_request.py
+-rw-r--r--   0        0        0     6907 2024-05-20 12:48:20.797312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_proxy_provider_request.py
+-rw-r--r--   0        0        0     3495 2024-05-20 12:48:20.797312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_rac_property_mapping_request.py
+-rw-r--r--   0        0        0     4413 2024-05-20 12:48:20.801312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_rac_provider_request.py
+-rw-r--r--   0        0        0     4563 2024-05-20 12:48:20.805312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_radius_provider_request.py
+-rw-r--r--   0        0        0     3276 2024-05-20 12:48:20.805312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_reputation_policy_request.py
+-rw-r--r--   0        0        0     2565 2024-05-20 12:48:20.809312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_role_request.py
+-rw-r--r--   0        0        0     3901 2024-05-20 12:48:20.813312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_saml_property_mapping_request.py
+-rw-r--r--   0        0        0     7539 2024-05-20 12:48:20.813312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_saml_provider_request.py
+-rw-r--r--   0        0        0     8676 2024-05-20 12:48:20.817312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_saml_source_request.py
+-rw-r--r--   0        0        0     3364 2024-05-20 12:48:20.821312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_scim_mapping_request.py
+-rw-r--r--   0        0        0     3888 2024-05-20 12:48:20.821312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_scim_provider_request.py
+-rw-r--r--   0        0        0     3095 2024-05-20 12:48:20.825312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_scim_source_group_request.py
+-rw-r--r--   0        0        0     3829 2024-05-20 12:48:20.825312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_scim_source_request.py
+-rw-r--r--   0        0        0     3098 2024-05-20 12:48:20.829312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_scim_source_user_request.py
+-rw-r--r--   0        0        0     3819 2024-05-20 12:48:20.833312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_scope_mapping_request.py
+-rw-r--r--   0        0        0     5079 2024-05-20 12:48:20.833312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_settings_request.py
+-rw-r--r--   0        0        0     2674 2024-05-20 12:48:20.829312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_sms_device_request.py
+-rw-r--r--   0        0        0     3562 2024-05-20 12:48:20.837312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_source_stage_request.py
+-rw-r--r--   0        0        0     2686 2024-05-20 12:48:20.837312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_static_device_request.py
+-rw-r--r--   0        0        0     2820 2024-05-20 12:48:20.841312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_tenant_request.py
+-rw-r--r--   0        0        0     4419 2024-05-20 12:48:20.845312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_token_request.py
+-rw-r--r--   0        0        0     2678 2024-05-20 12:48:20.841312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_totp_device_request.py
+-rw-r--r--   0        0        0     3167 2024-05-20 12:48:20.845312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_user_delete_stage_request.py
+-rw-r--r--   0        0        0     4766 2024-05-20 12:48:20.849312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_user_login_stage_request.py
+-rw-r--r--   0        0        0     3167 2024-05-20 12:48:20.849312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_user_logout_stage_request.py
+-rw-r--r--   0        0        0     3109 2024-05-20 12:48:20.853312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_user_o_auth_source_connection_request.py
+-rw-r--r--   0        0        0     3934 2024-05-20 12:48:20.853312 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_user_request.py
+-rw-r--r--   0        0        0     2733 2024-05-20 12:48:20.857313 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_user_saml_source_connection_request.py
+-rw-r--r--   0        0        0     4450 2024-05-20 12:48:20.857313 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_user_write_stage_request.py
+-rw-r--r--   0        0        0     2625 2024-05-20 12:48:20.857313 authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_web_authn_device_request.py
+-rw-r--r--   0        0        0     3548 2024-05-20 12:48:20.861312 authentik_client-2024.4.2.post1716209289/authentik_client/models/permission.py
+-rw-r--r--   0        0        0     2884 2024-05-20 12:48:20.865312 authentik_client-2024.4.2.post1716209289/authentik_client/models/permission_assign_request.py
+-rw-r--r--   0        0        0     4315 2024-05-20 12:48:20.865312 authentik_client-2024.4.2.post1716209289/authentik_client/models/plex_authentication_challenge.py
+-rw-r--r--   0        0        0     2726 2024-05-20 12:48:20.869313 authentik_client-2024.4.2.post1716209289/authentik_client/models/plex_authentication_challenge_response_request.py
+-rw-r--r--   0        0        0     7752 2024-05-20 12:48:20.869313 authentik_client-2024.4.2.post1716209289/authentik_client/models/plex_source.py
+-rw-r--r--   0        0        0     3265 2024-05-20 12:48:20.873313 authentik_client-2024.4.2.post1716209289/authentik_client/models/plex_source_connection.py
+-rw-r--r--   0        0        0     2719 2024-05-20 12:48:20.873313 authentik_client-2024.4.2.post1716209289/authentik_client/models/plex_source_connection_request.py
+-rw-r--r--   0        0        0     5760 2024-05-20 12:48:20.877313 authentik_client-2024.4.2.post1716209289/authentik_client/models/plex_source_request.py
+-rw-r--r--   0        0        0     2576 2024-05-20 12:48:20.877313 authentik_client-2024.4.2.post1716209289/authentik_client/models/plex_token_redeem_request.py
+-rw-r--r--   0        0        0     4055 2024-05-20 12:48:20.881312 authentik_client-2024.4.2.post1716209289/authentik_client/models/policy.py
+-rw-r--r--   0        0        0     5643 2024-05-20 12:48:20.881312 authentik_client-2024.4.2.post1716209289/authentik_client/models/policy_binding.py
+-rw-r--r--   0        0        0     4231 2024-05-20 12:48:20.885313 authentik_client-2024.4.2.post1716209289/authentik_client/models/policy_binding_request.py
+-rw-r--r--   0        0        0      711 2024-05-20 12:48:20.885313 authentik_client-2024.4.2.post1716209289/authentik_client/models/policy_engine_mode.py
+-rw-r--r--   0        0        0     2817 2024-05-20 12:48:20.889313 authentik_client-2024.4.2.post1716209289/authentik_client/models/policy_request.py
+-rw-r--r--   0        0        0     2583 2024-05-20 12:48:20.889313 authentik_client-2024.4.2.post1716209289/authentik_client/models/policy_test_request.py
+-rw-r--r--   0        0        0     3281 2024-05-20 12:48:20.893313 authentik_client-2024.4.2.post1716209289/authentik_client/models/policy_test_result.py
+-rw-r--r--   0        0        0     4885 2024-05-20 12:48:20.893313 authentik_client-2024.4.2.post1716209289/authentik_client/models/prompt.py
+-rw-r--r--   0        0        0     4649 2024-05-20 12:48:20.897313 authentik_client-2024.4.2.post1716209289/authentik_client/models/prompt_challenge.py
+-rw-r--r--   0        0        0     3325 2024-05-20 12:48:20.897313 authentik_client-2024.4.2.post1716209289/authentik_client/models/prompt_challenge_response_request.py
+-rw-r--r--   0        0        0     4927 2024-05-20 12:48:20.901313 authentik_client-2024.4.2.post1716209289/authentik_client/models/prompt_request.py
+-rw-r--r--   0        0        0     4321 2024-05-20 12:48:20.901313 authentik_client-2024.4.2.post1716209289/authentik_client/models/prompt_stage.py
+-rw-r--r--   0        0        0     3351 2024-05-20 12:48:20.905313 authentik_client-2024.4.2.post1716209289/authentik_client/models/prompt_stage_request.py
+-rw-r--r--   0        0        0     1185 2024-05-20 12:48:20.909313 authentik_client-2024.4.2.post1716209289/authentik_client/models/prompt_type_enum.py
+-rw-r--r--   0        0        0     4264 2024-05-20 12:48:20.909313 authentik_client-2024.4.2.post1716209289/authentik_client/models/property_mapping.py
+-rw-r--r--   0        0        0     2610 2024-05-20 12:48:20.913313 authentik_client-2024.4.2.post1716209289/authentik_client/models/property_mapping_preview.py
+-rw-r--r--   0        0        0     2744 2024-05-20 12:48:20.917313 authentik_client-2024.4.2.post1716209289/authentik_client/models/property_mapping_test_result.py
+-rw-r--r--   0        0        0      715 2024-05-20 12:48:20.917313 authentik_client-2024.4.2.post1716209289/authentik_client/models/protocol_enum.py
+-rw-r--r--   0        0        0     5722 2024-05-20 12:48:20.917313 authentik_client-2024.4.2.post1716209289/authentik_client/models/provider.py
+-rw-r--r--   0        0        0      713 2024-05-20 12:48:20.921313 authentik_client-2024.4.2.post1716209289/authentik_client/models/provider_enum.py
+-rw-r--r--   0        0        0     1578 2024-05-20 12:48:20.921313 authentik_client-2024.4.2.post1716209289/authentik_client/models/provider_model_enum.py
+-rw-r--r--   0        0        0     3397 2024-05-20 12:48:20.921313 authentik_client-2024.4.2.post1716209289/authentik_client/models/provider_request.py
+-rw-r--r--   0        0        0     1009 2024-05-20 12:48:20.925313 authentik_client-2024.4.2.post1716209289/authentik_client/models/provider_type_enum.py
+-rw-r--r--   0        0        0      754 2024-05-20 12:48:20.925313 authentik_client-2024.4.2.post1716209289/authentik_client/models/proxy_mode.py
+-rw-r--r--   0        0        0     7819 2024-05-20 12:48:20.929313 authentik_client-2024.4.2.post1716209289/authentik_client/models/proxy_outpost_config.py
+-rw-r--r--   0        0        0     9552 2024-05-20 12:48:20.929313 authentik_client-2024.4.2.post1716209289/authentik_client/models/proxy_provider.py
+-rw-r--r--   0        0        0     6828 2024-05-20 12:48:20.933313 authentik_client-2024.4.2.post1716209289/authentik_client/models/proxy_provider_request.py
+-rw-r--r--   0        0        0     4407 2024-05-20 12:48:20.937313 authentik_client-2024.4.2.post1716209289/authentik_client/models/rac_property_mapping.py
+-rw-r--r--   0        0        0     3440 2024-05-20 12:48:20.937313 authentik_client-2024.4.2.post1716209289/authentik_client/models/rac_property_mapping_request.py
+-rw-r--r--   0        0        0     6813 2024-05-20 12:48:20.941313 authentik_client-2024.4.2.post1716209289/authentik_client/models/rac_provider.py
+-rw-r--r--   0        0        0     4351 2024-05-20 12:48:20.945313 authentik_client-2024.4.2.post1716209289/authentik_client/models/rac_provider_request.py
+-rw-r--r--   0        0        0     3833 2024-05-20 12:48:20.945313 authentik_client-2024.4.2.post1716209289/authentik_client/models/radius_outpost_config.py
+-rw-r--r--   0        0        0     6924 2024-05-20 12:48:20.949313 authentik_client-2024.4.2.post1716209289/authentik_client/models/radius_provider.py
+-rw-r--r--   0        0        0     4501 2024-05-20 12:48:20.949313 authentik_client-2024.4.2.post1716209289/authentik_client/models/radius_provider_request.py
+-rw-r--r--   0        0        0     4184 2024-05-20 12:48:20.953313 authentik_client-2024.4.2.post1716209289/authentik_client/models/redirect_challenge.py
+-rw-r--r--   0        0        0     3642 2024-05-20 12:48:20.957313 authentik_client-2024.4.2.post1716209289/authentik_client/models/reputation.py
+-rw-r--r--   0        0        0     4516 2024-05-20 12:48:20.957313 authentik_client-2024.4.2.post1716209289/authentik_client/models/reputation_policy.py
+-rw-r--r--   0        0        0     3238 2024-05-20 12:48:20.961313 authentik_client-2024.4.2.post1716209289/authentik_client/models/reputation_policy_request.py
+-rw-r--r--   0        0        0      795 2024-05-20 12:48:20.961313 authentik_client-2024.4.2.post1716209289/authentik_client/models/resident_key_requirement_enum.py
+-rw-r--r--   0        0        0     2618 2024-05-20 12:48:20.965313 authentik_client-2024.4.2.post1716209289/authentik_client/models/role.py
+-rw-r--r--   0        0        0     3333 2024-05-20 12:48:20.969313 authentik_client-2024.4.2.post1716209289/authentik_client/models/role_assigned_object_permission.py
+-rw-r--r--   0        0        0     3293 2024-05-20 12:48:20.969313 authentik_client-2024.4.2.post1716209289/authentik_client/models/role_object_permission.py
+-rw-r--r--   0        0        0     2517 2024-05-20 12:48:20.973313 authentik_client-2024.4.2.post1716209289/authentik_client/models/role_request.py
+-rw-r--r--   0        0        0     2712 2024-05-20 12:48:20.973313 authentik_client-2024.4.2.post1716209289/authentik_client/models/saml_metadata.py
+-rw-r--r--   0        0        0     4718 2024-05-20 12:48:20.977313 authentik_client-2024.4.2.post1716209289/authentik_client/models/saml_property_mapping.py
+-rw-r--r--   0        0        0     3829 2024-05-20 12:48:20.981313 authentik_client-2024.4.2.post1716209289/authentik_client/models/saml_property_mapping_request.py
+-rw-r--r--   0        0        0    11056 2024-05-20 12:48:20.981313 authentik_client-2024.4.2.post1716209289/authentik_client/models/saml_provider.py
+-rw-r--r--   0        0        0     7460 2024-05-20 12:48:20.985313 authentik_client-2024.4.2.post1716209289/authentik_client/models/saml_provider_request.py
+-rw-r--r--   0        0        0    10563 2024-05-20 12:48:20.989313 authentik_client-2024.4.2.post1716209289/authentik_client/models/saml_source.py
+-rw-r--r--   0        0        0     8507 2024-05-20 12:48:20.989313 authentik_client-2024.4.2.post1716209289/authentik_client/models/saml_source_request.py
+-rw-r--r--   0        0        0     4248 2024-05-20 12:48:20.993313 authentik_client-2024.4.2.post1716209289/authentik_client/models/scim_mapping.py
+-rw-r--r--   0        0        0     3309 2024-05-20 12:48:20.997313 authentik_client-2024.4.2.post1716209289/authentik_client/models/scim_mapping_request.py
+-rw-r--r--   0        0        0     5454 2024-05-20 12:48:20.997313 authentik_client-2024.4.2.post1716209289/authentik_client/models/scim_provider.py
+-rw-r--r--   0        0        0     3802 2024-05-20 12:48:21.001313 authentik_client-2024.4.2.post1716209289/authentik_client/models/scim_provider_request.py
+-rw-r--r--   0        0        0     5999 2024-05-20 12:48:21.005313 authentik_client-2024.4.2.post1716209289/authentik_client/models/scim_source.py
+-rw-r--r--   0        0        0     3369 2024-05-20 12:48:21.005313 authentik_client-2024.4.2.post1716209289/authentik_client/models/scim_source_group.py
+-rw-r--r--   0        0        0     3023 2024-05-20 12:48:21.009313 authentik_client-2024.4.2.post1716209289/authentik_client/models/scim_source_group_request.py
+-rw-r--r--   0        0        0     3708 2024-05-20 12:48:21.013313 authentik_client-2024.4.2.post1716209289/authentik_client/models/scim_source_request.py
+-rw-r--r--   0        0        0     3370 2024-05-20 12:48:21.013313 authentik_client-2024.4.2.post1716209289/authentik_client/models/scim_source_user.py
+-rw-r--r--   0        0        0     3026 2024-05-20 12:48:21.017313 authentik_client-2024.4.2.post1716209289/authentik_client/models/scim_source_user_request.py
+-rw-r--r--   0        0        0     4629 2024-05-20 12:48:21.025313 authentik_client-2024.4.2.post1716209289/authentik_client/models/scope_mapping.py
+-rw-r--r--   0        0        0     3740 2024-05-20 12:48:21.025313 authentik_client-2024.4.2.post1716209289/authentik_client/models/scope_mapping_request.py
+-rw-r--r--   0        0        0     2738 2024-05-20 12:48:21.029313 authentik_client-2024.4.2.post1716209289/authentik_client/models/selectable_stage.py
+-rw-r--r--   0        0        0     3773 2024-05-20 12:48:21.029313 authentik_client-2024.4.2.post1716209289/authentik_client/models/service_connection.py
+-rw-r--r--   0        0        0     2776 2024-05-20 12:48:21.033313 authentik_client-2024.4.2.post1716209289/authentik_client/models/service_connection_request.py
+-rw-r--r--   0        0        0     2731 2024-05-20 12:48:21.033313 authentik_client-2024.4.2.post1716209289/authentik_client/models/service_connection_state.py
+-rw-r--r--   0        0        0     3178 2024-05-20 12:48:21.037313 authentik_client-2024.4.2.post1716209289/authentik_client/models/session_user.py
+-rw-r--r--   0        0        0     4931 2024-05-20 12:48:21.041313 authentik_client-2024.4.2.post1716209289/authentik_client/models/settings.py
+-rw-r--r--   0        0        0     5058 2024-05-20 12:48:21.041313 authentik_client-2024.4.2.post1716209289/authentik_client/models/settings_request.py
+-rw-r--r--   0        0        0      733 2024-05-20 12:48:21.045313 authentik_client-2024.4.2.post1716209289/authentik_client/models/severity_enum.py
+-rw-r--r--   0        0        0     4175 2024-05-20 12:48:21.045313 authentik_client-2024.4.2.post1716209289/authentik_client/models/shell_challenge.py
+-rw-r--r--   0        0        0     2172 2024-05-20 12:48:21.049313 authentik_client-2024.4.2.post1716209289/authentik_client/models/signature_algorithm_enum.py
+-rw-r--r--   0        0        0     2906 2024-05-20 12:48:21.017313 authentik_client-2024.4.2.post1716209289/authentik_client/models/sms_device.py
+-rw-r--r--   0        0        0     2619 2024-05-20 12:48:21.021313 authentik_client-2024.4.2.post1716209289/authentik_client/models/sms_device_request.py
+-rw-r--r--   0        0        0     6945 2024-05-20 12:48:21.049313 authentik_client-2024.4.2.post1716209289/authentik_client/models/source.py
+-rw-r--r--   0        0        0     4836 2024-05-20 12:48:21.053313 authentik_client-2024.4.2.post1716209289/authentik_client/models/source_request.py
+-rw-r--r--   0        0        0     4438 2024-05-20 12:48:21.057314 authentik_client-2024.4.2.post1716209289/authentik_client/models/source_stage.py
+-rw-r--r--   0        0        0     3507 2024-05-20 12:48:21.061313 authentik_client-2024.4.2.post1716209289/authentik_client/models/source_stage_request.py
+-rw-r--r--   0        0        0     5355 2024-05-20 12:48:21.061313 authentik_client-2024.4.2.post1716209289/authentik_client/models/source_type.py
+-rw-r--r--   0        0        0      714 2024-05-20 12:48:21.065313 authentik_client-2024.4.2.post1716209289/authentik_client/models/sp_binding_enum.py
+-rw-r--r--   0        0        0     4070 2024-05-20 12:48:21.065313 authentik_client-2024.4.2.post1716209289/authentik_client/models/stage.py
+-rw-r--r--   0        0        0     3437 2024-05-20 12:48:21.069313 authentik_client-2024.4.2.post1716209289/authentik_client/models/stage_prompt.py
+-rw-r--r--   0        0        0     3089 2024-05-20 12:48:21.073314 authentik_client-2024.4.2.post1716209289/authentik_client/models/stage_request.py
+-rw-r--r--   0        0        0     3385 2024-05-20 12:48:21.073314 authentik_client-2024.4.2.post1716209289/authentik_client/models/static_device.py
+-rw-r--r--   0        0        0     2631 2024-05-20 12:48:21.077314 authentik_client-2024.4.2.post1716209289/authentik_client/models/static_device_request.py
+-rw-r--r--   0        0        0     2546 2024-05-20 12:48:21.077314 authentik_client-2024.4.2.post1716209289/authentik_client/models/static_device_token.py
+-rw-r--r--   0        0        0     2581 2024-05-20 12:48:21.081313 authentik_client-2024.4.2.post1716209289/authentik_client/models/static_device_token_request.py
+-rw-r--r--   0        0        0      846 2024-05-20 12:48:21.081313 authentik_client-2024.4.2.post1716209289/authentik_client/models/sub_mode_enum.py
+-rw-r--r--   0        0        0     3114 2024-05-20 12:48:21.085314 authentik_client-2024.4.2.post1716209289/authentik_client/models/sync_status.py
+-rw-r--r--   0        0        0     4463 2024-05-20 12:48:21.085314 authentik_client-2024.4.2.post1716209289/authentik_client/models/system_info.py
+-rw-r--r--   0        0        0     2934 2024-05-20 12:48:21.089314 authentik_client-2024.4.2.post1716209289/authentik_client/models/system_info_runtime.py
+-rw-r--r--   0        0        0     4701 2024-05-20 12:48:21.093314 authentik_client-2024.4.2.post1716209289/authentik_client/models/system_task.py
+-rw-r--r--   0        0        0      789 2024-05-20 12:48:21.093314 authentik_client-2024.4.2.post1716209289/authentik_client/models/system_task_status_enum.py
+-rw-r--r--   0        0        0     2872 2024-05-20 12:48:21.097314 authentik_client-2024.4.2.post1716209289/authentik_client/models/tenant.py
+-rw-r--r--   0        0        0     2589 2024-05-20 12:48:21.101314 authentik_client-2024.4.2.post1716209289/authentik_client/models/tenant_admin_group_request_request.py
+-rw-r--r--   0        0        0     2705 2024-05-20 12:48:21.101314 authentik_client-2024.4.2.post1716209289/authentik_client/models/tenant_recovery_key_request_request.py
+-rw-r--r--   0        0        0     2599 2024-05-20 12:48:21.105314 authentik_client-2024.4.2.post1716209289/authentik_client/models/tenant_recovery_key_response.py
+-rw-r--r--   0        0        0     2765 2024-05-20 12:48:21.105314 authentik_client-2024.4.2.post1716209289/authentik_client/models/tenant_request.py
+-rw-r--r--   0        0        0     4802 2024-05-20 12:48:21.109314 authentik_client-2024.4.2.post1716209289/authentik_client/models/token.py
+-rw-r--r--   0        0        0     4198 2024-05-20 12:48:21.113314 authentik_client-2024.4.2.post1716209289/authentik_client/models/token_model.py
+-rw-r--r--   0        0        0     4329 2024-05-20 12:48:21.113314 authentik_client-2024.4.2.post1716209289/authentik_client/models/token_request.py
+-rw-r--r--   0        0        0     2521 2024-05-20 12:48:21.117314 authentik_client-2024.4.2.post1716209289/authentik_client/models/token_set_key_request.py
+-rw-r--r--   0        0        0     2494 2024-05-20 12:48:21.121314 authentik_client-2024.4.2.post1716209289/authentik_client/models/token_view.py
+-rw-r--r--   0        0        0     2724 2024-05-20 12:48:21.093314 authentik_client-2024.4.2.post1716209289/authentik_client/models/totp_device.py
+-rw-r--r--   0        0        0     2623 2024-05-20 12:48:21.097314 authentik_client-2024.4.2.post1716209289/authentik_client/models/totp_device_request.py
+-rw-r--r--   0        0        0     3389 2024-05-20 12:48:21.121314 authentik_client-2024.4.2.post1716209289/authentik_client/models/transaction_application_request.py
+-rw-r--r--   0        0        0     2595 2024-05-20 12:48:21.125314 authentik_client-2024.4.2.post1716209289/authentik_client/models/transaction_application_response.py
+-rw-r--r--   0        0        0     2936 2024-05-20 12:48:21.125314 authentik_client-2024.4.2.post1716209289/authentik_client/models/type_create.py
+-rw-r--r--   0        0        0      730 2024-05-20 12:48:21.129314 authentik_client-2024.4.2.post1716209289/authentik_client/models/ui_theme_enum.py
+-rw-r--r--   0        0        0     2808 2024-05-20 12:48:21.129314 authentik_client-2024.4.2.post1716209289/authentik_client/models/used_by.py
+-rw-r--r--   0        0        0      795 2024-05-20 12:48:21.129314 authentik_client-2024.4.2.post1716209289/authentik_client/models/used_by_action_enum.py
+-rw-r--r--   0        0        0     5459 2024-05-20 12:48:21.133314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user.py
+-rw-r--r--   0        0        0     2458 2024-05-20 12:48:21.133314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_account_request.py
+-rw-r--r--   0        0        0     4946 2024-05-20 12:48:21.137314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_assigned_object_permission.py
+-rw-r--r--   0        0        0     3828 2024-05-20 12:48:21.141314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_consent.py
+-rw-r--r--   0        0        0      811 2024-05-20 12:48:21.141314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_creation_mode_enum.py
+-rw-r--r--   0        0        0     4110 2024-05-20 12:48:21.141314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_delete_stage.py
+-rw-r--r--   0        0        0     3129 2024-05-20 12:48:21.145314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_delete_stage_request.py
+-rw-r--r--   0        0        0      735 2024-05-20 12:48:21.145314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_fields_enum.py
+-rw-r--r--   0        0        0     3909 2024-05-20 12:48:21.149314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_group.py
+-rw-r--r--   0        0        0     3193 2024-05-20 12:48:21.153314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_group_request.py
+-rw-r--r--   0        0        0     4334 2024-05-20 12:48:21.153314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_login_challenge.py
+-rw-r--r--   0        0        0     2805 2024-05-20 12:48:21.153314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_login_challenge_response_request.py
+-rw-r--r--   0        0        0     5631 2024-05-20 12:48:21.157314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_login_stage.py
+-rw-r--r--   0        0        0     4728 2024-05-20 12:48:21.157314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_login_stage_request.py
+-rw-r--r--   0        0        0     4110 2024-05-20 12:48:21.161314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_logout_stage.py
+-rw-r--r--   0        0        0     3129 2024-05-20 12:48:21.161314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_logout_stage_request.py
+-rw-r--r--   0        0        0      853 2024-05-20 12:48:21.165314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_matching_mode_enum.py
+-rw-r--r--   0        0        0     4160 2024-05-20 12:48:21.165314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_metrics.py
+-rw-r--r--   0        0        0     3188 2024-05-20 12:48:21.169314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_o_auth_source_connection.py
+-rw-r--r--   0        0        0     3054 2024-05-20 12:48:21.169314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_o_auth_source_connection_request.py
+-rw-r--r--   0        0        0     3293 2024-05-20 12:48:21.169314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_object_permission.py
+-rw-r--r--   0        0        0     2557 2024-05-20 12:48:21.173314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_password_set_request.py
+-rw-r--r--   0        0        0     2491 2024-05-20 12:48:21.173314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_path.py
+-rw-r--r--   0        0        0     3872 2024-05-20 12:48:21.177314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_request.py
+-rw-r--r--   0        0        0     3107 2024-05-20 12:48:21.177314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_saml_source_connection.py
+-rw-r--r--   0        0        0     2668 2024-05-20 12:48:21.181314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_saml_source_connection_request.py
+-rw-r--r--   0        0        0     5465 2024-05-20 12:48:21.185314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_self.py
+-rw-r--r--   0        0        0     2629 2024-05-20 12:48:21.185314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_self_groups.py
+-rw-r--r--   0        0        0     3074 2024-05-20 12:48:21.185314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_service_account_request.py
+-rw-r--r--   0        0        0     2844 2024-05-20 12:48:21.189314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_service_account_response.py
+-rw-r--r--   0        0        0     2866 2024-05-20 12:48:21.189314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_setting.py
+-rw-r--r--   0        0        0     3245 2024-05-20 12:48:21.193314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_source_connection.py
+-rw-r--r--   0        0        0      817 2024-05-20 12:48:21.193314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_type_enum.py
+-rw-r--r--   0        0        0      777 2024-05-20 12:48:21.193314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_verification_enum.py
+-rw-r--r--   0        0        0     5382 2024-05-20 12:48:21.197314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_write_stage.py
+-rw-r--r--   0        0        0     4412 2024-05-20 12:48:21.197314 authentik_client-2024.4.2.post1716209289/authentik_client/models/user_write_stage_request.py
+-rw-r--r--   0        0        0     3197 2024-05-20 12:48:21.201314 authentik_client-2024.4.2.post1716209289/authentik_client/models/validation_error.py
+-rw-r--r--   0        0        0     3589 2024-05-20 12:48:21.201314 authentik_client-2024.4.2.post1716209289/authentik_client/models/version.py
+-rw-r--r--   0        0        0     3786 2024-05-20 12:48:21.205314 authentik_client-2024.4.2.post1716209289/authentik_client/models/web_authn_device.py
+-rw-r--r--   0        0        0     2577 2024-05-20 12:48:21.205314 authentik_client-2024.4.2.post1716209289/authentik_client/models/web_authn_device_request.py
+-rw-r--r--   0        0        0     2562 2024-05-20 12:48:21.209314 authentik_client-2024.4.2.post1716209289/authentik_client/models/web_authn_device_type.py
+-rw-r--r--   0        0        0     2669 2024-05-20 12:48:21.213314 authentik_client-2024.4.2.post1716209289/authentik_client/models/web_authn_device_type_request.py
+-rw-r--r--   0        0        0     2410 2024-05-20 12:48:21.213314 authentik_client-2024.4.2.post1716209289/authentik_client/models/workers.py
+-rw-r--r--   0        0        0        0 2024-05-20 12:48:22.389320 authentik_client-2024.4.2.post1716209289/authentik_client/py.typed
+-rw-r--r--   0        0        0     9196 2024-05-20 12:48:22.401320 authentik_client-2024.4.2.post1716209289/authentik_client/rest.py
+-rw-r--r--   0        0        0     1936 2024-05-20 12:48:22.389320 authentik_client-2024.4.2.post1716209289/pyproject.toml
+-rw-r--r--   0        0        0   158698 1970-01-01 00:00:00.000000 authentik_client-2024.4.2.post1716209289/PKG-INFO
```

### Comparing `authentik_client-2024.4.2.post1715271061/README.md` & `authentik_client-2024.4.2.post1716209289/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # authentik-client
 Making authentication simple.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 2024.4.2
-- Package version: 2024.4.2-1715271061
+- Package version: 2024.4.2-1716209289
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/__init__.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "2024.4.2-1715271061"
+__version__ = "2024.4.2-1716209289"
 
 # import apis into sdk package
 from authentik_client.api.admin_api import AdminApi
 from authentik_client.api.authenticators_api import AuthenticatorsApi
 from authentik_client.api.core_api import CoreApi
 from authentik_client.api.crypto_api import CryptoApi
 from authentik_client.api.enterprise_api import EnterpriseApi
```

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/api/__init__.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/api/admin_api.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/api/admin_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/api/authenticators_api.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/api/authenticators_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/api/core_api.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/api/core_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -8775,14 +8775,15 @@
 
 
 
     @validate_call
     def core_groups_retrieve(
         self,
         group_uuid: Annotated[StrictStr, Field(description="A UUID string identifying this Group.")],
+        include_users: Optional[StrictBool] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -8794,14 +8795,16 @@
     ) -> Group:
         """core_groups_retrieve
 
         Group Viewset
 
         :param group_uuid: A UUID string identifying this Group. (required)
         :type group_uuid: str
+        :param include_users:
+        :type include_users: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -8818,14 +8821,15 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._core_groups_retrieve_serialize(
             group_uuid=group_uuid,
+            include_users=include_users,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -8844,14 +8848,15 @@
         ).data
 
 
     @validate_call
     def core_groups_retrieve_with_http_info(
         self,
         group_uuid: Annotated[StrictStr, Field(description="A UUID string identifying this Group.")],
+        include_users: Optional[StrictBool] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -8863,14 +8868,16 @@
     ) -> ApiResponse[Group]:
         """core_groups_retrieve
 
         Group Viewset
 
         :param group_uuid: A UUID string identifying this Group. (required)
         :type group_uuid: str
+        :param include_users:
+        :type include_users: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -8887,14 +8894,15 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._core_groups_retrieve_serialize(
             group_uuid=group_uuid,
+            include_users=include_users,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -8913,14 +8921,15 @@
         )
 
 
     @validate_call
     def core_groups_retrieve_without_preload_content(
         self,
         group_uuid: Annotated[StrictStr, Field(description="A UUID string identifying this Group.")],
+        include_users: Optional[StrictBool] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -8932,14 +8941,16 @@
     ) -> RESTResponseType:
         """core_groups_retrieve
 
         Group Viewset
 
         :param group_uuid: A UUID string identifying this Group. (required)
         :type group_uuid: str
+        :param include_users:
+        :type include_users: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -8956,14 +8967,15 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._core_groups_retrieve_serialize(
             group_uuid=group_uuid,
+            include_users=include_users,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -8977,14 +8989,15 @@
         )
         return response_data.response
 
 
     def _core_groups_retrieve_serialize(
         self,
         group_uuid,
+        include_users,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -8999,14 +9012,18 @@
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if group_uuid is not None:
             _path_params['group_uuid'] = group_uuid
         # process the query parameters
+        if include_users is not None:
+            
+            _query_params.append(('include_users', include_users))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
```

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/api/crypto_api.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/api/crypto_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/api/enterprise_api.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/api/enterprise_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/api/events_api.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/api/events_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/api/flows_api.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/api/flows_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/api/managed_api.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/api/managed_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/api/oauth2_api.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/api/oauth2_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/api/outposts_api.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/api/outposts_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/api/policies_api.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/api/policies_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/api/propertymappings_api.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/api/propertymappings_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/api/providers_api.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/api/providers_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/api/rac_api.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/api/rac_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/api/rbac_api.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/api/rbac_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/api/root_api.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/api/root_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/api/schema_api.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/api/schema_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/api/sources_api.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/api/sources_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/api/stages_api.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/api/stages_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/api/tenants_api.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/api/tenants_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/api_client.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2024.4.2-1715271061/python'
+        self.user_agent = 'OpenAPI-Generator/2024.4.2-1716209289/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/api_response.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/api_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/configuration.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,15 +375,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 2024.4.2\n"\
-               "SDK Package Version: 2024.4.2-1715271061".\
+               "SDK Package Version: 2024.4.2-1716209289".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/exceptions.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/__init__.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/access_denied_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/access_denied_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/alg_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/alg_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/app.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/app.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/app_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/app_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/apple_challenge_response_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/apple_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/apple_login_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/apple_login_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/application.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/application.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/application_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/application_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/auth_mode_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/auth_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/auth_type_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/auth_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticated_session.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticated_session.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticated_session_asn.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticated_session_asn.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticated_session_geo_ip.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticated_session_geo_ip.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticated_session_user_agent.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticated_session_user_agent.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticated_session_user_agent_device.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticated_session_user_agent_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticated_session_user_agent_os.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticated_session_user_agent_os.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticated_session_user_agent_user_agent.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticated_session_user_agent_user_agent.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authentication_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authentication_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_attachment_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_attachment_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_duo_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_duo_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_duo_challenge_response_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_duo_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_duo_stage.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_duo_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_duo_stage_device_import_response.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_duo_stage_device_import_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_duo_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_duo_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_sms_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_sms_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_sms_challenge_response_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_sms_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_sms_stage.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_sms_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_sms_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_sms_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_static_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_static_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_static_challenge_response_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_static_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_static_stage.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_static_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_static_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_static_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_totp_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_totp_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_totp_challenge_response_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_totp_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_totp_stage.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_totp_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_totp_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_totp_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_validate_stage.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_validate_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_validate_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_validate_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_validation_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_validation_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_validation_challenge_response_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_validation_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_web_authn_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_web_authn_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_web_authn_challenge_response_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_web_authn_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_web_authn_stage.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_web_authn_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/authenticator_web_authn_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/authenticator_web_authn_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/auto_submit_challenge_response_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/auto_submit_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/autosubmit_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/autosubmit_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/backends_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/backends_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/binding_type_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/binding_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/blueprint_file.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/blueprint_file.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/blueprint_instance.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/blueprint_instance.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/blueprint_instance_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/blueprint_instance_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/blueprint_instance_status_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/blueprint_instance_status_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/brand.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/brand.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/brand_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/brand_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/cache.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/cache.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/capabilities_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/capabilities_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/captcha_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/captcha_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/captcha_challenge_response_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/captcha_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/captcha_stage.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/captcha_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/captcha_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/captcha_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/certificate_data.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/certificate_data.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/certificate_generation_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/certificate_generation_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/certificate_key_pair.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/certificate_key_pair.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/certificate_key_pair_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/certificate_key_pair_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/challenge_choices.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/challenge_choices.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/challenge_types.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/challenge_types.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/client_type_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/client_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/config.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/connection_token.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/connection_token.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/connection_token_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/connection_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/consent_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/consent_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/consent_challenge_response_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/consent_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/consent_permission.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/consent_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/consent_stage.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/consent_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/consent_stage_mode_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/consent_stage_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/consent_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/consent_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/contextual_flow_info.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/contextual_flow_info.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/contextual_flow_info_layout_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/contextual_flow_info_layout_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/coordinate.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/coordinate.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/current_brand.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/current_brand.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/denied_action_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/denied_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/deny_stage.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/deny_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/deny_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/deny_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/device.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/device_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/device_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/device_challenge_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/device_challenge_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/device_classes_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/device_classes_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/digest_algorithm_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/digest_algorithm_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/digits_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/digits_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/docker_service_connection.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/docker_service_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/docker_service_connection_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/docker_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/domain.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/domain.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/domain_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/domain_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/dummy_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/dummy_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/dummy_challenge_response_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/dummy_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/dummy_policy.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/dummy_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/dummy_policy_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/dummy_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/dummy_stage.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/dummy_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/dummy_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/dummy_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/duo_device.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/duo_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/duo_device_enrollment_status.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/duo_device_enrollment_status.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/duo_device_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/duo_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/duo_response_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/duo_response_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/email_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/email_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/email_challenge_response_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/email_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/email_stage.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/email_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/email_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/email_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/endpoint.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/endpoint_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/endpoint_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/error_detail.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/error_detail.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/error_reporting_config.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/error_reporting_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/event.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/event.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/event_actions.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/event_actions.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/event_matcher_policy.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/event_matcher_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/event_matcher_policy_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/event_matcher_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/event_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/event_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/event_top_per_user.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/event_top_per_user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/expiring_base_grant_model.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/expiring_base_grant_model.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/expression_policy.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/expression_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/expression_policy_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/expression_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/extra_role_object_permission.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/extra_role_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/extra_user_object_permission.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/extra_user_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/file_path_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/file_path_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/flow.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/flow.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_challenge_response_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_designation_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_designation_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_diagram.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_diagram.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_error_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_error_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_import_result.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_import_result.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_inspection.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_inspection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_inspector_plan.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_inspector_plan.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_layout_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_layout_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_set.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_set.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_set_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_set_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_stage_binding.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_stage_binding.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/flow_stage_binding_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/flow_stage_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/footer_link.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/footer_link.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/generic_error.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/generic_error.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/geoip_binding_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/geoip_binding_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/google_workspace_provider.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/google_workspace_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/google_workspace_provider_group.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/google_workspace_provider_group.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/google_workspace_provider_group_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/google_workspace_provider_group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/google_workspace_provider_mapping.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/google_workspace_provider_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/google_workspace_provider_mapping_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/google_workspace_provider_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/google_workspace_provider_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/google_workspace_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/google_workspace_provider_user.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/google_workspace_provider_user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/google_workspace_provider_user_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/google_workspace_provider_user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/group.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/group.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/group_member.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/group_member.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/group_member_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/group_member_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/group_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/identification_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/identification_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/identification_challenge_response_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/identification_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/identification_stage.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/identification_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/identification_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/identification_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/install_id.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/install_id.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/intent_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/intent_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/invalid_response_action_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/invalid_response_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/invitation.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/invitation.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/invitation_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/invitation_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/invitation_stage.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/invitation_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/invitation_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/invitation_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/issuer_mode_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/issuer_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/kubernetes_service_connection.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/kubernetes_service_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/kubernetes_service_connection_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/kubernetes_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/ldap_debug.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/ldap_debug.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/ldap_outpost_config.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/ldap_outpost_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/ldap_property_mapping.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/ldap_property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/ldap_property_mapping_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/ldap_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/ldap_provider.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/ldap_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/ldap_provider_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/ldap_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/ldap_source.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/ldap_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/ldap_source_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/ldap_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/ldapapi_access_mode.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/ldapapi_access_mode.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/license.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/license.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/license_forecast.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/license_forecast.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/license_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/license_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/license_summary.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/license_summary.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/link.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/link.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/log_event.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/log_event.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/log_level_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/log_level_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/login_challenge_types.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/login_challenge_types.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/login_metrics.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/login_metrics.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/login_source.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/login_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/metadata.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/metadata.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/microsoft_entra_provider.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/microsoft_entra_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/microsoft_entra_provider_group.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/microsoft_entra_provider_group.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/microsoft_entra_provider_group_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/microsoft_entra_provider_group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/microsoft_entra_provider_mapping.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/microsoft_entra_provider_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/microsoft_entra_provider_mapping_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/microsoft_entra_provider_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/microsoft_entra_provider_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/microsoft_entra_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/microsoft_entra_provider_user.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/microsoft_entra_provider_user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/microsoft_entra_provider_user_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/microsoft_entra_provider_user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/model_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/model_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/model_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/model_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/name_id_policy_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/name_id_policy_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/network_binding_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/network_binding_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/not_configured_action_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/not_configured_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/notification.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/notification.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/notification_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/notification_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/notification_rule.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/notification_rule.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/notification_rule_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/notification_rule_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/notification_transport.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/notification_transport.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/notification_transport_mode_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/notification_transport_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/notification_transport_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/notification_transport_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/notification_transport_test.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/notification_transport_test.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/notification_webhook_mapping.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/notification_webhook_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/notification_webhook_mapping_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/notification_webhook_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/o_auth2_provider.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/o_auth2_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/o_auth2_provider_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/o_auth2_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/o_auth2_provider_setup_urls.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/o_auth2_provider_setup_urls.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/o_auth_device_code_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/o_auth_device_code_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/o_auth_device_code_challenge_response_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/o_auth_device_code_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/o_auth_device_code_finish_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/o_auth_device_code_finish_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/o_auth_source.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/o_auth_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/o_auth_source_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/o_auth_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/open_id_connect_configuration.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/open_id_connect_configuration.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/outgoing_sync_delete_action.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/outgoing_sync_delete_action.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/outpost.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/outpost.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/outpost_default_config.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/outpost_default_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/outpost_health.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/outpost_health.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/outpost_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/outpost_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/outpost_type_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/outpost_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_application_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_application_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_authenticated_session_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_authenticated_session_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_authenticator_duo_stage_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_authenticator_duo_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_authenticator_sms_stage_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_authenticator_sms_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_authenticator_static_stage_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_authenticator_static_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_authenticator_totp_stage_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_authenticator_totp_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_authenticator_validate_stage_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_authenticator_validate_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_authenticator_web_authn_stage_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_authenticator_web_authn_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_blueprint_instance_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_blueprint_instance_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_brand_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_brand_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_captcha_stage_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_captcha_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_certificate_key_pair_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_certificate_key_pair_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_connection_token_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_connection_token_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_consent_stage_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_consent_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_deny_stage_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_deny_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_docker_service_connection_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_docker_service_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_domain_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_domain_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_dummy_policy_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_dummy_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_dummy_stage_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_dummy_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_duo_device_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_duo_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_email_stage_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_email_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_endpoint_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_endpoint_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_event_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_event_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_event_matcher_policy_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_event_matcher_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_expiring_base_grant_model_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_expiring_base_grant_model_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_expression_policy_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_expression_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_extra_role_object_permission_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_extra_role_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_extra_user_object_permission_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_extra_user_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_flow_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_flow_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_flow_stage_binding_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_flow_stage_binding_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_google_workspace_provider_group_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_google_workspace_provider_group_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_google_workspace_provider_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_google_workspace_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_google_workspace_provider_mapping_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_google_workspace_provider_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_google_workspace_provider_user_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_google_workspace_provider_user_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_group_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_group_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_identification_stage_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_identification_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_invitation_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_invitation_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_invitation_stage_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_invitation_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_kubernetes_service_connection_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_kubernetes_service_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_ldap_outpost_config_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_ldap_outpost_config_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_ldap_property_mapping_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_ldap_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_ldap_provider_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_ldap_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_ldap_source_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_ldap_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_license_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_license_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_microsoft_entra_provider_group_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_microsoft_entra_provider_group_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_microsoft_entra_provider_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_microsoft_entra_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_microsoft_entra_provider_mapping_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_microsoft_entra_provider_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_microsoft_entra_provider_user_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_microsoft_entra_provider_user_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_notification_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_notification_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_notification_rule_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_notification_rule_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_notification_transport_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_notification_transport_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_notification_webhook_mapping_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_notification_webhook_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_o_auth2_provider_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_o_auth2_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_o_auth_source_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_o_auth_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_outpost_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_outpost_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_password_expiry_policy_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_password_expiry_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_password_policy_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_password_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_password_stage_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_password_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_permission_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_plex_source_connection_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_plex_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_plex_source_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_plex_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_policy_binding_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_policy_binding_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_policy_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_prompt_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_prompt_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_prompt_stage_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_prompt_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_property_mapping_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_provider_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_proxy_outpost_config_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_proxy_outpost_config_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_proxy_provider_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_proxy_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_rac_property_mapping_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_rac_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_rac_provider_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_rac_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_radius_outpost_config_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_radius_outpost_config_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_radius_provider_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_radius_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_reputation_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_reputation_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_reputation_policy_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_reputation_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_role_assigned_object_permission_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_role_assigned_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_role_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_role_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_saml_property_mapping_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_saml_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_saml_provider_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_saml_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_saml_source_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_saml_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_scim_mapping_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_scim_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_scim_provider_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_scim_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_scim_source_group_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_scim_source_group_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_scim_source_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_scim_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_scim_source_user_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_scim_source_user_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_scope_mapping_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_scope_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_service_connection_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_service_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_sms_device_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_sms_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_source_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_source_stage_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_source_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_stage_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_static_device_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_static_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_system_task_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_system_task_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_tenant_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_tenant_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_token_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_token_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_token_model_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_token_model_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_totp_device_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_totp_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_user_assigned_object_permission_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_user_assigned_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_user_consent_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_user_consent_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_user_delete_stage_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_user_delete_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_user_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_user_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_user_login_stage_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_user_login_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_user_logout_stage_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_user_logout_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_user_o_auth_source_connection_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_user_o_auth_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_user_saml_source_connection_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_user_saml_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_user_source_connection_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_user_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_user_write_stage_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_user_write_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_web_authn_device_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_web_authn_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/paginated_web_authn_device_type_list.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/paginated_web_authn_device_type_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/pagination.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/pagination.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/password_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/password_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/password_challenge_response_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/password_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/password_expiry_policy.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/password_expiry_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/password_expiry_policy_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/password_expiry_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/password_policy.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/password_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/password_policy_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/password_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/password_stage.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/password_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/password_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/password_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_application_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_application_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_authenticator_duo_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_authenticator_duo_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_authenticator_sms_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_authenticator_sms_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_authenticator_static_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_authenticator_static_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_authenticator_totp_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_authenticator_totp_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_authenticator_validate_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_authenticator_validate_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_authenticator_web_authn_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_authenticator_web_authn_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_blueprint_instance_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_blueprint_instance_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_brand_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_brand_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_captcha_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_captcha_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_certificate_key_pair_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_certificate_key_pair_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_connection_token_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_connection_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_consent_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_consent_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_deny_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_deny_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_docker_service_connection_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_docker_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_domain_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_domain_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_dummy_policy_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_dummy_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_dummy_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_dummy_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_duo_device_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_duo_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_email_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_email_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_endpoint_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_event_matcher_policy_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_event_matcher_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_event_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_event_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_expression_policy_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_expression_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_flow_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_flow_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_flow_stage_binding_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_flow_stage_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_google_workspace_provider_group_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_google_workspace_provider_group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_google_workspace_provider_mapping_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_google_workspace_provider_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_google_workspace_provider_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_google_workspace_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_google_workspace_provider_user_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_google_workspace_provider_user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_group_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_identification_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_identification_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_invitation_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_invitation_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_invitation_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_invitation_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_kubernetes_service_connection_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_kubernetes_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_ldap_property_mapping_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_ldap_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_ldap_provider_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_ldap_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_ldap_source_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_ldap_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_license_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_license_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_microsoft_entra_provider_group_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_microsoft_entra_provider_group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_microsoft_entra_provider_mapping_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_microsoft_entra_provider_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_microsoft_entra_provider_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_microsoft_entra_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_microsoft_entra_provider_user_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_microsoft_entra_provider_user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_notification_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_notification_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_notification_rule_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_notification_rule_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_notification_transport_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_notification_transport_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_notification_webhook_mapping_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_notification_webhook_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_o_auth2_provider_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_o_auth2_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_o_auth_source_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_o_auth_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_outpost_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_outpost_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_password_expiry_policy_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_password_expiry_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_password_policy_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_password_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_password_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_password_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_permission_assign_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_permission_assign_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_plex_source_connection_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_plex_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_plex_source_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_plex_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_policy_binding_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_policy_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_prompt_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_prompt_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_prompt_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_prompt_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_proxy_provider_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_proxy_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_rac_property_mapping_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_rac_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_rac_provider_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_rac_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_radius_provider_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_radius_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_reputation_policy_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_reputation_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_role_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_role_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_saml_property_mapping_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_saml_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_saml_provider_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_saml_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_saml_source_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_saml_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_scim_mapping_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_scim_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_scim_provider_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_scim_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_scim_source_group_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_scim_source_group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_scim_source_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_scim_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_scim_source_user_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_scim_source_user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_scope_mapping_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_scope_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_settings_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_settings_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_sms_device_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_sms_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_source_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_source_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_static_device_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_static_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_tenant_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_tenant_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_token_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_totp_device_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_totp_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_user_delete_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_user_delete_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_user_login_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_user_login_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_user_logout_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_user_logout_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_user_o_auth_source_connection_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_user_o_auth_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_user_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_user_saml_source_connection_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_user_saml_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_user_write_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_user_write_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/patched_web_authn_device_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/patched_web_authn_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/permission.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/permission_assign_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/permission_assign_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/plex_authentication_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/plex_authentication_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/plex_authentication_challenge_response_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/plex_authentication_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/plex_source.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/plex_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/plex_source_connection.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/plex_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/plex_source_connection_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/plex_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/plex_source_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/plex_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/plex_token_redeem_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/plex_token_redeem_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/policy.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/policy_binding.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/policy_binding.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/policy_binding_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/policy_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/policy_engine_mode.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/policy_engine_mode.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/policy_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/policy_test_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/policy_test_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/policy_test_result.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/policy_test_result.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/prompt.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/prompt.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/prompt_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/prompt_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/prompt_challenge_response_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/prompt_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/prompt_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/prompt_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/prompt_stage.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/prompt_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/prompt_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/prompt_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/prompt_type_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/prompt_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/property_mapping.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/property_mapping_preview.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/property_mapping_preview.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/property_mapping_test_result.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/property_mapping_test_result.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/protocol_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/protocol_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/provider.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/provider_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/provider_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/provider_model_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/provider_model_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/provider_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/provider_type_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/provider_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/proxy_mode.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/proxy_mode.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/proxy_outpost_config.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/proxy_outpost_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/proxy_provider.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/proxy_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/proxy_provider_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/proxy_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/rac_property_mapping.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/rac_property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/rac_property_mapping_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/rac_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/rac_provider.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/rac_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/rac_provider_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/rac_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/radius_outpost_config.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/radius_outpost_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/radius_provider.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/radius_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/radius_provider_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/radius_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/redirect_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/redirect_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/reputation.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/reputation.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/reputation_policy.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/reputation_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/reputation_policy_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/reputation_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/resident_key_requirement_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/resident_key_requirement_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/role.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/role.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/role_assigned_object_permission.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/role_assigned_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/role_object_permission.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/role_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/role_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/role_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/saml_metadata.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/saml_metadata.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/saml_property_mapping.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/saml_property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/saml_property_mapping_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/saml_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/saml_provider.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/saml_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/saml_provider_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/saml_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/saml_source.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/saml_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/saml_source_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/saml_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/scim_mapping.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/scim_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/scim_mapping_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/scim_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/scim_provider.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/scim_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/scim_provider_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/scim_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/scim_source.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/scim_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/scim_source_group.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/scim_source_group.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/scim_source_group_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/scim_source_group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/scim_source_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/scim_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/scim_source_user.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/scim_source_user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/scim_source_user_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/scim_source_user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/scope_mapping.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/scope_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/scope_mapping_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/scope_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/selectable_stage.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/selectable_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/service_connection.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/service_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/service_connection_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/service_connection_state.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/service_connection_state.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/session_user.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/session_user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/settings.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/settings.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/settings_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/settings_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/severity_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/severity_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/shell_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/shell_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/signature_algorithm_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/signature_algorithm_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/sms_device.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/sms_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/sms_device_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/sms_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/source.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/source_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/source_stage.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/source_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/source_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/source_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/source_type.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/source_type.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/sp_binding_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/sp_binding_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/stage.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/stage_prompt.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/stage_prompt.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/static_device.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/static_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/static_device_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/static_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/static_device_token.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/static_device_token.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/static_device_token_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/static_device_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/sub_mode_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/sub_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/sync_status.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/sync_status.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/system_info.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/system_info.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/system_info_runtime.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/system_info_runtime.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/system_task.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/system_task.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/system_task_status_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/system_task_status_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/tenant.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/tenant.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/tenant_admin_group_request_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/tenant_admin_group_request_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/tenant_recovery_key_request_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/tenant_recovery_key_request_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/tenant_recovery_key_response.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/tenant_recovery_key_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/tenant_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/tenant_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/token.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/token.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/token_model.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/token_model.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/token_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/token_set_key_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/token_set_key_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/token_view.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/token_view.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/totp_device.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/totp_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/totp_device_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/totp_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/transaction_application_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/transaction_application_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/transaction_application_response.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/transaction_application_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/type_create.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/type_create.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/ui_theme_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/ui_theme_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/used_by.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/used_by.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/used_by_action_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/used_by_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_account_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_account_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_assigned_object_permission.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_assigned_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_consent.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_consent.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_creation_mode_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_creation_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_delete_stage.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_delete_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_delete_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_delete_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_fields_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_fields_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_group.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_group.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_group_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_login_challenge.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_login_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_login_challenge_response_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_login_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_login_stage.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_login_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_login_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_login_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_logout_stage.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_logout_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_logout_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_logout_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_matching_mode_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_matching_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_metrics.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_metrics.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_o_auth_source_connection.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_o_auth_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_o_auth_source_connection_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_o_auth_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_object_permission.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_password_set_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_password_set_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_path.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_path.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_saml_source_connection.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_saml_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_saml_source_connection_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_saml_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_self.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_self.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_self_groups.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_self_groups.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_service_account_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_service_account_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_service_account_response.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_service_account_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_setting.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_setting.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_source_connection.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_type_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_verification_enum.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_verification_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_write_stage.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_write_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/user_write_stage_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/user_write_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/validation_error.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/version.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/version.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/web_authn_device.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/web_authn_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/web_authn_device_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/web_authn_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/web_authn_device_type.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/web_authn_device_type.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/web_authn_device_type_request.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/web_authn_device_type_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/models/workers.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/models/workers.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/authentik_client/rest.py` & `authentik_client-2024.4.2.post1716209289/authentik_client/rest.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1715271061/pyproject.toml` & `authentik_client-2024.4.2.post1716209289/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "authentik_client"
-version = "2024.4.2-1715271061"
+version = "2024.4.2-1716209289"
 description = "authentik"
 authors = ["authentik Team <hello@goauthentik.io>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/goauthentik/authentik"
 keywords = ["OpenAPI", "OpenAPI-Generator", "authentik"]
 include = ["authentik_client/py.typed"]
```

### Comparing `authentik_client-2024.4.2.post1715271061/PKG-INFO` & `authentik_client-2024.4.2.post1716209289/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authentik_client
-Version: 2024.4.2.post1715271061
+Version: 2024.4.2.post1716209289
 Summary: authentik
 Home-page: https://github.com/goauthentik/authentik
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,authentik
 Author: authentik Team
 Author-email: hello@goauthentik.io
 Requires-Python: >=3.7,<4.0
@@ -25,15 +25,15 @@
 
 # authentik-client
 Making authentication simple.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 2024.4.2
-- Package version: 2024.4.2-1715271061
+- Package version: 2024.4.2-1716209289
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
```

