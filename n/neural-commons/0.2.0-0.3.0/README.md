# Comparing `tmp/neural-commons-0.2.0.tar.gz` & `tmp/neural-commons-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural-commons-0.2.0.tar", last modified: Fri May  3 17:47:18 2024, max compression
+gzip compressed data, was "neural-commons-0.3.0.tar", last modified: Mon May 20 00:34:04 2024, max compression
```

## Comparing `neural-commons-0.2.0.tar` & `neural-commons-0.3.0.tar`

### file list

```diff
@@ -1,59 +1,69 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 17:47:18.525122 neural-commons-0.2.0/
--rw-rw-rw-   0        0        0      745 2024-05-03 17:47:18.525122 neural-commons-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-04-28 15:46:56.000000 neural-commons-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 17:47:18.462621 neural-commons-0.2.0/neural_commons/
--rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.2.0/neural_commons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 17:47:18.478246 neural-commons-0.2.0/neural_commons/cf_nn/
--rw-rw-rw-   0        0        0     3238 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/cf_nn/CFConv2d.py
--rw-rw-rw-   0        0        0     1511 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/cf_nn/CFLinear.py
--rw-rw-rw-   0        0        0      778 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/cf_nn/CFModule.py
--rw-rw-rw-   0        0        0    11347 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/cf_nn/CFTrainer.py
--rw-rw-rw-   0        0        0      361 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/cf_nn/LRStrategy.py
--rw-rw-rw-   0        0        0      166 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/cf_nn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 17:47:18.478246 neural-commons-0.2.0/neural_commons/cf_nn/lrs/
--rw-rw-rw-   0        0        0      998 2024-05-03 13:07:40.000000 neural-commons-0.2.0/neural_commons/cf_nn/lrs/CrossEntropyLossLRS.py
--rw-rw-rw-   0        0        0      989 2024-05-03 13:07:40.000000 neural-commons-0.2.0/neural_commons/cf_nn/lrs/MSELossLRS.py
--rw-rw-rw-   0        0        0     1472 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/cf_nn/lrs/SlideLRS.py
--rw-rw-rw-   0        0        0      120 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/cf_nn/lrs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 17:47:18.478246 neural-commons-0.2.0/neural_commons/cf_nn/lrs/tests/
--rw-rw-rw-   0        0        0        0 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/cf_nn/lrs/tests/__init__.py
--rw-rw-rw-   0        0        0     1260 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/cf_nn/lrs/tests/test_slide_lrs.py
-drwxrwxrwx   0        0        0        0 2024-05-03 17:47:18.493872 neural-commons-0.2.0/neural_commons/cf_nn/tests/
--rw-rw-rw-   0        0        0        0 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/cf_nn/tests/__init__.py
--rw-rw-rw-   0        0        0     6253 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/cf_nn/tests/test_cf_conv2d.py
--rw-rw-rw-   0        0        0     3186 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/cf_nn/tests/test_cf_linear.py
-drwxrwxrwx   0        0        0        0 2024-05-03 17:47:18.493872 neural-commons-0.2.0/neural_commons/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.2.0/neural_commons/helpers/__init__.py
--rw-rw-rw-   0        0        0     4887 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/helpers/torch_helper.py
-drwxrwxrwx   0        0        0        0 2024-05-03 17:47:18.525122 neural-commons-0.2.0/neural_commons/modules/
--rw-rw-rw-   0        0        0      699 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/modules/AdaptiveSimpleNorm.py
--rw-rw-rw-   0        0        0     1791 2024-04-10 19:02:18.000000 neural-commons-0.2.0/neural_commons/modules/ConvMixer2d.py
--rw-rw-rw-   0        0        0      248 2024-04-07 23:57:05.000000 neural-commons-0.2.0/neural_commons/modules/GTanh.py
--rw-rw-rw-   0        0        0      283 2024-04-07 23:57:05.000000 neural-commons-0.2.0/neural_commons/modules/GaELU.py
--rw-rw-rw-   0        0        0     1266 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/modules/InputEncoder.py
--rw-rw-rw-   0        0        0      463 2024-04-07 23:57:05.000000 neural-commons-0.2.0/neural_commons/modules/LogShape.py
--rw-rw-rw-   0        0        0      203 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/modules/MAELoss.py
--rw-rw-rw-   0        0        0     2188 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/modules/NeuralLayer.py
--rw-rw-rw-   0        0        0      842 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/modules/NeuralLayer2d.py
--rw-rw-rw-   0        0        0      477 2024-04-07 23:57:05.000000 neural-commons-0.2.0/neural_commons/modules/ParametricReLU.py
--rw-rw-rw-   0        0        0      225 2024-04-10 19:01:12.000000 neural-commons-0.2.0/neural_commons/modules/Permute.py
--rw-rw-rw-   0        0        0      472 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/modules/Quadratic.py
--rw-rw-rw-   0        0        0      235 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/modules/RMSELoss.py
--rw-rw-rw-   0        0        0      470 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/modules/RndNonLinearFunction.py
--rw-rw-rw-   0        0        0     1708 2024-04-07 23:57:05.000000 neural-commons-0.2.0/neural_commons/modules/RndProjection.py
--rw-rw-rw-   0        0        0     2952 2024-04-08 16:14:56.000000 neural-commons-0.2.0/neural_commons/modules/SMoE.py
--rw-rw-rw-   0        0        0      750 2024-04-07 23:57:05.000000 neural-commons-0.2.0/neural_commons/modules/SMoEMixIn.py
--rw-rw-rw-   0        0        0      578 2024-05-02 14:19:58.000000 neural-commons-0.2.0/neural_commons/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 17:47:18.525122 neural-commons-0.2.0/neural_commons/opt/
--rw-rw-rw-   0        0        0     1909 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/opt/CosineScheduleOptimizer.py
--rw-rw-rw-   0        0        0     1428 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/opt/CosineScheduler.py
--rw-rw-rw-   0        0        0     2066 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/opt/TBCosineScheduleOptimizer.py
--rw-rw-rw-   0        0        0      174 2024-04-28 15:00:31.000000 neural-commons-0.2.0/neural_commons/opt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 17:47:18.462621 neural-commons-0.2.0/neural_commons.egg-info/
--rw-rw-rw-   0        0        0      745 2024-05-03 17:47:18.000000 neural-commons-0.2.0/neural_commons.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1722 2024-05-03 17:47:18.000000 neural-commons-0.2.0/neural_commons.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 17:47:18.000000 neural-commons-0.2.0/neural_commons.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-05-03 17:47:18.000000 neural-commons-0.2.0/neural_commons.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-03 17:47:18.000000 neural-commons-0.2.0/neural_commons.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 17:47:18.525122 neural-commons-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      969 2024-05-03 17:46:06.000000 neural-commons-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 00:34:04.739375 neural-commons-0.3.0/
+-rw-rw-rw-   0        0        0      745 2024-05-20 00:34:04.739375 neural-commons-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-28 15:46:56.000000 neural-commons-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 00:34:04.675464 neural-commons-0.3.0/neural_commons/
+-rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.3.0/neural_commons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 00:34:04.687463 neural-commons-0.3.0/neural_commons/cf_nn/
+-rw-rw-rw-   0        0        0     3302 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/cf_nn/CFConv2d.py
+-rw-rw-rw-   0        0        0     1575 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/cf_nn/CFLinear.py
+-rw-rw-rw-   0        0        0     1228 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/cf_nn/CFModule.py
+-rw-rw-rw-   0        0        0    10497 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/cf_nn/CFOptimizer.py
+-rw-rw-rw-   0        0        0      363 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/cf_nn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 00:34:04.692496 neural-commons-0.3.0/neural_commons/cf_nn/lrs/
+-rw-rw-rw-   0        0        0     2832 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/cf_nn/lrs/AdaptiveLRS.py
+-rw-rw-rw-   0        0        0      985 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/cf_nn/lrs/CrossEntropyLossLRS.py
+-rw-rw-rw-   0        0        0      989 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/cf_nn/lrs/MSELossLRS.py
+-rw-rw-rw-   0        0        0     1437 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/cf_nn/lrs/SlideLRS.py
+-rw-rw-rw-   0        0        0      160 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/cf_nn/lrs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 00:34:04.692496 neural-commons-0.3.0/neural_commons/cf_nn/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-18 16:33:26.000000 neural-commons-0.3.0/neural_commons/cf_nn/tests/__init__.py
+-rw-rw-rw-   0        0        0     7672 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/cf_nn/tests/test_cf_optimizer.py
+-rw-rw-rw-   0        0        0     1073 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/cf_nn/tests/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-20 00:34:04.692496 neural-commons-0.3.0/neural_commons/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.3.0/neural_commons/helpers/__init__.py
+-rw-rw-rw-   0        0        0     5844 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/helpers/torch_helper.py
+drwxrwxrwx   0        0        0        0 2024-05-20 00:34:04.723748 neural-commons-0.3.0/neural_commons/modules/
+-rw-rw-rw-   0        0        0      699 2024-04-28 15:00:31.000000 neural-commons-0.3.0/neural_commons/modules/AdaptiveSimpleNorm.py
+-rw-rw-rw-   0        0        0      288 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/modules/ArgMax.py
+-rw-rw-rw-   0        0        0     1791 2024-04-10 19:02:18.000000 neural-commons-0.3.0/neural_commons/modules/ConvMixer2d.py
+-rw-rw-rw-   0        0        0      248 2024-04-07 23:57:05.000000 neural-commons-0.3.0/neural_commons/modules/GTanh.py
+-rw-rw-rw-   0        0        0      283 2024-04-07 23:57:05.000000 neural-commons-0.3.0/neural_commons/modules/GaELU.py
+-rw-rw-rw-   0        0        0      312 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/modules/GaussianNoise.py
+-rw-rw-rw-   0        0        0     1266 2024-04-28 15:00:31.000000 neural-commons-0.3.0/neural_commons/modules/InputEncoder.py
+-rw-rw-rw-   0        0        0      463 2024-04-07 23:57:05.000000 neural-commons-0.3.0/neural_commons/modules/LogShape.py
+-rw-rw-rw-   0        0        0      203 2024-05-02 14:19:58.000000 neural-commons-0.3.0/neural_commons/modules/MAELoss.py
+-rw-rw-rw-   0        0        0     2188 2024-04-28 15:00:31.000000 neural-commons-0.3.0/neural_commons/modules/NeuralLayer.py
+-rw-rw-rw-   0        0        0      842 2024-04-28 15:00:31.000000 neural-commons-0.3.0/neural_commons/modules/NeuralLayer2d.py
+-rw-rw-rw-   0        0        0      477 2024-04-07 23:57:05.000000 neural-commons-0.3.0/neural_commons/modules/ParametricReLU.py
+-rw-rw-rw-   0        0        0      225 2024-04-10 19:01:12.000000 neural-commons-0.3.0/neural_commons/modules/Permute.py
+-rw-rw-rw-   0        0        0      286 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/modules/Plus.py
+-rw-rw-rw-   0        0        0      472 2024-04-28 15:00:31.000000 neural-commons-0.3.0/neural_commons/modules/Quadratic.py
+-rw-rw-rw-   0        0        0      235 2024-04-28 15:00:31.000000 neural-commons-0.3.0/neural_commons/modules/RMSELoss.py
+-rw-rw-rw-   0        0        0      470 2024-04-28 15:00:31.000000 neural-commons-0.3.0/neural_commons/modules/RndNonLinearFunction.py
+-rw-rw-rw-   0        0        0     1708 2024-04-07 23:57:05.000000 neural-commons-0.3.0/neural_commons/modules/RndProjection.py
+-rw-rw-rw-   0        0        0     2952 2024-04-08 16:14:56.000000 neural-commons-0.3.0/neural_commons/modules/SMoE.py
+-rw-rw-rw-   0        0        0      750 2024-04-07 23:57:05.000000 neural-commons-0.3.0/neural_commons/modules/SMoEMixIn.py
+-rw-rw-rw-   0        0        0      232 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/modules/View.py
+-rw-rw-rw-   0        0        0      714 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 00:34:04.723748 neural-commons-0.3.0/neural_commons/opt/
+-rw-rw-rw-   0        0        0     1909 2024-04-28 15:00:31.000000 neural-commons-0.3.0/neural_commons/opt/CosineScheduleOptimizer.py
+-rw-rw-rw-   0        0        0     1428 2024-04-28 15:00:31.000000 neural-commons-0.3.0/neural_commons/opt/CosineScheduler.py
+-rw-rw-rw-   0        0        0     2066 2024-04-28 15:00:31.000000 neural-commons-0.3.0/neural_commons/opt/TBCosineScheduleOptimizer.py
+-rw-rw-rw-   0        0        0      174 2024-04-28 15:00:31.000000 neural-commons-0.3.0/neural_commons/opt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 00:34:04.739375 neural-commons-0.3.0/neural_commons/q_nn/
+-rw-rw-rw-   0        0        0     2287 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/q_nn/ParamModule.py
+-rw-rw-rw-   0        0        0     7158 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/q_nn/QGRFOptimizer.py
+-rw-rw-rw-   0        0        0     1196 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/q_nn/QLinear.py
+-rw-rw-rw-   0        0        0      342 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/q_nn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 00:34:04.739375 neural-commons-0.3.0/neural_commons/q_nn/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/q_nn/tests/__init__.py
+-rw-rw-rw-   0        0        0     5786 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/q_nn/tests/test_qgrf_optimizer.py
+-rw-rw-rw-   0        0        0     1073 2024-05-19 22:28:27.000000 neural-commons-0.3.0/neural_commons/q_nn/tests/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-20 00:34:04.680463 neural-commons-0.3.0/neural_commons.egg-info/
+-rw-rw-rw-   0        0        0      745 2024-05-20 00:34:04.000000 neural-commons-0.3.0/neural_commons.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2023 2024-05-20 00:34:04.000000 neural-commons-0.3.0/neural_commons.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 00:34:04.000000 neural-commons-0.3.0/neural_commons.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-05-20 00:34:04.000000 neural-commons-0.3.0/neural_commons.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-20 00:34:04.000000 neural-commons-0.3.0/neural_commons.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 00:34:04.739375 neural-commons-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      969 2024-05-20 00:33:55.000000 neural-commons-0.3.0/setup.py
```

### Comparing `neural-commons-0.2.0/PKG-INFO` & `neural-commons-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-commons
-Version: 0.2.0
+Version: 0.3.0
 Summary: A neural network utility library for PyTorch.
 Author: Jose Solorzano
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.23
```

### Comparing `neural-commons-0.2.0/neural_commons/cf_nn/CFConv2d.py` & `neural-commons-0.3.0/neural_commons/cf_nn/CFConv2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 
     def __init__(self, in_channels: int, out_channels: int,
                  kernel_size: _size_2_t,
                  stride: _size_2_t = 1,
                  padding: _size_2_t = 0,
                  dilation: _size_2_t = 1,
                  bias: bool = True,
+                 norm_output: bool = True,
                  ):
