# Comparing `tmp/django-jbank-4.4.7.tar.gz` & `tmp/django-jbank-4.4.8.tar.gz`

## Comparing `django-jbank-4.4.7.tar` & `django-jbank-4.4.8.tar`

### file list

```diff
@@ -1,251 +1,251 @@
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:15.000000 django-jbank-4.4.7/
--rw-r--r--   0 jani      (1000) jani      (1000)     1603 2024-03-12 19:45:07.000000 django-jbank-4.4.7/PKG-INFO
--rw-rw-r--   0 jani      (1000) jani      (1000)      234 2024-03-12 19:44:55.000000 django-jbank-4.4.7/requirements-dev.txt
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:07.000000 django-jbank-4.4.7/jbank/
--rw-rw-r--   0 jani      (1000) jani      (1000)    12789 2023-12-06 06:06:43.000000 django-jbank-4.4.7/jbank/tito.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1247 2023-05-16 17:40:29.000000 django-jbank-4.4.7/jbank/ecb.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1197 2023-10-24 22:41:23.000000 django-jbank-4.4.7/jbank/x509_helpers.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:07.000000 django-jbank-4.4.7/jbank/management/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:07.000000 django-jbank-4.4.7/jbank/management/commands/
--rw-rw-r--   0 jani      (1000) jani      (1000)     3193 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/make_x509.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1541 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/wsedi_export.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      859 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/xmlsec1_examples.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3091 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/parse_xp.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2464 2023-12-06 06:06:43.000000 django-jbank-4.4.7/jbank/management/commands/wsedi_exec.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      505 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/test_to.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2450 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/reparse_to.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     7308 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/parse_xt.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1287 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/test_app_req.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1154 2023-12-06 06:06:43.000000 django-jbank-4.4.7/jbank/management/commands/validate_xml.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     6058 2023-12-06 06:06:43.000000 django-jbank-4.4.7/jbank/management/commands/wsedi_download.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2286 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/reparse_svm.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3610 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/parse_svm.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1002 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/parse_saldo.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2557 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/wspki_exec.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2935 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/parse_xm.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2085 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/test_pain001.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      498 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/test_svm.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      397 2024-01-05 01:16:03.000000 django-jbank-4.4.7/jbank/management/commands/ibaninfo.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2146 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/wsedi_import.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3373 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/parse_to.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2237 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/make_parse_format.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      676 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/test_xp.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     6074 2023-12-06 06:06:43.000000 django-jbank-4.4.7/jbank/management/commands/make_pain001.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1102 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/parse_aeb43.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1195 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/test_payment.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2690 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/parse_ecb_rates.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      498 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/parse_x509.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     4983 2023-05-16 17:40:29.000000 django-jbank-4.4.7/jbank/management/commands/wsedi_upload.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1014 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/parse_ra.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1190 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/commands/parse_euribor_rates.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/management/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    19040 2023-05-16 17:40:29.000000 django-jbank-4.4.7/jbank/wspki.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1582 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/pain002.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     6641 2023-12-06 06:06:43.000000 django-jbank-4.4.7/jbank/aeb43.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    47752 2024-03-12 19:44:55.000000 django-jbank-4.4.7/jbank/models.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     5301 2023-05-16 17:40:29.000000 django-jbank-4.4.7/jbank/csr_helpers.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:06.000000 django-jbank-4.4.7/jbank/locale/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:06.000000 django-jbank-4.4.7/jbank/locale/fi/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:07.000000 django-jbank-4.4.7/jbank/locale/fi/LC_MESSAGES/
--rw-rw-r--   0 jani      (1000) jani      (1000)    16387 2023-09-13 01:10:20.000000 django-jbank-4.4.7/jbank/locale/fi/LC_MESSAGES/django.mo
--rw-rw-r--   0 jani      (1000) jani      (1000)    27763 2023-09-13 01:10:51.000000 django-jbank-4.4.7/jbank/locale/fi/LC_MESSAGES/django.po
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:06.000000 django-jbank-4.4.7/jbank/locale/sv/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:07.000000 django-jbank-4.4.7/jbank/locale/sv/LC_MESSAGES/
--rw-rw-r--   0 jani      (1000) jani      (1000)    18326 2023-09-13 01:10:51.000000 django-jbank-4.4.7/jbank/locale/sv/LC_MESSAGES/django.mo
--rw-rw-r--   0 jani      (1000) jani      (1000)    27097 2023-09-13 01:10:51.000000 django-jbank-4.4.7/jbank/locale/sv/LC_MESSAGES/django.po
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:06.000000 django-jbank-4.4.7/jbank/locale/en/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:07.000000 django-jbank-4.4.7/jbank/locale/en/LC_MESSAGES/
--rw-rw-r--   0 jani      (1000) jani      (1000)     1102 2023-09-13 01:10:20.000000 django-jbank-4.4.7/jbank/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 jani      (1000) jani      (1000)    22562 2023-09-13 01:10:51.000000 django-jbank-4.4.7/jbank/locale/en/LC_MESSAGES/django.po
--rw-rw-r--   0 jani      (1000) jani      (1000)    51664 2024-03-12 19:44:55.000000 django-jbank-4.4.7/jbank/admin.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:07.000000 django-jbank-4.4.7/jbank/migrations/
--rw-rw-r--   0 jani      (1000) jani      (1000)      655 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0026_auto_20181205_0034.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1451 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0026_referencepaymentbatch_identifier_and_more.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1175 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0013_euriborrate.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      967 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0018_alter_referencepaymentbatch_currency_identifier_and_more.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      692 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0062_auto_20200415_2300.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      551 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0005_statementfile_created.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      456 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0022_auto_20180411_1814.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      426 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0056_wsediconnection_debug_commands.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      482 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0017_alter_statementrecord_name.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      478 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0030_auto_20190727_1633.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      449 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0040_wsediconnection_signing_key_file.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      886 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0007_auto_20171102_2351.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      487 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0045_wsediconnection_receiver_identifier.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      934 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0019_alter_payout_state.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1672 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0008_auto_20171103_0007.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      600 2023-08-27 00:06:38.000000 django-jbank-4.4.7/jbank/migrations/0036_remove_referencepaymentrecord_manually_settled_and_more.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      494 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0049_wsediconnection_sender_identifier.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      523 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0011_referencepaymentbatch_cached_total_amount.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      623 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0051_payout_connection.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3784 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0028_referencepaymentrecord_creditor_bank_bic_and_more.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1930 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0012_auto_20180126_0858.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1192 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0015_auto_20180208_0643.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    11060 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0029_auto_20190727_1352.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    27144 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0064_auto_20200629_0344.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      488 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0035_auto_20190815_2137.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      462 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0065_wsediconnection_bank_root_cert_file.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      406 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0047_wsedisoapcall_error.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      591 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0023_remove_accountbalance_connection_accountbalance_bic.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      405 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0023_auto_20180419_1316.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      760 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0004_statementfile.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      520 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0029_alter_referencepaymentrecord_remittance_info.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      706 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0017_payoutparty_payouts_account.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      703 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0027_auto_20190304_1913.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3213 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0002_auto_20171031_0356.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      757 2023-08-15 22:51:45.000000 django-jbank-4.4.7/jbank/migrations/0035_wsediconnection_agreement_identifier_and_more.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      648 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0013_auto_20180126_0909.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1520 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0020_accountbalance.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      482 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0053_wsediconnection_target_identifier.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      754 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0016_alter_payoutstatus_timestamp.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      468 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0071_wsediconnection_ca_cert_file.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1019 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0024_auto_20180425_1704.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1096 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0007_auto_20210507_2122.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2493 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0011_auto_20180126_0851.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      412 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0003_auto_20200902_1354.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      441 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0057_wsediconnection_enabled.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      450 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0014_payoutstatus_timestamp.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      498 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0005_auto_20201203_2308.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      670 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0061_auto_20200325_2204.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      525 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0009_auto_20171107_1847.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      463 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0032_wsediconnection_use_sha256.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      534 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0025_auto_20230325_1014.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      703 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0041_auto_20191127_0559.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      452 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0044_auto_20191128_2231.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      748 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0031_wsediconnection_old_encryption_key_file_and_more.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      643 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0025_auto_20181101_1430.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      713 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0012_alter_referencepaymentrecord_delivery_method.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      434 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0067_wsediconnection_pki_endpoint.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      576 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0039_auto_20191127_0156.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     4229 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0014_payout_payoutstatus.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      479 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0032_auto_20190727_1655.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      707 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0006_auto_20210318_2130.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      711 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0022_accountbalance_connection.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      443 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0020_payout_due_date.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      480 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0066_wsediconnection_pin.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      428 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0004_refund_attachment.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      461 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0070_wsediconnection_bank_signing_cert_file.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1006 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0024_referencepaymentbatchfile_additional_info_and_more.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      424 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0046_auto_20191128_2242.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      577 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0048_wsediconnection_soap_endpoint.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      753 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0027_referencepaymentrecord_value_date_and_more.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      347 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0050_remove_wsedisoapcall_payout.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      464 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0028_auto_20190327_1830.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      523 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0010_statementrecorddetail_creditor_account_scheme.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      514 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0030_alter_referencepaymentrecord_remittance_info.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1621 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0031_auto_20190727_1639.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      748 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0037_auto_20191127_0132.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      467 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0042_wsediconnection_bank_encryption_cert_file.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      491 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0058_auto_20200316_1949.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2335 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0043_wsedisoapcall.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      698 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0060_auto_20200325_1906.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      638 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0003_statement_account.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    57170 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0001_squashed_0071_wsediconnection_ca_cert_file.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     2031 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0002_auto_20200817_2217.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      418 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0059_auto_20200324_0234.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      665 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0052_auto_20191130_1927.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      443 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0038_auto_20191127_0145.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      439 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0015_ps_timestamp_fill.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      500 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0009_referencepaymentbatchfile_cached_total_amount.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      486 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0010_auto_20171226_1013.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      665 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0006_auto_20171102_2341.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    15229 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0001_initial.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      462 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0033_alter_statement_begin_date.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      467 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0034_wsediconnection_use_wsse_timestamp.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1735 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0034_auto_20190815_2059.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      455 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0063_auto_20200608_1827.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1074 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0008_auto_20210512_2208.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      488 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0033_auto_20190801_2121.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      754 2023-08-27 00:06:38.000000 django-jbank-4.4.7/jbank/migrations/0037_alter_referencepaymentrecord_marked_reconciled_and_more.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      687 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0021_auto_20180209_0935.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3164 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0016_auto_20180208_0724.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      460 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0054_wsediconnection_environment.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      515 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0069_auto_20200717_2333.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1333 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0019_auto_20180209_0437.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1196 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0036_wsediconnection.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      580 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0055_auto_20191130_2011.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      667 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0018_auto_20180208_1130.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      422 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0068_auto_20200717_2327.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      433 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/migrations/0021_alter_accountbalance_balance.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     3769 2024-01-05 01:15:00.000000 django-jbank-4.4.7/jbank/helpers.py
--rw-rw-r--   0 jani      (1000) jani      (1000)       27 2020-05-26 21:27:46.000000 django-jbank-4.4.7/jbank/py.typed
--rw-rw-r--   0 jani      (1000) jani      (1000)    11635 2023-12-06 06:06:43.000000 django-jbank-4.4.7/jbank/svm.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     7881 2023-12-05 18:57:30.000000 django-jbank-4.4.7/jbank/wsedi.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/views.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    27119 2023-12-06 06:06:43.000000 django-jbank-4.4.7/jbank/tests.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    23211 2024-01-05 01:15:00.000000 django-jbank-4.4.7/jbank/sepa.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      235 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/apps.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     4704 2023-08-27 00:06:38.000000 django-jbank-4.4.7/jbank/services.py
--rw-rw-r--   0 jani      (1000) jani      (1000)    23900 2023-05-31 01:39:30.000000 django-jbank-4.4.7/jbank/camt.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:07.000000 django-jbank-4.4.7/jbank/xmlsec1-examples/
--rw-rw-r--   0 jani      (1000) jani      (1000)     9710 2020-05-21 16:43:43.000000 django-jbank-4.4.7/jbank/xmlsec1-examples/sign3.c
--rw-rw-r--   0 jani      (1000) jani      (1000)     7088 2020-05-21 16:43:43.000000 django-jbank-4.4.7/jbank/xmlsec1-examples/verify3.c
--rw-rw-r--   0 jani      (1000) jani      (1000)    10308 2020-05-21 16:43:43.000000 django-jbank-4.4.7/jbank/xmlsec1-examples/encrypt3.c
--rw-rw-r--   0 jani      (1000) jani      (1000)     7127 2020-05-21 16:43:43.000000 django-jbank-4.4.7/jbank/xmlsec1-examples/decrypt3.c
--rw-rw-r--   0 jani      (1000) jani      (1000)     9718 2023-04-05 11:04:17.000000 django-jbank-4.4.7/jbank/xmlsec1-examples/sign3-sha256.c
--rw-rw-r--   0 jani      (1000) jani      (1000)     1058 2023-04-05 11:04:17.000000 django-jbank-4.4.7/jbank/xmlsec1-examples/Makefile
--rw-rw-r--   0 jani      (1000) jani      (1000)    10367 2023-12-06 06:06:43.000000 django-jbank-4.4.7/jbank/parsers.py
--rw-rw-r--   0 jani      (1000) jani      (1000)     1562 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/euribor.py
--rw-rw-r--   0 jani      (1000) jani      (1000)       46 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      828 2023-05-16 17:40:29.000000 django-jbank-4.4.7/jbank/files.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:07.000000 django-jbank-4.4.7/jbank/templates/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:07.000000 django-jbank-4.4.7/jbank/templates/jbank/
--rw-rw-r--   0 jani      (1000) jani      (1000)      562 2021-07-06 21:13:32.000000 django-jbank-4.4.7/jbank/templates/jbank/pki_get_certificate_soap_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     2041 2021-12-23 17:01:04.000000 django-jbank-4.4.7/jbank/templates/jbank/pki_certificate_status_request_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     2079 2022-01-09 22:11:13.000000 django-jbank-4.4.7/jbank/templates/jbank/pki_renew_certificate_request_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)      962 2021-12-23 17:01:04.000000 django-jbank-4.4.7/jbank/templates/jbank/pki_create_certificate_request_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     2087 2023-04-05 11:04:17.000000 django-jbank-4.4.7/jbank/templates/jbank/pki_renew_certificate_request_template-sha256.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)      876 2020-05-21 16:43:43.000000 django-jbank-4.4.7/jbank/templates/jbank/soap_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)      911 2021-12-23 17:01:04.000000 django-jbank-4.4.7/jbank/templates/jbank/pki_soap_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     2223 2023-04-05 11:04:17.000000 django-jbank-4.4.7/jbank/templates/jbank/application_request_template-sha256.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)      568 2021-12-23 17:01:04.000000 django-jbank-4.4.7/jbank/templates/jbank/pki_get_certificate_request_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     1686 2023-04-05 11:04:17.000000 django-jbank-4.4.7/jbank/templates/jbank/pki_get_certificate_renew_request_template-sha256.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     1678 2021-12-23 17:01:04.000000 django-jbank-4.4.7/jbank/templates/jbank/pki_get_certificate_renew_request_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)      758 2020-05-21 16:43:43.000000 django-jbank-4.4.7/jbank/templates/jbank/encryption_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     5352 2023-04-05 11:04:17.000000 django-jbank-4.4.7/jbank/templates/jbank/enveloping-sha256-rsa-sha256.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     2215 2020-05-21 16:43:43.000000 django-jbank-4.4.7/jbank/templates/jbank/application_request_template.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/templates/jbank/__init__.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:07.000000 django-jbank-4.4.7/jbank/templates/admin/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:07.000000 django-jbank-4.4.7/jbank/templates/admin/jbank/
--rw-rw-r--   0 jani      (1000) jani      (1000)      691 2023-08-27 04:25:40.000000 django-jbank-4.4.7/jbank/templates/admin/jbank/mark_as_marked_reconciled.html
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:07.000000 django-jbank-4.4.7/jbank/templates/admin/jbank/statement/
--rw-rw-r--   0 jani      (1000) jani      (1000)      782 2020-05-21 16:43:43.000000 django-jbank-4.4.7/jbank/templates/admin/jbank/statement/change_form.html
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/templates/admin/jbank/statement/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/templates/admin/jbank/__init__.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:07.000000 django-jbank-4.4.7/jbank/templates/admin/jbank/referencepaymentbatch/
--rw-rw-r--   0 jani      (1000) jani      (1000)      793 2020-05-21 16:43:43.000000 django-jbank-4.4.7/jbank/templates/admin/jbank/referencepaymentbatch/change_form.html
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/templates/admin/jbank/referencepaymentbatch/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/templates/admin/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.4.7/jbank/templates/__init__.py
--rw-rw-r--   0 jani      (1000) jani      (1000)      931 2024-03-12 19:43:36.000000 django-jbank-4.4.7/pyproject.toml
--rw-rw-r--   0 jani      (1000) jani      (1000)       38 2024-03-12 19:45:07.000000 django-jbank-4.4.7/setup.cfg
--rw-rw-r--   0 jani      (1000) jani      (1000)     1064 2023-05-16 17:40:29.000000 django-jbank-4.4.7/README.md
--rw-rw-r--   0 jani      (1000) jani      (1000)     1082 2020-05-26 21:27:46.000000 django-jbank-4.4.7/LICENSE.txt
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:07.000000 django-jbank-4.4.7/django_jbank.egg-info/
--rw-rw-r--   0 jani      (1000) jani      (1000)   707364 2024-03-12 19:45:06.000000 django-jbank-4.4.7/django_jbank.egg-info/SOURCES.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)        6 2024-03-12 19:44:57.000000 django-jbank-4.4.7/django_jbank.egg-info/top_level.txt
--rw-r--r--   0 jani      (1000) jani      (1000)     1603 2024-03-12 19:44:57.000000 django-jbank-4.4.7/django_jbank.egg-info/PKG-INFO
--rw-rw-r--   0 jani      (1000) jani      (1000)      158 2024-03-12 19:44:57.000000 django-jbank-4.4.7/django_jbank.egg-info/requires.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)        1 2020-05-26 21:28:24.000000 django-jbank-4.4.7/django_jbank.egg-info/not-zip-safe
--rw-rw-r--   0 jani      (1000) jani      (1000)        1 2024-03-12 19:44:57.000000 django-jbank-4.4.7/django_jbank.egg-info/dependency_links.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)      158 2024-02-27 17:18:22.000000 django-jbank-4.4.7/requirements.txt
--rw-rw-r--   0 jani      (1000) jani      (1000)      247 2020-05-27 18:47:15.000000 django-jbank-4.4.7/mypy.ini
--rw-rw-r--   0 jani      (1000) jani      (1000)      867 2024-03-12 19:44:55.000000 django-jbank-4.4.7/setup.py
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:06.000000 django-jbank-4.4.7/data/
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:06.000000 django-jbank-4.4.7/data/x509/
--rw-rw-r--   0 jani      (1000) jani      (1000)     1486 2020-05-21 16:43:43.000000 django-jbank-4.4.7/data/x509/appreq.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     1561 2022-07-21 16:32:20.000000 django-jbank-4.4.7/data/x509/x509data.xml
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:06.000000 django-jbank-4.4.7/data/finvoice/
--rw-rw-r--   0 jani      (1000) jani      (1000)     5362 2020-05-21 16:43:43.000000 django-jbank-4.4.7/data/finvoice/xsd-test.xml
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:06.000000 django-jbank-4.4.7/data/pki/
--rw-rw-r--   0 jani      (1000) jani      (1000)    10099 2020-07-18 04:38:59.000000 django-jbank-4.4.7/data/pki/GetBankCertificate-res.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)      638 2020-07-20 22:19:28.000000 django-jbank-4.4.7/data/pki/CreateCertificate-res.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)     1547 2021-07-06 23:33:19.000000 django-jbank-4.4.7/data/x509-data.xml
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:06.000000 django-jbank-4.4.7/data/xm/
--rw-rw-r--   0 jani      (1000) jani      (1000)     6994 2023-03-27 06:59:59.000000 django-jbank-4.4.7/data/xm/camt_054_credit_notoification_example_finland.xml
-drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-03-12 19:45:06.000000 django-jbank-4.4.7/data/pain001/
--rw-rw-r--   0 jani      (1000) jani      (1000)     4044 2020-05-21 16:43:43.000000 django-jbank-4.4.7/data/pain001/pain.001.001.03.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)    91224 2020-05-21 16:43:43.000000 django-jbank-4.4.7/data/ecb-rates-2019-08-15.xml
--rw-rw-r--   0 jani      (1000) jani      (1000)      287 2023-08-11 14:50:29.000000 django-jbank-4.4.7/MANIFEST.in
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:30.000000 django-jbank-4.4.8/
+-rw-r--r--   0 jani      (1000) jani      (1000)     1603 2024-05-20 05:16:18.000000 django-jbank-4.4.8/PKG-INFO
+-rw-rw-r--   0 jani      (1000) jani      (1000)      234 2024-03-12 19:44:55.000000 django-jbank-4.4.8/requirements-dev.txt
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:18.000000 django-jbank-4.4.8/jbank/
+-rw-rw-r--   0 jani      (1000) jani      (1000)    12789 2023-12-06 06:06:43.000000 django-jbank-4.4.8/jbank/tito.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1247 2023-05-16 17:40:29.000000 django-jbank-4.4.8/jbank/ecb.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1197 2023-10-24 22:41:23.000000 django-jbank-4.4.8/jbank/x509_helpers.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:18.000000 django-jbank-4.4.8/jbank/management/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:18.000000 django-jbank-4.4.8/jbank/management/commands/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3193 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/make_x509.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1541 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/wsedi_export.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      859 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/xmlsec1_examples.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3091 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/parse_xp.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2464 2023-12-06 06:06:43.000000 django-jbank-4.4.8/jbank/management/commands/wsedi_exec.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      505 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/test_to.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2450 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/reparse_to.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     7308 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/parse_xt.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1287 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/test_app_req.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1154 2023-12-06 06:06:43.000000 django-jbank-4.4.8/jbank/management/commands/validate_xml.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     6058 2023-12-06 06:06:43.000000 django-jbank-4.4.8/jbank/management/commands/wsedi_download.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2286 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/reparse_svm.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3610 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/parse_svm.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1002 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/parse_saldo.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2557 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/wspki_exec.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2935 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/parse_xm.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2085 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/test_pain001.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      498 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/test_svm.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      397 2024-01-05 01:16:03.000000 django-jbank-4.4.8/jbank/management/commands/ibaninfo.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2146 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/wsedi_import.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3373 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/parse_to.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2237 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/make_parse_format.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      676 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/test_xp.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     6074 2023-12-06 06:06:43.000000 django-jbank-4.4.8/jbank/management/commands/make_pain001.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1102 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/parse_aeb43.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1195 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/test_payment.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2690 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/parse_ecb_rates.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      498 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/parse_x509.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4983 2023-05-16 17:40:29.000000 django-jbank-4.4.8/jbank/management/commands/wsedi_upload.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1014 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/parse_ra.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1190 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/commands/parse_euribor_rates.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/management/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    19040 2023-05-16 17:40:29.000000 django-jbank-4.4.8/jbank/wspki.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1582 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/pain002.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     6641 2023-12-06 06:06:43.000000 django-jbank-4.4.8/jbank/aeb43.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    47752 2024-03-12 19:44:55.000000 django-jbank-4.4.8/jbank/models.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     5301 2023-05-16 17:40:29.000000 django-jbank-4.4.8/jbank/csr_helpers.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:17.000000 django-jbank-4.4.8/jbank/locale/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:17.000000 django-jbank-4.4.8/jbank/locale/fi/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:18.000000 django-jbank-4.4.8/jbank/locale/fi/LC_MESSAGES/
+-rw-rw-r--   0 jani      (1000) jani      (1000)    16387 2023-09-13 01:10:20.000000 django-jbank-4.4.8/jbank/locale/fi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 jani      (1000) jani      (1000)    27763 2023-09-13 01:10:51.000000 django-jbank-4.4.8/jbank/locale/fi/LC_MESSAGES/django.po
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:17.000000 django-jbank-4.4.8/jbank/locale/sv/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:18.000000 django-jbank-4.4.8/jbank/locale/sv/LC_MESSAGES/
+-rw-rw-r--   0 jani      (1000) jani      (1000)    18326 2023-09-13 01:10:51.000000 django-jbank-4.4.8/jbank/locale/sv/LC_MESSAGES/django.mo
+-rw-rw-r--   0 jani      (1000) jani      (1000)    27097 2023-09-13 01:10:51.000000 django-jbank-4.4.8/jbank/locale/sv/LC_MESSAGES/django.po
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:17.000000 django-jbank-4.4.8/jbank/locale/en/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:18.000000 django-jbank-4.4.8/jbank/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1102 2023-09-13 01:10:20.000000 django-jbank-4.4.8/jbank/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 jani      (1000) jani      (1000)    22562 2023-09-13 01:10:51.000000 django-jbank-4.4.8/jbank/locale/en/LC_MESSAGES/django.po
+-rw-rw-r--   0 jani      (1000) jani      (1000)    51664 2024-03-12 19:44:55.000000 django-jbank-4.4.8/jbank/admin.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:18.000000 django-jbank-4.4.8/jbank/migrations/
+-rw-rw-r--   0 jani      (1000) jani      (1000)      655 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0026_auto_20181205_0034.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1451 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0026_referencepaymentbatch_identifier_and_more.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1175 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0013_euriborrate.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      967 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0018_alter_referencepaymentbatch_currency_identifier_and_more.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      692 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0062_auto_20200415_2300.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      551 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0005_statementfile_created.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      456 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0022_auto_20180411_1814.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      426 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0056_wsediconnection_debug_commands.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      482 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0017_alter_statementrecord_name.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      478 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0030_auto_20190727_1633.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      449 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0040_wsediconnection_signing_key_file.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      886 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0007_auto_20171102_2351.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      487 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0045_wsediconnection_receiver_identifier.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      934 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0019_alter_payout_state.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1672 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0008_auto_20171103_0007.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      600 2023-08-27 00:06:38.000000 django-jbank-4.4.8/jbank/migrations/0036_remove_referencepaymentrecord_manually_settled_and_more.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      494 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0049_wsediconnection_sender_identifier.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      523 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0011_referencepaymentbatch_cached_total_amount.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      623 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0051_payout_connection.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3784 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0028_referencepaymentrecord_creditor_bank_bic_and_more.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1930 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0012_auto_20180126_0858.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1192 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0015_auto_20180208_0643.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    11060 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0029_auto_20190727_1352.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    27144 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0064_auto_20200629_0344.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      488 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0035_auto_20190815_2137.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      462 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0065_wsediconnection_bank_root_cert_file.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      406 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0047_wsedisoapcall_error.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      591 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0023_remove_accountbalance_connection_accountbalance_bic.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      405 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0023_auto_20180419_1316.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      760 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0004_statementfile.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      520 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0029_alter_referencepaymentrecord_remittance_info.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      706 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0017_payoutparty_payouts_account.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      703 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0027_auto_20190304_1913.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3213 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0002_auto_20171031_0356.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      757 2023-08-15 22:51:45.000000 django-jbank-4.4.8/jbank/migrations/0035_wsediconnection_agreement_identifier_and_more.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      648 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0013_auto_20180126_0909.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1520 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0020_accountbalance.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      482 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0053_wsediconnection_target_identifier.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      754 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0016_alter_payoutstatus_timestamp.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      468 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0071_wsediconnection_ca_cert_file.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1019 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0024_auto_20180425_1704.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1096 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0007_auto_20210507_2122.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2493 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0011_auto_20180126_0851.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      412 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0003_auto_20200902_1354.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      441 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0057_wsediconnection_enabled.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      450 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0014_payoutstatus_timestamp.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      498 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0005_auto_20201203_2308.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      670 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0061_auto_20200325_2204.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      525 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0009_auto_20171107_1847.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      463 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0032_wsediconnection_use_sha256.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      534 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0025_auto_20230325_1014.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      703 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0041_auto_20191127_0559.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      452 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0044_auto_20191128_2231.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      748 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0031_wsediconnection_old_encryption_key_file_and_more.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      643 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0025_auto_20181101_1430.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      713 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0012_alter_referencepaymentrecord_delivery_method.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      434 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0067_wsediconnection_pki_endpoint.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      576 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0039_auto_20191127_0156.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4229 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0014_payout_payoutstatus.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      479 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0032_auto_20190727_1655.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      707 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0006_auto_20210318_2130.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      711 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0022_accountbalance_connection.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      443 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0020_payout_due_date.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      480 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0066_wsediconnection_pin.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      428 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0004_refund_attachment.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      461 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0070_wsediconnection_bank_signing_cert_file.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1006 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0024_referencepaymentbatchfile_additional_info_and_more.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      424 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0046_auto_20191128_2242.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      577 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0048_wsediconnection_soap_endpoint.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      753 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0027_referencepaymentrecord_value_date_and_more.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      347 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0050_remove_wsedisoapcall_payout.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      464 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0028_auto_20190327_1830.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      523 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0010_statementrecorddetail_creditor_account_scheme.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      514 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0030_alter_referencepaymentrecord_remittance_info.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1621 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0031_auto_20190727_1639.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      748 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0037_auto_20191127_0132.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      467 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0042_wsediconnection_bank_encryption_cert_file.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      491 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0058_auto_20200316_1949.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2335 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0043_wsedisoapcall.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      698 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0060_auto_20200325_1906.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      638 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0003_statement_account.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    57170 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0001_squashed_0071_wsediconnection_ca_cert_file.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2031 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0002_auto_20200817_2217.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      418 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0059_auto_20200324_0234.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      665 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0052_auto_20191130_1927.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      443 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0038_auto_20191127_0145.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      439 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0015_ps_timestamp_fill.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      500 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0009_referencepaymentbatchfile_cached_total_amount.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      486 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0010_auto_20171226_1013.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      665 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0006_auto_20171102_2341.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    15229 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0001_initial.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      462 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0033_alter_statement_begin_date.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      467 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0034_wsediconnection_use_wsse_timestamp.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1735 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0034_auto_20190815_2059.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      455 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0063_auto_20200608_1827.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1074 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0008_auto_20210512_2208.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      488 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0033_auto_20190801_2121.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      754 2023-08-27 00:06:38.000000 django-jbank-4.4.8/jbank/migrations/0037_alter_referencepaymentrecord_marked_reconciled_and_more.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      687 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0021_auto_20180209_0935.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3164 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0016_auto_20180208_0724.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      460 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0054_wsediconnection_environment.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      515 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0069_auto_20200717_2333.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1333 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0019_auto_20180209_0437.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1196 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0036_wsediconnection.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      580 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0055_auto_20191130_2011.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      667 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0018_auto_20180208_1130.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      422 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0068_auto_20200717_2327.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      433 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/migrations/0021_alter_accountbalance_balance.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     3769 2024-01-05 01:15:00.000000 django-jbank-4.4.8/jbank/helpers.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)       27 2020-05-26 21:27:46.000000 django-jbank-4.4.8/jbank/py.typed
+-rw-rw-r--   0 jani      (1000) jani      (1000)    11635 2023-12-06 06:06:43.000000 django-jbank-4.4.8/jbank/svm.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     7881 2023-12-05 18:57:30.000000 django-jbank-4.4.8/jbank/wsedi.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/views.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    27119 2023-12-06 06:06:43.000000 django-jbank-4.4.8/jbank/tests.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    23211 2024-01-05 01:15:00.000000 django-jbank-4.4.8/jbank/sepa.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      235 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/apps.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4704 2023-08-27 00:06:38.000000 django-jbank-4.4.8/jbank/services.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)    23910 2024-05-20 05:15:59.000000 django-jbank-4.4.8/jbank/camt.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:18.000000 django-jbank-4.4.8/jbank/xmlsec1-examples/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     9710 2020-05-21 16:43:43.000000 django-jbank-4.4.8/jbank/xmlsec1-examples/sign3.c
+-rw-rw-r--   0 jani      (1000) jani      (1000)     7088 2020-05-21 16:43:43.000000 django-jbank-4.4.8/jbank/xmlsec1-examples/verify3.c
+-rw-rw-r--   0 jani      (1000) jani      (1000)    10308 2020-05-21 16:43:43.000000 django-jbank-4.4.8/jbank/xmlsec1-examples/encrypt3.c
+-rw-rw-r--   0 jani      (1000) jani      (1000)     7127 2020-05-21 16:43:43.000000 django-jbank-4.4.8/jbank/xmlsec1-examples/decrypt3.c
+-rw-rw-r--   0 jani      (1000) jani      (1000)     9718 2023-04-05 11:04:17.000000 django-jbank-4.4.8/jbank/xmlsec1-examples/sign3-sha256.c
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1058 2023-04-05 11:04:17.000000 django-jbank-4.4.8/jbank/xmlsec1-examples/Makefile
+-rw-rw-r--   0 jani      (1000) jani      (1000)    10367 2023-12-06 06:06:43.000000 django-jbank-4.4.8/jbank/parsers.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1562 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/euribor.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)       46 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      828 2023-05-16 17:40:29.000000 django-jbank-4.4.8/jbank/files.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:18.000000 django-jbank-4.4.8/jbank/templates/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:18.000000 django-jbank-4.4.8/jbank/templates/jbank/
+-rw-rw-r--   0 jani      (1000) jani      (1000)      562 2021-07-06 21:13:32.000000 django-jbank-4.4.8/jbank/templates/jbank/pki_get_certificate_soap_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2041 2021-12-23 17:01:04.000000 django-jbank-4.4.8/jbank/templates/jbank/pki_certificate_status_request_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2079 2022-01-09 22:11:13.000000 django-jbank-4.4.8/jbank/templates/jbank/pki_renew_certificate_request_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      962 2021-12-23 17:01:04.000000 django-jbank-4.4.8/jbank/templates/jbank/pki_create_certificate_request_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2087 2023-04-05 11:04:17.000000 django-jbank-4.4.8/jbank/templates/jbank/pki_renew_certificate_request_template-sha256.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      876 2020-05-21 16:43:43.000000 django-jbank-4.4.8/jbank/templates/jbank/soap_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      911 2021-12-23 17:01:04.000000 django-jbank-4.4.8/jbank/templates/jbank/pki_soap_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2223 2023-04-05 11:04:17.000000 django-jbank-4.4.8/jbank/templates/jbank/application_request_template-sha256.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      568 2021-12-23 17:01:04.000000 django-jbank-4.4.8/jbank/templates/jbank/pki_get_certificate_request_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1686 2023-04-05 11:04:17.000000 django-jbank-4.4.8/jbank/templates/jbank/pki_get_certificate_renew_request_template-sha256.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1678 2021-12-23 17:01:04.000000 django-jbank-4.4.8/jbank/templates/jbank/pki_get_certificate_renew_request_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      758 2020-05-21 16:43:43.000000 django-jbank-4.4.8/jbank/templates/jbank/encryption_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     5352 2023-04-05 11:04:17.000000 django-jbank-4.4.8/jbank/templates/jbank/enveloping-sha256-rsa-sha256.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     2215 2020-05-21 16:43:43.000000 django-jbank-4.4.8/jbank/templates/jbank/application_request_template.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/templates/jbank/__init__.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:18.000000 django-jbank-4.4.8/jbank/templates/admin/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:18.000000 django-jbank-4.4.8/jbank/templates/admin/jbank/
+-rw-rw-r--   0 jani      (1000) jani      (1000)      691 2023-08-27 04:25:40.000000 django-jbank-4.4.8/jbank/templates/admin/jbank/mark_as_marked_reconciled.html
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:18.000000 django-jbank-4.4.8/jbank/templates/admin/jbank/statement/
+-rw-rw-r--   0 jani      (1000) jani      (1000)      782 2020-05-21 16:43:43.000000 django-jbank-4.4.8/jbank/templates/admin/jbank/statement/change_form.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/templates/admin/jbank/statement/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/templates/admin/jbank/__init__.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:18.000000 django-jbank-4.4.8/jbank/templates/admin/jbank/referencepaymentbatch/
+-rw-rw-r--   0 jani      (1000) jani      (1000)      793 2020-05-21 16:43:43.000000 django-jbank-4.4.8/jbank/templates/admin/jbank/referencepaymentbatch/change_form.html
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/templates/admin/jbank/referencepaymentbatch/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/templates/admin/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)        0 2023-05-15 21:54:48.000000 django-jbank-4.4.8/jbank/templates/__init__.py
+-rw-rw-r--   0 jani      (1000) jani      (1000)      931 2024-03-12 19:43:36.000000 django-jbank-4.4.8/pyproject.toml
+-rw-rw-r--   0 jani      (1000) jani      (1000)       38 2024-05-20 05:16:18.000000 django-jbank-4.4.8/setup.cfg
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1064 2023-05-16 17:40:29.000000 django-jbank-4.4.8/README.md
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1082 2020-05-26 21:27:46.000000 django-jbank-4.4.8/LICENSE.txt
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:18.000000 django-jbank-4.4.8/django_jbank.egg-info/
+-rw-rw-r--   0 jani      (1000) jani      (1000)   707364 2024-05-20 05:16:17.000000 django-jbank-4.4.8/django_jbank.egg-info/SOURCES.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)        6 2024-05-20 05:16:02.000000 django-jbank-4.4.8/django_jbank.egg-info/top_level.txt
+-rw-r--r--   0 jani      (1000) jani      (1000)     1603 2024-05-20 05:16:02.000000 django-jbank-4.4.8/django_jbank.egg-info/PKG-INFO
+-rw-rw-r--   0 jani      (1000) jani      (1000)      158 2024-05-20 05:16:02.000000 django-jbank-4.4.8/django_jbank.egg-info/requires.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)        1 2020-05-26 21:28:24.000000 django-jbank-4.4.8/django_jbank.egg-info/not-zip-safe
+-rw-rw-r--   0 jani      (1000) jani      (1000)        1 2024-05-20 05:16:02.000000 django-jbank-4.4.8/django_jbank.egg-info/dependency_links.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)      158 2024-02-27 17:18:22.000000 django-jbank-4.4.8/requirements.txt
+-rw-rw-r--   0 jani      (1000) jani      (1000)      247 2020-05-27 18:47:15.000000 django-jbank-4.4.8/mypy.ini
+-rw-rw-r--   0 jani      (1000) jani      (1000)      867 2024-05-20 05:15:59.000000 django-jbank-4.4.8/setup.py
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:17.000000 django-jbank-4.4.8/data/
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:17.000000 django-jbank-4.4.8/data/x509/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1486 2020-05-21 16:43:43.000000 django-jbank-4.4.8/data/x509/appreq.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1561 2022-07-21 16:32:20.000000 django-jbank-4.4.8/data/x509/x509data.xml
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:17.000000 django-jbank-4.4.8/data/finvoice/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     5362 2020-05-21 16:43:43.000000 django-jbank-4.4.8/data/finvoice/xsd-test.xml
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:17.000000 django-jbank-4.4.8/data/pki/
+-rw-rw-r--   0 jani      (1000) jani      (1000)    10099 2020-07-18 04:38:59.000000 django-jbank-4.4.8/data/pki/GetBankCertificate-res.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      638 2020-07-20 22:19:28.000000 django-jbank-4.4.8/data/pki/CreateCertificate-res.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)     1547 2021-07-06 23:33:19.000000 django-jbank-4.4.8/data/x509-data.xml
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:17.000000 django-jbank-4.4.8/data/xm/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     6994 2023-03-27 06:59:59.000000 django-jbank-4.4.8/data/xm/camt_054_credit_notoification_example_finland.xml
+drwxrwxr-x   0 jani      (1000) jani      (1000)        0 2024-05-20 05:16:17.000000 django-jbank-4.4.8/data/pain001/
+-rw-rw-r--   0 jani      (1000) jani      (1000)     4044 2020-05-21 16:43:43.000000 django-jbank-4.4.8/data/pain001/pain.001.001.03.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)    91224 2020-05-21 16:43:43.000000 django-jbank-4.4.8/data/ecb-rates-2019-08-15.xml
+-rw-rw-r--   0 jani      (1000) jani      (1000)      287 2023-08-11 14:50:29.000000 django-jbank-4.4.8/MANIFEST.in
```

