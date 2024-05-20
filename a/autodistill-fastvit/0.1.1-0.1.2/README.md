# Comparing `tmp/autodistill-fastvit-0.1.1.tar.gz` & `tmp/autodistill_fastvit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill-fastvit-0.1.1.tar", last modified: Wed Dec  6 09:29:03 2023, max compression
+gzip compressed data, was "autodistill_fastvit-0.1.2.tar", last modified: Mon May 20 14:47:41 2024, max compression
```

## Comparing `autodistill-fastvit-0.1.1.tar` & `autodistill_fastvit-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-12-06 09:29:03.145279 autodistill-fastvit-0.1.1/
--rw-r--r--   0 james      (501) staff       (20)     1822 2023-12-06 07:34:42.000000 autodistill-fastvit-0.1.1/.gitignore
--rw-r--r--   0 james      (501) staff       (20)    37036 2023-12-06 07:34:42.000000 autodistill-fastvit-0.1.1/ACKNOWLEDGEMENTS
--rw-r--r--   0 james      (501) staff       (20)     2666 2023-12-06 07:34:42.000000 autodistill-fastvit-0.1.1/LICENSE
--rw-r--r--   0 james      (501) staff       (20)      865 2023-12-06 07:34:42.000000 autodistill-fastvit-0.1.1/Makefile
--rw-r--r--   0 james      (501) staff       (20)     2871 2023-12-06 09:29:03.145048 autodistill-fastvit-0.1.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     2037 2023-12-06 07:34:42.000000 autodistill-fastvit-0.1.1/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-12-06 09:29:03.143582 autodistill-fastvit-0.1.1/autodistill_fastvit/
--rw-r--r--   0 james      (501) staff       (20)      100 2023-12-06 09:25:21.000000 autodistill-fastvit-0.1.1/autodistill_fastvit/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    14208 2023-12-06 07:34:42.000000 autodistill-fastvit-0.1.1/autodistill_fastvit/classes.json
--rw-r--r--   0 james      (501) staff       (20)     3259 2023-12-06 09:28:41.000000 autodistill-fastvit-0.1.1/autodistill_fastvit/fastvit.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-12-06 09:29:03.144449 autodistill-fastvit-0.1.1/autodistill_fastvit.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     2871 2023-12-06 09:29:03.000000 autodistill-fastvit-0.1.1/autodistill_fastvit.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      373 2023-12-06 09:29:03.000000 autodistill-fastvit-0.1.1/autodistill_fastvit.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-12-06 09:29:03.000000 autodistill-fastvit-0.1.1/autodistill_fastvit.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)      103 2023-12-06 09:29:03.000000 autodistill-fastvit-0.1.1/autodistill_fastvit.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       20 2023-12-06 09:29:03.000000 autodistill-fastvit-0.1.1/autodistill_fastvit.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-12-06 09:29:03.145334 autodistill-fastvit-0.1.1/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1198 2023-12-06 09:27:06.000000 autodistill-fastvit-0.1.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-20 14:47:41.195101 autodistill_fastvit-0.1.2/
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-20 14:47:41.190097 autodistill_fastvit-0.1.2/.github/
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-20 14:47:41.192165 autodistill_fastvit-0.1.2/.github/workflows/
+-rw-r--r--   0 james      (501) staff       (20)      954 2024-05-20 14:44:50.000000 autodistill_fastvit-0.1.2/.github/workflows/publish.yml
+-rw-r--r--   0 james      (501) staff       (20)      749 2024-05-20 14:44:50.000000 autodistill_fastvit-0.1.2/.github/workflows/test.yml
+-rw-r--r--   0 james      (501) staff       (20)      539 2024-05-20 14:44:50.000000 autodistill_fastvit-0.1.2/.github/workflows/welcome.yml
+-rw-r--r--   0 james      (501) staff       (20)     1822 2024-05-20 14:44:50.000000 autodistill_fastvit-0.1.2/.gitignore
+-rw-r--r--   0 james      (501) staff       (20)    37036 2024-05-20 14:44:50.000000 autodistill_fastvit-0.1.2/ACKNOWLEDGEMENTS
+-rw-r--r--   0 james      (501) staff       (20)     2666 2024-05-20 14:44:50.000000 autodistill_fastvit-0.1.2/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)      865 2024-05-20 14:44:50.000000 autodistill_fastvit-0.1.2/Makefile
+-rw-r--r--   0 james      (501) staff       (20)     2863 2024-05-20 14:47:41.194793 autodistill_fastvit-0.1.2/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     2037 2024-05-20 14:44:50.000000 autodistill_fastvit-0.1.2/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-20 14:47:41.192832 autodistill_fastvit-0.1.2/autodistill_fastvit/
+-rw-r--r--   0 james      (501) staff       (20)      100 2024-05-20 14:47:28.000000 autodistill_fastvit-0.1.2/autodistill_fastvit/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    14208 2024-05-20 14:44:50.000000 autodistill_fastvit-0.1.2/autodistill_fastvit/classes.json
+-rw-r--r--   0 james      (501) staff       (20)     3328 2024-05-20 14:47:17.000000 autodistill_fastvit-0.1.2/autodistill_fastvit/fastvit.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-20 14:47:41.194064 autodistill_fastvit-0.1.2/autodistill_fastvit.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     2863 2024-05-20 14:47:41.000000 autodistill_fastvit-0.1.2/autodistill_fastvit.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      460 2024-05-20 14:47:41.000000 autodistill_fastvit-0.1.2/autodistill_fastvit.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2024-05-20 14:47:41.000000 autodistill_fastvit-0.1.2/autodistill_fastvit.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       95 2024-05-20 14:47:41.000000 autodistill_fastvit-0.1.2/autodistill_fastvit.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       20 2024-05-20 14:47:41.000000 autodistill_fastvit-0.1.2/autodistill_fastvit.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2024-05-20 14:47:41.195164 autodistill_fastvit-0.1.2/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1239 2024-05-20 14:46:04.000000 autodistill_fastvit-0.1.2/setup.py
```

### Comparing `autodistill-fastvit-0.1.1/.gitignore` & `autodistill_fastvit-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `autodistill-fastvit-0.1.1/ACKNOWLEDGEMENTS` & `autodistill_fastvit-0.1.2/ACKNOWLEDGEMENTS`

 * *Files identical despite different names*

