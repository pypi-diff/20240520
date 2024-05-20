# Comparing `tmp/coherent_test-0.2.0.tar.gz` & `tmp/coherent_test-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coherent_test-0.2.0.tar", last modified: Sat May 18 21:32:18 2024, max compression
+gzip compressed data, was "coherent_test-0.2.1.tar", last modified: Sun May 19 19:23:06 2024, max compression
```

## Comparing `coherent_test-0.2.0.tar` & `coherent_test-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-18 21:32:17.914752 coherent_test-0.2.0/
--rw-r--r--   0 jaraco     (501) staff       (20)      164 2024-05-07 20:09:59.271765 coherent_test-0.2.0/README.md
--rw-r--r--   0 jaraco     (501) staff       (20)       48 2024-05-07 20:08:12.369636 coherent_test-0.2.0/__init__.py
--rw-r--r--   0 jaraco     (501) staff       (20)      382 2024-05-18 21:31:39.180074 coherent_test-0.2.0/__main__.py
--rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-18 21:32:17.238087 coherent_test-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      494 2024-05-18 21:32:18.538205 coherent_test-0.2.0/PKG-INFO
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-19 19:23:04.620228 coherent_test-0.2.1/
+-rw-r--r--   0 jaraco     (501) staff       (20)      162 2024-05-19 19:18:00.123702 coherent_test-0.2.1/README.md
+-rw-r--r--   0 jaraco     (501) staff       (20)       48 2024-05-07 20:08:12.369636 coherent_test-0.2.1/__init__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)      382 2024-05-18 21:31:39.180074 coherent_test-0.2.1/__main__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-19 19:23:04.620298 coherent_test-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      492 2024-05-19 19:23:06.060826 coherent_test-0.2.1/PKG-INFO
```

