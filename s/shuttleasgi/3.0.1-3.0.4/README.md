# Comparing `tmp/shuttleasgi-3.0.1.tar.gz` & `tmp/shuttleasgi-3.0.4-cp312-cp312-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shuttleasgi-3.0.1.tar", last modified: Mon Apr  1 21:44:08 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