### Comparing `autodistill-fastvit-0.1.1/LICENSE` & `autodistill_fastvit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autodistill-fastvit-0.1.1/Makefile` & `autodistill_fastvit-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `autodistill-fastvit-0.1.1/PKG-INFO` & `autodistill_fastvit-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: autodistill-fastvit
-Version: 0.1.1
+Version: 0.1.2
 Summary: FastViT model for use with Autodistill
 Home-page: https://github.com/autodistill/autodistill-fastvit
 Author: Roboflow
 Author-email: support@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: timm>=0.4.12
+Requires-Dist: timm
 Requires-Dist: torch
 Requires-Dist: autodistill
 Requires-Dist: Pillow
 Requires-Dist: supervision
 Provides-Extra: dev
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: black==22.3.0; extra == "dev"
```

### Comparing `autodistill-fastvit-0.1.1/README.md` & `autodistill_fastvit-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `autodistill-fastvit-0.1.1/autodistill_fastvit/classes.json` & `autodistill_fastvit-0.1.2/autodistill_fastvit/classes.json`

 * *Files identical despite different names*

### Comparing `autodistill-fastvit-0.1.1/autodistill_fastvit/fastvit.py` & `autodistill_fastvit-0.1.2/autodistill_fastvit/fastvit.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,17 @@
 
         self.model = model
         self.transforms = transforms
 
     def predict(self, input: Any, confidence: int = 0.5) -> sv.Detections:
         img = load_image(input, return_format="PIL")
 
+        if img.mode == "RGBA":
+            img = img.convert("RGB")
+
         output = self.model(self.transforms(img).unsqueeze(0))
 
         prompts = self.ontology.prompts() if self.ontology is not None else []
 
         if len(prompts) == 0:
             probs, class_indices = torch.topk(output.softmax(dim=1) * 100, k=5)
```

### Comparing `autodistill-fastvit-0.1.1/autodistill_fastvit.egg-info/PKG-INFO` & `autodistill_fastvit-0.1.2/autodistill_fastvit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: autodistill-fastvit
-Version: 0.1.1
+Version: 0.1.2
 Summary: FastViT model for use with Autodistill
 Home-page: https://github.com/autodistill/autodistill-fastvit
 Author: Roboflow
 Author-email: support@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: timm>=0.4.12
+Requires-Dist: timm
 Requires-Dist: torch
 Requires-Dist: autodistill
 Requires-Dist: Pillow
 Requires-Dist: supervision
 Provides-Extra: dev
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: black==22.3.0; extra == "dev"
```

### Comparing `autodistill-fastvit-0.1.1/setup.py` & `autodistill_fastvit-0.1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,35 @@
-import re
-
 import setuptools
 from setuptools import find_packages
+import re
 
-with open("./autodistill_fastvit/__init__.py", "r") as f:
+with open("./autodistill_fastvit/__init__.py", 'r') as f:
     content = f.read()
     # from https://www.py4u.net/discuss/139845
     version = re.search(r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]', content).group(1)
-
+    
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autodistill-fastvit",
     version=version,
     author="Roboflow",
     author_email="support@roboflow.com",
     description="FastViT model for use with Autodistill",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/autodistill/autodistill-fastvit",
-    install_requires=["timm>=0.4.12", "torch", "autodistill", "Pillow", "supervision"],
+    install_requires=[
+        "timm",
+        "torch",
+        "autodistill",
+        "Pillow",
+        "supervision"
+    ],
     packages=find_packages(exclude=("tests",)),
     package_data={"autodistill_fastvit": ["classes.json"]},
     extras_require={
         "dev": ["flake8", "black==22.3.0", "isort", "twine", "pytest", "wheel"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
```