-        super().__init__()
+        super().__init__(norm_output=norm_output)
         if isinstance(kernel_size, int):
             kernel_size = (kernel_size, kernel_size,)
         if isinstance(stride, int):
             stride = (stride, stride,)
         if isinstance(dilation, int):
             dilation = (dilation, dilation,)
         bias_param = None if not bias else torch.randn((out_channels,)) / _sqrt_2
@@ -41,15 +42,15 @@
         self.padding = padding
 
     def forward(self, x: torch.Tensor):
         return torch.conv2d(x, self.weight, self.bias, self.stride, self.padding, self.dilation,
                             groups=1)
 
     def cf_learn(self, inputs: tuple[torch.Tensor, ...], output: torch.Tensor, residual: torch.Tensor,
-                 reg_lambda: float = 1.0, **kwargs):
+                 l2_lambda: float = 1.0, **kwargs):
         has_bias = self.bias is not None
         x = inputs[0]
         # x: (batch_size, in_channels, height, width)
         # residual: (batch_size, out_channels, out_height, out_width)
         batch_size, _, height, width = x.shape
         unfolded_x = F.unfold(x, self.kernel_size, self.dilation, self.padding, self.stride)
         # unfolded_x: (batch_size, 9 * in_channels, height * width // 2)
@@ -60,11 +61,11 @@
         # unfolded_x: (batch_size * out_height * out_width, 9 * in_channels)
         weight = self.weight.view(self.weight.size(0), -1)
         # weight: (out_channels, 9 * in_channels)
         unfolded_residual = torch.permute(residual, (0, 2, 3, 1))
         # unfolded_residual: (batch_size, out_height, out_width, out_channels)
         unfolded_residual = unfolded_residual.contiguous().view(batch_size * unfolded_dim_1, -1)
         # unfolded_residual: (batch_size * out_height * out_width, out_channels)
