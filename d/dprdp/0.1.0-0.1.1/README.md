# Comparing `tmp/dprdp-0.1.0.tar.gz` & `tmp/dprdp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dprdp-0.1.0.tar", last modified: Fri May 17 05:38:42 2024, max compression
+gzip compressed data, was "dist\dprdp-0.1.1.tar", last modified: Mon May 20 05:17:00 2024, max compression
```

## Comparing `dprdp-0.1.0.tar` & `dprdp-0.1.1.tar`

### file list

```diff
@@ -1,199 +1,200 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.956529 dprdp-0.1.0/
--rw-rw-rw-   0        0        0       73 2024-05-17 05:38:42.956529 dprdp-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.956529 dprdp-0.1.0/dprdp.egg-info/
--rw-rw-rw-   0        0        0       73 2024-05-17 05:38:42.000000 dprdp-0.1.0/dprdp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6663 2024-05-17 05:38:42.000000 dprdp-0.1.0/dprdp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 05:38:42.000000 dprdp-0.1.0/dprdp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-17 05:38:42.000000 dprdp-0.1.0/dprdp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.906847 dprdp-0.1.0/pypykatz/
--rw-rw-rw-   0        0        0       73 2024-05-17 05:34:15.000000 dprdp-0.1.0/pypykatz/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.906847 dprdp-0.1.0/pypykatz/alsadecryptor/
--rw-rw-rw-   0        0        0       82 2024-05-16 08:36:24.000000 dprdp-0.1.0/pypykatz/alsadecryptor/__init__.py
--rw-rw-rw-   0        0        0     1871 2024-05-16 08:36:24.000000 dprdp-0.1.0/pypykatz/alsadecryptor/asbmfile.py
--rw-rw-rw-   0        0        0      627 2024-05-16 08:35:15.000000 dprdp-0.1.0/pypykatz/alsadecryptor/lsa_decryptor.py
--rw-rw-rw-   0        0        0    14542 2024-05-16 08:35:15.000000 dprdp-0.1.0/pypykatz/alsadecryptor/lsa_decryptor_nt5.py
--rw-rw-rw-   0        0        0     4415 2024-05-17 03:54:20.000000 dprdp-0.1.0/pypykatz/alsadecryptor/lsa_decryptor_nt6.py
--rw-rw-rw-   0        0        0     3877 2024-05-16 08:34:21.000000 dprdp-0.1.0/pypykatz/alsadecryptor/lsa_template_nt5.py
--rw-rw-rw-   0        0        0    19362 2024-05-17 03:54:10.000000 dprdp-0.1.0/pypykatz/alsadecryptor/lsa_template_nt6.py
--rw-rw-rw-   0        0        0     1498 2024-05-16 08:34:21.000000 dprdp-0.1.0/pypykatz/alsadecryptor/lsa_templates.py
--rw-rw-rw-   0        0        0     6152 2024-05-16 08:33:15.000000 dprdp-0.1.0/pypykatz/alsadecryptor/package_commons.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.915848 dprdp-0.1.0/pypykatz/alsadecryptor/packages/
--rw-rw-rw-   0        0        0     1184 2024-05-16 08:36:24.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.915848 dprdp-0.1.0/pypykatz/alsadecryptor/packages/cloudap/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/cloudap/__init__.py
--rw-rw-rw-   0        0        0     3577 2024-05-16 08:46:33.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/cloudap/decryptor.py
--rw-rw-rw-   0        0        0     7530 2024-05-16 08:46:33.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/cloudap/templates.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.915848 dprdp-0.1.0/pypykatz/alsadecryptor/packages/credman/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/credman/__init__.py
--rw-rw-rw-   0        0        0    16437 2024-05-16 08:46:33.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/credman/templates.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.915848 dprdp-0.1.0/pypykatz/alsadecryptor/packages/dpapi/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/dpapi/__init__.py
--rw-rw-rw-   0        0        0     2570 2024-05-16 08:45:34.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/dpapi/decryptor.py
--rw-rw-rw-   0        0        0     4353 2024-05-16 08:45:34.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/dpapi/templates.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.915848 dprdp-0.1.0/pypykatz/alsadecryptor/packages/kerberos/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/kerberos/__init__.py
--rw-rw-rw-   0        0        0     7880 2024-05-16 08:44:57.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/kerberos/decryptor.py
--rw-rw-rw-   0        0        0    75450 2024-05-16 08:44:00.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/kerberos/templates.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.915848 dprdp-0.1.0/pypykatz/alsadecryptor/packages/livessp/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/livessp/__init__.py
--rw-rw-rw-   0        0        0     2815 2024-05-16 08:40:58.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/livessp/decryptor.py
--rw-rw-rw-   0        0        0     3461 2024-05-16 08:40:38.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/livessp/templates.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.922351 dprdp-0.1.0/pypykatz/alsadecryptor/packages/msv/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/msv/__init__.py
--rw-rw-rw-   0        0        0    18571 2024-05-16 08:40:06.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/msv/decryptor.py
--rw-rw-rw-   0        0        0    40604 2024-05-16 08:38:40.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/msv/templates.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.922351 dprdp-0.1.0/pypykatz/alsadecryptor/packages/ssp/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/ssp/__init__.py
--rw-rw-rw-   0        0        0     2932 2024-05-16 08:37:52.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/ssp/decryptor.py
--rw-rw-rw-   0        0        0     3192 2024-05-16 08:37:52.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/ssp/templates.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.922351 dprdp-0.1.0/pypykatz/alsadecryptor/packages/tspkg/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/tspkg/__init__.py
--rw-rw-rw-   0        0        0     3560 2024-05-16 08:37:06.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/tspkg/decryptor.py
--rw-rw-rw-   0        0        0     5566 2024-05-16 08:37:06.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/tspkg/templates.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.922351 dprdp-0.1.0/pypykatz/alsadecryptor/packages/wdigest/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/wdigest/__init__.py
--rw-rw-rw-   0        0        0     3176 2024-05-16 08:36:24.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/wdigest/decryptor.py
--rw-rw-rw-   0        0        0     5628 2024-05-16 08:36:24.000000 dprdp-0.1.0/pypykatz/alsadecryptor/packages/wdigest/templates.py
--rw-rw-rw-   0        0        0    28639 2024-05-16 08:32:21.000000 dprdp-0.1.0/pypykatz/alsadecryptor/win_datatypes.py
--rw-rw-rw-   0        0        0    13052 2024-05-16 09:23:53.000000 dprdp-0.1.0/pypykatz/apypykatz.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.922351 dprdp-0.1.0/pypykatz/commons/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/commons/__init__.py
--rw-rw-rw-   0        0        0    12434 2024-05-16 08:05:42.000000 dprdp-0.1.0/pypykatz/commons/common.py
--rw-rw-rw-   0        0        0      776 2024-05-16 08:03:20.000000 dprdp-0.1.0/pypykatz/commons/filetime.py
--rw-rw-rw-   0        0        0     9436 2024-05-16 08:02:44.000000 dprdp-0.1.0/pypykatz/commons/kerberosticket.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.922351 dprdp-0.1.0/pypykatz/commons/readers/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/commons/readers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.922351 dprdp-0.1.0/pypykatz/commons/readers/local/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/commons/readers/local/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.922351 dprdp-0.1.0/pypykatz/commons/readers/local/common/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/commons/readers/local/common/__init__.py
--rw-rw-rw-   0        0        0    91352 2024-05-16 08:29:35.000000 dprdp-0.1.0/pypykatz/commons/readers/local/common/advapi32.py
--rw-rw-rw-   0        0        0    13176 2024-05-16 08:29:21.000000 dprdp-0.1.0/pypykatz/commons/readers/local/common/defines.py
--rw-rw-rw-   0        0        0      608 2024-05-16 08:29:21.000000 dprdp-0.1.0/pypykatz/commons/readers/local/common/fileinfo.py
--rw-rw-rw-   0        0        0    15230 2024-05-16 08:28:56.000000 dprdp-0.1.0/pypykatz/commons/readers/local/common/kernel32.py
--rw-rw-rw-   0        0        0     6461 2024-05-16 08:28:40.000000 dprdp-0.1.0/pypykatz/commons/readers/local/common/live_reader_ctypes.py
--rw-rw-rw-   0        0        0      927 2024-05-16 08:28:40.000000 dprdp-0.1.0/pypykatz/commons/readers/local/common/privileges.py
--rw-rw-rw-   0        0        0     2799 2024-05-16 08:27:42.000000 dprdp-0.1.0/pypykatz/commons/readers/local/common/privileges_types.py
--rw-rw-rw-   0        0        0     9808 2024-05-16 08:25:50.000000 dprdp-0.1.0/pypykatz/commons/readers/local/common/psapi.py
--rw-rw-rw-   0        0        0    22048 2024-05-16 08:25:25.000000 dprdp-0.1.0/pypykatz/commons/readers/local/common/version.py
--rw-rw-rw-   0        0        0     1828 2024-05-16 08:25:25.000000 dprdp-0.1.0/pypykatz/commons/readers/local/common/winreg.py
--rw-rw-rw-   0        0        0    13003 2024-05-16 08:24:02.000000 dprdp-0.1.0/pypykatz/commons/readers/local/live_reader.py
--rw-rw-rw-   0        0        0    12828 2024-05-16 08:23:11.000000 dprdp-0.1.0/pypykatz/commons/readers/local/process.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.922351 dprdp-0.1.0/pypykatz/commons/readers/registry/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/commons/readers/registry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.922351 dprdp-0.1.0/pypykatz/commons/readers/registry/live/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/commons/readers/registry/live/__init__.py
--rw-rw-rw-   0        0        0     2059 2024-05-17 03:52:15.000000 dprdp-0.1.0/pypykatz/commons/readers/registry/live/reader.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.922351 dprdp-0.1.0/pypykatz/commons/readers/rekall/
--rw-rw-rw-   0        0        0      121 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/commons/readers/rekall/__init__.py
--rw-rw-rw-   0        0        0     7222 2024-05-16 08:22:28.000000 dprdp-0.1.0/pypykatz/commons/readers/rekall/rekallreader.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.922351 dprdp-0.1.0/pypykatz/commons/readers/volatility3/
--rw-rw-rw-   0        0        0      494 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/commons/readers/volatility3/__init__.py
--rw-rw-rw-   0        0        0     8396 2024-05-16 08:21:45.000000 dprdp-0.1.0/pypykatz/commons/readers/volatility3/volreader.py
--rw-rw-rw-   0        0        0     7141 2024-05-16 08:01:58.000000 dprdp-0.1.0/pypykatz/commons/win_datatypes.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.937976 dprdp-0.1.0/pypykatz/commons/winapi/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/commons/winapi/__init__.py
--rw-rw-rw-   0        0        0     6802 2024-05-16 08:08:26.000000 dprdp-0.1.0/pypykatz/commons/winapi/constants.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.939520 dprdp-0.1.0/pypykatz/commons/winapi/local/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/commons/winapi/local/__init__.py
--rw-rw-rw-   0        0        0     3778 2024-05-16 08:10:08.000000 dprdp-0.1.0/pypykatz/commons/winapi/local/advapi32.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.939520 dprdp-0.1.0/pypykatz/commons/winapi/local/function_defs/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/commons/winapi/local/function_defs/__init__.py
--rw-rw-rw-   0        0        0    92856 2024-05-16 08:21:45.000000 dprdp-0.1.0/pypykatz/commons/winapi/local/function_defs/advapi32.py
--rw-rw-rw-   0        0        0    13268 2024-05-16 08:19:44.000000 dprdp-0.1.0/pypykatz/commons/winapi/local/function_defs/defines.py
--rw-rw-rw-   0        0        0    15264 2024-05-16 08:17:29.000000 dprdp-0.1.0/pypykatz/commons/winapi/local/function_defs/kernel32.py
--rw-rw-rw-   0        0        0     3558 2024-05-16 08:14:50.000000 dprdp-0.1.0/pypykatz/commons/winapi/local/function_defs/live_reader_ctypes.py
--rw-rw-rw-   0        0        0     5707 2024-05-16 08:10:44.000000 dprdp-0.1.0/pypykatz/commons/winapi/local/function_defs/ntdll.py
--rw-rw-rw-   0        0        0     9796 2024-05-16 08:10:08.000000 dprdp-0.1.0/pypykatz/commons/winapi/local/function_defs/psapi.py
--rw-rw-rw-   0        0        0      496 2024-05-16 08:10:08.000000 dprdp-0.1.0/pypykatz/commons/winapi/local/kernel32.py
--rw-rw-rw-   0        0        0      397 2024-05-16 08:10:08.000000 dprdp-0.1.0/pypykatz/commons/winapi/local/localwindowsapi.py
--rw-rw-rw-   0        0        0      318 2024-05-16 08:10:08.000000 dprdp-0.1.0/pypykatz/commons/winapi/local/ntdll.py
--rw-rw-rw-   0        0        0      203 2024-05-16 08:10:08.000000 dprdp-0.1.0/pypykatz/commons/winapi/local/psapi.py
--rw-rw-rw-   0        0        0     5284 2024-05-16 08:07:40.000000 dprdp-0.1.0/pypykatz/commons/winapi/processmanipulator.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.939520 dprdp-0.1.0/pypykatz/dpapi/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/dpapi/__init__.py
--rw-rw-rw-   0        0        0     5983 2024-05-16 07:44:29.000000 dprdp-0.1.0/pypykatz/dpapi/constants.py
--rw-rw-rw-   0        0        0    31069 2024-05-16 07:43:23.000000 dprdp-0.1.0/pypykatz/dpapi/dpapi.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.939520 dprdp-0.1.0/pypykatz/dpapi/finders/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/dpapi/finders/__init__.py
--rw-rw-rw-   0        0        0     1749 2024-05-16 07:50:11.000000 dprdp-0.1.0/pypykatz/dpapi/finders/cryptokeys.py
--rw-rw-rw-   0        0        0     2814 2024-05-16 07:49:48.000000 dprdp-0.1.0/pypykatz/dpapi/finders/ngc.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.939520 dprdp-0.1.0/pypykatz/dpapi/functiondefs/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/dpapi/functiondefs/__init__.py
--rw-rw-rw-   0        0        0     2043 2024-05-17 03:52:09.000000 dprdp-0.1.0/pypykatz/dpapi/functiondefs/dpapi.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.947025 dprdp-0.1.0/pypykatz/dpapi/structures/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/dpapi/structures/__init__.py
--rw-rw-rw-   0        0        0     6479 2024-05-16 07:49:48.000000 dprdp-0.1.0/pypykatz/dpapi/structures/blob.py
--rw-rw-rw-   0        0        0     7435 2024-05-16 07:46:28.000000 dprdp-0.1.0/pypykatz/dpapi/structures/credentialfile.py
--rw-rw-rw-   0        0        0     7591 2024-05-16 07:46:28.000000 dprdp-0.1.0/pypykatz/dpapi/structures/masterkeyfile.py
--rw-rw-rw-   0        0        0      853 2024-05-16 07:45:14.000000 dprdp-0.1.0/pypykatz/dpapi/structures/system.py
--rw-rw-rw-   0        0        0    10986 2024-05-16 07:45:14.000000 dprdp-0.1.0/pypykatz/dpapi/structures/vault.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.947025 dprdp-0.1.0/pypykatz/lsadecryptor/
--rw-rw-rw-   0        0        0       82 2024-05-16 07:03:56.000000 dprdp-0.1.0/pypykatz/lsadecryptor/__init__.py
--rw-rw-rw-   0        0        0      556 2024-05-16 07:03:56.000000 dprdp-0.1.0/pypykatz/lsadecryptor/lsa_decryptor.py
--rw-rw-rw-   0        0        0    14260 2024-05-16 07:00:39.000000 dprdp-0.1.0/pypykatz/lsadecryptor/lsa_decryptor_nt5.py
--rw-rw-rw-   0        0        0     4510 2024-05-16 07:00:39.000000 dprdp-0.1.0/pypykatz/lsadecryptor/lsa_decryptor_nt6.py
--rw-rw-rw-   0        0        0     3293 2024-05-16 06:55:25.000000 dprdp-0.1.0/pypykatz/lsadecryptor/lsa_template_nt5.py
--rw-rw-rw-   0        0        0    17671 2024-05-16 06:54:31.000000 dprdp-0.1.0/pypykatz/lsadecryptor/lsa_template_nt6.py
--rw-rw-rw-   0        0        0     1496 2024-05-16 06:54:31.000000 dprdp-0.1.0/pypykatz/lsadecryptor/lsa_templates.py
--rw-rw-rw-   0        0        0     6257 2024-05-16 06:52:49.000000 dprdp-0.1.0/pypykatz/lsadecryptor/package_commons.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.947025 dprdp-0.1.0/pypykatz/lsadecryptor/packages/
--rw-rw-rw-   0        0        0     1184 2024-05-16 07:03:56.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.954028 dprdp-0.1.0/pypykatz/lsadecryptor/packages/cloudap/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/cloudap/__init__.py
--rw-rw-rw-   0        0        0     2964 2024-05-16 07:30:10.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/cloudap/decryptor.py
--rw-rw-rw-   0        0        0     3919 2024-05-17 03:54:51.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/cloudap/templates.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.954028 dprdp-0.1.0/pypykatz/lsadecryptor/packages/credman/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/credman/__init__.py
--rw-rw-rw-   0        0        0     9241 2024-05-16 07:28:40.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/credman/templates.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.956529 dprdp-0.1.0/pypykatz/lsadecryptor/packages/dpapi/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/dpapi/__init__.py
--rw-rw-rw-   0        0        0     2504 2024-05-16 07:28:40.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/dpapi/decryptor.py
--rw-rw-rw-   0        0        0     3838 2024-05-16 07:24:57.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/dpapi/templates.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.956529 dprdp-0.1.0/pypykatz/lsadecryptor/packages/kerberos/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/kerberos/__init__.py
--rw-rw-rw-   0        0        0     7736 2024-05-16 07:23:35.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/kerberos/decryptor.py
--rw-rw-rw-   0        0        0    46344 2024-05-16 07:19:51.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/kerberos/templates.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.956529 dprdp-0.1.0/pypykatz/lsadecryptor/packages/livessp/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/livessp/__init__.py
--rw-rw-rw-   0        0        0     2716 2024-05-16 07:17:21.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/livessp/decryptor.py
--rw-rw-rw-   0        0        0     2261 2024-05-16 07:17:21.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/livessp/templates.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.956529 dprdp-0.1.0/pypykatz/lsadecryptor/packages/msv/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/msv/__init__.py
--rw-rw-rw-   0        0        0    18147 2024-05-16 07:12:26.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/msv/decryptor.py
--rw-rw-rw-   0        0        0    28797 2024-05-16 07:07:25.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/msv/templates.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.956529 dprdp-0.1.0/pypykatz/lsadecryptor/packages/ssp/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/ssp/__init__.py
--rw-rw-rw-   0        0        0     2812 2024-05-16 07:07:25.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/ssp/decryptor.py
--rw-rw-rw-   0        0        0     2536 2024-05-16 07:07:25.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/ssp/templates.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.956529 dprdp-0.1.0/pypykatz/lsadecryptor/packages/tspkg/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/tspkg/__init__.py
--rw-rw-rw-   0        0        0     3403 2024-05-16 07:07:25.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/tspkg/decryptor.py
--rw-rw-rw-   0        0        0     3998 2024-05-16 07:03:56.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/tspkg/templates.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.956529 dprdp-0.1.0/pypykatz/lsadecryptor/packages/wdigest/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/wdigest/__init__.py
--rw-rw-rw-   0        0        0     2982 2024-05-16 07:03:56.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/wdigest/decryptor.py
--rw-rw-rw-   0        0        0     5038 2024-05-16 07:03:56.000000 dprdp-0.1.0/pypykatz/lsadecryptor/packages/wdigest/templates.py
--rw-rw-rw-   0        0        0    11729 2024-05-16 09:21:28.000000 dprdp-0.1.0/pypykatz/pypykatz.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.956529 dprdp-0.1.0/pypykatz/registry/
--rw-rw-rw-   0        0        0       54 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/registry/__init__.py
--rw-rw-rw-   0        0        0     3137 2024-05-16 06:29:08.000000 dprdp-0.1.0/pypykatz/registry/live_parser.py
--rw-rw-rw-   0        0        0     8325 2024-05-16 06:37:00.000000 dprdp-0.1.0/pypykatz/registry/offline_parser.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.956529 dprdp-0.1.0/pypykatz/registry/sam/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/registry/sam/__init__.py
--rw-rw-rw-   0        0        0      501 2024-05-16 06:44:14.000000 dprdp-0.1.0/pypykatz/registry/sam/common.py
--rw-rw-rw-   0        0        0     5798 2024-05-16 06:44:01.000000 dprdp-0.1.0/pypykatz/registry/sam/sam.py
--rw-rw-rw-   0        0        0    14379 2024-05-16 06:42:05.000000 dprdp-0.1.0/pypykatz/registry/sam/structures.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.956529 dprdp-0.1.0/pypykatz/registry/security/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/registry/security/__init__.py
--rw-rw-rw-   0        0        0     7299 2024-05-16 06:40:13.000000 dprdp-0.1.0/pypykatz/registry/security/common.py
--rw-rw-rw-   0        0        0    10347 2024-05-16 06:38:33.000000 dprdp-0.1.0/pypykatz/registry/security/security.py
--rw-rw-rw-   0        0        0     5707 2024-05-16 06:34:41.000000 dprdp-0.1.0/pypykatz/registry/security/structures.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.956529 dprdp-0.1.0/pypykatz/registry/software/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/registry/software/__init__.py
--rw-rw-rw-   0        0        0     2192 2024-05-16 06:33:04.000000 dprdp-0.1.0/pypykatz/registry/software/software.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:38:42.956529 dprdp-0.1.0/pypykatz/registry/system/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.0/pypykatz/registry/system/__init__.py
--rw-rw-rw-   0        0        0     2133 2024-05-16 06:33:04.000000 dprdp-0.1.0/pypykatz/registry/system/system.py
--rw-rw-rw-   0        0        0       42 2024-05-17 05:38:42.956529 dprdp-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      220 2024-05-17 04:50:24.000000 dprdp-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.927685 dprdp-0.1.1/
+-rw-rw-rw-   0        0        0       73 2024-05-20 05:17:00.927685 dprdp-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.871739 dprdp-0.1.1/dprdp.egg-info/
+-rw-rw-rw-   0        0        0       73 2024-05-20 05:17:00.000000 dprdp-0.1.1/dprdp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6691 2024-05-20 05:17:00.000000 dprdp-0.1.1/dprdp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 05:17:00.000000 dprdp-0.1.1/dprdp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2024-05-20 05:17:00.000000 dprdp-0.1.1/dprdp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-20 05:17:00.000000 dprdp-0.1.1/dprdp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.872740 dprdp-0.1.1/pypykatz/
+-rw-rw-rw-   0        0        0       73 2024-05-17 05:34:15.000000 dprdp-0.1.1/pypykatz/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.876231 dprdp-0.1.1/pypykatz/alsadecryptor/
+-rw-rw-rw-   0        0        0       82 2024-05-16 08:36:24.000000 dprdp-0.1.1/pypykatz/alsadecryptor/__init__.py
+-rw-rw-rw-   0        0        0     1871 2024-05-16 08:36:24.000000 dprdp-0.1.1/pypykatz/alsadecryptor/asbmfile.py
+-rw-rw-rw-   0        0        0      627 2024-05-16 08:35:15.000000 dprdp-0.1.1/pypykatz/alsadecryptor/lsa_decryptor.py
+-rw-rw-rw-   0        0        0    14542 2024-05-16 08:35:15.000000 dprdp-0.1.1/pypykatz/alsadecryptor/lsa_decryptor_nt5.py
+-rw-rw-rw-   0        0        0     4415 2024-05-17 03:54:20.000000 dprdp-0.1.1/pypykatz/alsadecryptor/lsa_decryptor_nt6.py
+-rw-rw-rw-   0        0        0     3877 2024-05-16 08:34:21.000000 dprdp-0.1.1/pypykatz/alsadecryptor/lsa_template_nt5.py
+-rw-rw-rw-   0        0        0    19362 2024-05-17 03:54:10.000000 dprdp-0.1.1/pypykatz/alsadecryptor/lsa_template_nt6.py
+-rw-rw-rw-   0        0        0     1498 2024-05-16 08:34:21.000000 dprdp-0.1.1/pypykatz/alsadecryptor/lsa_templates.py
+-rw-rw-rw-   0        0        0     6152 2024-05-16 08:33:15.000000 dprdp-0.1.1/pypykatz/alsadecryptor/package_commons.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.877228 dprdp-0.1.1/pypykatz/alsadecryptor/packages/
+-rw-rw-rw-   0        0        0     1184 2024-05-16 08:36:24.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.878225 dprdp-0.1.1/pypykatz/alsadecryptor/packages/cloudap/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/cloudap/__init__.py
+-rw-rw-rw-   0        0        0     3577 2024-05-16 08:46:33.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/cloudap/decryptor.py
+-rw-rw-rw-   0        0        0     7530 2024-05-16 08:46:33.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/cloudap/templates.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.878225 dprdp-0.1.1/pypykatz/alsadecryptor/packages/credman/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/credman/__init__.py
+-rw-rw-rw-   0        0        0    16437 2024-05-16 08:46:33.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/credman/templates.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.880218 dprdp-0.1.1/pypykatz/alsadecryptor/packages/dpapi/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/dpapi/__init__.py
+-rw-rw-rw-   0        0        0     2570 2024-05-16 08:45:34.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/dpapi/decryptor.py
+-rw-rw-rw-   0        0        0     4353 2024-05-16 08:45:34.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/dpapi/templates.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.881215 dprdp-0.1.1/pypykatz/alsadecryptor/packages/kerberos/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/kerberos/__init__.py
+-rw-rw-rw-   0        0        0     7880 2024-05-16 08:44:57.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/kerberos/decryptor.py
+-rw-rw-rw-   0        0        0    75450 2024-05-16 08:44:00.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/kerberos/templates.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.882211 dprdp-0.1.1/pypykatz/alsadecryptor/packages/livessp/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/livessp/__init__.py
+-rw-rw-rw-   0        0        0     2815 2024-05-16 08:40:58.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/livessp/decryptor.py
+-rw-rw-rw-   0        0        0     3461 2024-05-16 08:40:38.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/livessp/templates.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.884205 dprdp-0.1.1/pypykatz/alsadecryptor/packages/msv/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/msv/__init__.py
+-rw-rw-rw-   0        0        0    18571 2024-05-16 08:40:06.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/msv/decryptor.py
+-rw-rw-rw-   0        0        0    40604 2024-05-16 08:38:40.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/msv/templates.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.884706 dprdp-0.1.1/pypykatz/alsadecryptor/packages/ssp/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/ssp/__init__.py
+-rw-rw-rw-   0        0        0     2932 2024-05-16 08:37:52.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/ssp/decryptor.py
+-rw-rw-rw-   0        0        0     3192 2024-05-16 08:37:52.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/ssp/templates.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.885708 dprdp-0.1.1/pypykatz/alsadecryptor/packages/tspkg/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/tspkg/__init__.py
+-rw-rw-rw-   0        0        0     3560 2024-05-16 08:37:06.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/tspkg/decryptor.py
+-rw-rw-rw-   0        0        0     5566 2024-05-16 08:37:06.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/tspkg/templates.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.886704 dprdp-0.1.1/pypykatz/alsadecryptor/packages/wdigest/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/wdigest/__init__.py
+-rw-rw-rw-   0        0        0     3176 2024-05-16 08:36:24.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/wdigest/decryptor.py
+-rw-rw-rw-   0        0        0     5628 2024-05-16 08:36:24.000000 dprdp-0.1.1/pypykatz/alsadecryptor/packages/wdigest/templates.py
+-rw-rw-rw-   0        0        0    28639 2024-05-16 08:32:21.000000 dprdp-0.1.1/pypykatz/alsadecryptor/win_datatypes.py
+-rw-rw-rw-   0        0        0    13052 2024-05-16 09:23:53.000000 dprdp-0.1.1/pypykatz/apypykatz.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.889202 dprdp-0.1.1/pypykatz/commons/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/commons/__init__.py
+-rw-rw-rw-   0        0        0    12434 2024-05-16 08:05:42.000000 dprdp-0.1.1/pypykatz/commons/common.py
+-rw-rw-rw-   0        0        0      776 2024-05-16 08:03:20.000000 dprdp-0.1.1/pypykatz/commons/filetime.py
+-rw-rw-rw-   0        0        0     9436 2024-05-16 08:02:44.000000 dprdp-0.1.1/pypykatz/commons/kerberosticket.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.890200 dprdp-0.1.1/pypykatz/commons/readers/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/commons/readers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.891196 dprdp-0.1.1/pypykatz/commons/readers/local/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/commons/readers/local/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.894762 dprdp-0.1.1/pypykatz/commons/readers/local/common/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/commons/readers/local/common/__init__.py
+-rw-rw-rw-   0        0        0    91352 2024-05-16 08:29:35.000000 dprdp-0.1.1/pypykatz/commons/readers/local/common/advapi32.py
+-rw-rw-rw-   0        0        0    13176 2024-05-16 08:29:21.000000 dprdp-0.1.1/pypykatz/commons/readers/local/common/defines.py
+-rw-rw-rw-   0        0        0      608 2024-05-16 08:29:21.000000 dprdp-0.1.1/pypykatz/commons/readers/local/common/fileinfo.py
+-rw-rw-rw-   0        0        0    15230 2024-05-16 08:28:56.000000 dprdp-0.1.1/pypykatz/commons/readers/local/common/kernel32.py
+-rw-rw-rw-   0        0        0     6461 2024-05-16 08:28:40.000000 dprdp-0.1.1/pypykatz/commons/readers/local/common/live_reader_ctypes.py
+-rw-rw-rw-   0        0        0      927 2024-05-16 08:28:40.000000 dprdp-0.1.1/pypykatz/commons/readers/local/common/privileges.py
+-rw-rw-rw-   0        0        0     2799 2024-05-16 08:27:42.000000 dprdp-0.1.1/pypykatz/commons/readers/local/common/privileges_types.py
+-rw-rw-rw-   0        0        0     9808 2024-05-16 08:25:50.000000 dprdp-0.1.1/pypykatz/commons/readers/local/common/psapi.py
+-rw-rw-rw-   0        0        0    22048 2024-05-16 08:25:25.000000 dprdp-0.1.1/pypykatz/commons/readers/local/common/version.py
+-rw-rw-rw-   0        0        0     1828 2024-05-16 08:25:25.000000 dprdp-0.1.1/pypykatz/commons/readers/local/common/winreg.py
+-rw-rw-rw-   0        0        0    13003 2024-05-16 08:24:02.000000 dprdp-0.1.1/pypykatz/commons/readers/local/live_reader.py
+-rw-rw-rw-   0        0        0    12828 2024-05-16 08:23:11.000000 dprdp-0.1.1/pypykatz/commons/readers/local/process.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.895763 dprdp-0.1.1/pypykatz/commons/readers/registry/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/commons/readers/registry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.896759 dprdp-0.1.1/pypykatz/commons/readers/registry/live/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/commons/readers/registry/live/__init__.py
+-rw-rw-rw-   0        0        0     2059 2024-05-17 03:52:15.000000 dprdp-0.1.1/pypykatz/commons/readers/registry/live/reader.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.896759 dprdp-0.1.1/pypykatz/commons/readers/rekall/
+-rw-rw-rw-   0        0        0      121 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/commons/readers/rekall/__init__.py
+-rw-rw-rw-   0        0        0     7222 2024-05-16 08:22:28.000000 dprdp-0.1.1/pypykatz/commons/readers/rekall/rekallreader.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.897756 dprdp-0.1.1/pypykatz/commons/readers/volatility3/
+-rw-rw-rw-   0        0        0      494 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/commons/readers/volatility3/__init__.py
+-rw-rw-rw-   0        0        0     8396 2024-05-16 08:21:45.000000 dprdp-0.1.1/pypykatz/commons/readers/volatility3/volreader.py
+-rw-rw-rw-   0        0        0     7141 2024-05-16 08:01:58.000000 dprdp-0.1.1/pypykatz/commons/win_datatypes.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.898753 dprdp-0.1.1/pypykatz/commons/winapi/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/commons/winapi/__init__.py
+-rw-rw-rw-   0        0        0     6802 2024-05-16 08:08:26.000000 dprdp-0.1.1/pypykatz/commons/winapi/constants.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.900746 dprdp-0.1.1/pypykatz/commons/winapi/local/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/commons/winapi/local/__init__.py
+-rw-rw-rw-   0        0        0     3778 2024-05-16 08:10:08.000000 dprdp-0.1.1/pypykatz/commons/winapi/local/advapi32.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.903736 dprdp-0.1.1/pypykatz/commons/winapi/local/function_defs/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/commons/winapi/local/function_defs/__init__.py
+-rw-rw-rw-   0        0        0    92856 2024-05-16 08:21:45.000000 dprdp-0.1.1/pypykatz/commons/winapi/local/function_defs/advapi32.py
+-rw-rw-rw-   0        0        0    13268 2024-05-16 08:19:44.000000 dprdp-0.1.1/pypykatz/commons/winapi/local/function_defs/defines.py
+-rw-rw-rw-   0        0        0    15264 2024-05-16 08:17:29.000000 dprdp-0.1.1/pypykatz/commons/winapi/local/function_defs/kernel32.py
+-rw-rw-rw-   0        0        0     3558 2024-05-16 08:14:50.000000 dprdp-0.1.1/pypykatz/commons/winapi/local/function_defs/live_reader_ctypes.py
+-rw-rw-rw-   0        0        0     5707 2024-05-16 08:10:44.000000 dprdp-0.1.1/pypykatz/commons/winapi/local/function_defs/ntdll.py
+-rw-rw-rw-   0        0        0     9796 2024-05-16 08:10:08.000000 dprdp-0.1.1/pypykatz/commons/winapi/local/function_defs/psapi.py
+-rw-rw-rw-   0        0        0      496 2024-05-16 08:10:08.000000 dprdp-0.1.1/pypykatz/commons/winapi/local/kernel32.py
+-rw-rw-rw-   0        0        0      397 2024-05-16 08:10:08.000000 dprdp-0.1.1/pypykatz/commons/winapi/local/localwindowsapi.py
+-rw-rw-rw-   0        0        0      318 2024-05-16 08:10:08.000000 dprdp-0.1.1/pypykatz/commons/winapi/local/ntdll.py
+-rw-rw-rw-   0        0        0      203 2024-05-16 08:10:08.000000 dprdp-0.1.1/pypykatz/commons/winapi/local/psapi.py
+-rw-rw-rw-   0        0        0     5284 2024-05-16 08:07:40.000000 dprdp-0.1.1/pypykatz/commons/winapi/processmanipulator.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.904732 dprdp-0.1.1/pypykatz/dpapi/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/dpapi/__init__.py
+-rw-rw-rw-   0        0        0     5983 2024-05-16 07:44:29.000000 dprdp-0.1.1/pypykatz/dpapi/constants.py
+-rw-rw-rw-   0        0        0    31069 2024-05-16 07:43:23.000000 dprdp-0.1.1/pypykatz/dpapi/dpapi.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.904732 dprdp-0.1.1/pypykatz/dpapi/finders/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/dpapi/finders/__init__.py
+-rw-rw-rw-   0        0        0     1749 2024-05-16 07:50:11.000000 dprdp-0.1.1/pypykatz/dpapi/finders/cryptokeys.py
+-rw-rw-rw-   0        0        0     2814 2024-05-16 07:49:48.000000 dprdp-0.1.1/pypykatz/dpapi/finders/ngc.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.906233 dprdp-0.1.1/pypykatz/dpapi/functiondefs/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/dpapi/functiondefs/__init__.py
+-rw-rw-rw-   0        0        0     2043 2024-05-17 03:52:09.000000 dprdp-0.1.1/pypykatz/dpapi/functiondefs/dpapi.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.908231 dprdp-0.1.1/pypykatz/dpapi/structures/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/dpapi/structures/__init__.py
+-rw-rw-rw-   0        0        0     6479 2024-05-16 07:49:48.000000 dprdp-0.1.1/pypykatz/dpapi/structures/blob.py
+-rw-rw-rw-   0        0        0     7435 2024-05-16 07:46:28.000000 dprdp-0.1.1/pypykatz/dpapi/structures/credentialfile.py
+-rw-rw-rw-   0        0        0     7591 2024-05-16 07:46:28.000000 dprdp-0.1.1/pypykatz/dpapi/structures/masterkeyfile.py
+-rw-rw-rw-   0        0        0      853 2024-05-16 07:45:14.000000 dprdp-0.1.1/pypykatz/dpapi/structures/system.py
+-rw-rw-rw-   0        0        0    10986 2024-05-16 07:45:14.000000 dprdp-0.1.1/pypykatz/dpapi/structures/vault.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.911222 dprdp-0.1.1/pypykatz/lsadecryptor/
+-rw-rw-rw-   0        0        0       82 2024-05-16 07:03:56.000000 dprdp-0.1.1/pypykatz/lsadecryptor/__init__.py
+-rw-rw-rw-   0        0        0      556 2024-05-16 07:03:56.000000 dprdp-0.1.1/pypykatz/lsadecryptor/lsa_decryptor.py
+-rw-rw-rw-   0        0        0    14260 2024-05-16 07:00:39.000000 dprdp-0.1.1/pypykatz/lsadecryptor/lsa_decryptor_nt5.py
+-rw-rw-rw-   0        0        0     4510 2024-05-16 07:00:39.000000 dprdp-0.1.1/pypykatz/lsadecryptor/lsa_decryptor_nt6.py
+-rw-rw-rw-   0        0        0     3293 2024-05-16 06:55:25.000000 dprdp-0.1.1/pypykatz/lsadecryptor/lsa_template_nt5.py
+-rw-rw-rw-   0        0        0    17671 2024-05-16 06:54:31.000000 dprdp-0.1.1/pypykatz/lsadecryptor/lsa_template_nt6.py
+-rw-rw-rw-   0        0        0     1496 2024-05-16 06:54:31.000000 dprdp-0.1.1/pypykatz/lsadecryptor/lsa_templates.py
+-rw-rw-rw-   0        0        0     6257 2024-05-16 06:52:49.000000 dprdp-0.1.1/pypykatz/lsadecryptor/package_commons.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.912218 dprdp-0.1.1/pypykatz/lsadecryptor/packages/
+-rw-rw-rw-   0        0        0     1184 2024-05-16 07:03:56.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.913215 dprdp-0.1.1/pypykatz/lsadecryptor/packages/cloudap/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/cloudap/__init__.py
+-rw-rw-rw-   0        0        0     2964 2024-05-16 07:30:10.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/cloudap/decryptor.py
+-rw-rw-rw-   0        0        0     3919 2024-05-17 03:54:51.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/cloudap/templates.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.913215 dprdp-0.1.1/pypykatz/lsadecryptor/packages/credman/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/credman/__init__.py
+-rw-rw-rw-   0        0        0     9241 2024-05-16 07:28:40.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/credman/templates.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.914716 dprdp-0.1.1/pypykatz/lsadecryptor/packages/dpapi/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/dpapi/__init__.py
+-rw-rw-rw-   0        0        0     2504 2024-05-16 07:28:40.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/dpapi/decryptor.py
+-rw-rw-rw-   0        0        0     3838 2024-05-16 07:24:57.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/dpapi/templates.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.916214 dprdp-0.1.1/pypykatz/lsadecryptor/packages/kerberos/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/kerberos/__init__.py
+-rw-rw-rw-   0        0        0     7736 2024-05-16 07:23:35.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/kerberos/decryptor.py
+-rw-rw-rw-   0        0        0    46344 2024-05-16 07:19:51.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/kerberos/templates.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.917212 dprdp-0.1.1/pypykatz/lsadecryptor/packages/livessp/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/livessp/__init__.py
+-rw-rw-rw-   0        0        0     2716 2024-05-16 07:17:21.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/livessp/decryptor.py
+-rw-rw-rw-   0        0        0     2261 2024-05-16 07:17:21.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/livessp/templates.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.918209 dprdp-0.1.1/pypykatz/lsadecryptor/packages/msv/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/msv/__init__.py
+-rw-rw-rw-   0        0        0    18147 2024-05-16 07:12:26.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/msv/decryptor.py
+-rw-rw-rw-   0        0        0    28797 2024-05-16 07:07:25.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/msv/templates.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.919205 dprdp-0.1.1/pypykatz/lsadecryptor/packages/ssp/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/ssp/__init__.py
+-rw-rw-rw-   0        0        0     2812 2024-05-16 07:07:25.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/ssp/decryptor.py
+-rw-rw-rw-   0        0        0     2536 2024-05-16 07:07:25.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/ssp/templates.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.920202 dprdp-0.1.1/pypykatz/lsadecryptor/packages/tspkg/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/tspkg/__init__.py
+-rw-rw-rw-   0        0        0     3403 2024-05-16 07:07:25.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/tspkg/decryptor.py
+-rw-rw-rw-   0        0        0     3998 2024-05-16 07:03:56.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/tspkg/templates.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.921198 dprdp-0.1.1/pypykatz/lsadecryptor/packages/wdigest/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/wdigest/__init__.py
+-rw-rw-rw-   0        0        0     2982 2024-05-16 07:03:56.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/wdigest/decryptor.py
+-rw-rw-rw-   0        0        0     5038 2024-05-16 07:03:56.000000 dprdp-0.1.1/pypykatz/lsadecryptor/packages/wdigest/templates.py
+-rw-rw-rw-   0        0        0    11729 2024-05-16 09:21:28.000000 dprdp-0.1.1/pypykatz/pypykatz.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.922195 dprdp-0.1.1/pypykatz/registry/
+-rw-rw-rw-   0        0        0       54 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/registry/__init__.py
+-rw-rw-rw-   0        0        0     3137 2024-05-16 06:29:08.000000 dprdp-0.1.1/pypykatz/registry/live_parser.py
+-rw-rw-rw-   0        0        0     8325 2024-05-16 06:37:00.000000 dprdp-0.1.1/pypykatz/registry/offline_parser.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.924694 dprdp-0.1.1/pypykatz/registry/sam/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/registry/sam/__init__.py
+-rw-rw-rw-   0        0        0      501 2024-05-16 06:44:14.000000 dprdp-0.1.1/pypykatz/registry/sam/common.py
+-rw-rw-rw-   0        0        0     5798 2024-05-16 06:44:01.000000 dprdp-0.1.1/pypykatz/registry/sam/sam.py
+-rw-rw-rw-   0        0        0    14379 2024-05-16 06:42:05.000000 dprdp-0.1.1/pypykatz/registry/sam/structures.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.925691 dprdp-0.1.1/pypykatz/registry/security/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/registry/security/__init__.py
+-rw-rw-rw-   0        0        0     7299 2024-05-16 06:40:13.000000 dprdp-0.1.1/pypykatz/registry/security/common.py
+-rw-rw-rw-   0        0        0    10347 2024-05-16 06:38:33.000000 dprdp-0.1.1/pypykatz/registry/security/security.py
+-rw-rw-rw-   0        0        0     5707 2024-05-16 06:34:41.000000 dprdp-0.1.1/pypykatz/registry/security/structures.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.926689 dprdp-0.1.1/pypykatz/registry/software/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/registry/software/__init__.py
+-rw-rw-rw-   0        0        0     2192 2024-05-16 06:33:04.000000 dprdp-0.1.1/pypykatz/registry/software/software.py
+drwxrwxrwx   0        0        0        0 2024-05-20 05:17:00.927685 dprdp-0.1.1/pypykatz/registry/system/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:12:54.000000 dprdp-0.1.1/pypykatz/registry/system/__init__.py
+-rw-rw-rw-   0        0        0     2133 2024-05-16 06:33:04.000000 dprdp-0.1.1/pypykatz/registry/system/system.py
+-rw-rw-rw-   0        0        0       42 2024-05-20 05:17:00.927685 dprdp-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      374 2024-05-20 05:16:00.000000 dprdp-0.1.1/setup.py
```

### Comparing `dprdp-0.1.0/dprdp.egg-info/SOURCES.txt` & `dprdp-0.1.1/dprdp.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 setup.py
 dprdp.egg-info/PKG-INFO
 dprdp.egg-info/SOURCES.txt
 dprdp.egg-info/dependency_links.txt