### Comparing `django-jbank-4.4.7/PKG-INFO` & `django-jbank-4.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jbank
-Version: 4.4.7
+Version: 4.4.8
 Summary: Finnish bank file format support for Django projects
 Home-page: 
 Author: Jani Kajala
 Author-email: kajala@gmail.com
 License: MIT licence, see LICENCE.txt
 License-File: LICENSE.txt
 Requires-Dist: Django>=3.0.0
```

### Comparing `django-jbank-4.4.7/jbank/tito.py` & `django-jbank-4.4.8/jbank/tito.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/ecb.py` & `django-jbank-4.4.8/jbank/ecb.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/x509_helpers.py` & `django-jbank-4.4.8/jbank/x509_helpers.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/make_x509.py` & `django-jbank-4.4.8/jbank/management/commands/make_x509.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/wsedi_export.py` & `django-jbank-4.4.8/jbank/management/commands/wsedi_export.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/xmlsec1_examples.py` & `django-jbank-4.4.8/jbank/management/commands/xmlsec1_examples.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/parse_xp.py` & `django-jbank-4.4.8/jbank/management/commands/parse_xp.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/wsedi_exec.py` & `django-jbank-4.4.8/jbank/management/commands/wsedi_exec.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/reparse_to.py` & `django-jbank-4.4.8/jbank/management/commands/reparse_to.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/parse_xt.py` & `django-jbank-4.4.8/jbank/management/commands/parse_xt.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/test_app_req.py` & `django-jbank-4.4.8/jbank/management/commands/test_app_req.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/validate_xml.py` & `django-jbank-4.4.8/jbank/management/commands/validate_xml.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/wsedi_download.py` & `django-jbank-4.4.8/jbank/management/commands/wsedi_download.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/reparse_svm.py` & `django-jbank-4.4.8/jbank/management/commands/reparse_svm.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/parse_svm.py` & `django-jbank-4.4.8/jbank/management/commands/parse_svm.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/parse_saldo.py` & `django-jbank-4.4.8/jbank/management/commands/parse_saldo.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/wspki_exec.py` & `django-jbank-4.4.8/jbank/management/commands/wspki_exec.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/parse_xm.py` & `django-jbank-4.4.8/jbank/management/commands/parse_xm.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/test_pain001.py` & `django-jbank-4.4.8/jbank/management/commands/test_pain001.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/wsedi_import.py` & `django-jbank-4.4.8/jbank/management/commands/wsedi_import.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/parse_to.py` & `django-jbank-4.4.8/jbank/management/commands/parse_to.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/make_parse_format.py` & `django-jbank-4.4.8/jbank/management/commands/make_parse_format.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/test_xp.py` & `django-jbank-4.4.8/jbank/management/commands/test_xp.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/make_pain001.py` & `django-jbank-4.4.8/jbank/management/commands/make_pain001.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/parse_aeb43.py` & `django-jbank-4.4.8/jbank/management/commands/parse_aeb43.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/test_payment.py` & `django-jbank-4.4.8/jbank/management/commands/test_payment.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/parse_ecb_rates.py` & `django-jbank-4.4.8/jbank/management/commands/parse_ecb_rates.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/wsedi_upload.py` & `django-jbank-4.4.8/jbank/management/commands/wsedi_upload.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/parse_ra.py` & `django-jbank-4.4.8/jbank/management/commands/parse_ra.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/management/commands/parse_euribor_rates.py` & `django-jbank-4.4.8/jbank/management/commands/parse_euribor_rates.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/wspki.py` & `django-jbank-4.4.8/jbank/wspki.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/pain002.py` & `django-jbank-4.4.8/jbank/pain002.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/aeb43.py` & `django-jbank-4.4.8/jbank/aeb43.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/models.py` & `django-jbank-4.4.8/jbank/models.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/csr_helpers.py` & `django-jbank-4.4.8/jbank/csr_helpers.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/locale/fi/LC_MESSAGES/django.mo` & `django-jbank-4.4.8/jbank/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/locale/fi/LC_MESSAGES/django.po` & `django-jbank-4.4.8/jbank/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/locale/sv/LC_MESSAGES/django.mo` & `django-jbank-4.4.8/jbank/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/locale/sv/LC_MESSAGES/django.po` & `django-jbank-4.4.8/jbank/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/locale/en/LC_MESSAGES/django.mo` & `django-jbank-4.4.8/jbank/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/locale/en/LC_MESSAGES/django.po` & `django-jbank-4.4.8/jbank/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/admin.py` & `django-jbank-4.4.8/jbank/admin.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0026_auto_20181205_0034.py` & `django-jbank-4.4.8/jbank/migrations/0026_auto_20181205_0034.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0026_referencepaymentbatch_identifier_and_more.py` & `django-jbank-4.4.8/jbank/migrations/0026_referencepaymentbatch_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0013_euriborrate.py` & `django-jbank-4.4.8/jbank/migrations/0013_euriborrate.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0018_alter_referencepaymentbatch_currency_identifier_and_more.py` & `django-jbank-4.4.8/jbank/migrations/0018_alter_referencepaymentbatch_currency_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0062_auto_20200415_2300.py` & `django-jbank-4.4.8/jbank/migrations/0062_auto_20200415_2300.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0005_statementfile_created.py` & `django-jbank-4.4.8/jbank/migrations/0005_statementfile_created.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0007_auto_20171102_2351.py` & `django-jbank-4.4.8/jbank/migrations/0007_auto_20171102_2351.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0019_alter_payout_state.py` & `django-jbank-4.4.8/jbank/migrations/0019_alter_payout_state.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0008_auto_20171103_0007.py` & `django-jbank-4.4.8/jbank/migrations/0008_auto_20171103_0007.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0036_remove_referencepaymentrecord_manually_settled_and_more.py` & `django-jbank-4.4.8/jbank/migrations/0036_remove_referencepaymentrecord_manually_settled_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0011_referencepaymentbatch_cached_total_amount.py` & `django-jbank-4.4.8/jbank/migrations/0011_referencepaymentbatch_cached_total_amount.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0051_payout_connection.py` & `django-jbank-4.4.8/jbank/migrations/0051_payout_connection.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0028_referencepaymentrecord_creditor_bank_bic_and_more.py` & `django-jbank-4.4.8/jbank/migrations/0028_referencepaymentrecord_creditor_bank_bic_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0012_auto_20180126_0858.py` & `django-jbank-4.4.8/jbank/migrations/0012_auto_20180126_0858.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0015_auto_20180208_0643.py` & `django-jbank-4.4.8/jbank/migrations/0015_auto_20180208_0643.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0029_auto_20190727_1352.py` & `django-jbank-4.4.8/jbank/migrations/0029_auto_20190727_1352.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0064_auto_20200629_0344.py` & `django-jbank-4.4.8/jbank/migrations/0064_auto_20200629_0344.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0023_remove_accountbalance_connection_accountbalance_bic.py` & `django-jbank-4.4.8/jbank/migrations/0023_remove_accountbalance_connection_accountbalance_bic.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0004_statementfile.py` & `django-jbank-4.4.8/jbank/migrations/0004_statementfile.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0029_alter_referencepaymentrecord_remittance_info.py` & `django-jbank-4.4.8/jbank/migrations/0029_alter_referencepaymentrecord_remittance_info.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0017_payoutparty_payouts_account.py` & `django-jbank-4.4.8/jbank/migrations/0017_payoutparty_payouts_account.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0027_auto_20190304_1913.py` & `django-jbank-4.4.8/jbank/migrations/0027_auto_20190304_1913.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0002_auto_20171031_0356.py` & `django-jbank-4.4.8/jbank/migrations/0002_auto_20171031_0356.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0035_wsediconnection_agreement_identifier_and_more.py` & `django-jbank-4.4.8/jbank/migrations/0035_wsediconnection_agreement_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0013_auto_20180126_0909.py` & `django-jbank-4.4.8/jbank/migrations/0013_auto_20180126_0909.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0020_accountbalance.py` & `django-jbank-4.4.8/jbank/migrations/0020_accountbalance.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0016_alter_payoutstatus_timestamp.py` & `django-jbank-4.4.8/jbank/migrations/0016_alter_payoutstatus_timestamp.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0024_auto_20180425_1704.py` & `django-jbank-4.4.8/jbank/migrations/0024_auto_20180425_1704.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0007_auto_20210507_2122.py` & `django-jbank-4.4.8/jbank/migrations/0007_auto_20210507_2122.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0011_auto_20180126_0851.py` & `django-jbank-4.4.8/jbank/migrations/0011_auto_20180126_0851.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0061_auto_20200325_2204.py` & `django-jbank-4.4.8/jbank/migrations/0061_auto_20200325_2204.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0009_auto_20171107_1847.py` & `django-jbank-4.4.8/jbank/migrations/0009_auto_20171107_1847.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0025_auto_20230325_1014.py` & `django-jbank-4.4.8/jbank/migrations/0025_auto_20230325_1014.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0041_auto_20191127_0559.py` & `django-jbank-4.4.8/jbank/migrations/0041_auto_20191127_0559.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0031_wsediconnection_old_encryption_key_file_and_more.py` & `django-jbank-4.4.8/jbank/migrations/0031_wsediconnection_old_encryption_key_file_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0025_auto_20181101_1430.py` & `django-jbank-4.4.8/jbank/migrations/0025_auto_20181101_1430.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0012_alter_referencepaymentrecord_delivery_method.py` & `django-jbank-4.4.8/jbank/migrations/0012_alter_referencepaymentrecord_delivery_method.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0039_auto_20191127_0156.py` & `django-jbank-4.4.8/jbank/migrations/0039_auto_20191127_0156.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0014_payout_payoutstatus.py` & `django-jbank-4.4.8/jbank/migrations/0014_payout_payoutstatus.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0006_auto_20210318_2130.py` & `django-jbank-4.4.8/jbank/migrations/0006_auto_20210318_2130.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0022_accountbalance_connection.py` & `django-jbank-4.4.8/jbank/migrations/0022_accountbalance_connection.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0024_referencepaymentbatchfile_additional_info_and_more.py` & `django-jbank-4.4.8/jbank/migrations/0024_referencepaymentbatchfile_additional_info_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0048_wsediconnection_soap_endpoint.py` & `django-jbank-4.4.8/jbank/migrations/0048_wsediconnection_soap_endpoint.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0027_referencepaymentrecord_value_date_and_more.py` & `django-jbank-4.4.8/jbank/migrations/0027_referencepaymentrecord_value_date_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0010_statementrecorddetail_creditor_account_scheme.py` & `django-jbank-4.4.8/jbank/migrations/0010_statementrecorddetail_creditor_account_scheme.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0030_alter_referencepaymentrecord_remittance_info.py` & `django-jbank-4.4.8/jbank/migrations/0030_alter_referencepaymentrecord_remittance_info.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0031_auto_20190727_1639.py` & `django-jbank-4.4.8/jbank/migrations/0031_auto_20190727_1639.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0037_auto_20191127_0132.py` & `django-jbank-4.4.8/jbank/migrations/0037_auto_20191127_0132.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0043_wsedisoapcall.py` & `django-jbank-4.4.8/jbank/migrations/0043_wsedisoapcall.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0060_auto_20200325_1906.py` & `django-jbank-4.4.8/jbank/migrations/0060_auto_20200325_1906.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0003_statement_account.py` & `django-jbank-4.4.8/jbank/migrations/0003_statement_account.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0001_squashed_0071_wsediconnection_ca_cert_file.py` & `django-jbank-4.4.8/jbank/migrations/0001_squashed_0071_wsediconnection_ca_cert_file.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0002_auto_20200817_2217.py` & `django-jbank-4.4.8/jbank/migrations/0002_auto_20200817_2217.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0052_auto_20191130_1927.py` & `django-jbank-4.4.8/jbank/migrations/0052_auto_20191130_1927.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0006_auto_20171102_2341.py` & `django-jbank-4.4.8/jbank/migrations/0006_auto_20171102_2341.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0001_initial.py` & `django-jbank-4.4.8/jbank/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0034_auto_20190815_2059.py` & `django-jbank-4.4.8/jbank/migrations/0034_auto_20190815_2059.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0008_auto_20210512_2208.py` & `django-jbank-4.4.8/jbank/migrations/0008_auto_20210512_2208.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0037_alter_referencepaymentrecord_marked_reconciled_and_more.py` & `django-jbank-4.4.8/jbank/migrations/0037_alter_referencepaymentrecord_marked_reconciled_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0021_auto_20180209_0935.py` & `django-jbank-4.4.8/jbank/migrations/0021_auto_20180209_0935.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0016_auto_20180208_0724.py` & `django-jbank-4.4.8/jbank/migrations/0016_auto_20180208_0724.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0069_auto_20200717_2333.py` & `django-jbank-4.4.8/jbank/migrations/0069_auto_20200717_2333.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0019_auto_20180209_0437.py` & `django-jbank-4.4.8/jbank/migrations/0019_auto_20180209_0437.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0036_wsediconnection.py` & `django-jbank-4.4.8/jbank/migrations/0036_wsediconnection.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0055_auto_20191130_2011.py` & `django-jbank-4.4.8/jbank/migrations/0055_auto_20191130_2011.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/migrations/0018_auto_20180208_1130.py` & `django-jbank-4.4.8/jbank/migrations/0018_auto_20180208_1130.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/helpers.py` & `django-jbank-4.4.8/jbank/helpers.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/svm.py` & `django-jbank-4.4.8/jbank/svm.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/wsedi.py` & `django-jbank-4.4.8/jbank/wsedi.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/tests.py` & `django-jbank-4.4.8/jbank/tests.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/sepa.py` & `django-jbank-4.4.8/jbank/sepa.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/services.py` & `django-jbank-4.4.8/jbank/services.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/camt.py` & `django-jbank-4.4.8/jbank/camt.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,19 +330,19 @@
                 d.end_to_end_identifier = d_refs.get("EndToEndId", "")
 
                 d_parties = dtl.get("RltdPties", {})
                 d_dbt = d_parties.get("Dbtr", {})
                 d.debtor_name = d_dbt.get("Nm", "")
                 d_udbt = d_parties.get("UltmtDbtr", {})
                 d.ultimate_debtor_name = d_udbt.get("Nm", "")