-        w, b = ridge_regression(unfolded_x, unfolded_residual, bias=has_bias, reg_lambda=reg_lambda)
+        w, b = ridge_regression(unfolded_x, unfolded_residual, bias=has_bias, l2_lambda=l2_lambda)
         weight = weight + w.t()
         self.weight = weight.view(*self.weight.shape)
         self.bias = None if b is None else self.bias + b
```

### Comparing `neural-commons-0.2.0/neural_commons/cf_nn/CFLinear.py` & `neural-commons-0.3.0/neural_commons/cf_nn/CFLinear.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,32 +9,33 @@
 
 
 class CFLinear(CFModule):
     __constants__ = ["in_features", "out_features"]
     weight: torch.Tensor
     bias: torch.Tensor
 
-    def __init__(self, in_features: int, out_features: int, bias: bool = True):
-        super().__init__()
+    def __init__(self, in_features: int, out_features: int, bias: bool = True,
+                 norm_output: bool = True):
+        super().__init__(norm_output=norm_output)
         scale = math.sqrt(in_features)
         if bias:
             scale *= _sqrt_2
         weight = torch.randn((out_features, in_features)) / scale
         bias_param = torch.randn((out_features,)) / _sqrt_2 if bias else None
         self.register_buffer("weight", weight)
         self.register_buffer("bias", bias_param)
         self.in_features = in_features
         self.out_features = out_features
 
     def forward(self, x: torch.Tensor):
         return F.linear(x, self.weight, self.bias)
 
     def cf_learn(self, inputs: tuple[torch.Tensor, ...], output: torch.Tensor, residual: torch.Tensor,
-                 reg_lambda: float = 1.0, **kwargs):
+                 l2_lambda: float = 1.0, **kwargs):
         has_bias = self.bias is not None
         x = inputs[0]
-        w, b = ridge_regression(x, residual, bias=has_bias, reg_lambda=reg_lambda)
+        w, b = ridge_regression(x, residual, bias=has_bias, l2_lambda=l2_lambda)
         self.weight = self.weight + w.t()
         self.bias = None if b is None else self.bias + b
 
     def extra_repr(self) -> str:
         return f'in_features={self.in_features}, out_features={self.out_features}, bias={self.bias is not None}'
```

### Comparing `neural-commons-0.2.0/neural_commons/cf_nn/CFTrainer.py` & `neural-commons-0.3.0/neural_commons/cf_nn/CFOptimizer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,247 +1,233 @@
-import logging
 import math
