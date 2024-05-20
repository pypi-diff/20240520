# Comparing `tmp/stytch-9.4.0.tar.gz` & `tmp/stytch-9.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stytch-9.4.0.tar", last modified: Fri May 10 19:42:29 2024, max compression
+gzip compressed data, was "stytch-9.5.0.tar", last modified: Mon May 20 17:51:00 2024, max compression
```

## Comparing `stytch-9.4.0.tar` & `stytch-9.5.0.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.551035 stytch-9.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-10 19:42:15.000000 stytch-9.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-10 19:42:29.551035 stytch-9.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-10 19:42:15.000000 stytch-9.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-10 19:42:29.551035 stytch-9.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-10 19:42:15.000000 stytch-9.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.531035 stytch-9.4.0/stytch/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.531035 stytch-9.4.0/stytch/b2b/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.535035 stytch-9.4.0/stytch/b2b/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/discovery_intermediate_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)    31712 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/discovery_organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    14518 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/magic_links_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/magic_links_email_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    13039 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/oauth_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    52736 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    54165 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/organizations_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/organizations_members_oauth_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/otp.py
--rw-r--r--   0 runner    (1001) docker     (127)    26141 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)    29234 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/passwords.py
--rw-r--r--   0 runner    (1001) docker     (127)    22956 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/rbac.py
--rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/recovery_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/scim.py
--rw-r--r--   0 runner    (1001) docker     (127)    18700 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/scim_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    44960 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16885 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/sso_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/sso_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    21306 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/api/totps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.539035 stytch-9.4.0/stytch/b2b/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/discovery_intermediate_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/discovery_organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/magic_links_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/magic_links_email_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/oauth_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    20944 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/organizations_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/organizations_members_oauth_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/passwords.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/rbac.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/recovery_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/scim.py
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/scim_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     8489 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/sso_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/sso_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/b2b/models/totps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.543035 stytch-9.4.0/stytch/consumer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.543035 stytch-9.4.0/stytch/consumer/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/crypto_wallets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/m2m.py
--rw-r--r--   0 runner    (1001) docker     (127)    18434 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/m2m_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/m2m_clients_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (127)    33694 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (127)    12591 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/otp.py
--rw-r--r--   0 runner    (1001) docker     (127)    17305 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/otp_email.py
--rw-r--r--   0 runner    (1001) docker     (127)    17857 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)    15907 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/otp_whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (127)    32236 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/passwords.py
--rw-r--r--   0 runner    (1001) docker     (127)    18193 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    16547 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15372 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/totps.py
--rw-r--r--   0 runner    (1001) docker     (127)    33576 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/users.py
--rw-r--r--   0 runner    (1001) docker     (127)    26192 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/api/webauthn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.547035 stytch-9.4.0/stytch/consumer/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/crypto_wallets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/m2m.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/m2m_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/m2m_clients_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/otp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/otp_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/otp_whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/passwords.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/totps.py
--rw-r--r--   0 runner    (1001) docker     (127)    15941 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/consumer/models/webauthn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.551035 stytch-9.4.0/stytch/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/core/api_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/core/client_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.551035 stytch-9.4.0/stytch/core/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/core/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/core/http/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/core/response_base.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.551035 stytch-9.4.0/stytch/shared/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/shared/jwt_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/shared/lazy_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/shared/method_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/shared/policy_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/shared/rbac_local.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 19:42:15.000000 stytch-9.4.0/stytch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.551035 stytch-9.4.0/stytch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-10 19:42:29.000000 stytch-9.4.0/stytch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-10 19:42:29.000000 stytch-9.4.0/stytch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:42:29.000000 stytch-9.4.0/stytch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 19:42:29.000000 stytch-9.4.0/stytch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 19:42:29.000000 stytch-9.4.0/stytch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:42:29.551035 stytch-9.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-05-10 19:42:15.000000 stytch-9.4.0/test/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    12544 2024-05-10 19:42:15.000000 stytch-9.4.0/test/test_integration_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.052755 stytch-9.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-20 17:50:47.000000 stytch-9.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-20 17:51:00.052755 stytch-9.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-20 17:50:47.000000 stytch-9.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 17:51:00.052755 stytch-9.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-20 17:50:47.000000 stytch-9.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.032755 stytch-9.5.0/stytch/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.036755 stytch-9.5.0/stytch/b2b/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.040755 stytch-9.5.0/stytch/b2b/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/discovery_intermediate_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31710 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/discovery_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14518 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/magic_links_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/magic_links_email_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13039 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/oauth_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52736 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55751 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/organizations_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/organizations_members_oauth_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/otp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26141 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29234 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22956 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/rbac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/recovery_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/scim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18700 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/scim_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45478 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16885 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13616 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/sso_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21459 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/sso_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21306 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/api/totps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.044755 stytch-9.5.0/stytch/b2b/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/discovery_intermediate_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/discovery_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/magic_links_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/magic_links_email_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/oauth_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20941 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/organizations_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/organizations_members_oauth_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/rbac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/recovery_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/scim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/scim_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8488 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7353 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/sso_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/sso_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/b2b/models/totps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.044755 stytch-9.5.0/stytch/consumer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.048755 stytch-9.5.0/stytch/consumer/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/m2m.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18434 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/m2m_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/m2m_clients_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33694 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12591 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/otp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17305 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17857 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15907 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32236 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18193 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17473 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15372 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/totps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33576 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26192 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/api/webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.052755 stytch-9.5.0/stytch/consumer/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/m2m.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/m2m_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/m2m_clients_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/otp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/totps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15941 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/consumer/models/webauthn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.052755 stytch-9.5.0/stytch/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/core/api_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/core/client_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.052755 stytch-9.5.0/stytch/core/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/core/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/core/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/core/response_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.052755 stytch-9.5.0/stytch/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/shared/jwt_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/shared/lazy_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/shared/method_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/shared/policy_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/shared/rbac_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 17:50:47.000000 stytch-9.5.0/stytch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.052755 stytch-9.5.0/stytch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-20 17:51:00.000000 stytch-9.5.0/stytch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-20 17:51:00.000000 stytch-9.5.0/stytch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 17:51:00.000000 stytch-9.5.0/stytch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-20 17:51:00.000000 stytch-9.5.0/stytch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 17:51:00.000000 stytch-9.5.0/stytch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:51:00.052755 stytch-9.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-05-20 17:50:47.000000 stytch-9.5.0/test/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12544 2024-05-20 17:50:47.000000 stytch-9.5.0/test/test_integration_async.py
```

### Comparing `stytch-9.4.0/LICENSE.txt` & `stytch-9.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/PKG-INFO` & `stytch-9.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 9.4.0
+Version: 9.5.0
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stytch-9.4.0/README.md` & `stytch-9.5.0/README.md`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/setup.py` & `stytch-9.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/api/discovery.py` & `stytch-9.5.0/stytch/b2b/api/discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/api/discovery_intermediate_sessions.py` & `stytch-9.5.0/stytch/b2b/api/discovery_intermediate_sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/api/discovery_organizations.py` & `stytch-9.5.0/stytch/b2b/api/discovery_organizations.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         [Organization](https://stytch.com/docs/b2b/api/organization-object) and [Member](https://stytch.com/docs/b2b/api/member-object).
 
         This operation consumes the Intermediate Session.
 
         This endpoint will also create an initial Member Session for the newly created Member.
 
         The Member created by this endpoint will automatically be granted the `stytch_admin` Role. See the
-        [RBAC guide](https://stytch.com/docs/b2b/guides/rbac/stytch-defaults) for more details on this Role.
+        [RBAC guide](https://stytch.com/docs/b2b/guides/rbac/stytch-default) for more details on this Role.
 
         If the new Organization is created with a `mfa_policy` of `REQUIRED_FOR_ALL`, the newly created Member will need to complete an MFA step to log in to the Organization.
         The `intermediate_session_token` will not be consumed and instead will be returned in the response.
         The `intermediate_session_token` can be passed into the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms) to complete the MFA step and acquire a full member session.
         The `intermediate_session_token` can also be used with the [Exchange Intermediate Session endpoint](https://stytch.com/docs/b2b/api/exchange-intermediate-session) or the [Create Organization via Discovery endpoint](https://stytch.com/docs/b2b/api/create-organization-via-discovery) to join a different Organization or create a new one.
         The `session_duration_minutes` and `session_custom_claims` parameters will be ignored.
 
@@ -203,15 +203,15 @@
         [Organization](https://stytch.com/docs/b2b/api/organization-object) and [Member](https://stytch.com/docs/b2b/api/member-object).
 
         This operation consumes the Intermediate Session.
 
         This endpoint will also create an initial Member Session for the newly created Member.
 
         The Member created by this endpoint will automatically be granted the `stytch_admin` Role. See the
-        [RBAC guide](https://stytch.com/docs/b2b/guides/rbac/stytch-defaults) for more details on this Role.
+        [RBAC guide](https://stytch.com/docs/b2b/guides/rbac/stytch-default) for more details on this Role.
 
         If the new Organization is created with a `mfa_policy` of `REQUIRED_FOR_ALL`, the newly created Member will need to complete an MFA step to log in to the Organization.
         The `intermediate_session_token` will not be consumed and instead will be returned in the response.
         The `intermediate_session_token` can be passed into the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms) to complete the MFA step and acquire a full member session.
         The `intermediate_session_token` can also be used with the [Exchange Intermediate Session endpoint](https://stytch.com/docs/b2b/api/exchange-intermediate-session) or the [Create Organization via Discovery endpoint](https://stytch.com/docs/b2b/api/create-organization-via-discovery) to join a different Organization or create a new one.
         The `session_duration_minutes` and `session_custom_claims` parameters will be ignored.
```

