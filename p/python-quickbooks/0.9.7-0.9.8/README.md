# Comparing `tmp/python-quickbooks-0.9.7.tar.gz` & `tmp/python-quickbooks-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-quickbooks-0.9.7.tar", last modified: Tue Mar 12 20:34:53 2024, max compression
+gzip compressed data, was "python-quickbooks-0.9.8.tar", last modified: Mon May 20 20:38:37 2024, max compression
```

## Comparing `python-quickbooks-0.9.7.tar` & `python-quickbooks-0.9.8.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-03-12 20:34:53.805436 python-quickbooks-0.9.7/
--rw-r--r--   0 root         (0) staff       (20)     1085 2022-05-14 23:22:04.000000 python-quickbooks-0.9.7/LICENSE
--rw-r--r--   0 root         (0) staff       (20)       59 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)    12086 2024-03-12 20:34:53.805321 python-quickbooks-0.9.7/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)    10956 2024-03-11 20:02:52.000000 python-quickbooks-0.9.7/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-03-12 20:34:53.798734 python-quickbooks-0.9.7/python_quickbooks.egg-info/
--rw-r--r--   0 root         (0) staff       (20)    12086 2024-03-12 20:34:53.000000 python-quickbooks-0.9.7/python_quickbooks.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1921 2024-03-12 20:34:53.000000 python-quickbooks-0.9.7/python_quickbooks.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-03-12 20:34:53.000000 python-quickbooks-0.9.7/python_quickbooks.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       68 2024-03-12 20:34:53.000000 python-quickbooks-0.9.7/python_quickbooks.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)      108 2024-03-12 20:34:53.000000 python-quickbooks-0.9.7/python_quickbooks.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       17 2024-03-12 20:34:53.000000 python-quickbooks-0.9.7/python_quickbooks.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-03-12 20:34:53.799714 python-quickbooks-0.9.7/quickbooks/
--rw-r--r--   0 root         (0) staff       (20)       30 2022-05-14 23:22:04.000000 python-quickbooks-0.9.7/quickbooks/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3110 2022-05-14 23:22:04.000000 python-quickbooks-0.9.7/quickbooks/batch.py
--rw-r--r--   0 root         (0) staff       (20)     1453 2022-05-14 23:22:04.000000 python-quickbooks-0.9.7/quickbooks/cdc.py
--rw-r--r--   0 root         (0) staff       (20)    12455 2024-03-12 20:29:22.000000 python-quickbooks-0.9.7/quickbooks/client.py
--rw-r--r--   0 root         (0) staff       (20)     1831 2022-08-03 20:04:42.000000 python-quickbooks-0.9.7/quickbooks/exceptions.py
--rw-r--r--   0 root         (0) staff       (20)      681 2022-05-14 23:22:04.000000 python-quickbooks-0.9.7/quickbooks/helpers.py
--rw-r--r--   0 root         (0) staff       (20)    12378 2024-01-02 20:31:52.000000 python-quickbooks-0.9.7/quickbooks/mixins.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-03-12 20:34:53.805076 python-quickbooks-0.9.7/quickbooks/objects/
--rw-r--r--   0 root         (0) staff       (20)     2245 2022-05-14 23:22:04.000000 python-quickbooks-0.9.7/quickbooks/objects/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1620 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/account.py
--rw-r--r--   0 root         (0) staff       (20)     2407 2024-01-04 18:35:43.000000 python-quickbooks-0.9.7/quickbooks/objects/attachable.py
--rw-r--r--   0 root         (0) staff       (20)     3616 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/base.py
--rw-r--r--   0 root         (0) staff       (20)     2270 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/batchrequest.py
--rw-r--r--   0 root         (0) staff       (20)     2129 2024-01-04 15:38:58.000000 python-quickbooks-0.9.7/quickbooks/objects/bill.py
--rw-r--r--   0 root         (0) staff       (20)     2633 2024-01-02 20:31:52.000000 python-quickbooks-0.9.7/quickbooks/objects/billpayment.py
--rw-r--r--   0 root         (0) staff       (20)     1590 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/budget.py
--rw-r--r--   0 root         (0) staff       (20)      357 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/changedatacapture.py
--rw-r--r--   0 root         (0) staff       (20)     1680 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/company_info.py
--rw-r--r--   0 root         (0) staff       (20)     1153 2024-03-12 20:29:22.000000 python-quickbooks-0.9.7/quickbooks/objects/companycurrency.py
--rw-r--r--   0 root         (0) staff       (20)      996 2022-05-14 23:22:04.000000 python-quickbooks-0.9.7/quickbooks/objects/creditcardpayment.py
--rw-r--r--   0 root         (0) staff       (20)     1444 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/creditcardpayment_entity.py
--rw-r--r--   0 root         (0) staff       (20)     2349 2024-01-02 20:31:52.000000 python-quickbooks-0.9.7/quickbooks/objects/creditmemo.py
--rw-r--r--   0 root         (0) staff       (20)     2750 2024-03-12 20:29:22.000000 python-quickbooks-0.9.7/quickbooks/objects/customer.py
--rw-r--r--   0 root         (0) staff       (20)      894 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/customertype.py
--rw-r--r--   0 root         (0) staff       (20)     1245 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/department.py
--rw-r--r--   0 root         (0) staff       (20)     2973 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/deposit.py
--rw-r--r--   0 root         (0) staff       (20)     6211 2024-01-04 15:38:58.000000 python-quickbooks-0.9.7/quickbooks/objects/detailline.py
--rw-r--r--   0 root         (0) staff       (20)     1419 2024-01-04 15:38:58.000000 python-quickbooks-0.9.7/quickbooks/objects/employee.py
--rw-r--r--   0 root         (0) staff       (20)     2728 2024-01-04 15:38:58.000000 python-quickbooks-0.9.7/quickbooks/objects/estimate.py
--rw-r--r--   0 root         (0) staff       (20)     1152 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/exchangerate.py
--rw-r--r--   0 root         (0) staff       (20)     3831 2024-01-02 20:31:52.000000 python-quickbooks-0.9.7/quickbooks/objects/invoice.py
--rw-r--r--   0 root         (0) staff       (20)     2476 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/item.py
--rw-r--r--   0 root         (0) staff       (20)     2643 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/journalentry.py
--rw-r--r--   0 root         (0) staff       (20)     2968 2024-01-02 20:31:52.000000 python-quickbooks-0.9.7/quickbooks/objects/payment.py
--rw-r--r--   0 root         (0) staff       (20)      952 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/paymentmethod.py
--rw-r--r--   0 root         (0) staff       (20)     7203 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/preferences.py
--rw-r--r--   0 root         (0) staff       (20)     2593 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/purchase.py
--rw-r--r--   0 root         (0) staff       (20)     2169 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/purchaseorder.py
--rw-r--r--   0 root         (0) staff       (20)     3682 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/recurringtransaction.py
--rw-r--r--   0 root         (0) staff       (20)     2646 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/refundreceipt.py
--rw-r--r--   0 root         (0) staff       (20)     2559 2024-01-02 20:31:52.000000 python-quickbooks-0.9.7/quickbooks/objects/salesreceipt.py
--rw-r--r--   0 root         (0) staff       (20)     1033 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/tax.py
--rw-r--r--   0 root         (0) staff       (20)      678 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/taxagency.py
--rw-r--r--   0 root         (0) staff       (20)     2014 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/taxcode.py
--rw-r--r--   0 root         (0) staff       (20)      974 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/taxrate.py
--rw-r--r--   0 root         (0) staff       (20)     1982 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/taxservice.py
--rw-r--r--   0 root         (0) staff       (20)     1357 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/term.py
--rw-r--r--   0 root         (0) staff       (20)     1337 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/timeactivity.py
--rw-r--r--   0 root         (0) staff       (20)     1044 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/trackingclass.py
--rw-r--r--   0 root         (0) staff       (20)      818 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/transfer.py
--rw-r--r--   0 root         (0) staff       (20)     1976 2024-01-04 15:38:58.000000 python-quickbooks-0.9.7/quickbooks/objects/vendor.py
--rw-r--r--   0 root         (0) staff       (20)     1447 2023-08-29 16:12:31.000000 python-quickbooks-0.9.7/quickbooks/objects/vendorcredit.py
--rw-r--r--   0 root         (0) staff       (20)      871 2024-01-03 21:46:49.000000 python-quickbooks-0.9.7/quickbooks/utils.py
--rw-r--r--   0 root         (0) staff       (20)      358 2024-03-12 20:34:53.805687 python-quickbooks-0.9.7/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     1696 2024-03-12 20:29:22.000000 python-quickbooks-0.9.7/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-20 20:38:37.680029 python-quickbooks-0.9.8/
+-rw-r--r--   0 root         (0) staff       (20)     1085 2022-05-14 23:22:04.000000 python-quickbooks-0.9.8/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)       59 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)    12099 2024-05-20 20:38:37.679923 python-quickbooks-0.9.8/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)    10969 2024-05-20 20:37:16.000000 python-quickbooks-0.9.8/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-20 20:38:37.668547 python-quickbooks-0.9.8/python_quickbooks.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)    12099 2024-05-20 20:38:37.000000 python-quickbooks-0.9.8/python_quickbooks.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1921 2024-05-20 20:38:37.000000 python-quickbooks-0.9.8/python_quickbooks.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-05-20 20:38:37.000000 python-quickbooks-0.9.8/python_quickbooks.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       68 2024-05-20 20:38:37.000000 python-quickbooks-0.9.8/python_quickbooks.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)      108 2024-05-20 20:38:37.000000 python-quickbooks-0.9.8/python_quickbooks.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       17 2024-05-20 20:38:37.000000 python-quickbooks-0.9.8/python_quickbooks.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-20 20:38:37.670562 python-quickbooks-0.9.8/quickbooks/
+-rw-r--r--   0 root         (0) staff       (20)       30 2022-05-14 23:22:04.000000 python-quickbooks-0.9.8/quickbooks/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3110 2022-05-14 23:22:04.000000 python-quickbooks-0.9.8/quickbooks/batch.py
+-rw-r--r--   0 root         (0) staff       (20)     1453 2022-05-14 23:22:04.000000 python-quickbooks-0.9.8/quickbooks/cdc.py
+-rw-r--r--   0 root         (0) staff       (20)    12455 2024-03-12 20:29:22.000000 python-quickbooks-0.9.8/quickbooks/client.py
+-rw-r--r--   0 root         (0) staff       (20)     1831 2022-08-03 20:04:42.000000 python-quickbooks-0.9.8/quickbooks/exceptions.py
+-rw-r--r--   0 root         (0) staff       (20)      681 2022-05-14 23:22:04.000000 python-quickbooks-0.9.8/quickbooks/helpers.py
+-rw-r--r--   0 root         (0) staff       (20)    12378 2024-05-20 18:32:29.000000 python-quickbooks-0.9.8/quickbooks/mixins.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-20 20:38:37.679619 python-quickbooks-0.9.8/quickbooks/objects/
+-rw-r--r--   0 root         (0) staff       (20)     2245 2022-05-14 23:22:04.000000 python-quickbooks-0.9.8/quickbooks/objects/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1620 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/account.py
+-rw-r--r--   0 root         (0) staff       (20)     2407 2024-01-04 18:35:43.000000 python-quickbooks-0.9.8/quickbooks/objects/attachable.py
+-rw-r--r--   0 root         (0) staff       (20)     3616 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/base.py
+-rw-r--r--   0 root         (0) staff       (20)     2270 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/batchrequest.py
+-rw-r--r--   0 root         (0) staff       (20)     2129 2024-01-04 15:38:58.000000 python-quickbooks-0.9.8/quickbooks/objects/bill.py
+-rw-r--r--   0 root         (0) staff       (20)     2633 2024-01-02 20:31:52.000000 python-quickbooks-0.9.8/quickbooks/objects/billpayment.py
+-rw-r--r--   0 root         (0) staff       (20)     1590 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/budget.py
+-rw-r--r--   0 root         (0) staff       (20)      357 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/changedatacapture.py
+-rw-r--r--   0 root         (0) staff       (20)     1680 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/company_info.py
+-rw-r--r--   0 root         (0) staff       (20)     1153 2024-03-12 20:29:22.000000 python-quickbooks-0.9.8/quickbooks/objects/companycurrency.py
+-rw-r--r--   0 root         (0) staff       (20)      996 2022-05-14 23:22:04.000000 python-quickbooks-0.9.8/quickbooks/objects/creditcardpayment.py
+-rw-r--r--   0 root         (0) staff       (20)     1444 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/creditcardpayment_entity.py
+-rw-r--r--   0 root         (0) staff       (20)     2349 2024-01-02 20:31:52.000000 python-quickbooks-0.9.8/quickbooks/objects/creditmemo.py
+-rw-r--r--   0 root         (0) staff       (20)     2750 2024-03-12 20:29:22.000000 python-quickbooks-0.9.8/quickbooks/objects/customer.py
+-rw-r--r--   0 root         (0) staff       (20)      894 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/customertype.py
+-rw-r--r--   0 root         (0) staff       (20)     1245 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/department.py
+-rw-r--r--   0 root         (0) staff       (20)     2973 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/deposit.py
+-rw-r--r--   0 root         (0) staff       (20)     6277 2024-05-20 20:37:16.000000 python-quickbooks-0.9.8/quickbooks/objects/detailline.py
+-rw-r--r--   0 root         (0) staff       (20)     1419 2024-01-04 15:38:58.000000 python-quickbooks-0.9.8/quickbooks/objects/employee.py
+-rw-r--r--   0 root         (0) staff       (20)     2728 2024-01-04 15:38:58.000000 python-quickbooks-0.9.8/quickbooks/objects/estimate.py
+-rw-r--r--   0 root         (0) staff       (20)     1152 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/exchangerate.py
+-rw-r--r--   0 root         (0) staff       (20)     3831 2024-01-02 20:31:52.000000 python-quickbooks-0.9.8/quickbooks/objects/invoice.py
+-rw-r--r--   0 root         (0) staff       (20)     2476 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/item.py
+-rw-r--r--   0 root         (0) staff       (20)     2643 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/journalentry.py
+-rw-r--r--   0 root         (0) staff       (20)     2968 2024-01-02 20:31:52.000000 python-quickbooks-0.9.8/quickbooks/objects/payment.py
+-rw-r--r--   0 root         (0) staff       (20)      952 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/paymentmethod.py
+-rw-r--r--   0 root         (0) staff       (20)     7203 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/preferences.py
+-rw-r--r--   0 root         (0) staff       (20)     2593 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/purchase.py
+-rw-r--r--   0 root         (0) staff       (20)     2169 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/purchaseorder.py
+-rw-r--r--   0 root         (0) staff       (20)     3682 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/recurringtransaction.py
+-rw-r--r--   0 root         (0) staff       (20)     2646 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/refundreceipt.py
+-rw-r--r--   0 root         (0) staff       (20)     2559 2024-01-02 20:31:52.000000 python-quickbooks-0.9.8/quickbooks/objects/salesreceipt.py
+-rw-r--r--   0 root         (0) staff       (20)     1033 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/tax.py
+-rw-r--r--   0 root         (0) staff       (20)      678 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/taxagency.py
+-rw-r--r--   0 root         (0) staff       (20)     2014 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/taxcode.py
+-rw-r--r--   0 root         (0) staff       (20)      974 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/taxrate.py
+-rw-r--r--   0 root         (0) staff       (20)     1982 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/taxservice.py
+-rw-r--r--   0 root         (0) staff       (20)     1357 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/term.py
+-rw-r--r--   0 root         (0) staff       (20)     1337 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/timeactivity.py
+-rw-r--r--   0 root         (0) staff       (20)     1044 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/trackingclass.py
+-rw-r--r--   0 root         (0) staff       (20)      818 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/transfer.py
+-rw-r--r--   0 root         (0) staff       (20)     1976 2024-01-04 15:38:58.000000 python-quickbooks-0.9.8/quickbooks/objects/vendor.py
+-rw-r--r--   0 root         (0) staff       (20)     1447 2023-08-29 16:12:31.000000 python-quickbooks-0.9.8/quickbooks/objects/vendorcredit.py
+-rw-r--r--   0 root         (0) staff       (20)      871 2024-01-03 21:46:49.000000 python-quickbooks-0.9.8/quickbooks/utils.py
+-rw-r--r--   0 root         (0) staff       (20)      358 2024-05-20 20:38:37.680321 python-quickbooks-0.9.8/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     1696 2024-05-20 20:37:16.000000 python-quickbooks-0.9.8/setup.py
```

### Comparing `python-quickbooks-0.9.7/LICENSE` & `python-quickbooks-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/PKG-INFO` & `python-quickbooks-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-quickbooks
-Version: 0.9.7
+Version: 0.9.8
 Summary: A Python library for accessing the QuickBooks API.
 Home-page: https://github.com/ej2/python-quickbooks
 Author: Edward Emanuel Jr.
 Author-email: edward.emanuel@gmail.com
 License: MIT
 Keywords: quickbooks,qbo,accounting
 Classifier: Development Status :: 3 - Alpha