-                d_cdtr = d_parties.get("Cdtr", {})
-                d.creditor_name = d_cdtr.get("Nm", "")
-                d_cdtr_acct = d_parties.get("CdtrAcct", {})
-                d_cdtr_acct_id = d_cdtr_acct.get("Id", {})
-                d.creditor_account = d_cdtr_acct_id.get("IBAN", "")
+                d_cdtr = d_parties.get("Cdtr") or {}
+                d.creditor_name = d_cdtr.get("Nm") or ""
+                d_cdtr_acct = d_parties.get("CdtrAcct") or {}
+                d_cdtr_acct_id = d_cdtr_acct.get("Id") or {}
+                d.creditor_account = d_cdtr_acct_id.get("IBAN") or ""
                 if d.creditor_account:
                     d.creditor_account_scheme = "IBAN"
                 else:
                     d_cdtr_acct_id_othr = d_cdtr_acct_id.get("Othr") or {}
                     d.creditor_account_scheme = d_cdtr_acct_id_othr.get("SchmeNm", {}).get("Cd", "")
                     d.creditor_account = d_cdtr_acct_id_othr.get("Id") or ""
```

### Comparing `django-jbank-4.4.7/jbank/xmlsec1-examples/sign3.c` & `django-jbank-4.4.8/jbank/xmlsec1-examples/sign3.c`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/xmlsec1-examples/verify3.c` & `django-jbank-4.4.8/jbank/xmlsec1-examples/verify3.c`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/xmlsec1-examples/encrypt3.c` & `django-jbank-4.4.8/jbank/xmlsec1-examples/encrypt3.c`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/xmlsec1-examples/decrypt3.c` & `django-jbank-4.4.8/jbank/xmlsec1-examples/decrypt3.c`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/xmlsec1-examples/sign3-sha256.c` & `django-jbank-4.4.8/jbank/xmlsec1-examples/sign3-sha256.c`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/xmlsec1-examples/Makefile` & `django-jbank-4.4.8/jbank/xmlsec1-examples/Makefile`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/parsers.py` & `django-jbank-4.4.8/jbank/parsers.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/euribor.py` & `django-jbank-4.4.8/jbank/euribor.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/files.py` & `django-jbank-4.4.8/jbank/files.py`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/templates/jbank/pki_get_certificate_soap_template.xml` & `django-jbank-4.4.8/jbank/templates/jbank/pki_get_certificate_soap_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/templates/jbank/pki_certificate_status_request_template.xml` & `django-jbank-4.4.8/jbank/templates/jbank/pki_certificate_status_request_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/templates/jbank/pki_renew_certificate_request_template.xml` & `django-jbank-4.4.8/jbank/templates/jbank/pki_renew_certificate_request_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/templates/jbank/pki_create_certificate_request_template.xml` & `django-jbank-4.4.8/jbank/templates/jbank/pki_create_certificate_request_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/templates/jbank/pki_renew_certificate_request_template-sha256.xml` & `django-jbank-4.4.8/jbank/templates/jbank/pki_renew_certificate_request_template-sha256.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/templates/jbank/soap_template.xml` & `django-jbank-4.4.8/jbank/templates/jbank/soap_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/templates/jbank/pki_soap_template.xml` & `django-jbank-4.4.8/jbank/templates/jbank/pki_soap_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/templates/jbank/application_request_template-sha256.xml` & `django-jbank-4.4.8/jbank/templates/jbank/application_request_template-sha256.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/templates/jbank/pki_get_certificate_request_template.xml` & `django-jbank-4.4.8/jbank/templates/jbank/pki_get_certificate_request_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/templates/jbank/pki_get_certificate_renew_request_template-sha256.xml` & `django-jbank-4.4.8/jbank/templates/jbank/pki_get_certificate_renew_request_template-sha256.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/templates/jbank/pki_get_certificate_renew_request_template.xml` & `django-jbank-4.4.8/jbank/templates/jbank/pki_get_certificate_renew_request_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/templates/jbank/encryption_template.xml` & `django-jbank-4.4.8/jbank/templates/jbank/encryption_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/templates/jbank/enveloping-sha256-rsa-sha256.xml` & `django-jbank-4.4.8/jbank/templates/jbank/enveloping-sha256-rsa-sha256.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/templates/jbank/application_request_template.xml` & `django-jbank-4.4.8/jbank/templates/jbank/application_request_template.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/templates/admin/jbank/mark_as_marked_reconciled.html` & `django-jbank-4.4.8/jbank/templates/admin/jbank/mark_as_marked_reconciled.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/templates/admin/jbank/statement/change_form.html` & `django-jbank-4.4.8/jbank/templates/admin/jbank/statement/change_form.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/jbank/templates/admin/jbank/referencepaymentbatch/change_form.html` & `django-jbank-4.4.8/jbank/templates/admin/jbank/referencepaymentbatch/change_form.html`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/pyproject.toml` & `django-jbank-4.4.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/README.md` & `django-jbank-4.4.8/README.md`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/LICENSE.txt` & `django-jbank-4.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/django_jbank.egg-info/SOURCES.txt` & `django-jbank-4.4.8/django_jbank.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/django_jbank.egg-info/PKG-INFO` & `django-jbank-4.4.8/django_jbank.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jbank
-Version: 4.4.7
+Version: 4.4.8
 Summary: Finnish bank file format support for Django projects
 Home-page: 
 Author: Jani Kajala
 Author-email: kajala@gmail.com
 License: MIT licence, see LICENCE.txt
 License-File: LICENSE.txt
 Requires-Dist: Django>=3.0.0
```