### Comparing `stytch-9.4.0/stytch/b2b/api/magic_links.py` & `stytch-9.5.0/stytch/b2b/api/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/api/magic_links_discovery.py` & `stytch-9.5.0/stytch/b2b/api/magic_links_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/api/magic_links_email.py` & `stytch-9.5.0/stytch/b2b/api/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/api/magic_links_email_discovery.py` & `stytch-9.5.0/stytch/b2b/api/magic_links_email_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/api/oauth.py` & `stytch-9.5.0/stytch/b2b/api/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/api/oauth_discovery.py` & `stytch-9.5.0/stytch/b2b/api/oauth_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/api/organizations.py` & `stytch-9.5.0/stytch/b2b/api/organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/api/organizations_members.py` & `stytch-9.5.0/stytch/b2b/api/organizations_members.py`

 * *Files 2% similar despite different names*

```diff
@@ -442,14 +442,25 @@
 
     def delete_totp(
         self,
         organization_id: str,
         member_id: str,
         method_options: Optional[DeleteTOTPRequestOptions] = None,
     ) -> DeleteTOTPResponse:
+        """Delete a Member's MFA TOTP registration.
+
+        To mint a new registration for a Member, you must first call this endpoint to delete the existing registration.
+
+        Existing Member Sessions that include the TOTP authentication factor will not be revoked if the registration is deleted, and MFA will not be enforced until the Member logs in again.
+         /%}
+
+        Fields:
+          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+          - member_id: Globally unique UUID that identifies a specific Member. The `member_id` is critical to perform operations on a Member, so be sure to preserve this value.
+        """  # noqa
         headers: Dict[str, str] = {}
         if method_options is not None:
             headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "member_id": member_id,
         }
@@ -462,14 +473,25 @@
 
     async def delete_totp_async(
         self,
         organization_id: str,
         member_id: str,
         method_options: Optional[DeleteTOTPRequestOptions] = None,
     ) -> DeleteTOTPResponse:
+        """Delete a Member's MFA TOTP registration.
+
+        To mint a new registration for a Member, you must first call this endpoint to delete the existing registration.
+
+        Existing Member Sessions that include the TOTP authentication factor will not be revoked if the registration is deleted, and MFA will not be enforced until the Member logs in again.
+         /%}
+
+        Fields:
+          - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+          - member_id: Globally unique UUID that identifies a specific Member. The `member_id` is critical to perform operations on a Member, so be sure to preserve this value.
+        """  # noqa
         headers: Dict[str, str] = {}
         if method_options is not None:
             headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "member_id": member_id,
         }
```

### Comparing `stytch-9.4.0/stytch/b2b/api/organizations_members_oauth_providers.py` & `stytch-9.5.0/stytch/b2b/api/organizations_members_oauth_providers.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,16 @@
         member_id: str,
         include_refresh_token: Optional[bool] = None,
     ) -> GoogleResponse:
         """Retrieve the saved Google access token and ID token for a member. After a successful OAuth login, Stytch will save the
         issued access token and ID token from the identity provider. If a refresh token has been issued, Stytch will refresh the
         access token automatically.
 
+        Google One Tap does not return access tokens. If the member has only authenticated through Google One Tap and not through a regular Google OAuth flow, this endpoint will not return any tokens.
+
         __Note:__ Google does not issue a refresh token on every login, and refresh tokens may expire if unused.
         To force a refresh token to be issued, pass the `?provider_prompt=consent` query param into the
         [Start Google OAuth flow](https://stytch.com/docs/b2b/api/oauth-google-start) endpoint.
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - member_id: Globally unique UUID that identifies a specific Member. The `member_id` is critical to perform operations on a Member, so be sure to preserve this value.
@@ -64,14 +66,16 @@
         member_id: str,
         include_refresh_token: Optional[bool] = None,
     ) -> GoogleResponse:
         """Retrieve the saved Google access token and ID token for a member. After a successful OAuth login, Stytch will save the
         issued access token and ID token from the identity provider. If a refresh token has been issued, Stytch will refresh the
         access token automatically.
 
+        Google One Tap does not return access tokens. If the member has only authenticated through Google One Tap and not through a regular Google OAuth flow, this endpoint will not return any tokens.
+
         __Note:__ Google does not issue a refresh token on every login, and refresh tokens may expire if unused.
         To force a refresh token to be issued, pass the `?provider_prompt=consent` query param into the
         [Start Google OAuth flow](https://stytch.com/docs/b2b/api/oauth-google-start) endpoint.
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - member_id: Globally unique UUID that identifies a specific Member. The `member_id` is critical to perform operations on a Member, so be sure to preserve this value.
```

### Comparing `stytch-9.4.0/stytch/b2b/api/otp.py` & `stytch-9.5.0/stytch/b2b/api/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/api/otp_sms.py` & `stytch-9.5.0/stytch/b2b/api/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/api/passwords.py` & `stytch-9.5.0/stytch/b2b/api/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/api/passwords_email.py` & `stytch-9.5.0/stytch/b2b/api/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/api/passwords_existing_password.py` & `stytch-9.5.0/stytch/b2b/api/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/api/passwords_session.py` & `stytch-9.5.0/stytch/b2b/api/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/api/rbac.py` & `stytch-9.5.0/stytch/b2b/api/rbac.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/api/recovery_codes.py` & `stytch-9.5.0/stytch/b2b/api/recovery_codes.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/api/scim.py` & `stytch-9.5.0/stytch/b2b/api/scim.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/api/scim_connections.py` & `stytch-9.5.0/stytch/b2b/api/scim_connections.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/api/sessions.py` & `stytch-9.5.0/stytch/b2b/api/sessions.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         session_duration_minutes: Optional[int] = None,
         session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
         authorization_check: Optional[Union[AuthorizationCheck, Dict[str, Any]]] = None,
     ) -> AuthenticateResponse:
         """Authenticates a Session and updates its lifetime by the specified `session_duration_minutes`. If the `session_duration_minutes` is not specified, a Session will not be extended. This endpoint requires either a `session_jwt` or `session_token` be included in the request. It will return an error if both are present.
 
-        You may provide a JWT that needs to be refreshed and is expired according to its `exp` claim. A new JWT will be returned if both the signature and the underlying Session are still valid.
+        You may provide a JWT that needs to be refreshed and is expired according to its `exp` claim. A new JWT will be returned if both the signature and the underlying Session are still valid. See our [How to use Stytch Session JWTs](https://stytch.com/docs/b2b/guides/sessions/using-jwts) guide for more information.
 
         If an `authorization_check` object is passed in, this method will also check if the Member is authorized to perform the given action on the given Resource in the specified Organization. A Member is authorized if their Member Session contains a Role, assigned [explicitly or implicitly](https://stytch.com/docs/b2b/guides/rbac/role-assignment), with adequate permissions.
         In addition, the `organization_id` passed in the authorization check must match the Member's Organization.
 
         If the Member is not authorized to perform the specified action on the specified Resource, or if the
         `organization_id` does not match the Member's Organization, a 403 error will be thrown.
         Otherwise, the response will contain a list of Roles that satisfied the authorization check.
@@ -164,15 +164,15 @@
         session_duration_minutes: Optional[int] = None,
         session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
         authorization_check: Optional[AuthorizationCheck] = None,
     ) -> AuthenticateResponse:
         """Authenticates a Session and updates its lifetime by the specified `session_duration_minutes`. If the `session_duration_minutes` is not specified, a Session will not be extended. This endpoint requires either a `session_jwt` or `session_token` be included in the request. It will return an error if both are present.
 
