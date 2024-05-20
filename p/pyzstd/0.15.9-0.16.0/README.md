# Comparing `tmp/pyzstd-0.15.9.tar.gz` & `tmp/pyzstd-0.16.0-cp38-cp38-musllinux_1_2_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzstd-0.15.9.tar", last modified: Sat Jun 24 03:18:31 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