### Comparing `django-jbank-4.4.7/setup.py` & `django-jbank-4.4.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     return [line for line in lineiter if line and not line.startswith("#")]
 
 
 install_requires = parse_requirements("requirements.txt", session=False)
 
 setup(
     name="django-jbank",
-    version="4.4.7",
+    version="4.4.8",
     author="Jani Kajala",
     author_email="kajala@gmail.com",
     packages=find_packages(exclude=["project", "venv"]),
     include_package_data=True,
     url="",
     license="MIT licence, see LICENCE.txt",
     description="Finnish bank file format support for Django projects",
```

### Comparing `django-jbank-4.4.7/data/x509/appreq.xml` & `django-jbank-4.4.8/data/x509/appreq.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/data/x509/x509data.xml` & `django-jbank-4.4.8/data/x509/x509data.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/data/finvoice/xsd-test.xml` & `django-jbank-4.4.8/data/finvoice/xsd-test.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/data/pki/GetBankCertificate-res.xml` & `django-jbank-4.4.8/data/pki/GetBankCertificate-res.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/data/pki/CreateCertificate-res.xml` & `django-jbank-4.4.8/data/pki/CreateCertificate-res.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/data/x509-data.xml` & `django-jbank-4.4.8/data/x509-data.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/data/xm/camt_054_credit_notoification_example_finland.xml` & `django-jbank-4.4.8/data/xm/camt_054_credit_notoification_example_finland.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/data/pain001/pain.001.001.03.xml` & `django-jbank-4.4.8/data/pain001/pain.001.001.03.xml`

 * *Files identical despite different names*

### Comparing `django-jbank-4.4.7/data/ecb-rates-2019-08-15.xml` & `django-jbank-4.4.8/data/ecb-rates-2019-08-15.xml`

 * *Files identical despite different names*