-        You may provide a JWT that needs to be refreshed and is expired according to its `exp` claim. A new JWT will be returned if both the signature and the underlying Session are still valid.
+        You may provide a JWT that needs to be refreshed and is expired according to its `exp` claim. A new JWT will be returned if both the signature and the underlying Session are still valid. See our [How to use Stytch Session JWTs](https://stytch.com/docs/b2b/guides/sessions/using-jwts) guide for more information.
 
         If an `authorization_check` object is passed in, this method will also check if the Member is authorized to perform the given action on the given Resource in the specified Organization. A Member is authorized if their Member Session contains a Role, assigned [explicitly or implicitly](https://stytch.com/docs/b2b/guides/rbac/role-assignment), with adequate permissions.
         In addition, the `organization_id` passed in the authorization check must match the Member's Organization.
 
         If the Member is not authorized to perform the specified action on the specified Resource, or if the
         `organization_id` does not match the Member's Organization, a 403 error will be thrown.
         Otherwise, the response will contain a list of Roles that satisfied the authorization check.
@@ -517,14 +517,16 @@
 
         JWTs have a set lifetime of 5 minutes, so there will be a 5 minute period where some JWTs will be signed by the old JWKS, and some JWTs will be signed by the new JWKS. The correct JWKS to use for validation is determined by matching the `kid` value of the JWT and JWKS.
 
         If you're using one of our [backend SDKs](https://stytch.com/docs/b2b/sdks), the JWKS roll will be handled for you.
 
         If you're using your own JWT validation library, many have built-in support for JWKS rotation, and you'll just need to supply this API endpoint. If not, your application should decide which JWKS to use for validation by inspecting the `kid` value.
 
+        See our [How to use Stytch Session JWTs](https://stytch.com/docs/b2b/guides/sessions/using-jwts) guide for more information.
+
         Fields:
           - project_id: The `project_id` to get the JWKS for.
         """  # noqa
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "project_id": project_id,
         }
@@ -543,14 +545,16 @@
 
         JWTs have a set lifetime of 5 minutes, so there will be a 5 minute period where some JWTs will be signed by the old JWKS, and some JWTs will be signed by the new JWKS. The correct JWKS to use for validation is determined by matching the `kid` value of the JWT and JWKS.
 
         If you're using one of our [backend SDKs](https://stytch.com/docs/b2b/sdks), the JWKS roll will be handled for you.
 
         If you're using your own JWT validation library, many have built-in support for JWKS rotation, and you'll just need to supply this API endpoint. If not, your application should decide which JWKS to use for validation by inspecting the `kid` value.
 
+        See our [How to use Stytch Session JWTs](https://stytch.com/docs/b2b/guides/sessions/using-jwts) guide for more information.
+
         Fields:
           - project_id: The `project_id` to get the JWKS for.
         """  # noqa
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "project_id": project_id,
         }
```

### Comparing `stytch-9.4.0/stytch/b2b/api/sso.py` & `stytch-9.5.0/stytch/b2b/api/sso.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/api/sso_oidc.py` & `stytch-9.5.0/stytch/b2b/api/sso_oidc.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Union
 
 from stytch.b2b.models.sso_oidc import (
+    CreateConnectionRequestIdentityProvider,
     CreateConnectionRequestOptions,
     CreateConnectionResponse,
+    UpdateConnectionRequestIdentityProvider,
     UpdateConnectionRequestOptions,
     UpdateConnectionResponse,
 )
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
@@ -26,55 +28,65 @@
         self.sync_client = sync_client
         self.async_client = async_client
 
     def create_connection(
         self,
         organization_id: str,
         display_name: Optional[str] = None,
+        identity_provider: Optional[
+            Union[CreateConnectionRequestIdentityProvider, str]
+        ] = None,
         method_options: Optional[CreateConnectionRequestOptions] = None,
     ) -> CreateConnectionResponse:
         """Create a new OIDC Connection. /%}
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - display_name: A human-readable display name for the connection.
+          - identity_provider: The identity provider of this connection. For OIDC, the accepted values are `generic`, `okta`, and `microsoft-entra`. For SAML, the accepted values are `generic`, `okta`, `microsoft-entra`, and `google-workspace`.
         """  # noqa
         headers: Dict[str, str] = {}
         if method_options is not None:
             headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
         }
         if display_name is not None:
             data["display_name"] = display_name
+        if identity_provider is not None:
+            data["identity_provider"] = identity_provider
 
         url = self.api_base.url_for("/v1/b2b/sso/oidc/{organization_id}", data)
         res = self.sync_client.post(url, data, headers)
         return CreateConnectionResponse.from_json(res.response.status_code, res.json)
 
     async def create_connection_async(
         self,
         organization_id: str,
         display_name: Optional[str] = None,
+        identity_provider: Optional[CreateConnectionRequestIdentityProvider] = None,
         method_options: Optional[CreateConnectionRequestOptions] = None,
     ) -> CreateConnectionResponse:
         """Create a new OIDC Connection. /%}
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - display_name: A human-readable display name for the connection.
+          - identity_provider: The identity provider of this connection. For OIDC, the accepted values are `generic`, `okta`, and `microsoft-entra`. For SAML, the accepted values are `generic`, `okta`, `microsoft-entra`, and `google-workspace`.
         """  # noqa
         headers: Dict[str, str] = {}
         if method_options is not None:
             headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
         }
         if display_name is not None:
             data["display_name"] = display_name
+        if identity_provider is not None:
+            data["identity_provider"] = identity_provider
 
         url = self.api_base.url_for("/v1/b2b/sso/oidc/{organization_id}", data)
         res = await self.async_client.post(url, data, headers)
         return CreateConnectionResponse.from_json(res.response.status, res.json)
 
     def update_connection(
         self,
@@ -84,14 +96,17 @@
         client_id: Optional[str] = None,
         client_secret: Optional[str] = None,
         issuer: Optional[str] = None,
         authorization_url: Optional[str] = None,
         token_url: Optional[str] = None,
         userinfo_url: Optional[str] = None,
         jwks_url: Optional[str] = None,
+        identity_provider: Optional[
+            Union[UpdateConnectionRequestIdentityProvider, str]
+        ] = None,
         method_options: Optional[UpdateConnectionRequestOptions] = None,
     ) -> UpdateConnectionResponse:
         """Updates an existing OIDC connection.
 
         When the value of `issuer` changes, Stytch will attempt to retrieve the [OpenID Provider Metadata](https://openid.net/specs/openid-connect-discovery-1_0.html#ProviderMetadata) document found at `$/.well-known/openid-configuration`.
         If the metadata document can be retrieved successfully, Stytch will use it to infer the values of `authorization_url`, `token_url`, `jwks_url`, and `userinfo_url`.
         The `client_id` and `client_secret` values cannot be inferred from the metadata document, and *must* be passed in explicitly.
@@ -117,14 +132,15 @@
           - client_id: The OAuth2.0 client ID used to authenticate login attempts. This will be provided by the IdP.
           - client_secret: The secret belonging to the OAuth2.0 client used to authenticate login attempts. This will be provided by the IdP.
           - issuer: A case-sensitive `https://` URL that uniquely identifies the IdP. This will be provided by the IdP.
           - authorization_url: The location of the URL that starts an OAuth login at the IdP. This will be provided by the IdP.
           - token_url: The location of the URL that issues OAuth2.0 access tokens and OIDC ID tokens. This will be provided by the IdP.
           - userinfo_url: The location of the IDP's [UserInfo Endpoint](https://openid.net/specs/openid-connect-core-1_0.html#UserInfo). This will be provided by the IdP.
           - jwks_url: The location of the IdP's JSON Web Key Set, used to verify credentials issued by the IdP. This will be provided by the IdP.
+          - identity_provider: The identity provider of this connection. For OIDC, the accepted values are `generic`, `okta`, and `microsoft-entra`. For SAML, the accepted values are `generic`, `okta`, `microsoft-entra`, and `google-workspace`.
         """  # noqa
         headers: Dict[str, str] = {}
         if method_options is not None:
             headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "connection_id": connection_id,