-from typing import Callable, Any, Optional
-
+from typing import Iterable, Protocol, Union, Optional
 import torch
 from torch import autograd, nn
-from neural_commons.cf_nn import CFModule, LRStrategy
-from neural_commons.helpers.torch_helper import detach_tuple, concatenate_tensors
 
-_logger = logging.getLogger("neural-commons")
+from neural_commons.cf_nn import CFModule
+from neural_commons.helpers.torch_helper import concatenate_tensors, rms
+
+
+class _TLossFn1(Protocol):
+    def __call__(self) -> torch.Tensor:
+        ...
+
+
+class _TLossFn2(Protocol):
+    def __call__(self, **kwargs) -> torch.Tensor:
+        ...
+
+
+_TLossFn = Union[_TLossFn1, _TLossFn2]
 
 
 class InvalidCFStateException(BaseException):
     def __init__(self, msg: str):
         super().__init__(msg)
 
 
-class _CFForwardContext:
-    def __init__(self, trainer: 'CFTrainer'):
-        self.trainer = trainer
-        self.lrs = trainer.lrs
-        self.visits: list[tuple[tuple[torch.Tensor, ...], torch.Tensor]] = list()
+class CFOptimizer:
+    def __init__(self, cf_modules: Iterable[CFModule], stochastic_selection: bool = False):
+        self.cf_modules = list(cf_modules)
+        if len(self.cf_modules) == 0:
+            raise ValueError("Empty collection of ParamModules provided.")
+        self.selected_index = -1
+        self.selected_module: Optional[CFModule] = None
+        self.stochastic_selection = stochastic_selection
+        self.data_queue: list[tuple[tuple[torch.Tensor, ...], torch.Tensor, torch.Tensor]] = list()
+        self._select_next()
+
+    def _full_loss(self, base_loss: torch.Tensor, output: torch.Tensor, std_lambda: float):
+        if not self.selected_module.norm_output:
+            return base_loss
+        extra_loss = (torch.std(output) - 1.0).pow(2) * std_lambda
+        return base_loss + extra_loss
+
+    def _grad_pass(self, fwd_fn: _TLossFn, std_lambda: float,
+                   **kwargs) -> tuple[torch.Tensor, list[tuple[tuple[torch.Tensor, ...], torch.Tensor, torch.Tensor]]]:
+        # Returns list of (input, output, grad)
+        inout_list = list()
+
+        def _hook(m: nn.Module, _inputs: tuple[torch.Tensor, ...], _output: torch.Tensor):
+            new_output = _output.requires_grad_()
+            _in_tuple = tuple(t.detach() for t in _inputs)
+            inout_list.append((_in_tuple, new_output,))
+            return new_output
 
-    @staticmethod
-    def _get_final_output_size(outputs: tuple[torch.Tensor, ...]) -> int:
-        sizes = [math.prod(x.shape[1:]) for x in outputs]
-        if len(sizes) == 1:
-            return sizes[0]
-        elif len(sizes) == 0:
-            raise InvalidCFStateException("Empty tuple. At least one output should be provided.")
-        else:
-            return sum(sizes)
+        sm = self.selected_module
+        h = sm.register_forward_hook(_hook)
+        try:
+            loss = fwd_fn(**kwargs)
+        finally:
+            h.remove()
 
-    @staticmethod
-    def _ref_in_tuple(obj: Any, objects: tuple[Any, ...]) -> bool:
-        for o in objects:
-            if obj is o:
-                return True
-        return False
-
-    def on_visit(self, inputs: tuple[torch.Tensor, ...], output: torch.Tensor):
-        new_output = output.requires_grad_()
-        self.visits.append((inputs, new_output,))
-
-    def register_forward_pass(self, final_outputs: tuple[torch.Tensor, ...],
-                              loss: torch.Tensor, pick_random_visit: bool = False,
-                              update_rate: float = 1.0,
-                              std_lambda: float = 0.03, max_displacement: float = 0.03):
-        if update_rate > 1.0 or update_rate <= 0:
-            raise ValueError("update_rate must be in ]0, 1].")
-        picked_visits = self.visits
-        if len(picked_visits) == 0:
-            raise InvalidCFStateException("No CFModules registered any visits.")
-        if pick_random_visit:
-            index = torch.randint(0, len(picked_visits), size=(1,)).item()
-            picked_visits = [picked_visits[index]]
-        final_output_size = self._get_final_output_size(final_outputs)
-        lrs = self.lrs
-        create_graph = lrs.requires_second_derivative()
-        for inputs, output in picked_visits:
-            is_final_output = self._ref_in_tuple(output, final_outputs)
-            actual_loss = loss
-            if not is_final_output:
-                actual_loss += (torch.std(output) - 1.0).pow(2) * std_lambda
-            grad1 = autograd.grad(actual_loss, output, create_graph=create_graph)[0]
-            raw_residual = lrs.get_residual(is_final_output, output, loss, grad1,
-                                            final_output_size=final_output_size)
-            residual = raw_residual * update_rate
-            if not is_final_output:
-                residual_mag = torch.sqrt(torch.mean(residual.pow(2))).item()
-                if residual_mag > max_displacement:
-                    residual = residual * max_displacement / residual_mag
-            self.trainer.on_forward_pass(detach_tuple(inputs), output.detach(), residual.detach())
-
-
-class _CFTrainContext:
-    def __init__(self, trainer: 'CFTrainer', selected_module: CFModule):
-        self.selected_module = selected_module
-        self.trainer = trainer
-        self.passes: list[tuple[tuple[torch.Tensor, ...], torch.Tensor, torch.Tensor]] = list()
-
-    def register_pass(self, inputs: tuple[torch.Tensor, ...], output: torch.Tensor, residual: torch.Tensor):
-        self.passes.append((inputs, output, residual))
-
-    def get_data_batch(self):
-        if len(self.passes) == 0:
-            raise ValueError("No forward passes registered in current training context.")
-        inputs_c, output_c, residual_c = zip(*self.passes)
-        inputs = concatenate_tensors(inputs_c, dim=0)
-        output = torch.cat(output_c, dim=0)
-        residual = torch.cat(residual_c, dim=0)
-        return inputs, output, residual,
+        result = list()
+        for inputs, output in inout_list:
+            full_loss = self._full_loss(loss, output, std_lambda)
+            grad1 = autograd.grad(full_loss, output)[0]
+            result.append((inputs, output.detach(), grad1.detach()))
+        return loss, result,
+
+    def _lr_loss_grad(self, fwd_fn: _TLossFn, gradients: list[torch.Tensor],
+                      lr: float, std_lambda: float, **kwargs) -> tuple[float, float]:
+        # Returns loss and LR gradient
+        gradient_count = len(gradients)
+        lr_t_list = list()
+
+        def _hook(m: nn.Module, _inputs: tuple[torch.Tensor, ...], _output: torch.Tensor):
+            index = len(lr_t_list)
+            if index >= gradient_count:
+                raise InvalidCFStateException("List of gradients obtained in prior forward "
+                                              "pass is shorter than the number of module "
+                                              "visits in current pass.")
+            lr_t = torch.tensor(lr, dtype=torch.float, device=_output.device).requires_grad_()
+            new_output = _output - lr_t * gradients[index]
+            lr_t_list.append((new_output, lr_t,))
+            return new_output
 