@@ -303,18 +303,18 @@
 Converting an object to JSON data:
 
     account = Account.get(1, qb=client)
     json_data = account.to_json()
 
 Loading JSON data into a quickbooks object:
 
-    account = Account()
-    account.from_json(
+    account = Account.from_json(
      {
       "AccountType": "Accounts Receivable",
+      "AcctNum": "123123",
       "Name": "MyJobs"
      }
     )
     account.save(qb=client)
 
 Date formatting
 ----------------
```

### Comparing `python-quickbooks-0.9.7/README.md` & `python-quickbooks-0.9.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -273,18 +273,18 @@
 Converting an object to JSON data:
 
     account = Account.get(1, qb=client)
     json_data = account.to_json()
 
 Loading JSON data into a quickbooks object:
 
-    account = Account()
-    account.from_json(
+    account = Account.from_json(
      {
       "AccountType": "Accounts Receivable",
+      "AcctNum": "123123",
       "Name": "MyJobs"
      }
     )
     account.save(qb=client)
 
 Date formatting
 ----------------
```

### Comparing `python-quickbooks-0.9.7/python_quickbooks.egg-info/PKG-INFO` & `python-quickbooks-0.9.8/python_quickbooks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-quickbooks
-Version: 0.9.7
+Version: 0.9.8
 Summary: A Python library for accessing the QuickBooks API.
 Home-page: https://github.com/ej2/python-quickbooks
 Author: Edward Emanuel Jr.
 Author-email: edward.emanuel@gmail.com
 License: MIT
 Keywords: quickbooks,qbo,accounting
 Classifier: Development Status :: 3 - Alpha
@@ -303,18 +303,18 @@
 Converting an object to JSON data:
 
     account = Account.get(1, qb=client)
     json_data = account.to_json()
 
 Loading JSON data into a quickbooks object:
 
-    account = Account()
-    account.from_json(
+    account = Account.from_json(
      {
       "AccountType": "Accounts Receivable",
+      "AcctNum": "123123",
       "Name": "MyJobs"
      }
     )
     account.save(qb=client)
 
 Date formatting
 ----------------
```

### Comparing `python-quickbooks-0.9.7/python_quickbooks.egg-info/SOURCES.txt` & `python-quickbooks-0.9.8/python_quickbooks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/batch.py` & `python-quickbooks-0.9.8/quickbooks/batch.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/cdc.py` & `python-quickbooks-0.9.8/quickbooks/cdc.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/client.py` & `python-quickbooks-0.9.8/quickbooks/client.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/exceptions.py` & `python-quickbooks-0.9.8/quickbooks/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/helpers.py` & `python-quickbooks-0.9.8/quickbooks/helpers.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/mixins.py` & `python-quickbooks-0.9.8/quickbooks/mixins.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/__init__.py` & `python-quickbooks-0.9.8/quickbooks/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/account.py` & `python-quickbooks-0.9.8/quickbooks/objects/account.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/attachable.py` & `python-quickbooks-0.9.8/quickbooks/objects/attachable.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/base.py` & `python-quickbooks-0.9.8/quickbooks/objects/base.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/batchrequest.py` & `python-quickbooks-0.9.8/quickbooks/objects/batchrequest.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/bill.py` & `python-quickbooks-0.9.8/quickbooks/objects/bill.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/billpayment.py` & `python-quickbooks-0.9.8/quickbooks/objects/billpayment.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/budget.py` & `python-quickbooks-0.9.8/quickbooks/objects/budget.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/company_info.py` & `python-quickbooks-0.9.8/quickbooks/objects/company_info.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/companycurrency.py` & `python-quickbooks-0.9.8/quickbooks/objects/companycurrency.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/creditcardpayment.py` & `python-quickbooks-0.9.8/quickbooks/objects/creditcardpayment.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/creditcardpayment_entity.py` & `python-quickbooks-0.9.8/quickbooks/objects/creditcardpayment_entity.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/creditmemo.py` & `python-quickbooks-0.9.8/quickbooks/objects/creditmemo.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/customer.py` & `python-quickbooks-0.9.8/quickbooks/objects/customer.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/customertype.py` & `python-quickbooks-0.9.8/quickbooks/objects/customertype.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/department.py` & `python-quickbooks-0.9.8/quickbooks/objects/department.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/deposit.py` & `python-quickbooks-0.9.8/quickbooks/objects/deposit.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/detailline.py` & `python-quickbooks-0.9.8/quickbooks/objects/detailline.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,14 +98,15 @@
         self.ServiceDate = ""
         self.TaxCodeRef = None
 
 
 class SalesItemLineDetail(QuickbooksBaseObject):
     class_dict = {
         "ItemRef": Ref,
+        "ItemAccountRef": Ref,
         "ClassRef": Ref,
         "TaxCodeRef": Ref,
         "PriceLevelRef": Ref,
         "MarkupInfo": MarkupInfo,
     }
 
     def __init__(self):
@@ -113,14 +114,15 @@
         self.UnitPrice = 0
         self.Qty = 0
         self.ServiceDate = ""
         self.TaxInclusiveAmt = 0
 
         self.MarkupInfo = None
         self.ItemRef = None
+        self.ItemAccountRef = None
         self.ClassRef = None
         self.TaxCodeRef = None
         self.PriceLevelRef = None
 
     def __str__(self):
         return str(self.UnitPrice)
```

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/employee.py` & `python-quickbooks-0.9.8/quickbooks/objects/employee.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/estimate.py` & `python-quickbooks-0.9.8/quickbooks/objects/estimate.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/exchangerate.py` & `python-quickbooks-0.9.8/quickbooks/objects/exchangerate.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/invoice.py` & `python-quickbooks-0.9.8/quickbooks/objects/invoice.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/item.py` & `python-quickbooks-0.9.8/quickbooks/objects/item.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/journalentry.py` & `python-quickbooks-0.9.8/quickbooks/objects/journalentry.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/payment.py` & `python-quickbooks-0.9.8/quickbooks/objects/payment.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/paymentmethod.py` & `python-quickbooks-0.9.8/quickbooks/objects/paymentmethod.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/preferences.py` & `python-quickbooks-0.9.8/quickbooks/objects/preferences.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/purchase.py` & `python-quickbooks-0.9.8/quickbooks/objects/purchase.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/purchaseorder.py` & `python-quickbooks-0.9.8/quickbooks/objects/purchaseorder.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/recurringtransaction.py` & `python-quickbooks-0.9.8/quickbooks/objects/recurringtransaction.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/refundreceipt.py` & `python-quickbooks-0.9.8/quickbooks/objects/refundreceipt.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/salesreceipt.py` & `python-quickbooks-0.9.8/quickbooks/objects/salesreceipt.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/tax.py` & `python-quickbooks-0.9.8/quickbooks/objects/tax.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/taxagency.py` & `python-quickbooks-0.9.8/quickbooks/objects/taxagency.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/taxcode.py` & `python-quickbooks-0.9.8/quickbooks/objects/taxcode.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/taxrate.py` & `python-quickbooks-0.9.8/quickbooks/objects/taxrate.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/taxservice.py` & `python-quickbooks-0.9.8/quickbooks/objects/taxservice.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/term.py` & `python-quickbooks-0.9.8/quickbooks/objects/term.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/timeactivity.py` & `python-quickbooks-0.9.8/quickbooks/objects/timeactivity.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/trackingclass.py` & `python-quickbooks-0.9.8/quickbooks/objects/trackingclass.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/transfer.py` & `python-quickbooks-0.9.8/quickbooks/objects/transfer.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/vendor.py` & `python-quickbooks-0.9.8/quickbooks/objects/vendor.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/objects/vendorcredit.py` & `python-quickbooks-0.9.8/quickbooks/objects/vendorcredit.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/quickbooks/utils.py` & `python-quickbooks-0.9.8/quickbooks/utils.py`

 * *Files identical despite different names*

### Comparing `python-quickbooks-0.9.7/setup.py` & `python-quickbooks-0.9.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 def read(*parts):
     filename = os.path.join(os.path.dirname(__file__), *parts)
     with codecs.open(filename, encoding='utf-8') as fp:
         return fp.read()
 
 
-VERSION = (0, 9, 7)
+VERSION = (0, 9, 8)
 version = '.'.join(map(str, VERSION))
 
 setup(
     name='python-quickbooks',
     version=version,
     author='Edward Emanuel Jr.',
     author_email='edward.emanuel@gmail.com',
```