+dprdp.egg-info/requires.txt
 dprdp.egg-info/top_level.txt
 pypykatz/__init__.py
 pypykatz/apypykatz.py
 pypykatz/pypykatz.py
 pypykatz/alsadecryptor/__init__.py
 pypykatz/alsadecryptor/asbmfile.py
 pypykatz/alsadecryptor/lsa_decryptor.py
```

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/asbmfile.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/asbmfile.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/lsa_decryptor.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/lsa_decryptor.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/lsa_decryptor_nt5.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/lsa_decryptor_nt5.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/lsa_decryptor_nt6.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/lsa_decryptor_nt6.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/lsa_template_nt5.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/lsa_template_nt5.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/lsa_template_nt6.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/lsa_template_nt6.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/lsa_templates.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/lsa_templates.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/package_commons.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/package_commons.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/packages/__init__.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/packages/cloudap/decryptor.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/packages/cloudap/decryptor.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/packages/cloudap/templates.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/packages/cloudap/templates.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/packages/credman/templates.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/packages/credman/templates.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/packages/dpapi/decryptor.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/packages/dpapi/decryptor.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/packages/dpapi/templates.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/packages/dpapi/templates.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/packages/kerberos/decryptor.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/packages/kerberos/decryptor.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/packages/kerberos/templates.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/packages/kerberos/templates.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/packages/livessp/decryptor.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/packages/livessp/decryptor.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/packages/livessp/templates.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/packages/livessp/templates.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/packages/msv/decryptor.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/packages/msv/decryptor.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/packages/msv/templates.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/packages/msv/templates.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/packages/ssp/decryptor.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/packages/ssp/decryptor.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/packages/ssp/templates.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/packages/ssp/templates.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/packages/tspkg/decryptor.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/packages/tspkg/decryptor.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/packages/tspkg/templates.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/packages/tspkg/templates.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/packages/wdigest/decryptor.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/packages/wdigest/decryptor.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/packages/wdigest/templates.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/packages/wdigest/templates.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/alsadecryptor/win_datatypes.py` & `dprdp-0.1.1/pypykatz/alsadecryptor/win_datatypes.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/apypykatz.py` & `dprdp-0.1.1/pypykatz/apypykatz.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/common.py` & `dprdp-0.1.1/pypykatz/commons/common.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/filetime.py` & `dprdp-0.1.1/pypykatz/commons/filetime.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/kerberosticket.py` & `dprdp-0.1.1/pypykatz/commons/kerberosticket.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/readers/local/common/advapi32.py` & `dprdp-0.1.1/pypykatz/commons/readers/local/common/advapi32.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/readers/local/common/defines.py` & `dprdp-0.1.1/pypykatz/commons/readers/local/common/defines.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/readers/local/common/fileinfo.py` & `dprdp-0.1.1/pypykatz/commons/readers/local/common/fileinfo.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/readers/local/common/kernel32.py` & `dprdp-0.1.1/pypykatz/commons/readers/local/common/kernel32.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/readers/local/common/live_reader_ctypes.py` & `dprdp-0.1.1/pypykatz/commons/readers/local/common/live_reader_ctypes.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/readers/local/common/privileges.py` & `dprdp-0.1.1/pypykatz/commons/readers/local/common/privileges.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/readers/local/common/privileges_types.py` & `dprdp-0.1.1/pypykatz/commons/readers/local/common/privileges_types.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/readers/local/common/psapi.py` & `dprdp-0.1.1/pypykatz/commons/readers/local/common/psapi.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/readers/local/common/version.py` & `dprdp-0.1.1/pypykatz/commons/readers/local/common/version.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/readers/local/common/winreg.py` & `dprdp-0.1.1/pypykatz/commons/readers/local/common/winreg.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/readers/local/live_reader.py` & `dprdp-0.1.1/pypykatz/commons/readers/local/live_reader.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/readers/local/process.py` & `dprdp-0.1.1/pypykatz/commons/readers/local/process.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/readers/registry/live/reader.py` & `dprdp-0.1.1/pypykatz/commons/readers/registry/live/reader.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/readers/rekall/rekallreader.py` & `dprdp-0.1.1/pypykatz/commons/readers/rekall/rekallreader.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/readers/volatility3/volreader.py` & `dprdp-0.1.1/pypykatz/commons/readers/volatility3/volreader.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/win_datatypes.py` & `dprdp-0.1.1/pypykatz/commons/win_datatypes.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/winapi/constants.py` & `dprdp-0.1.1/pypykatz/commons/winapi/constants.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/winapi/local/advapi32.py` & `dprdp-0.1.1/pypykatz/commons/winapi/local/advapi32.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/winapi/local/function_defs/advapi32.py` & `dprdp-0.1.1/pypykatz/commons/winapi/local/function_defs/advapi32.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/winapi/local/function_defs/defines.py` & `dprdp-0.1.1/pypykatz/commons/winapi/local/function_defs/defines.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/winapi/local/function_defs/kernel32.py` & `dprdp-0.1.1/pypykatz/commons/winapi/local/function_defs/kernel32.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/winapi/local/function_defs/live_reader_ctypes.py` & `dprdp-0.1.1/pypykatz/commons/winapi/local/function_defs/live_reader_ctypes.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/winapi/local/function_defs/ntdll.py` & `dprdp-0.1.1/pypykatz/commons/winapi/local/function_defs/ntdll.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/winapi/local/function_defs/psapi.py` & `dprdp-0.1.1/pypykatz/commons/winapi/local/function_defs/psapi.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/commons/winapi/processmanipulator.py` & `dprdp-0.1.1/pypykatz/commons/winapi/processmanipulator.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/dpapi/constants.py` & `dprdp-0.1.1/pypykatz/dpapi/constants.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/dpapi/dpapi.py` & `dprdp-0.1.1/pypykatz/dpapi/dpapi.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/dpapi/finders/cryptokeys.py` & `dprdp-0.1.1/pypykatz/dpapi/finders/cryptokeys.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/dpapi/finders/ngc.py` & `dprdp-0.1.1/pypykatz/dpapi/finders/ngc.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/dpapi/functiondefs/dpapi.py` & `dprdp-0.1.1/pypykatz/dpapi/functiondefs/dpapi.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/dpapi/structures/blob.py` & `dprdp-0.1.1/pypykatz/dpapi/structures/blob.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/dpapi/structures/credentialfile.py` & `dprdp-0.1.1/pypykatz/dpapi/structures/credentialfile.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/dpapi/structures/masterkeyfile.py` & `dprdp-0.1.1/pypykatz/dpapi/structures/masterkeyfile.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/dpapi/structures/system.py` & `dprdp-0.1.1/pypykatz/dpapi/structures/system.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/dpapi/structures/vault.py` & `dprdp-0.1.1/pypykatz/dpapi/structures/vault.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/lsa_decryptor.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/lsa_decryptor.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/lsa_decryptor_nt5.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/lsa_decryptor_nt5.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/lsa_decryptor_nt6.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/lsa_decryptor_nt6.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/lsa_template_nt5.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/lsa_template_nt5.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/lsa_template_nt6.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/lsa_template_nt6.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/lsa_templates.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/lsa_templates.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/package_commons.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/package_commons.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/packages/__init__.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/packages/cloudap/decryptor.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/packages/cloudap/decryptor.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/packages/cloudap/templates.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/packages/cloudap/templates.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/packages/credman/templates.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/packages/credman/templates.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/packages/dpapi/decryptor.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/packages/dpapi/decryptor.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/packages/dpapi/templates.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/packages/dpapi/templates.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/packages/kerberos/decryptor.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/packages/kerberos/decryptor.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/packages/kerberos/templates.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/packages/kerberos/templates.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/packages/livessp/decryptor.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/packages/livessp/decryptor.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/packages/livessp/templates.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/packages/livessp/templates.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/packages/msv/decryptor.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/packages/msv/decryptor.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/packages/msv/templates.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/packages/msv/templates.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/packages/ssp/decryptor.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/packages/ssp/decryptor.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/packages/ssp/templates.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/packages/ssp/templates.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/packages/tspkg/decryptor.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/packages/tspkg/decryptor.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/packages/tspkg/templates.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/packages/tspkg/templates.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/packages/wdigest/decryptor.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/packages/wdigest/decryptor.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/lsadecryptor/packages/wdigest/templates.py` & `dprdp-0.1.1/pypykatz/lsadecryptor/packages/wdigest/templates.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/pypykatz.py` & `dprdp-0.1.1/pypykatz/pypykatz.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/registry/live_parser.py` & `dprdp-0.1.1/pypykatz/registry/live_parser.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/registry/offline_parser.py` & `dprdp-0.1.1/pypykatz/registry/offline_parser.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/registry/sam/sam.py` & `dprdp-0.1.1/pypykatz/registry/sam/sam.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/registry/sam/structures.py` & `dprdp-0.1.1/pypykatz/registry/sam/structures.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/registry/security/common.py` & `dprdp-0.1.1/pypykatz/registry/security/common.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/registry/security/security.py` & `dprdp-0.1.1/pypykatz/registry/security/security.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/registry/security/structures.py` & `dprdp-0.1.1/pypykatz/registry/security/structures.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/registry/software/software.py` & `dprdp-0.1.1/pypykatz/registry/software/software.py`

 * *Files identical despite different names*

### Comparing `dprdp-0.1.0/pypykatz/registry/system/system.py` & `dprdp-0.1.1/pypykatz/registry/system/system.py`

 * *Files identical despite different names*