-    def get_total_batch_size(self):
-        return sum([output.size(0) for _, output, _ in self.passes])
+        h = self.selected_module.register_forward_hook(_hook)
+        try:
+            loss = fwd_fn(**kwargs)
+        finally:
+            h.remove()
+
+        lr_count = len(lr_t_list)
+        if lr_count != gradient_count:
+            raise InvalidCFStateException("The number of module visits in current forward pass "
+                                          "does not match those of prior pass.")
+        sum_grad = 0
+        full_loss_sum = 0
+        for output, lr_tensor in lr_t_list:
+            full_loss = self._full_loss(loss, output, std_lambda)
+            grad1 = autograd.grad(full_loss, lr_tensor)[0]
+            sum_grad += grad1.item()
+            full_loss_sum += full_loss.item()
+        return full_loss_sum / lr_count, sum_grad / lr_count,
+
+    def _simple_loss(self, fwd_fn: _TLossFn, gradients: list[torch.Tensor],
+                     lr: float, std_lambda: float, **kwargs) -> float:
+        gradient_count = len(gradients)
+        out_list = list()
+
+        def _hook(m: nn.Module, _inputs: tuple[torch.Tensor, ...], _output: torch.Tensor):
+            index = len(out_list)
+            if index >= gradient_count:
+                raise InvalidCFStateException("List of gradients obtained in prior forward "
+                                              "pass is shorter than the number of module "
+                                              "visits in current pass.")
+            new_output = _output - lr * gradients[index]
+            out_list.append(new_output)
+            return new_output
 
-    def train_step(self, **kwargs):
         with torch.no_grad():
-            inputs, output, residual = self.get_data_batch()
-            self.selected_module.cf_learn(inputs, output, residual, **kwargs)
+            h = self.selected_module.register_forward_hook(_hook)
+            try:
+                loss = fwd_fn(**kwargs)
+            finally:
+                h.remove()
+            num_outputs = len(out_list)
+            if num_outputs != gradient_count:
+                raise InvalidCFStateException("The number of module visits in current forward pass "
+                                              "does not match those of prior pass.")
+            full_loss_sum = 0
+            for output in out_list:
+                full_loss = self._full_loss(loss, output, std_lambda)
+                full_loss_sum += full_loss.item()
+            return full_loss_sum / num_outputs
 
+    @staticmethod
+    def _optimal_lr(lr1: float, lr2: float, lr_loss1: float, lr_loss2: float,
+                    lr_grad1: float, lr_grad2: float, lr_expansion=2.0,
+                    grad_reduction_threshold=0.03) -> tuple[float, Optional[float]]:
+        if math.isinf(lr_grad2) or math.isnan(lr_grad2):
+            return lr1, 1.0 / lr_expansion,
+        elif math.copysign(1, lr_grad1) != math.copysign(1, lr_grad2):
+            # Secant root-finding method
+            return (lr1 * lr_grad2 - lr2 * lr_grad1) / (lr_grad2 - lr_grad1), None,
+        elif lr_loss2 == lr_loss1:
+            return lr1, 1.0,
+        elif lr_loss2 < lr_loss1:
+            if abs(lr_grad2) < abs(lr_grad1) * grad_reduction_threshold:
+                return lr2, 1.0,
+            else:
+                return lr2, lr_expansion,
+        else:
+            return lr1, 1.0 / lr_expansion,
 
-class CFTrainer:
-    def __init__(self, *root_modules: nn.Module, lrs: LRStrategy,
-                 rnd_module_selection: bool = False):
-        """
-        Constructs a CFTrainer instance.
-        Args:
-            *root_modules: The root module or modules of the trained model.
-            lrs: An instance of a class that extends LRStrategy. It implements a learning-rate strategy for
-            loss minimization in the layer output space.
-            rnd_module_selection: Whether modules are selected at random at every pass, rather than in
-            a round-robin fashion.
-        """
-        super().__init__()
-        self.rnd_module_selection = rnd_module_selection
-        self.lrs = lrs
-        all_modules = list()
-        for root in root_modules:
-            modules = root.modules()
-            modules = [m for m in modules if isinstance(m, CFModule)]
-            all_modules.extend(modules)
-        n = len(all_modules)
-        if n <= 0:
-            raise ValueError(f"No modules of type {CFModule.__name__} found!")
-        self.modules = all_modules
-        self.index = -1
-        self.hooks = list()
-        self._fwd_context: Optional[_CFForwardContext] = None
-        self._train_context: Optional[_CFTrainContext] = None
-        self._warned_eval = False
-        self._hooks_enabled = True
-
-    def __enter__(self):
-        self._fwd_context = self._new_forward_context()
-        self._train_context = self._new_train_context()
-        self.hooks = list()
-        for module in self.modules:
-            h = module.register_forward_hook(self._fwd_hook)
-            self.hooks.append(h)
-        return self
+    def _update_sm_lr(self, lr: float, prior_approx_lr: float, approx_lr_expansion: float,
+                      out_size: int):
+        if approx_lr_expansion is not None:
+            new_approx_lr = prior_approx_lr * approx_lr_expansion
+        else:
+            new_approx_lr = lr
+        self.selected_module.update_lr_factor(new_approx_lr / out_size)
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        for h in self.hooks:
-            h.remove()
+    def _select_next(self):
+        cf_modules = self.cf_modules
+        num_modules = len(cf_modules)
+        if self.stochastic_selection:
+            m_lr = [m.lr_factor_ma for m in cf_modules]
+            m_lr = torch.tensor(m_lr, dtype=torch.float)
+            m_weight = torch.ones_like(m_lr)
+            self.selected_index = torch.multinomial(m_weight, 1).item()
+        else:
+            self.selected_index = (self.selected_index + 1) % num_modules
+        self.selected_module = cf_modules[self.selected_index]
 