@@ -141,14 +157,16 @@
             data["authorization_url"] = authorization_url
         if token_url is not None:
             data["token_url"] = token_url
         if userinfo_url is not None:
             data["userinfo_url"] = userinfo_url
         if jwks_url is not None:
             data["jwks_url"] = jwks_url
+        if identity_provider is not None:
+            data["identity_provider"] = identity_provider
 
         url = self.api_base.url_for(
             "/v1/b2b/sso/oidc/{organization_id}/connections/{connection_id}", data
         )
         res = self.sync_client.put(url, data, headers)
         return UpdateConnectionResponse.from_json(res.response.status_code, res.json)
 
@@ -160,14 +178,15 @@
         client_id: Optional[str] = None,
         client_secret: Optional[str] = None,
         issuer: Optional[str] = None,
         authorization_url: Optional[str] = None,
         token_url: Optional[str] = None,
         userinfo_url: Optional[str] = None,
         jwks_url: Optional[str] = None,
+        identity_provider: Optional[UpdateConnectionRequestIdentityProvider] = None,
         method_options: Optional[UpdateConnectionRequestOptions] = None,
     ) -> UpdateConnectionResponse:
         """Updates an existing OIDC connection.
 
         When the value of `issuer` changes, Stytch will attempt to retrieve the [OpenID Provider Metadata](https://openid.net/specs/openid-connect-discovery-1_0.html#ProviderMetadata) document found at `$/.well-known/openid-configuration`.
         If the metadata document can be retrieved successfully, Stytch will use it to infer the values of `authorization_url`, `token_url`, `jwks_url`, and `userinfo_url`.
         The `client_id` and `client_secret` values cannot be inferred from the metadata document, and *must* be passed in explicitly.
@@ -193,14 +212,15 @@
           - client_id: The OAuth2.0 client ID used to authenticate login attempts. This will be provided by the IdP.
           - client_secret: The secret belonging to the OAuth2.0 client used to authenticate login attempts. This will be provided by the IdP.
           - issuer: A case-sensitive `https://` URL that uniquely identifies the IdP. This will be provided by the IdP.
           - authorization_url: The location of the URL that starts an OAuth login at the IdP. This will be provided by the IdP.
           - token_url: The location of the URL that issues OAuth2.0 access tokens and OIDC ID tokens. This will be provided by the IdP.
           - userinfo_url: The location of the IDP's [UserInfo Endpoint](https://openid.net/specs/openid-connect-core-1_0.html#UserInfo). This will be provided by the IdP.
           - jwks_url: The location of the IdP's JSON Web Key Set, used to verify credentials issued by the IdP. This will be provided by the IdP.
+          - identity_provider: The identity provider of this connection. For OIDC, the accepted values are `generic`, `okta`, and `microsoft-entra`. For SAML, the accepted values are `generic`, `okta`, `microsoft-entra`, and `google-workspace`.
         """  # noqa
         headers: Dict[str, str] = {}
         if method_options is not None:
             headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "connection_id": connection_id,
@@ -217,13 +237,15 @@
             data["authorization_url"] = authorization_url
         if token_url is not None:
             data["token_url"] = token_url
         if userinfo_url is not None:
             data["userinfo_url"] = userinfo_url
         if jwks_url is not None:
             data["jwks_url"] = jwks_url
+        if identity_provider is not None:
+            data["identity_provider"] = identity_provider
 
         url = self.api_base.url_for(
             "/v1/b2b/sso/oidc/{organization_id}/connections/{connection_id}", data
         )
         res = await self.async_client.put(url, data, headers)
         return UpdateConnectionResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-9.4.0/stytch/b2b/api/sso_saml.py` & `stytch-9.5.0/stytch/b2b/api/sso_saml.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 from typing import Any, Dict, List, Optional, Union
 
 from stytch.b2b.models.sso import (
     SAMLConnectionImplicitRoleAssignment,
     SAMLGroupImplicitRoleAssignment,
 )
 from stytch.b2b.models.sso_saml import (
+    CreateConnectionRequestIdentityProvider,
     CreateConnectionRequestOptions,
     CreateConnectionResponse,
     DeleteVerificationCertificateRequestOptions,
     DeleteVerificationCertificateResponse,
     UpdateByURLRequestOptions,
     UpdateByURLResponse,
+    UpdateConnectionRequestIdentityProvider,
     UpdateConnectionRequestOptions,
     UpdateConnectionResponse,
 )
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
@@ -34,55 +36,65 @@
         self.sync_client = sync_client
         self.async_client = async_client
 
     def create_connection(
         self,
         organization_id: str,
         display_name: Optional[str] = None,
+        identity_provider: Optional[
+            Union[CreateConnectionRequestIdentityProvider, str]
+        ] = None,
         method_options: Optional[CreateConnectionRequestOptions] = None,
     ) -> CreateConnectionResponse:
         """Create a new SAML Connection. /%}
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - display_name: A human-readable display name for the connection.
+          - identity_provider: The identity provider of this connection. For OIDC, the accepted values are `generic`, `okta`, and `microsoft-entra`. For SAML, the accepted values are `generic`, `okta`, `microsoft-entra`, and `google-workspace`.
         """  # noqa
         headers: Dict[str, str] = {}
         if method_options is not None:
             headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
         }
         if display_name is not None:
             data["display_name"] = display_name
+        if identity_provider is not None:
+            data["identity_provider"] = identity_provider
 
         url = self.api_base.url_for("/v1/b2b/sso/saml/{organization_id}", data)
         res = self.sync_client.post(url, data, headers)
         return CreateConnectionResponse.from_json(res.response.status_code, res.json)
 
     async def create_connection_async(
         self,
         organization_id: str,
         display_name: Optional[str] = None,
+        identity_provider: Optional[CreateConnectionRequestIdentityProvider] = None,
         method_options: Optional[CreateConnectionRequestOptions] = None,
     ) -> CreateConnectionResponse:
         """Create a new SAML Connection. /%}
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - display_name: A human-readable display name for the connection.
+          - identity_provider: The identity provider of this connection. For OIDC, the accepted values are `generic`, `okta`, and `microsoft-entra`. For SAML, the accepted values are `generic`, `okta`, `microsoft-entra`, and `google-workspace`.
         """  # noqa
         headers: Dict[str, str] = {}
         if method_options is not None:
             headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
         }
         if display_name is not None:
             data["display_name"] = display_name
