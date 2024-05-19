# Comparing `tmp/pybigtools-0.1.3.tar.gz` & `tmp/pybigtools-0.1.4-cp312-cp312-manylinux_2_28_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

