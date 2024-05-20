# Comparing `tmp/ambit_fe-1.2.6.tar.gz` & `tmp/ambit_fe-1.2.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambit_fe-1.2.6.tar", last modified: Fri Apr 26 13:05:20 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