+        if identity_provider is not None:
+            data["identity_provider"] = identity_provider
 
         url = self.api_base.url_for("/v1/b2b/sso/saml/{organization_id}", data)
         res = await self.async_client.post(url, data, headers)
         return CreateConnectionResponse.from_json(res.response.status, res.json)
 
     def update_connection(
         self,
@@ -96,14 +108,17 @@
         saml_connection_implicit_role_assignments: Optional[
             List[Union[SAMLConnectionImplicitRoleAssignment, Dict[str, Any]]]
         ] = None,
         saml_group_implicit_role_assignments: Optional[
             List[Union[SAMLGroupImplicitRoleAssignment, Dict[str, Any]]]
         ] = None,
         alternative_audience_uri: Optional[str] = None,
+        identity_provider: Optional[
+            Union[UpdateConnectionRequestIdentityProvider, str]
+        ] = None,
         method_options: Optional[UpdateConnectionRequestOptions] = None,
     ) -> UpdateConnectionResponse:
         """Updates an existing SAML connection.
 
         Note that a newly created connection will not become active until all of the following are provided:
         * `idp_sso_url`
         * `attribute_mapping`
@@ -123,14 +138,15 @@
           - saml_group_implicit_role_assignments: Defines the names of the SAML groups
          that grant specific role assignments. For each group-Role pair, if a Member logs in with this SAML connection and
          belongs to the specified SAML group, they will be granted the associated Role. See the
          [RBAC guide](https://stytch.com/docs/b2b/guides/rbac/role-assignment) for more information about role assignment.
                  Before adding any group implicit role assignments, you must add a "groups" key to your SAML connection's
                  `attribute_mapping`. Make sure that your IdP is configured to correctly send the group information.
           - alternative_audience_uri: An alternative URL to use for the Audience Restriction. This value can be used when you wish to migrate an existing SAML integration to Stytch with zero downtime.
+          - identity_provider: The identity provider of this connection. For OIDC, the accepted values are `generic`, `okta`, and `microsoft-entra`. For SAML, the accepted values are `generic`, `okta`, `microsoft-entra`, and `google-workspace`.
         """  # noqa
         headers: Dict[str, str] = {}
         if method_options is not None:
             headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "connection_id": connection_id,
@@ -153,14 +169,16 @@
         if saml_group_implicit_role_assignments is not None:
             data["saml_group_implicit_role_assignments"] = [
                 item if isinstance(item, dict) else item.dict()
                 for item in saml_group_implicit_role_assignments
             ]
         if alternative_audience_uri is not None:
             data["alternative_audience_uri"] = alternative_audience_uri
+        if identity_provider is not None:
+            data["identity_provider"] = identity_provider
 
         url = self.api_base.url_for(
             "/v1/b2b/sso/saml/{organization_id}/connections/{connection_id}", data
         )
         res = self.sync_client.put(url, data, headers)
         return UpdateConnectionResponse.from_json(res.response.status_code, res.json)
 
@@ -176,14 +194,15 @@
         saml_connection_implicit_role_assignments: Optional[
             List[SAMLConnectionImplicitRoleAssignment]
         ] = None,
         saml_group_implicit_role_assignments: Optional[
             List[SAMLGroupImplicitRoleAssignment]
         ] = None,
         alternative_audience_uri: Optional[str] = None,
+        identity_provider: Optional[UpdateConnectionRequestIdentityProvider] = None,
         method_options: Optional[UpdateConnectionRequestOptions] = None,
     ) -> UpdateConnectionResponse:
         """Updates an existing SAML connection.
 
         Note that a newly created connection will not become active until all of the following are provided:
         * `idp_sso_url`
         * `attribute_mapping`
@@ -203,14 +222,15 @@
           - saml_group_implicit_role_assignments: Defines the names of the SAML groups
          that grant specific role assignments. For each group-Role pair, if a Member logs in with this SAML connection and
          belongs to the specified SAML group, they will be granted the associated Role. See the
          [RBAC guide](https://stytch.com/docs/b2b/guides/rbac/role-assignment) for more information about role assignment.
                  Before adding any group implicit role assignments, you must add a "groups" key to your SAML connection's
                  `attribute_mapping`. Make sure that your IdP is configured to correctly send the group information.
           - alternative_audience_uri: An alternative URL to use for the Audience Restriction. This value can be used when you wish to migrate an existing SAML integration to Stytch with zero downtime.
+          - identity_provider: The identity provider of this connection. For OIDC, the accepted values are `generic`, `okta`, and `microsoft-entra`. For SAML, the accepted values are `generic`, `okta`, `microsoft-entra`, and `google-workspace`.
         """  # noqa
         headers: Dict[str, str] = {}
         if method_options is not None:
             headers = method_options.add_headers(headers)
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "connection_id": connection_id,
@@ -233,14 +253,16 @@
         if saml_group_implicit_role_assignments is not None:
             data["saml_group_implicit_role_assignments"] = [
                 item if isinstance(item, dict) else item.dict()
                 for item in saml_group_implicit_role_assignments
             ]
         if alternative_audience_uri is not None:
             data["alternative_audience_uri"] = alternative_audience_uri