-    @property
-    def queued_forward_pass_count(self) -> int:
-        """
-        Returns: The number of queued forward passes since the last training step.
-        """
-        if self._train_context is None:
-            raise InvalidCFStateException("queued_forward_pass_count not available outside of CFTrainer context.")
-        return len(self._train_context.passes)
+    def enqueue_data(self, fwd_fn: _TLossFn, std_lambda: float = 0.0001,
+                     lr_expansion=2.0, **kwargs) -> float:
+        loss, pass_info = self._grad_pass(fwd_fn, std_lambda, **kwargs)
+        loss = loss.item()
+        gradients = [g for _, _, g in pass_info]
+        outputs = [out for _, out, _ in pass_info]
+        if len(outputs) == 0:
+            raise InvalidCFStateException("CFModule instances not visited in forward pass.")
+        sm = self.selected_module
+        out_size = torch.numel(outputs[0])
+        approx_lr = sm.lr_factor_ma * out_size
+        lr1 = 0
+        lr2 = approx_lr * 2.0
+        lr_loss1, lr_grad1 = self._lr_loss_grad(fwd_fn, gradients, lr1, std_lambda, **kwargs)
+        lr_loss2, lr_grad2 = self._lr_loss_grad(fwd_fn, gradients, lr2, std_lambda, **kwargs)
+        opt_lr, approx_lr_expansion = self._optimal_lr(lr1, lr2, lr_loss1, lr_loss2, lr_grad1, lr_grad2)
+        if approx_lr_expansion is None:
+            opt_loss = self._simple_loss(fwd_fn, gradients, opt_lr, std_lambda, **kwargs)
+            if opt_loss > lr_loss1:
+                # Failed to decrease loss. Reduce approx LR.
+                opt_lr = lr1
+                approx_lr_expansion = 1.0 / lr_expansion
+        self._update_sm_lr(opt_lr, approx_lr, approx_lr_expansion, out_size)
+        if opt_lr != 0:
+            for inputs, output, gradient in pass_info:
+                residual = (-gradient * opt_lr).detach()
+                self.data_queue.append((inputs, output, residual,))
+        return loss
 
     @property
-    def queued_forward_pass_batch_size(self) -> int:
-        """
-        Returns: The cumulative batch size of all forward passes since the last training step.
-        """
-        if self._train_context is None:
-            raise InvalidCFStateException("queued_forward_pass_batch_size not available outside of CFTrainer context.")
-        return self._train_context.get_total_batch_size()
-
-    def set_hooks_enabled(self, mode: bool):
-        self._hooks_enabled = mode
-
-    def _fwd_hook(self, module: nn.Module, inputs: tuple[torch.Tensor, ...], output: torch.Tensor):
-        if self._hooks_enabled:
-            sm = self._train_context.selected_module
-            if module is sm:
-                if not sm.training:
-                    if not self._warned_eval:
-                        _logger.warning("Selected module visited in eval mode. "
-                                        "To run validation in a CFTrainer context, disable hooks.")
-                        self._warned_eval = True
-                self._fwd_context.on_visit(inputs, output)
-
-    def _next_module(self) -> CFModule:
-        if self.rnd_module_selection:
-            next_index = torch.randint(0, len(self.modules), size=(1,)).item()
-        else:
-            next_index = self.index + 1
-            if next_index >= len(self.modules):
-                next_index = 0
-        self.index = next_index
-        return self.modules[next_index]
-
-    def _new_forward_context(self) -> _CFForwardContext:
-        return _CFForwardContext(self)
-
-    def _new_train_context(self) -> _CFTrainContext:
-        return _CFTrainContext(self, self._next_module())
-
-    def _register_forward_pass_impl(self, outputs: tuple[torch.Tensor, ...], loss: torch.Tensor,
-                                    update_rate: float, std_lambda: float, max_displacement: float):
-        self._fwd_context.register_forward_pass(outputs, loss, update_rate=update_rate,
-                                                std_lambda=std_lambda,
-                                                max_displacement=max_displacement)
-
-    def register_forward_pass(self, outputs: tuple[torch.Tensor, ...], loss: torch.Tensor,
-                              update_rate: float = 1.0,
-                              std_lambda: float = 0.001, max_displacement: float = 0.03):
-        """
-        Call after a forward pass to estimate gradients and residuals of the selected layer's output.
-        These results are queued until they get processed in the next training step.
-        Args:
-            outputs: A tuple of model outputs. These should be the outputs used to calculate the loss,
-            and they should be direct outputs of a module that extends `CFModule`.
-            loss: The loss that needs to be minimized.
-            update_rate: A factor between 0 and 1 that is multiplied by the estimated residual.
-            std_lambda: A parameter multiplied by an internal loss function that tries to maintain the
-            standard deviation of internal layer outputs at 1.
-            max_displacement: Output residuals are trimmed such that their root mean square (RMS)
-            does not exceed this number.
-
-        """
-        if self._fwd_context is None:
-            raise InvalidCFStateException("Call to register_forward_pass() outside of CFTrainer context.")
-        try:
-            self._register_forward_pass_impl(outputs, loss, update_rate=update_rate, std_lambda=std_lambda,
-                                             max_displacement=max_displacement)
-        finally:
-            self._fwd_context = self._new_forward_context()
+    def queued_batch_size(self) -> int:
+        return sum(output.size(0) for _, output, _ in self.data_queue)
 
-    def on_forward_pass(self, inputs: tuple[torch.Tensor, ...], output: torch.Tensor, residual: torch.Tensor):
-        if self._train_context is None:
-            raise InvalidCFStateException("Call to on_forward_pass() outside of CFTrainer context.")
-        self._train_context.register_pass(inputs, output, residual)
-
-    def _train_step_impl(self, **kwargs):
-        self._train_context.train_step(**kwargs)
-
-    def train_step(self, **kwargs):
-        """
-        Collects data from queued forward passes, invokes a learning method of the selected
-        `CFModule` instance, clears the forward pass queue, and selects the next CF module.
-        Args:
-            **kwargs: Arguments passed to `CFModule` instances. For example, `reg_lambda` is a
-            parameter used by `CFLinear`.
-        """
-        if self._train_context is None:
-            raise InvalidCFStateException("Call to train_step() outside of CFTrainer context.")
+    def _step(self, update_rate: float, max_residual_rel_rms: float, **kwargs):
+        if len(self.data_queue) == 0:
+            raise InvalidCFStateException("No data has been queued. Call enqueue_data() before calling step().")
+        inputs_list = [i for i, _, _ in self.data_queue]
+        output_list = [out for _, out, _ in self.data_queue]
+        residual_list = [res for _, _, res in self.data_queue]
+        with torch.no_grad():
+            inputs = concatenate_tensors(inputs_list, dim=0)
+            output = torch.cat(output_list, dim=0)
+            residual = torch.cat(residual_list, dim=0)
+            partial_residual = residual * update_rate
+            max_pr_rms = rms(output) * max_residual_rel_rms
+            pr_rms = rms(partial_residual)
+            if pr_rms > max_pr_rms:
+                partial_residual *= max_pr_rms / pr_rms
+            self.selected_module.cf_learn(inputs, output, partial_residual, **kwargs)
+
+    def step(self, update_rate: float = 1.0, max_residual_rel_rms = 1.0, **kwargs):
+        if update_rate <= 0 or update_rate > 1.0:
+            raise ValueError("update_rate expected to be in ]0, 1].")
         try:
-            self._train_step_impl(**kwargs)
+            self._step(update_rate, max_residual_rel_rms, **kwargs)
         finally:
-            self._train_context = self._new_train_context()
+            self.data_queue = list()
+            self._select_next()
```

### Comparing `neural-commons-0.2.0/neural_commons/cf_nn/lrs/CrossEntropyLossLRS.py` & `neural-commons-0.3.0/neural_commons/cf_nn/lrs/CrossEntropyLossLRS.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-import datetime
 import math
-import os
 
 import torch
 from neural_commons.cf_nn import LRStrategy
+from neural_commons.cf_nn.lrs import SlideLRS
+
+_slide_factor = 10.0
 
 
 class CrossEntropyLossLRS(LRStrategy):
-    def __init__(self):
+    def __init__(self, min_loss: float = 0):
         super().__init__()
+        self.slide_lrs = SlideLRS(min_loss=min_loss)
 
     def requires_second_derivative(self) -> bool:
         return False
 
     def get_residual(self, is_final: bool, output: torch.Tensor, loss: torch.Tensor, grad1: torch.Tensor,
                      final_output_size: int):
-        batch_size = output.size(0)
         output_size = math.prod(output.shape[1:])
-        fos = output_size if is_final else final_output_size
-        base_result = 1.5 * batch_size * fos
         if is_final:
-            lr = base_result
+            lr = 1.0 * output_size
         else:
             factor_min = 1.0
-            factor_max = 14.0
-            partial_os = output_size / 3
+            factor_max = 10.0
+            partial_os = output_size / 2
             max_w = partial_os / (partial_os + final_output_size)
             factor = factor_min * (1 - max_w) + factor_max * max_w
-            lr = factor * base_result
+            lr = factor * final_output_size
         return -lr * grad1
+
```

### Comparing `neural-commons-0.2.0/neural_commons/cf_nn/lrs/MSELossLRS.py` & `neural-commons-0.3.0/neural_commons/cf_nn/lrs/MSELossLRS.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,14 +18,14 @@
         batch_size = output.size(0)
         output_size = math.prod(output.shape[1:])
         fos = output_size if is_final else final_output_size
         base_result = 0.5 * batch_size * fos
         if is_final:
             lr = base_result
         else:
-            factor_min = 0.5
+            factor_min = 1.0
             factor_max = 10.0
-            partial_os = output_size / 3
+            partial_os = output_size / 2
             max_w = partial_os / (partial_os + final_output_size)
             factor = factor_min * (1 - max_w) + factor_max * max_w
             lr = factor * base_result
         return -lr * grad1
```

### Comparing `neural-commons-0.2.0/neural_commons/helpers/torch_helper.py` & `neural-commons-0.3.0/neural_commons/helpers/torch_helper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math
-from typing import Iterable, Optional
+from typing import Iterable, Optional, Union, Sequence
 import numpy as np
 import torch
-from torch import nn
+from torch import nn, autograd, vmap
 import torch.nn.functional as F
 
 _sqrt_2 = math.sqrt(2)
 
 
 def count_parameters(model):
     return sum(p.numel() for p in model.parameters() if p.requires_grad)
@@ -78,33 +78,33 @@
     if hasattr(torch, dtype_str):
         return getattr(torch, dtype_str)
     else:
         raise ValueError(f"Unknown dtype string: {dtype_str}")
 
 
 def ridge_regression(x: torch.Tensor, y: torch.Tensor, bias: bool = True,
-                     reg_lambda: float = 1e-5) -> tuple[torch.Tensor, torch.Tensor]:
+                     l2_lambda: float = 1e-5) -> tuple[torch.Tensor, torch.Tensor]:
     """
     Performs ridge regression.
     Args:
         x: Input variables.
         y: Output variables.
         bias: Whether a bias parameter should be returned.
-        reg_lambda: An L2 regularization parameter.
+        l2_lambda: An L2 regularization parameter.
     Returns: A weight matrix of shape (in_features, out_features), and a bias parameter
     array of size (out_features) if the bias parameter is True.
     """
     with torch.no_grad():
         dev = x.device
         x_actual = x if not bias else torch.cat([x, torch.ones((x.size(0), 1),
                                                                device=dev)], dim=1)
         x_t = x_actual.t()
         sq_matrix = x_t @ x_actual
         weights = torch.inverse(
-            sq_matrix + reg_lambda * torch.eye(x_t.size(0), device=dev)) @ x_t @ y
+            sq_matrix + l2_lambda * torch.eye(x_t.size(0), device=dev)) @ x_t @ y
         # weights: (in_features, out_features)
         bias_param = torch.clone(weights[-1, :]) if bias else None
         if bias:
             weights = weights[:-1, :]
         return weights, bias_param,
 
 
@@ -125,7 +125,38 @@
         mean = 0 if zero_based else torch.mean(sub_tensor).item()
         sd = torch.sqrt(torch.mean((sub_tensor - mean).pow(2)))
         z_score = torch.abs(tensor - mean) / torch.clamp(sd, min=eps)
         is_outlier = z_score >= z_score_threshold
     tensor_copy = torch.clone(tensor)
     tensor_copy[is_outlier] = mean + torch.sign(tensor_copy[is_outlier] - mean) * sd * z_score_threshold
     return tensor_copy
