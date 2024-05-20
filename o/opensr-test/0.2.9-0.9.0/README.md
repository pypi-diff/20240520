# Comparing `tmp/opensr_test-0.2.9.tar.gz` & `tmp/opensr_test-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensr_test-0.2.9.tar", max compression
+gzip compressed data, was "opensr_test-0.9.0.tar", max compression
```

## Comparing `opensr_test-0.2.9.tar` & `opensr_test-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2024-05-09 08:13:17.278355 opensr_test-0.2.9/LICENSE
--rw-r--r--   0        0        0    12100 2024-05-13 15:41:27.379466 opensr_test-0.2.9/README.md
--rw-r--r--   0        0        0      111 2024-05-10 17:01:30.595335 opensr_test-0.2.9/opensr_test/__init__.py
--rw-r--r--   0        0        0     3303 2024-05-14 15:00:31.255299 opensr_test-0.2.9/opensr_test/config.py
--rw-r--r--   0        0        0     3925 2024-05-14 15:04:04.089140 opensr_test-0.2.9/opensr_test/correctness.py
--rw-r--r--   0        0        0     2154 2024-05-14 11:04:14.042783 opensr_test-0.2.9/opensr_test/dataset.py
--rw-r--r--   0        0        0    17828 2024-05-14 14:54:26.605895 opensr_test-0.2.9/opensr_test/distance.py
--rw-r--r--   0        0        0    20917 2024-05-14 15:17:02.456527 opensr_test-0.2.9/opensr_test/main.py
--rw-r--r--   0        0        0    11321 2024-05-14 15:05:56.813535 opensr_test-0.2.9/opensr_test/plot.py
--rw-r--r--   0        0        0     2200 2024-05-12 16:32:21.798342 opensr_test-0.2.9/opensr_test/spatial.py
--rw-r--r--   0        0        0     4270 2024-05-14 11:12:03.733377 opensr_test-0.2.9/opensr_test/utils.py
--rw-r--r--   0        0        0     2076 2024-05-15 05:42:10.708329 opensr_test-0.2.9/pyproject.toml
--rw-r--r--   0        0        0    13296 1970-01-01 00:00:00.000000 opensr_test-0.2.9/setup.py
--rw-r--r--   0        0        0    12965 1970-01-01 00:00:00.000000 opensr_test-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-09 08:13:17.278355 opensr_test-0.9.0/LICENSE
+-rw-r--r--   0        0        0    12100 2024-05-13 15:41:27.379466 opensr_test-0.9.0/README.md
+-rw-r--r--   0        0        0      244 2024-05-18 13:08:32.084169 opensr_test-0.9.0/opensr_test/__init__.py
+-rw-r--r--   0        0        0     3425 2024-05-18 12:28:54.547515 opensr_test-0.9.0/opensr_test/config.py
+-rw-r--r--   0        0        0     5853 2024-05-18 14:08:52.601223 opensr_test-0.9.0/opensr_test/correctness.py
+-rw-r--r--   0        0        0     2154 2024-05-14 11:04:14.042783 opensr_test-0.9.0/opensr_test/dataset.py
+-rw-r--r--   0        0        0    17828 2024-05-14 14:54:26.605895 opensr_test-0.9.0/opensr_test/distance.py
+-rw-r--r--   0        0        0    20870 2024-05-18 14:06:34.257202 opensr_test-0.9.0/opensr_test/main.py
+-rw-r--r--   0        0        0    11321 2024-05-14 15:05:56.813535 opensr_test-0.9.0/opensr_test/plot.py
+-rw-r--r--   0        0        0     2200 2024-05-12 16:32:21.798342 opensr_test-0.9.0/opensr_test/spatial.py
+-rw-r--r--   0        0        0     4270 2024-05-18 12:07:37.563317 opensr_test-0.9.0/opensr_test/utils.py
+-rw-r--r--   0        0        0     2076 2024-05-18 13:06:37.495411 opensr_test-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    13296 1970-01-01 00:00:00.000000 opensr_test-0.9.0/setup.py
+-rw-r--r--   0        0        0    12965 1970-01-01 00:00:00.000000 opensr_test-0.9.0/PKG-INFO
```

### Comparing `opensr_test-0.2.9/LICENSE` & `opensr_test-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opensr_test-0.2.9/README.md` & `opensr_test-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `opensr_test-0.2.9/opensr_test/config.py` & `opensr_test-0.9.0/opensr_test/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,17 +31,19 @@
 
 
     # Synthesis parameters
     synthesis_distance: DistanceMetrics = "l1"
 
     # Correctness parameters
     correctness_distance: DistanceMetrics = "l1"
+    correctness_norm: Literal["softmax", "standard", "percent"] = "softmax"
     im_score: Optional[float] = 0.80
     om_score: Optional[float] = 0.80
-    ha_score: Optional[float] = 0.40
+    ha_score: Optional[float] = 0.30 # be quiet conservative about hallucinations
+
 
     # General parameters - validator ----------------------------
     @field_validator("device")
     def check_device(cls, value) -> str:
         return torch.device(value)
 
     @field_validator("agg_method")
```