+        if identity_provider is not None:
+            data["identity_provider"] = identity_provider
 
         url = self.api_base.url_for(
             "/v1/b2b/sso/saml/{organization_id}/connections/{connection_id}", data
         )
         res = await self.async_client.put(url, data, headers)
         return UpdateConnectionResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-9.4.0/stytch/b2b/api/totps.py` & `stytch-9.5.0/stytch/b2b/api/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/client.py` & `stytch-9.5.0/stytch/b2b/client.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/models/discovery.py` & `stytch-9.5.0/stytch/b2b/models/discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/models/discovery_intermediate_sessions.py` & `stytch-9.5.0/stytch/b2b/models/discovery_intermediate_sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/models/discovery_organizations.py` & `stytch-9.5.0/stytch/b2b/models/discovery_organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/models/magic_links.py` & `stytch-9.5.0/stytch/b2b/models/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/models/magic_links_discovery.py` & `stytch-9.5.0/stytch/b2b/models/magic_links_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/models/magic_links_email.py` & `stytch-9.5.0/stytch/b2b/models/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/models/mfa.py` & `stytch-9.5.0/stytch/b2b/models/mfa.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/models/oauth.py` & `stytch-9.5.0/stytch/b2b/models/oauth.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
       - organization: The [Organization object](https://stytch.com/docs/b2b/api/organization-object).
       - reset_sessions: (no documentation yet)
       - member_authenticated: Indicates whether the Member is fully authenticated. If false, the Member needs to complete an MFA step to log in to the Organization.
       - intermediate_session_token: The returned Intermediate Session Token contains an OAuth factor associated with the Member's email address. If this value is non-empty, the member must complete an MFA step to finish logging in to the Organization. The token can be used with the [OTP SMS Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-otp-sms), [TOTP Authenticate endpoint](https://stytch.com/docs/b2b/api/authenticate-totp), or [Recovery Codes Recover endpoint](https://stytch.com/docs/b2b/api/recovery-codes-recover) to complete an MFA flow and log in to the Organization. It can also be used with the [Exchange Intermediate Session endpoint](https://stytch.com/docs/b2b/api/exchange-intermediate-session) to join a specific Organization that allows the factors represented by the intermediate session token; or the [Create Organization via Discovery endpoint](https://stytch.com/docs/b2b/api/create-organization-via-discovery) to create a new Organization and Member.
       - member_session: The [Session object](https://stytch.com/docs/b2b/api/session-object).
       - provider_values: The `provider_values` object lists relevant identifiers, values, and scopes for a given OAuth provider. For example this object will include a provider's `access_token` that you can use to access the provider's API for a given user.
 
-      Note that these values will vary based on the OAuth provider in question, e.g. `id_token` is only returned by Microsoft.
+      Note that these values will vary based on the OAuth provider in question, e.g. `id_token` is only returned by Microsoft. Google One Tap does not return access tokens or refresh tokens.
       - mfa_required: Information about the MFA requirements of the Organization and the Member's options for fulfilling MFA.
       - primary_required: (no documentation yet)
     """  # noqa
 
     member_id: str
     provider_subject: str
     provider_type: str
```

### Comparing `stytch-9.4.0/stytch/b2b/models/oauth_discovery.py` & `stytch-9.5.0/stytch/b2b/models/oauth_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/models/organizations.py` & `stytch-9.5.0/stytch/b2b/models/organizations.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
       - role_id: The unique identifier of the RBAC Role, provided by the developer and intended to be human-readable.
 
       Reserved `role_id`s that are predefined by Stytch include:
 
       * `stytch_member`
       * `stytch_admin`
 
-      Check out the [guide on Stytch default Roles](https://stytch.com/docs/b2b/guides/rbac/stytch-defaults) for a more detailed explanation.
+      Check out the [guide on Stytch default Roles](https://stytch.com/docs/b2b/guides/rbac/stytch-default) for a more detailed explanation.
 
 
     """  # noqa
 
     domain: str
     role_id: str
 
@@ -143,15 +143,15 @@
       - role_id: The unique identifier of the RBAC Role, provided by the developer and intended to be human-readable.
 
       Reserved `role_id`s that are predefined by Stytch include:
 
       * `stytch_member`
       * `stytch_admin`
 
-      Check out the [guide on Stytch default Roles](https://stytch.com/docs/b2b/guides/rbac/stytch-defaults) for a more detailed explanation.
+      Check out the [guide on Stytch default Roles](https://stytch.com/docs/b2b/guides/rbac/stytch-default) for a more detailed explanation.
 
 
       - sources: A list of sources for this role assignment. A role assignment can come from multiple sources - for example, the Role could be both explicitly assigned and implicitly granted from the Member's email domain.
     """  # noqa
 
     role_id: str
     sources: List[MemberRoleSource]
@@ -312,15 +312,15 @@
       - is_breakglass: Identifies the Member as a break glass user - someone who has permissions to authenticate into an Organization by bypassing the Organization's settings. A break glass account is typically used for emergency purposes to gain access outside of normal authentication procedures. Refer to the [Organization object](organization-object) and its `auth_methods` and `allowed_auth_methods` fields for more details.
       - member_password_id: Globally unique UUID that identifies a Member's password.
       - oauth_registrations: A list of OAuth registrations for this member.
       - email_address_verified: Whether or not the Member's email address is verified.
       - mfa_phone_number_verified: Whether or not the Member's phone number is verified.
       - is_admin: Whether or not the Member has the `stytch_admin` Role. This Role is automatically granted to Members
       who create an Organization through the [discovery flow](https://stytch.com/docs/b2b/api/create-organization-via-discovery). See the
-      [RBAC guide](https://stytch.com/docs/b2b/guides/rbac/stytch-defaults) for more details on this Role.
+      [RBAC guide](https://stytch.com/docs/b2b/guides/rbac/stytch-default) for more details on this Role.
       - totp_registration_id: (no documentation yet)
       - scim_registrations: An array of scim member registrations, each one referencing a [SCIM Connection](scim-connection-object) object in use for the Member creation.
       - mfa_enrolled: Sets whether the Member is enrolled in MFA. If true, the Member must complete an MFA step whenever they wish to log in to their Organization. If false, the Member only needs to complete an MFA step if the Organization's MFA policy is set to `REQUIRED_FOR_ALL`.
       - mfa_phone_number: The Member's phone number. A Member may only have one phone number.
       - default_mfa_method: (no documentation yet)
       - roles: Explicit or implicit Roles assigned to this Member, along with details about the role assignment source.
        See the [RBAC guide](https://stytch.com/docs/b2b/guides/rbac/role-assignment) for more information about role assignment.
```

### Comparing `stytch-9.4.0/stytch/b2b/models/organizations_members.py` & `stytch-9.5.0/stytch/b2b/models/organizations_members.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,14 +188,21 @@
       - member_id: Globally unique UUID that identifies a specific Member.
     """  # noqa
 
     member_id: str
 
 
 class DeleteTOTPResponse(ResponseBase):
+    """Response type for `Members.delete_totp`.
+    Fields:
+      - member_id: Globally unique UUID that identifies a specific Member.
+      - member: The [Member object](https://stytch.com/docs/b2b/api/member-object)
+      - organization: The [Organization object](https://stytch.com/docs/b2b/api/organization-object).
+    """  # noqa
+
     member_id: str
     member: Member
     organization: Organization
 
 
 class GetResponse(ResponseBase):
     """Response type for `Members.dangerously_get`, `Members.get`.
```

### Comparing `stytch-9.4.0/stytch/b2b/models/organizations_members_oauth_providers.py` & `stytch-9.5.0/stytch/b2b/models/organizations_members_oauth_providers.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/models/otp_sms.py` & `stytch-9.5.0/stytch/b2b/models/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/models/passwords.py` & `stytch-9.5.0/stytch/b2b/models/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/models/passwords_email.py` & `stytch-9.5.0/stytch/b2b/models/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/models/passwords_existing_password.py` & `stytch-9.5.0/stytch/b2b/models/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/models/passwords_session.py` & `stytch-9.5.0/stytch/b2b/models/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/models/rbac.py` & `stytch-9.5.0/stytch/b2b/models/rbac.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
       A `resource_id` is not allowed to start with `stytch`, which is a special prefix used for Stytch default Resources with reserved  `resource_id`s. These include:
 
       * `stytch.organization`
       * `stytch.member`
       * `stytch.sso`
       * `stytch.self`
 
-      Check out the [guide on Stytch default Resources](https://stytch.com/docs/b2b/guides/rbac/stytch-defaults) for a more detailed explanation.
+      Check out the [guide on Stytch default Resources](https://stytch.com/docs/b2b/guides/rbac/stytch-default) for a more detailed explanation.
 
 
       - description: The description of the RBAC Resource.
       - actions: A list of all possible actions for a provided Resource.
 
       Reserved `actions` that are predefined by Stytch include:
 
@@ -86,15 +86,15 @@
       A `resource_id` is not allowed to start with `stytch`, which is a special prefix used for Stytch default Resources with reserved  `resource_id`s. These include:
 
       * `stytch.organization`
       * `stytch.member`
       * `stytch.sso`
       * `stytch.self`
 
-      Check out the [guide on Stytch default Resources](https://stytch.com/docs/b2b/guides/rbac/stytch-defaults) for a more detailed explanation.
+      Check out the [guide on Stytch default Resources](https://stytch.com/docs/b2b/guides/rbac/stytch-default) for a more detailed explanation.
 
 
       - actions: A list of permitted actions the Role is authorized to take with the provided Resource. You can use `*` as a wildcard to grant a Role permission to use all possible actions related to the Resource.
     """  # noqa
 
     resource_id: str
     actions: List[str]
@@ -106,15 +106,15 @@
       - role_id: The unique identifier of the RBAC Role, provided by the developer and intended to be human-readable.
 
       Reserved `role_id`s that are predefined by Stytch include:
 
       * `stytch_member`
       * `stytch_admin`
 
-      Check out the [guide on Stytch default Roles](https://stytch.com/docs/b2b/guides/rbac/stytch-defaults) for a more detailed explanation.
+      Check out the [guide on Stytch default Roles](https://stytch.com/docs/b2b/guides/rbac/stytch-default) for a more detailed explanation.
 
 
       - description: The description of the RBAC Role.
       - permissions: A list of permissions that link a [Resource](https://stytch.com/docs/b2b/api/rbac-resource-object) to a list of actions.
     """  # noqa
 
     role_id: str
```

### Comparing `stytch-9.4.0/stytch/b2b/models/recovery_codes.py` & `stytch-9.5.0/stytch/b2b/models/recovery_codes.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/models/scim.py` & `stytch-9.5.0/stytch/b2b/models/scim.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/models/scim_connections.py` & `stytch-9.5.0/stytch/b2b/models/scim_connections.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/b2b/models/sessions.py` & `stytch-9.5.0/stytch/b2b/models/sessions.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
       A `resource_id` is not allowed to start with `stytch`, which is a special prefix used for Stytch default Resources with reserved  `resource_id`s. These include:
 
       * `stytch.organization`
       * `stytch.member`
       * `stytch.sso`
       * `stytch.self`
 
-      Check out the [guide on Stytch default Resources](https://stytch.com/docs/b2b/guides/rbac/stytch-defaults) for a more detailed explanation.
+      Check out the [guide on Stytch default Resources](https://stytch.com/docs/b2b/guides/rbac/stytch-default) for a more detailed explanation.
 
 
       - action: An action to take on a Resource.
     """  # noqa
 
     organization_id: str
     resource_id: str
```

### Comparing `stytch-9.4.0/stytch/b2b/models/sso.py` & `stytch-9.5.0/stytch/b2b/models/sso.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,23 @@
 
 class AuthenticateRequestLocale(str, enum.Enum):
     EN = "en"
     ES = "es"
     PTBR = "pt-br"
 
 
+class Connection(pydantic.BaseModel):
+    organization_id: str
+    connection_id: str
+    external_organization_id: str
+    external_connection_id: str
+    display_name: str
+    status: str
+
+
 class DeleteConnectionRequestOptions(pydantic.BaseModel):
     """
     Fields:
       - authorization: Optional authorization object.
     Pass in an active Stytch Member session token or session JWT and the request
     will be run using that member's permissions.
     """  # noqa
@@ -66,27 +75,28 @@
     client_id: str
     client_secret: str
     issuer: str
     authorization_url: str
     token_url: str
     userinfo_url: str
     jwks_url: str
+    identity_provider: str
 
 
 class SAMLConnectionImplicitRoleAssignment(pydantic.BaseModel):
     """
     Fields:
       - role_id: The unique identifier of the RBAC Role, provided by the developer and intended to be human-readable.
 
       Reserved `role_id`s that are predefined by Stytch include:
 
       * `stytch_member`
       * `stytch_admin`
 
-      Check out the [guide on Stytch default Roles](https://stytch.com/docs/b2b/guides/rbac/stytch-defaults) for a more detailed explanation.
+      Check out the [guide on Stytch default Roles](https://stytch.com/docs/b2b/guides/rbac/stytch-default) for a more detailed explanation.
 
 
     """  # noqa
 
     role_id: str
 
 
@@ -96,15 +106,15 @@
       - role_id: The unique identifier of the RBAC Role, provided by the developer and intended to be human-readable.
 
       Reserved `role_id`s that are predefined by Stytch include:
 
       * `stytch_member`
       * `stytch_admin`
 
-      Check out the [guide on Stytch default Roles](https://stytch.com/docs/b2b/guides/rbac/stytch-defaults) for a more detailed explanation.
+      Check out the [guide on Stytch default Roles](https://stytch.com/docs/b2b/guides/rbac/stytch-default) for a more detailed explanation.
 
 
       - group: The name of the SAML group that grants the specified role assignment.
     """  # noqa
 
     role_id: str
     group: str
@@ -130,14 +140,15 @@
     signing_certificates: List[X509Certificate]
     verification_certificates: List[X509Certificate]
     saml_connection_implicit_role_assignments: List[
         SAMLConnectionImplicitRoleAssignment
     ]
     saml_group_implicit_role_assignments: List[SAMLGroupImplicitRoleAssignment]
     alternative_audience_uri: str
+    identity_provider: str
     attribute_mapping: Optional[Dict[str, Any]] = None
 
 
 class AuthenticateResponse(ResponseBase):
     """Response type for `SSO.authenticate`.
     Fields:
       - member_id: Globally unique UUID that identifies a specific Member.
@@ -177,11 +188,13 @@
 
 
 class GetConnectionsResponse(ResponseBase):
     """Response type for `SSO.get_connections`.
     Fields:
       - saml_connections: The list of [SAML Connections](https://stytch.com/docs/b2b/api/saml-connection-object) owned by this organization.
       - oidc_connections: The list of [OIDC Connections](https://stytch.com/docs/b2b/api/oidc-connection-object) owned by this organization.
+      - external_connections: (no documentation yet)
     """  # noqa
 
     saml_connections: List[SAMLConnection]
     oidc_connections: List[OIDCConnection]
+    external_connections: List[Connection]
```

### Comparing `stytch-9.4.0/stytch/b2b/models/sso_oidc.py` & `stytch-9.5.0/stytch/b2b/models/sso_oidc.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,38 @@
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
+import enum
 from typing import Dict, Optional
 
 import pydantic
 
 from stytch.b2b.models.sso import OIDCConnection
 from stytch.core.response_base import ResponseBase
 from stytch.shared.method_options import Authorization
 
 
+class CreateConnectionRequestIdentityProvider(str, enum.Enum):
+    GENERIC = "generic"
+    OKTA = "okta"
+    MICROSOFTENTRA = "microsoft-entra"
+    GOOGLEWORKSPACE = "google-workspace"
+
+
+class UpdateConnectionRequestIdentityProvider(str, enum.Enum):
+    GENERIC = "generic"
+    OKTA = "okta"
+    MICROSOFTENTRA = "microsoft-entra"
+    GOOGLEWORKSPACE = "google-workspace"
+
+
 class CreateConnectionRequestOptions(pydantic.BaseModel):
     """
     Fields:
       - authorization: Optional authorization object.
     Pass in an active Stytch Member session token or session JWT and the request
     will be run using that member's permissions.
     """  # noqa
```

### Comparing `stytch-9.4.0/stytch/b2b/models/sso_saml.py` & `stytch-9.5.0/stytch/b2b/models/sso_saml.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,23 +2,38 @@
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
+import enum
 from typing import Dict, Optional
 
 import pydantic
 
 from stytch.b2b.models.sso import SAMLConnection
 from stytch.core.response_base import ResponseBase
 from stytch.shared.method_options import Authorization
 
 
+class CreateConnectionRequestIdentityProvider(str, enum.Enum):
+    GENERIC = "generic"
+    OKTA = "okta"
+    MICROSOFTENTRA = "microsoft-entra"
+    GOOGLEWORKSPACE = "google-workspace"
+
+
+class UpdateConnectionRequestIdentityProvider(str, enum.Enum):
+    GENERIC = "generic"
+    OKTA = "okta"
+    MICROSOFTENTRA = "microsoft-entra"
+    GOOGLEWORKSPACE = "google-workspace"
+
+
 class CreateConnectionRequestOptions(pydantic.BaseModel):
     """
     Fields:
       - authorization: Optional authorization object.
     Pass in an active Stytch Member session token or session JWT and the request
     will be run using that member's permissions.
     """  # noqa
```

### Comparing `stytch-9.4.0/stytch/b2b/models/totps.py` & `stytch-9.5.0/stytch/b2b/models/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/api/crypto_wallets.py` & `stytch-9.5.0/stytch/consumer/api/crypto_wallets.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/api/m2m.py` & `stytch-9.5.0/stytch/consumer/api/m2m.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/api/m2m_clients.py` & `stytch-9.5.0/stytch/consumer/api/m2m_clients.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/api/m2m_clients_secrets.py` & `stytch-9.5.0/stytch/consumer/api/m2m_clients_secrets.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/api/magic_links.py` & `stytch-9.5.0/stytch/consumer/api/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/api/magic_links_email.py` & `stytch-9.5.0/stytch/consumer/api/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/api/oauth.py` & `stytch-9.5.0/stytch/consumer/api/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/api/otp.py` & `stytch-9.5.0/stytch/consumer/api/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/api/otp_email.py` & `stytch-9.5.0/stytch/consumer/api/otp_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/api/otp_sms.py` & `stytch-9.5.0/stytch/consumer/api/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/api/otp_whatsapp.py` & `stytch-9.5.0/stytch/consumer/api/otp_whatsapp.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/api/passwords.py` & `stytch-9.5.0/stytch/consumer/api/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/api/passwords_email.py` & `stytch-9.5.0/stytch/consumer/api/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/api/passwords_existing_password.py` & `stytch-9.5.0/stytch/consumer/api/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/api/passwords_session.py` & `stytch-9.5.0/stytch/consumer/api/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/api/project.py` & `stytch-9.5.0/stytch/consumer/api/project.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/api/sessions.py` & `stytch-9.5.0/stytch/consumer/api/sessions.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,15 +76,17 @@
     def authenticate(
         self,
         session_token: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
     ) -> AuthenticateResponse:
-        """Authenticate a session token and retrieve associated session data. If `session_duration_minutes` is included, update the lifetime of the session to be that many minutes from now. All timestamps are formatted according to the RFC 3339 standard and are expressed in UTC, e.g. `2021-12-29T12:33:09Z`. This endpoint requires exactly one `session_jwt` or `session_token` as part of the request. If both are included you will receive a `too_many_session_arguments` error.
+        """Authenticate a session token or session JWT and retrieve associated session data. If `session_duration_minutes` is included, update the lifetime of the session to be that many minutes from now. All timestamps are formatted according to the RFC 3339 standard and are expressed in UTC, e.g. `2021-12-29T12:33:09Z`. This endpoint requires exactly one `session_jwt` or `session_token` as part of the request. If both are included, you will receive a `too_many_session_arguments` error.
+
+        You may provide a JWT that needs to be refreshed and is expired according to its `exp` claim. A new JWT will be returned if both the signature and the underlying Session are still valid. See our [How to use Stytch Session JWTs](https://stytch.com/docs/guides/sessions/using-jwts) guide for more information.
 
         Fields:
           - session_token: The session token to authenticate.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now; minimum of 5 and a maximum of 527040 minutes (366 days). Note that a successful authentication will continue to extend the session this many minutes.
           - session_jwt: The JWT to authenticate. You may provide a JWT that has expired according to its `exp` claim and needs to be refreshed. If the signature is valid and the underlying session is still active then Stytch will return a new JWT.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To delete a key, supply a null value.
 
@@ -108,15 +110,17 @@
     async def authenticate_async(
         self,
         session_token: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
     ) -> AuthenticateResponse:
-        """Authenticate a session token and retrieve associated session data. If `session_duration_minutes` is included, update the lifetime of the session to be that many minutes from now. All timestamps are formatted according to the RFC 3339 standard and are expressed in UTC, e.g. `2021-12-29T12:33:09Z`. This endpoint requires exactly one `session_jwt` or `session_token` as part of the request. If both are included you will receive a `too_many_session_arguments` error.
+        """Authenticate a session token or session JWT and retrieve associated session data. If `session_duration_minutes` is included, update the lifetime of the session to be that many minutes from now. All timestamps are formatted according to the RFC 3339 standard and are expressed in UTC, e.g. `2021-12-29T12:33:09Z`. This endpoint requires exactly one `session_jwt` or `session_token` as part of the request. If both are included, you will receive a `too_many_session_arguments` error.
+
+        You may provide a JWT that needs to be refreshed and is expired according to its `exp` claim. A new JWT will be returned if both the signature and the underlying Session are still valid. See our [How to use Stytch Session JWTs](https://stytch.com/docs/guides/sessions/using-jwts) guide for more information.
 
         Fields:
           - session_token: The session token to authenticate.
           - session_duration_minutes: Set the session lifetime to be this many minutes from now; minimum of 5 and a maximum of 527040 minutes (366 days). Note that a successful authentication will continue to extend the session this many minutes.
           - session_jwt: The JWT to authenticate. You may provide a JWT that has expired according to its `exp` claim and needs to be refreshed. If the signature is valid and the underlying session is still active then Stytch will return a new JWT.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To delete a key, supply a null value.
 
@@ -199,14 +203,16 @@
 
         JWTs have a set lifetime of 5 minutes, so there will be a 5 minute period where some JWTs will be signed by the old JWKS, and some JWTs will be signed by the new JWKS. The correct JWKS to use for validation is determined by matching the `kid` value of the JWT and JWKS.
 
         If you're using one of our [backend SDKs](https://stytch.com/docs/sdks), the JWKS roll will be handled for you.
 
         If you're using your own JWT validation library, many have built-in support for JWKS rotation, and you'll just need to supply this API endpoint. If not, your application should decide which JWKS to use for validation by inspecting the `kid` value.
 
+        See our [How to use Stytch Session JWTs](https://stytch.com/docs/guides/sessions/using-jwts) guide for more information.
+
         Fields:
           - project_id: The `project_id` to get the JWKS for.
         """  # noqa
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "project_id": project_id,
         }
@@ -225,14 +231,16 @@
 
         JWTs have a set lifetime of 5 minutes, so there will be a 5 minute period where some JWTs will be signed by the old JWKS, and some JWTs will be signed by the new JWKS. The correct JWKS to use for validation is determined by matching the `kid` value of the JWT and JWKS.
 
         If you're using one of our [backend SDKs](https://stytch.com/docs/sdks), the JWKS roll will be handled for you.
 
         If you're using your own JWT validation library, many have built-in support for JWKS rotation, and you'll just need to supply this API endpoint. If not, your application should decide which JWKS to use for validation by inspecting the `kid` value.
 
+        See our [How to use Stytch Session JWTs](https://stytch.com/docs/guides/sessions/using-jwts) guide for more information.
+
         Fields:
           - project_id: The `project_id` to get the JWKS for.
         """  # noqa
         headers: Dict[str, str] = {}
         data: Dict[str, Any] = {
             "project_id": project_id,
         }
```

### Comparing `stytch-9.4.0/stytch/consumer/api/totps.py` & `stytch-9.5.0/stytch/consumer/api/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/api/users.py` & `stytch-9.5.0/stytch/consumer/api/users.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/api/webauthn.py` & `stytch-9.5.0/stytch/consumer/api/webauthn.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/client.py` & `stytch-9.5.0/stytch/consumer/client.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/models/crypto_wallets.py` & `stytch-9.5.0/stytch/consumer/models/crypto_wallets.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/models/m2m.py` & `stytch-9.5.0/stytch/consumer/models/m2m.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/models/m2m_clients.py` & `stytch-9.5.0/stytch/consumer/models/m2m_clients.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/models/m2m_clients_secrets.py` & `stytch-9.5.0/stytch/consumer/models/m2m_clients_secrets.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/models/magic_links.py` & `stytch-9.5.0/stytch/consumer/models/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/models/magic_links_email.py` & `stytch-9.5.0/stytch/consumer/models/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/models/oauth.py` & `stytch-9.5.0/stytch/consumer/models/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/models/otp.py` & `stytch-9.5.0/stytch/consumer/models/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/models/otp_email.py` & `stytch-9.5.0/stytch/consumer/models/otp_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/models/otp_sms.py` & `stytch-9.5.0/stytch/consumer/models/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/models/otp_whatsapp.py` & `stytch-9.5.0/stytch/consumer/models/otp_whatsapp.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/models/passwords.py` & `stytch-9.5.0/stytch/consumer/models/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/models/passwords_email.py` & `stytch-9.5.0/stytch/consumer/models/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/models/passwords_existing_password.py` & `stytch-9.5.0/stytch/consumer/models/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/models/passwords_session.py` & `stytch-9.5.0/stytch/consumer/models/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/models/project.py` & `stytch-9.5.0/stytch/consumer/models/project.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/models/sessions.py` & `stytch-9.5.0/stytch/consumer/models/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/models/totps.py` & `stytch-9.5.0/stytch/consumer/models/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/models/users.py` & `stytch-9.5.0/stytch/consumer/models/users.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/consumer/models/webauthn.py` & `stytch-9.5.0/stytch/consumer/models/webauthn.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/core/api_base.py` & `stytch-9.5.0/stytch/core/api_base.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/core/client_base.py` & `stytch-9.5.0/stytch/core/client_base.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/core/http/client.py` & `stytch-9.5.0/stytch/core/http/client.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/core/response_base.py` & `stytch-9.5.0/stytch/core/response_base.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/shared/jwt_helpers.py` & `stytch-9.5.0/stytch/shared/jwt_helpers.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/shared/lazy_cache.py` & `stytch-9.5.0/stytch/shared/lazy_cache.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/shared/method_options.py` & `stytch-9.5.0/stytch/shared/method_options.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/shared/policy_cache.py` & `stytch-9.5.0/stytch/shared/policy_cache.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch/shared/rbac_local.py` & `stytch-9.5.0/stytch/shared/rbac_local.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/stytch.egg-info/PKG-INFO` & `stytch-9.5.0/stytch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 9.4.0
+Version: 9.5.0
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stytch-9.4.0/stytch.egg-info/SOURCES.txt` & `stytch-9.5.0/stytch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/test/test_integration.py` & `stytch-9.5.0/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `stytch-9.4.0/test/test_integration_async.py` & `stytch-9.5.0/test/test_integration_async.py`

 * *Files identical despite different names*