+
+
+def ps_grad(outputs: torch.Tensor, inputs: Union[torch.Tensor, Sequence[torch.Tensor]],
+            create_graph: bool = False,
+            retain_graph: bool = False) -> tuple[torch.Tensor, ...]:
+    """
+    Per-sample gradients given per-sample outputs/loss.
+    """
+    return autograd.grad(outputs.sum(), inputs, create_graph=create_graph,
+                         retain_graph=retain_graph)
+
+
+def view_dims(t: torch.Tensor, n_dims: int):
+    s = t.size()
+    num_existing = len(s)
+    if num_existing > n_dims:
+        raise ValueError(f"Provided tensor already has more than {n_dims} axes.")
+    return t.view(s + (1,) * (n_dims - num_existing))
+
+
+def dims_from(t: torch.Tensor, start_dim: int = 1):
+    n = len(t.size())
+    return tuple(range(start_dim, n))
+
+
+def num_dims(t: torch.Tensor):
+    return len(t.size())
+
+
+def rms(t: torch.Tensor):
+    return torch.sqrt(torch.mean(t.pow(2)))
```

### Comparing `neural-commons-0.2.0/neural_commons/modules/AdaptiveSimpleNorm.py` & `neural-commons-0.3.0/neural_commons/modules/AdaptiveSimpleNorm.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.2.0/neural_commons/modules/ConvMixer2d.py` & `neural-commons-0.3.0/neural_commons/modules/ConvMixer2d.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.2.0/neural_commons/modules/InputEncoder.py` & `neural-commons-0.3.0/neural_commons/modules/InputEncoder.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.2.0/neural_commons/modules/NeuralLayer.py` & `neural-commons-0.3.0/neural_commons/modules/NeuralLayer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.2.0/neural_commons/modules/NeuralLayer2d.py` & `neural-commons-0.3.0/neural_commons/modules/NeuralLayer2d.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.2.0/neural_commons/modules/RndProjection.py` & `neural-commons-0.3.0/neural_commons/modules/RndProjection.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.2.0/neural_commons/modules/SMoE.py` & `neural-commons-0.3.0/neural_commons/modules/SMoE.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.2.0/neural_commons/modules/SMoEMixIn.py` & `neural-commons-0.3.0/neural_commons/modules/SMoEMixIn.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.2.0/neural_commons/opt/CosineScheduleOptimizer.py` & `neural-commons-0.3.0/neural_commons/opt/CosineScheduleOptimizer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.2.0/neural_commons/opt/CosineScheduler.py` & `neural-commons-0.3.0/neural_commons/opt/CosineScheduler.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.2.0/neural_commons/opt/TBCosineScheduleOptimizer.py` & `neural-commons-0.3.0/neural_commons/opt/TBCosineScheduleOptimizer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.2.0/neural_commons.egg-info/PKG-INFO` & `neural-commons-0.3.0/neural_commons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-commons
-Version: 0.2.0
+Version: 0.3.0
 Summary: A neural network utility library for PyTorch.
 Author: Jose Solorzano
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.23
```

### Comparing `neural-commons-0.2.0/neural_commons.egg-info/SOURCES.txt` & `neural-commons-0.3.0/neural_commons.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,43 +5,52 @@
 neural_commons.egg-info/SOURCES.txt
 neural_commons.egg-info/dependency_links.txt
 neural_commons.egg-info/requires.txt
 neural_commons.egg-info/top_level.txt
 neural_commons/cf_nn/CFConv2d.py
 neural_commons/cf_nn/CFLinear.py
 neural_commons/cf_nn/CFModule.py
-neural_commons/cf_nn/CFTrainer.py
-neural_commons/cf_nn/LRStrategy.py
+neural_commons/cf_nn/CFOptimizer.py
 neural_commons/cf_nn/__init__.py
+neural_commons/cf_nn/lrs/AdaptiveLRS.py
 neural_commons/cf_nn/lrs/CrossEntropyLossLRS.py
 neural_commons/cf_nn/lrs/MSELossLRS.py
 neural_commons/cf_nn/lrs/SlideLRS.py
 neural_commons/cf_nn/lrs/__init__.py
-neural_commons/cf_nn/lrs/tests/__init__.py
-neural_commons/cf_nn/lrs/tests/test_slide_lrs.py
 neural_commons/cf_nn/tests/__init__.py
-neural_commons/cf_nn/tests/test_cf_conv2d.py
-neural_commons/cf_nn/tests/test_cf_linear.py
+neural_commons/cf_nn/tests/test_cf_optimizer.py
+neural_commons/cf_nn/tests/utils.py
 neural_commons/helpers/__init__.py
 neural_commons/helpers/torch_helper.py
 neural_commons/modules/AdaptiveSimpleNorm.py
+neural_commons/modules/ArgMax.py
 neural_commons/modules/ConvMixer2d.py
 neural_commons/modules/GTanh.py
 neural_commons/modules/GaELU.py
+neural_commons/modules/GaussianNoise.py
 neural_commons/modules/InputEncoder.py
 neural_commons/modules/LogShape.py
 neural_commons/modules/MAELoss.py
 neural_commons/modules/NeuralLayer.py
 neural_commons/modules/NeuralLayer2d.py
 neural_commons/modules/ParametricReLU.py
 neural_commons/modules/Permute.py
+neural_commons/modules/Plus.py
 neural_commons/modules/Quadratic.py
 neural_commons/modules/RMSELoss.py
 neural_commons/modules/RndNonLinearFunction.py
 neural_commons/modules/RndProjection.py
 neural_commons/modules/SMoE.py
 neural_commons/modules/SMoEMixIn.py
+neural_commons/modules/View.py
 neural_commons/modules/__init__.py
 neural_commons/opt/CosineScheduleOptimizer.py
 neural_commons/opt/CosineScheduler.py
 neural_commons/opt/TBCosineScheduleOptimizer.py
-neural_commons/opt/__init__.py
+neural_commons/opt/__init__.py
+neural_commons/q_nn/ParamModule.py
+neural_commons/q_nn/QGRFOptimizer.py
+neural_commons/q_nn/QLinear.py
+neural_commons/q_nn/__init__.py
+neural_commons/q_nn/tests/__init__.py
+neural_commons/q_nn/tests/test_qgrf_optimizer.py
+neural_commons/q_nn/tests/utils.py
```

### Comparing `neural-commons-0.2.0/setup.py` & `neural-commons-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import codecs
 
 from setuptools import setup, find_packages
 
 # Define project metadata
 NAME = 'neural-commons'
-VERSION = '0.2.0'
+VERSION = '0.3.0'
 DESCRIPTION = 'A neural network utility library for PyTorch.'
 AUTHOR = 'Jose Solorzano'
 
 REQUIRES = [
     'numpy>=1.23',
     'tqdm>=4.0.0',
     'torch>=2.1.0',
```

