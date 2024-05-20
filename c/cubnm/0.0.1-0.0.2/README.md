# Comparing `tmp/cuBNM-0.0.1.tar.gz` & `tmp/cubnm-0.0.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuBNM-0.0.1.tar", last modified: Fri Dec  8 17:00:38 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