### Comparing `opensr_test-0.2.9/opensr_test/dataset.py` & `opensr_test-0.9.0/opensr_test/dataset.py`

 * *Files identical despite different names*

### Comparing `opensr_test-0.2.9/opensr_test/distance.py` & `opensr_test-0.9.0/opensr_test/distance.py`

 * *Files identical despite different names*

### Comparing `opensr_test-0.2.9/opensr_test/main.py` & `opensr_test-0.9.0/opensr_test/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     apply_downsampling, apply_upsampling,
     apply_mask, hq_histogram_matching,
     seed_everything
 )
 from opensr_test.spatial import SpatialMetricAlign
 from opensr_test.config import Config, Results, Consistency, Synthesis, Correctness, Auxiliar
 from opensr_test.distance import get_distance
-from opensr_test.correctness import get_distances, tc_improvement, tc_omission, tc_hallucination
+from opensr_test.correctness import get_distances, tc_improvement, tc_omission, tc_hallucination, get_correctness_stats
 from opensr_test import plot
 
 class Metrics:
     def __init__(
         self,
         params: Optional[Config] = None,
         **kwargs
@@ -410,15 +410,14 @@
         # Apply the mask to remove the pixels with gradients 
         mask = self._create_mask(
             d_ref=d_ref,
             d_im=d_im,
             d_om=d_om,
             gradient_threshold=gradient_threshold
         )
-        self.potential_pixels = torch.nansum(mask)
         self.d_ref = d_ref * mask
         self.d_im =  d_im * mask
         self.d_om =  d_om * mask
         
         # Compute relative distance
         self.d_im_ref = self.d_im / self.d_ref
         self.d_om_ref = self.d_om / self.d_ref
@@ -440,27 +439,29 @@
         # Estimate Improvement
         self.improvement = tc_improvement(
             d_im=self.d_im_ref,
             d_om=self.d_om_ref,
             plambda=self.params.im_score
         )
 
-        # Classify the pixels based on the distance
-        tensor_stack = torch.stack([
-            self.improvement,
-            self.omission,
-            self.hallucination
-        ], dim=0)
-        self.classification = torch.argmin(tensor_stack, dim=0) * mask
-
-        # Get the percentage of omission, improvement, and hallucination
-        self.im_percentage = torch.sum(self.classification==0) / self.potential_pixels
-        self.om_percentage = torch.sum(self.classification==1) / self.potential_pixels
-        self.ha_percentage = torch.sum(self.classification==2) / self.potential_pixels        
-            
+        #  Get stats
+        total_stats = get_correctness_stats(
+            im_tensor=self.improvement,
+            om_tensor=self.omission,
+            ha_tensor=self.hallucination,
+            mask=mask,
+            correctness_norm=self.params.correctness_norm
+        )
+        
+        self.classification = total_stats["classification"]
+        self.improvement, self.omission, self.hallucination = total_stats["tensor_stack"]
+        self.im_percentage = total_stats["stats"][0]
+        self.om_percentage = total_stats["stats"][1]
+        self.ha_percentage = total_stats["stats"][2]
+        
         return {
             "ha_percent": self.ha_percentage.item(),
             "om_percent": self.om_percentage.item(),
             "im_percent": self.im_percentage.item()
         }
 
     def compute(
```

### Comparing `opensr_test-0.2.9/opensr_test/plot.py` & `opensr_test-0.9.0/opensr_test/plot.py`

 * *Files identical despite different names*

### Comparing `opensr_test-0.2.9/opensr_test/spatial.py` & `opensr_test-0.9.0/opensr_test/spatial.py`

 * *Files identical despite different names*

### Comparing `opensr_test-0.2.9/opensr_test/utils.py` & `opensr_test-0.9.0/opensr_test/utils.py`

 * *Files identical despite different names*

### Comparing `opensr_test-0.2.9/pyproject.toml` & `opensr_test-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "opensr_test"
-version = "0.2.9"
+version = "0.9.0"
 description = "A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution"
 authors = ["Cesar Aybar <cesar.aybar@uv.es>"]
 repository = "https://github.com/csaybar/opensr-test"
 documentation = "https://csaybar.github.io/opensr-test/"
 readme = "README.md"
 packages = [
   {include = "opensr_test"}
```

### Comparing `opensr_test-0.2.9/setup.py` & `opensr_test-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'requests>=2.25.0',
  'satalign>=0.1.0',
  'scikit-image>=0.19.0',
  'torchvision>=0.17.0']
 
 setup_kwargs = {
     'name': 'opensr-test',
-    'version': '0.2.9',
+    'version': '0.9.0',
     'description': 'A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution',
     'long_description': '<p align="center">\n  <a href="https://github.com/ESAOpenSR/opensr-test"><img src="docs/images/logo.png" alt="header" width="50%"></a>\n</p>\n\n<p align="center">\n    <em>\n    A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution\n    </em>\n</p>\n\n<p align="center">\n<a href=\'https://pypi.python.org/pypi/opensr-test\'>\n<img src=\'https://img.shields.io/pypi/v/opensr-test.svg\' alt=\'PyPI\' />\n</a>\n<a href="https://opensource.org/licenses/MIT" target="_blank">\n    <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License">\n</a>\n<a href="https://github.com/psf/black" target="_blank">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Black">\n</a>\n<a href="https://pycqa.github.io/isort/" target="_blank">\n    <img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" alt="isort">\n</a>\n</p>\n\n---\n\n**GitHub**: [https://github.com/ESAOpenSR/opensr-test](https://github.com/ESAOpenSR/opensr-test)\n\n**Documentation**: [https://esaopensr.github.io/opensr-test](https://esaopensr.github.io/opensr-test)\n\n**PyPI**: [https://pypi.org/project/opensr-test/](https://pypi.org/project/opensr-test/)\n\n**Paper**: [https://www.techrxiv.org/users/760184/articles/735467-a-comprehensive-benchmark-for-optical-remote-sensing-image-super-resolution](https://www.techrxiv.org/users/760184/articles/735467-a-comprehensive-benchmark-for-optical-remote-sensing-image-super-resolution)\n\n---\n\n#\n\n## **Overview**\n\nSuper-Resolution (SR) aims to improve satellite imagery ground sampling distance. However, two problems are common in the literature. First, most models are **tested on synthetic data**, raising doubts about their real-world applicability and performance. Second, traditional evaluation metrics such as PSNR, LPIPS, and SSIM are not designed to assess SR performance. These metrics fall short, especially in conditions involving changes in luminance or spatial misalignments - scenarios frequently encountered in real world.\n\nTo address these challenges, \'opensr-test\' provides a fair approach for SR benchmark. We provide three datasets carefully crafted to minimize spatial and spectral misalignment. Besides, \'opensr-test\' precisely assesses SR algorithm performance across three independent metrics groups that measure consistency, synthesis, and correctness.\n\n<p align="center">\n  <img src="docs/images/diagram.png" alt="header">\n</p>\n\n## **How to use**\n\nThe example below shows how to use `opensr-test` to benchmark your SR model.\n\n\n```python\nimport torch\nimport opensr_test\n\nlr = torch.rand(4, 64, 64)\nhr = torch.rand(4, 256, 256)\nsr = torch.rand(4, 256, 256)\n\nmetrics = opensr_test.Metrics()\nmetrics.compute(lr=lr, sr=sr, hr=hr)\n>>> {\'reflectance\': 0.253, \'spectral\': 26.967, \'spatial\': 0.0, \'synthesis\': 0.2870, \'ha_percent\': 0.892, \'om_percent\': 0.0613, \'im_percent\': 0.04625}\n```\n\nThis model returns:\n\n- **reflectance**: How SR affects the reflectance values of the LR image. By default, it uses the L1 norm. The lower the value, the better the reflectance consistency.\n\n- **spectral**: How SR affects the spectral signature of the LR image. By default, it uses the spectral angle distance (SAM). The lower the value, the better the spectral consistency. The angles are in degrees.\n\n- **spatial**: The spatial alignment between the SR and LR images. By default, it uses Phase Correlation Coefficient (PCC). Some SR models introduce spatial shift, which can be detected by this metric.\n\n- **synthesis**: The high-frequency details introduced by the SR model. By default, it uses the L1 norm. The lower the value, the better the synthesis quality.\n\n- **ha_percent**: The percentage of pixels in the SR image that are classified as hallucinations. A hallucination is a detail in the SR image that **is not present in the HR image.**\n\n- **om_percent**: The percentage of pixels in the SR image that are classified as omissions. An omission is a detail in the HR image that **is not present in the SR image.**\n\n- **im_percent**: The percentage of pixels in the SR image that are classified as improvements. An improvement is a detail in the SR image that **is present in the HR image and not in the LR image.**\n\n## **Benchmark**\n\nBenchmark comparison of SR models. Downward arrows (↓) denote metrics in which lower values are preferable, and upward arrows (↑) indicate metrics in which higher values reflect better performance.\n\n\n## **Installation**\n\nInstall the latest version from PyPI:\n\n```\npip install opensr-test\n```\n\nUpgrade `opensr-test` by running:\n\n```\npip install -U opensr-test\n```\n\nInstall the latest dev version from GitHub by running:\n\n```\npip install git+https://github.com/ESAOpenSR/opensr-test\n```\n\n## **Datasets**\n\nThe `opensr-test` package provides five datasets for benchmarking SR models. These datasets are carefully crafted to minimize spatial and spectral misalignment. See our Hugging Face repository for more details about the datasets. [**https://huggingface.co/datasets/isp-uv-es/opensr-test**](https://huggingface.co/datasets/isp-uv-es/opensr-test)\n\n### **NAIP (X4 scale factor)**\n\nThe National Agriculture Imagery Program (NAIP) dataset is a high-resolution aerial imagery dataset that covers the continental United States. The dataset consists of 2.5m NAIP imagery captured in the visible and near-infrared spectrum (RGBNIR) and all Sentinel-2 L1C and L2A bands. The dataset focus in **crop fields, forests, and bare soil areas**.\n\n```python\nimport opensr_test\n\nnaip = opensr_test.load("naip")\n```\n\n<p align="center">\n  <a href="https://github.com/ESAOpenSR/opensr-test"><img src="docs/images/NAIP.gif" alt="header" width="80%"></a>\n</p>\n\n### **SPOT (X4 scale factor)**\n\nThe SPOT imagery were obtained from the worldstat dataset. The dataset consists of 2.5m SPOT imagery captured in the visible and near-infrared spectrum (RGBNIR) and all Sentinel-2 L1C and L2A bands. The dataset focus in **urban areas, crop fields, and bare soil areas**.\n\n```python\nimport opensr_test\n\nspot = opensr_test.load("spot")\n```\n\n<p align="center">\n  <a href="https://github.com/ESAOpenSR/opensr-test"><img src="docs/images/SPOT.gif" alt="header" width="80%"></a>\n</p>\n\n\n### **Venµs (X2 scale factor)**\n\nThe Venµs images were obtained from the [**Sen2Venµs dataset**](https://zenodo.org/records/6514159). The dataset consists of 5m Venµs imagery captured in the visible and near-infrared spectrum (RGBNIR) and all Sentinel-2 L1C and L2A bands. The dataset focus in **crop fields, forests, urban areas, and bare soil areas**.\n\n```python\nimport opensr_test\n\nvenus = opensr_test.load("venus")\n```\n\n<p align="center">\n  <a href="https://github.com/ESAOpenSR/opensr-test"><img src="docs/images/VENUS.gif" alt="header" width="80%"></a>\n</p>\n\n\n### **SPAIN CROPS (x4 scale factor)**\n\nThe SPAIN CROPS dataset consists of 2.5m aerial imagery captured in the visible and near-infrared spectrum (RGBNIR) by the Spanish National Geographic Institute (IGN). The dataset includes all Sentinel-2 L1C and L2A bands. The dataset focus in **crop fields and forests**.\n\n```python\nimport opensr_test\n\nspain_crops = opensr_test.load("spain_crops")\n```\n\n<p align="center">\n  <a href="https://github.com/ESAOpenSR/opensr-test"><img src="docs/images/SPAIN_CROPS.gif" alt="header" width="80%"></a>\n</p>\n\n\n### **SPAIN URBAN (x4 scale factor)**\n\nThe SPAIN URBAN dataset consists of 2.5m aerial imagery captured in the visible and near-infrared spectrum (RGBNIR) by the Spanish National Geographic Institute (IGN). The dataset includes all Sentinel-2 L1C and L2A bands. The dataset focus in **urban areas**.\n\n```python\n\nspain_urban = opensr_test.load("spain_urban")\n```\n\n<p align="center">\n  <a href="https://github.com/ESAOpenSR/opensr-test"><img src="docs/images/SPAIN_URBAN.gif" alt="header" width="80%"></a>\n</p>\n\n\n## **Examples**\n\nThe following examples show how to use `opensr-test` to benchmark your SR model.\n\n- Use `opensr-test` with TensorFlow model (SR4RS) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1cAGDGlj5Kqt343inNni3ByLE1856z0gE#scrollTo=xaivkcD5Zfw1&uniqifier=1)\n\n- Use `opensr-test` with PyTorch model (SuperImage) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Db8-JSMTF-hNZQv2UyBDclxkO5hgP9VR#scrollTo=jVL7o6yOrJkY)\n\n- Use `opensr-test` with a diffuser model (LDMSuperResolutionPipeline) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1banDovG43c2OBh9MODPN4OXgaSCXu1Dc#scrollTo=zz4Aw7_52ulT)\n\n- Use `opensr-test` with a diffuser model (opensr-model) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1banDovG43c2OBh9MODPN4OXgaSCXu1Dc#scrollTo=zz4Aw7_52ulT)\n\n\n- Use `opensr-test` with Pytorch (EvoLand) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1banDovG43c2OBh9MODPN4OXgaSCXu1Dc#scrollTo=zz4Aw7_52ulT)\n\n\n- Use `opensr-test` with Pytorch (SWIN2-MOSE) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1banDovG43c2OBh9MODPN4OXgaSCXu1Dc#scrollTo=zz4Aw7_52ulT)\n\n- Use `opensr-test` with Pytorch (synthetic dataset) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1banDovG43c2OBh9MODPN4OXgaSCXu1Dc#scrollTo=zz4Aw7_52ulT)\n\n## **Visualizations**\n\nThe `opensr-test` package provides a set of visualizations to help you understand the performance of your SR model.\n\n```python\nimport torch\nimport opensr_test\nimport matplotlib.pyplot as plt\n\nfrom super_image import HanModel\n\n# Define the SR model\nsrmodel = HanModel.from_pretrained(\'eugenesiow/han\', scale=4)\n\n# Load the data\nlr, hr, parameters = opensr_test.load("spot").values()\n\n# Define the benchmark experiment\nmetrics = opensr_test.Metrics()\n\n# Define the image to be tested\nidx = 0\nlr_img = torch.from_numpy(lr[idx, 0:3])\nhr_img = torch.from_numpy(hr[idx, 0:3])\nsr_img = srmodel(lr_img[None]).squeeze().detach()\n\n# Compute the metrics\nmetrics.compute(\n    lr=lr_img, sr=sr_img, hr=hr_img,\n    gradient_threshold=parameters[idx]\n)\n```\n\nNow, we can visualize the results using the `opensr_test.visualize` module.\nfDisplay the triplets LR, SR and HR images:\n\n```python\nmetrics.plot_triplets()\n```\n\n<p align="center">\n  <img src="docs/images/example01.png">\n</p>\n\nDisplay a summary of all the metrics:\n\n```python\nmetrics.plot_summary()\n```\n\n<p align="center">\n  <img src="docs/images/example04.png">\n</p>\n\n\nDisplay the correctness of the SR image:\n\n```python\nmetrics.plot_tc()\n```\n\n<p align="center">\n  <img src="docs/images/example05.png">\n</p>\n\n## **Deeper understanding**\n\nExplore the [API](https://esaopensr.github.io/opensr-test/docs/API/config_pydantic.html) section for more details about personalizing your benchmark experiments.\n\n<p align="center">\n    <a href="/docs/api.md"><img src="docs/images/image02.png" alt="opensr-test" width="30%"></a>\n</p>\n\n## **Citation**\n\nIf you use `opensr-test` in your research, please cite our paper:\n\n```\n@article{aybar2024comprehensive,\n  title={A Comprehensive Benchmark for Optical Remote Sensing Image Super-Resolution},\n  author={Aybar, Cesar and Montero, David and Donike, Simon and Kalaitzis, Freddie and G{\\\'o}mez-Chova, Luis},\n  journal={Authorea Preprints},\n  year={2024},\n  publisher={Authorea}\n}\n```\n\n## **Acknowledgements**\n\nThis work was make with the support of the European Space Agency (ESA) under the project “Explainable AI: application to trustworthy super-resolution (OpenSR)”. Cesar Aybar acknowledges support by the National Council of Science, Technology, and Technological Innovation (CONCYTEC, Peru) through the “PROYECTOS DE INVESTIGACIÓN BÁSICA – 2023-01” program with contract number PE501083135-2023-PROCIENCIA. Luis Gómez-Chova acknowledges support from the Spanish Ministry of Science and Innovation (project PID2019-109026RB-I00 funded by MCIN/AEI/10.13039/501100011033).\n',
     'author': 'Cesar Aybar',
     'author_email': 'cesar.aybar@uv.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/csaybar/opensr-test',
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['opensr_test'] package_data = \ {'': ['*']} install_requires = \
 ['kornia>=0.7.2', 'matplotlib>=3.7.0', 'numpy>=1.25.2', 'opencv-
 python>=4.8.0.0', 'pydantic>=2.7.1', 'requests>=2.25.0', 'satalign>=0.1.0',
 'scikit-image>=0.19.0', 'torchvision>=0.17.0'] setup_kwargs = { 'name':
-'opensr-test', 'version': '0.2.9', 'description': 'A comprehensive benchmark
+'opensr-test', 'version': '0.9.0', 'description': 'A comprehensive benchmark
 for real-world Sentinel-2 imagery super-resolution', 'long_description': '
                                  \n _[_h_e_a_d_e_r_]\n
 \n\n
    \n \\nn AA ccoommpprreehheennssiivvee bbeenncchhmmaarrkk ffoorr rreeaall--wwoorrlldd SSeennttiinneell--22 iimmaaggeerryy ssuuppeerr--
                                 rreessoolluuttiioonn\\nn \n
 \n\n
         \n_\_n_[_\_'_P_y_P_I_\_'_]_\_n\n_\_n_ _[_L_i_c_e_n_s_e_]_\_n\n_\_n_ _[_B_l_a_c_k_]_\_n\n_\_n_ _[_i_s_o_r_t_]_\_n\n
```

### Comparing `opensr_test-0.2.9/PKG-INFO` & `opensr_test-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensr-test
-Version: 0.2.9
+Version: 0.9.0
 Summary: A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution
 Home-page: https://github.com/csaybar/opensr-test
 Author: Cesar Aybar
 Author-email: cesar.aybar@uv.es
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opensr-test Version: 0.2.9 Summary: A comprehensive
+Metadata-Version: 2.1 Name: opensr-test Version: 0.9.0 Summary: A comprehensive
 benchmark for real-world Sentinel-2 imagery super-resolution Home-page: https:/
 /github.com/csaybar/opensr-test Author: Cesar Aybar Author-email:
 cesar.aybar@uv.es Requires-Python: >=3.10,<4.0 Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.10 Requires-
 Dist: kornia (>=0.7.2) Requires-Dist: matplotlib (>=3.7.0) Requires-Dist: numpy
 (>=1.25.2) Requires-Dist: opencv-python (>=4.8.0.0) Requires-Dist: pydantic
 (>=2.7.1) Requires-Dist: requests (>=2.25.0) Requires-Dist: satalign (>=0.1.0)
```

