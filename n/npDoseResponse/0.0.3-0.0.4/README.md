# Comparing `tmp/npdoseresponse-0.0.3.tar.gz` & `tmp/npdoseresponse-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npdoseresponse-0.0.3.tar", last modified: Mon May 13 19:35:34 2024, max compression
+gzip compressed data, was "npdoseresponse-0.0.4.tar", last modified: Sun May 19 23:03:32 2024, max compression
```

## Comparing `npdoseresponse-0.0.3.tar` & `npdoseresponse-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-13 19:35:34.444910 npdoseresponse-0.0.3/
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1070 2024-05-07 04:36:16.000000 npdoseresponse-0.0.3/LICENSE
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1928 2024-05-13 19:35:34.444302 npdoseresponse-0.0.3/PKG-INFO
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1428 2024-05-13 19:23:52.000000 npdoseresponse-0.0.3/README.md
-drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-13 19:35:34.439766 npdoseresponse-0.0.3/npDoseResponse/
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)      211 2024-05-13 19:35:15.000000 npdoseresponse-0.0.3/npDoseResponse/__init__.py
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)    22845 2024-05-13 01:22:31.000000 npdoseresponse-0.0.3/npDoseResponse/npDoseResponse.py
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     2837 2024-05-13 01:23:42.000000 npdoseresponse-0.0.3/npDoseResponse/rbf.py
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     5430 2024-05-12 19:21:37.000000 npdoseresponse-0.0.3/npDoseResponse/utils.py
-drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-13 19:35:34.443759 npdoseresponse-0.0.3/npDoseResponse.egg-info/
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1928 2024-05-13 19:35:34.000000 npdoseresponse-0.0.3/npDoseResponse.egg-info/PKG-INFO
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)      321 2024-05-13 19:35:34.000000 npdoseresponse-0.0.3/npDoseResponse.egg-info/SOURCES.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)        1 2024-05-13 19:35:34.000000 npdoseresponse-0.0.3/npDoseResponse.egg-info/dependency_links.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)       12 2024-05-13 19:35:34.000000 npdoseresponse-0.0.3/npDoseResponse.egg-info/requires.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)       15 2024-05-13 19:35:34.000000 npdoseresponse-0.0.3/npDoseResponse.egg-info/top_level.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)       38 2024-05-13 19:35:34.445093 npdoseresponse-0.0.3/setup.cfg
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)      805 2024-05-13 19:35:18.000000 npdoseresponse-0.0.3/setup.py
+drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-19 23:03:32.984838 npdoseresponse-0.0.4/
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1070 2024-05-07 04:36:16.000000 npdoseresponse-0.0.4/LICENSE
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     2141 2024-05-19 23:03:32.983833 npdoseresponse-0.0.4/PKG-INFO
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1641 2024-05-18 23:50:54.000000 npdoseresponse-0.0.4/README.md
+drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-19 23:03:32.978672 npdoseresponse-0.0.4/npDoseResponse/
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)      211 2024-05-19 22:54:58.000000 npdoseresponse-0.0.4/npDoseResponse/__init__.py
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)    24960 2024-05-19 22:39:45.000000 npdoseresponse-0.0.4/npDoseResponse/npDoseResponse.py
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     5934 2024-05-19 22:45:09.000000 npdoseresponse-0.0.4/npDoseResponse/rbf.py
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     5929 2024-05-19 22:42:14.000000 npdoseresponse-0.0.4/npDoseResponse/utils.py
+drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-19 23:03:32.983206 npdoseresponse-0.0.4/npDoseResponse.egg-info/
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     2141 2024-05-19 23:03:32.000000 npdoseresponse-0.0.4/npDoseResponse.egg-info/PKG-INFO
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)      321 2024-05-19 23:03:32.000000 npdoseresponse-0.0.4/npDoseResponse.egg-info/SOURCES.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)        1 2024-05-19 23:03:32.000000 npdoseresponse-0.0.4/npDoseResponse.egg-info/dependency_links.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)       12 2024-05-19 23:03:32.000000 npdoseresponse-0.0.4/npDoseResponse.egg-info/requires.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)       15 2024-05-19 23:03:32.000000 npdoseresponse-0.0.4/npDoseResponse.egg-info/top_level.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)       38 2024-05-19 23:03:32.984962 npdoseresponse-0.0.4/setup.cfg
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)      805 2024-05-19 22:54:36.000000 npdoseresponse-0.0.4/setup.py
```

### Comparing `npdoseresponse-0.0.3/LICENSE` & `npdoseresponse-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `npdoseresponse-0.0.3/PKG-INFO` & `npdoseresponse-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npDoseResponse
-Version: 0.0.3
+Version: 0.0.4
 Summary: Nonparametric Estimation and Inference on Dose-Response Curves
 Home-page: https://github.com/zhangyk8/npDoseResponse
 Author: Yikun Zhang
 Author-email: yikunzhang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,9 +38,9 @@
 ```
 pip install npDoseResponse
 ```
 
 References
 --------
 
-
+<a name="npdoseresponse">[1]</a> Y. Zhang, Y.-C. Chen, and A. Giessing (2024+) Nonparametric Inference on Dose-Response Curves Without the Positivity Condition [arXiv:2405.09003](https://arxiv.org/abs/2405.09003).
```

### Comparing `npdoseresponse-0.0.3/README.md` & `npdoseresponse-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -23,9 +23,9 @@
 ```
 pip install npDoseResponse
 ```
 
 References
 --------
 
-
+<a name="npdoseresponse">[1]</a> Y. Zhang, Y.-C. Chen, and A. Giessing (2024+) Nonparametric Inference on Dose-Response Curves Without the Positivity Condition [arXiv:2405.09003](https://arxiv.org/abs/2405.09003).
```

### Comparing `npdoseresponse-0.0.3/npDoseResponse/npDoseResponse.py` & `npdoseresponse-0.0.4/npDoseResponse/npDoseResponse.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 
 # Author: Yikun Zhang
-# Last Editing: May 12, 2024
+# Last Editing: May 19, 2024
 
 # Description: This script contains the implementation of local polynomial regression 
 # as well as our proposed integral estimator and its localized derivative estimator.
 
 import numpy as np
 from .rbf import KernelRetrieval
 from multiprocessing import Pool
 from functools import partial
 from .utils import *
 
 #=======================================================================================#
 
-def LocalPolyReg(Y, X, x_eval=None, degree=2, deriv_ord=1, h=None, b=None, 
-                 kernT="epanechnikov", kernS="epanechnikov", 
+def LocalPolyReg(Y, X, x_eval=None, degree=2, deriv_ord=1, h=None, b=None, C_h=7, 
+                 C_b=3, kernT="epanechnikov", kernS="epanechnikov", 
                  h_lst=np.linspace(0.5, 15, 30), b_lst=np.linspace(0.2, 6, 30)):
     '''
     (Partial) Local polynomial regression for estimating the conditional mean outcome 
     function and its partial derivatives. We use higher order local monomials for 
     the treatment variable and first-order local monomials for the confounding variables.
     
     
@@ -44,30 +44,40 @@
             function. (Default: deriv_ord=1. Then, it estimates the partial 
             derivative of the conditional mean outcome function with respect to 
             the treatment variable.)
             
         h,b: float
             The bandwidth parameters for the treatment/exposure variable and 
             confounding variables. (Default: h=None, b=None. Then, the rule-of-thumb 
-            bandwidth selector in Eq.(A1) of Yang and Tschernig (1999) is used.)
+            bandwidth selector in Eq.(A1) of Yang and Tschernig (1999) is used 
+            with additional scaling factors C_h and C_b, respectively.)
             
         kernT, kernS: str
             The names of kernel functions for the treatment/exposure variable 
             and confounding variables. (Default: "epanechnikov".)
+            
+        h_lst, b_lst: (k1,)-array and (k2,)-array
+            Candidate searching values of h,b for LOOCV.
+            
+    Return
+    ----------
+        Y_est: (m,)-array
+            The estimated conditional mean outcome function or its partial derivatives 
+            evaluated at points "x_eval".
     '''
     if x_eval is None: 
         x_eval = X.copy()
         
     if (h is None) and (b is None):
         # Apply the rule-of-thumb bandwidth selector in Eq.(A1) of Yang and Tschernig (1999)
-        h, b = RoTBWLocalPoly(Y, X, kernT=kernT, kernS=kernS)
+        h, b = RoTBWLocalPoly(Y, X, kernT=kernT, kernS=kernS, C_h=C_h, C_b=C_b)
     elif h is None:
-        h, b_can = RoTBWLocalPoly(Y, X, kernT=kernT, kernS=kernS)
+        h, b_can = RoTBWLocalPoly(Y, X, kernT=kernT, kernS=kernS, C_h=C_h, C_b=C_b)
     elif b is None:
-        h_can, b = RoTBWLocalPoly(Y, X, kernT=kernT, kernS=kernS)
+        h_can, b = RoTBWLocalPoly(Y, X, kernT=kernT, kernS=kernS, C_h=C_h, C_b=C_b)
         
     if (h == "cv") and (b == "cv"):
         cv_mse = np.zeros((len(h_lst), len(b_lst)))
         for i in range(len(h_lst)):
             for j in range(len(b_lst)):
                 Y_reg_est = LocalPolyRegMain(Y, X, x_eval=X, degree=1, deriv_ord=0, 
                                              h=h_lst[i], b=b_lst[i], 
@@ -115,20 +125,25 @@
             The order of the estimated derivative the conditional mean outcome 
             function. (Default: deriv_ord=1. Then, it estimates the partial 
             derivative of the conditional mean outcome function with respect to 
             the treatment variable.)
             
         h,b: float
             The bandwidth parameters for the treatment/exposure variable and 
-            confounding variables. (Default: h=None, b=None. Then, the rule-of-thumb 
-            bandwidth selector in Eq.(A1) of Yang and Tschernig (1999) is used.)
+            confounding variables.
             
         kernT, kernS: str
             The names of kernel functions for the treatment/exposure variable 
             and confounding variables. (Default: "epanechnikov".)
+            
+    Return
+    ----------
+        Y_est: (m,)-array
+            The estimated conditional mean outcome function or its partial derivatives 
+            evaluated at points "x_eval".
     '''
     kernT, sigmaK_sq, K_sq = KernelRetrieval(kernT)
     kernS, sigmaK_sq, K_sq = KernelRetrieval(kernS)
     
     n = X.shape[0]  ## Number of data points
     d = X.shape[1] - 1
     Y_est = np.zeros((x_eval.shape[0],))
@@ -146,24 +161,23 @@
         rhs = weight_sqrt*Y[inds]
         rcond = np.finfo(lhs.dtype).eps * max(*lhs.shape)
         beta = np.linalg.lstsq(lhs, rhs, rcond=rcond)[0]
         Y_est[i] = np.math.factorial(deriv_ord)*beta[deriv_ord]
     return Y_est
 
 
-def LocalPolyReg_Fs(x_eval, Y, X, degree=2, deriv_ord=1, h=None, b=None, 
-                 kernT="epanechnikov", kernS="epanechnikov", 
-                 h_lst=np.linspace(0.5, 15, 30), b_lst=np.linspace(0.2, 6, 30)):
+def LocalPolyReg_Fs(x_eval, Y, X, degree=2, deriv_ord=1, h=None, b=None, C_h=7, 
+                    C_b=3, kernT="epanechnikov", kernS="epanechnikov", 
+                    h_lst=np.linspace(0.5, 15, 30), b_lst=np.linspace(0.2, 6, 30)):
     '''
     (Partial) Local polynomial regression for estimating the conditional mean outcome 
     function and its partial derivatives. We use higher order local monomials for 
     the treatment variable and first-order local monomials for the confounding variables.
     (This function is for multi-process execution only.)
     
-    
     Parameters
     ----------
         Y: (n,)-array
             The outcomes of n observations.
         
         X: (n,d+1)-array
             The first column of X is the treatment/exposure variable, while 
@@ -181,30 +195,40 @@
             function. (Default: deriv_ord=1. Then, it estimates the partial 
             derivative of the conditional mean outcome function with respect to 
             the treatment variable.)
             
         h,b: float
             The bandwidth parameters for the treatment/exposure variable and 
             confounding variables. (Default: h=None, b=None. Then, the rule-of-thumb 
-            bandwidth selector in Eq.(A1) of Yang and Tschernig (1999) is used.)
+            bandwidth selector in Eq.(A1) of Yang and Tschernig (1999) is used
+            with additional scaling factors C_h and C_b, respectively.)
             
         kernT, kernS: str
             The names of kernel functions for the treatment/exposure variable 
             and confounding variables. (Default: "epanechnikov".)
+            
+        h_lst, b_lst: (k1,)-array and (k2,)-array
+            Candidate searching values of h,b for LOOCV.
+            
+    Return
+    ----------
+        Y_est: (m,)-array
+            The estimated conditional mean outcome function or its partial derivatives 
+            evaluated at points "x_eval".
     '''
     if x_eval is None: 
         x_eval = X.copy()
         
     if (h is None) and (b is None):
         # Apply the rule-of-thumb bandwidth selector in Eq.(A1) of Yang and Tschernig (1999)
-        h, b = RoTBWLocalPoly(Y, X, kernT=kernT, kernS=kernS)
+        h, b = RoTBWLocalPoly(Y, X, kernT=kernT, kernS=kernS, C_h=C_h, C_b=C_b)
     elif h is None:
-        h, b_can = RoTBWLocalPoly(Y, X, kernT=kernT, kernS=kernS)
+        h, b_can = RoTBWLocalPoly(Y, X, kernT=kernT, kernS=kernS, C_h=C_h, C_b=C_b)
     elif b is None:
-        h_can, b = RoTBWLocalPoly(Y, X, kernT=kernT, kernS=kernS)
+        h_can, b = RoTBWLocalPoly(Y, X, kernT=kernT, kernS=kernS, C_h=C_h, C_b=C_b)
         
     if (h == "cv") and (b == "cv"):
         cv_mse = np.zeros((len(h_lst), len(b_lst)))
         for i in range(len(h_lst)):
             for j in range(len(b_lst)):
                 Y_reg_est = LocalPolyRegMain(Y, X, x_eval=X, degree=1, deriv_ord=0, 
                                              h=h_lst[i], b=b_lst[i], 
@@ -223,16 +247,16 @@
     
     Y_est = LocalPolyRegMain(Y, X, x_eval=x_eval, degree=degree, deriv_ord=deriv_ord, 
                              h=h, b=b, kernT=kernT, kernS=kernS)
     return Y_est
 
 
 def DerivEffect(Y, X, t_eval=None, h_bar=None, kernT_bar="gaussian", h=None, b=None, 
-                degree=2, deriv_ord=1, kernT="epanechnikov", kernS="epanechnikov", 
-                parallel=False, processes=20):
+                C_h=7, C_b=3, degree=2, deriv_ord=1, kernT="epanechnikov", 
+                kernS="epanechnikov", parallel=False, processes=20):
     '''
     Estimating the derivative of the dose-response curve via Nadaraya-Watson 
     conditional CDF estimator.
     
     
     Parameters
     ----------
@@ -241,29 +265,30 @@
             
         X: (n,d+1)-array
             The first column of X is the treatment/exposure variable, while 
             the other d columns are confounding variables of n observations.
             
         t_eval: (m,)-array
             The coordinates of the m evaluation points. (Default: t_eval=None. 
-            Then, t_eval=X[:,0].)
+            Then, t_eval=X[:,0], which consists of the observed treatment variables.)
             
         h_bar: float
             The bandwidth parameters for the Nadaraya-Watson conditional CDF estimator. 
             (Default: h_bar=None. Then, the Silverman's rule of thumb is applied. 
             See Chen et al.(2016) for details.)
             
         kernT_bar: str
             The name of the kernel function for Nadaraya-Watson conditional CDF 
             estimator. (Default: "gaussian".)
             
         h,b: float
             The bandwidth parameters for the treatment/exposure variable and 
             confounding variables. (Default: h=None, b=None. Then, the rule-of-thumb 
-            bandwidth selector in Eq.(A1) of Yang and Tschernig (1999) is used.)
+            bandwidth selector in Eq.(A1) of Yang and Tschernig (1999) is used
+            with additional scaling factors C_h and C_b, respectively.)
             
         degree: int
             Degree of local polynomials. (Default: degree=2.)
             
         deriv_ord: int
             The order of the estimated derivative the conditional mean outcome function. 
             (Default: deriv_ord=1. Then, it estimates the partial derivative of the 
@@ -275,14 +300,20 @@
             
         parallel: boolean
             The indicator of whether the function should be parallel executed by
             multi-processing. (Default: parallel=False.)
             
         processes: int
             The number of processes for parallel execution. (Default: processes=20.)
+    
+    Return
+    ----------
+        theta_C: (m,)-array
+            The estimated derivative of the dose-response curve evaluated at 
+            points "t_eval".
     '''
     
     if t_eval is None: 
         t_eval = X[:,0].copy()
         
     n = X.shape[0]  ## Number of data points
     d = 1
@@ -295,31 +326,31 @@
         
     weight_mat = kernT_bar((t_eval - X[:,0].reshape(-1,1)) / h_bar)
     weight_mat = weight_mat / np.sum(weight_mat, axis=0)
     weight_mat[np.isnan(weight_mat)] = 0
     if parallel:
         with Pool(processes=processes) as pool:
             part_fun = partial(LocalPolyReg_Fs, Y=Y, X=X, degree=degree, deriv_ord=deriv_ord, 
-                               h=h, b=b, kernT=kernT, kernS=kernS)
+                               h=h, b=b, C_h=C_h, C_b=C_b, kernT=kernT, kernS=kernS)
             beta_mat = pool.map(part_fun, [np.concatenate([t_eval[i]*np.ones((n,1)), X[:,1:]], axis=1) for i in range(t_eval.shape[0])])
             beta_mat = np.concatenate(beta_mat, axis=0).reshape(t_eval.shape[0], n).T
     else:
         beta_mat = np.zeros((n, t_eval.shape[0]))
         for i in range(t_eval.shape[0]):
             X_mat = np.concatenate([t_eval[i]*np.ones((n,1)), X[:,1:]], axis=1)
             beta_mat[:,i] = LocalPolyReg(Y, X, x_eval=X_mat, degree=degree, deriv_ord=deriv_ord, 
-                                         h=h, b=b, kernT=kernT, kernS=kernS)
+                                         h=h, b=b, C_h=C_h, C_b=C_b, kernT=kernT, kernS=kernS)
     
     theta_C = np.sum(weight_mat * beta_mat, axis=0)
     return theta_C
 
 
 def IntegEst(Y, X, t_eval=None, h_bar=None, kernT_bar="gaussian", h=None, b=None, 
-             degree=2, deriv_ord=1, kernT="epanechnikov", kernS="epanechnikov",
-             parallel=False, processes=20):
+             C_h=7, C_b=3, degree=2, deriv_ord=1, kernT="epanechnikov", 
+             kernS="epanechnikov", parallel=False, processes=20):
     '''
     Estimating the dose-response curve via our integral estimator with linear 
     interpolation approximation.
     
     
     Parameters
     ----------
@@ -327,29 +358,31 @@
             The outcomes of n observations.
             
         X: (n,d+1)-array
             The first column of X is the treatment/exposure variable, while 
             the other d columns are confounding variables of n observations.
             
         t_eval: (m,)-array
-            The coordinates of the m evaluation points. (Default: t_eval=None. Then, t_eval=X[:,0].)
+            The coordinates of the m evaluation points. (Default: t_eval=None. 
+            Then, t_eval=X[:,0].)
             
         h_bar: float
             The bandwidth parameters for the Nadaraya-Watson conditional CDF estimator. 
             (Default: h_bar=None. Then, the Silverman's rule of thumb is applied. 
             See Chen et al.(2016) for details.)
             
         kernT_bar: str
             The name of the kernel function for Nadaraya-Watson conditional CDF estimator.
             (Default: "gaussian".)
             
         h,b: float
-            The bandwidth parameters for the treatment/exposure variable and confounding variables. 
-            (Default: h=None, b=None. Then, the rule-of-thumb bandwidth selector in Eq.(A1) of 
-             Yang and Tschernig (1999) is used.)
+            The bandwidth parameters for the treatment/exposure variable and 
+            confounding variables. (Default: h=None, b=None. Then, the rule-of-thumb 
+            bandwidth selector in Eq.(A1) of Yang and Tschernig (1999) is used
+            with additional scaling factors C_h and C_b, respectively.)
             
         degree: int
             Degree of local polynomials. (Default: degree=2.)
             
         deriv_ord: int
             The order of the estimated derivative the conditional mean outcome function. 
             (Default: deriv_ord=1. Then, it estimates the partial derivative of the 
@@ -361,25 +394,31 @@
         
         parallel: boolean
             The indicator of whether the function should be parallel executed by
             multi-processing. (Default: parallel=False.)
             
         processes: int
             The number of processes for parallel execution. (Default: processes=20.)
+            
+    Return
+    ----------
+        m_est: (m,)-array
+            The estimated dose-response curve evaluated at points "t_eval".
     '''
     
     if t_eval is None: 
         t_eval = X[:,0].copy()
     
     T_sort = np.sort(X[:,0])
     n = X.shape[0]  ## Number of data points
     
     # Compute theta_C at the order statistics of T
     theta_est = DerivEffect(Y, X, t_eval=T_sort, h_bar=h_bar, kernT_bar=kernT_bar, 
-                            h=h, b=b, degree=degree, deriv_ord=deriv_ord, kernT=kernT, kernS=kernS,
+                            h=h, b=b, C_h=C_h, C_b=C_b, degree=degree, 
+                            deriv_ord=deriv_ord, kernT=kernT, kernS=kernS,
                             parallel=parallel, processes=processes)
     T_delta = T_sort[1:] - T_sort[:(n-1)]
     
     int_mat_up = np.ones((n,)) * (T_delta*(np.arange(1, n)*theta_est[:(n-1)])).reshape(-1,1)
     int_mat_up = int_mat_up * (np.arange(n-1).reshape(-1,1) < np.arange(n))
     
     int_mat_down = np.ones((n,)) * (T_delta*((n-np.arange(1, n))*theta_est[1:])).reshape(-1,1)
@@ -411,14 +450,20 @@
             
         degree: int
             Degree of local polynomials. (Default: degree=2.)
             
         deriv_ord: int
             The order of derivatives of the regression function that are estimated. 
             (Default: deriv_ord=0. Then, it is the usual local polynomial regression.)
+            
+    Return
+    ----------
+        Y_est: (m,)-array
+            The estimated function or its derivatives by local polynomial regression
+            evaluated at points "x_eval".
     '''
     if x_eval is None: 
         x_eval = X.copy()
         
     n = X.shape[0]  ## Number of data points
         
     kernel, sigmaK_sq, K_sq = KernelRetrieval(kernel)
@@ -452,70 +497,79 @@
         rcond = np.finfo(lhs.dtype).eps * max(*lhs.shape)
         beta = np.linalg.lstsq(lhs, rhs, rcond=rcond)[0]
         Y_est[i] = np.math.factorial(deriv_ord)*beta[deriv_ord]
     return Y_est
 
 
 
-def RegAdjust(Y, X, t_eval=None, h=None, b=None, degree=2, deriv_ord=0, 
+def RegAdjust(Y, X, t_eval=None, h=None, b=None, C_h=7, C_b=3, degree=2, deriv_ord=0, 
               kernT="epanechnikov", kernS="epanechnikov", parallel=False, 
               processes=20):
     '''
-    Estimating the dose-response curve via simple integral estimator with linear interpolation approximation.
-    
+    Estimating the dose-response curve via simple integral estimator with linear 
+    interpolation approximation.
     
     Parameters
     ----------
         Y: (n,)-array
             The outcomes of n observations.
             
         X: (n,d+1)-array
             The first column of X is the treatment/exposure variable, while 
             the other d columns are confounding variables of n observations.
             
         t_eval: (m,)-array
-            The coordinates of the m evaluation points. (Default: t_eval=None. Then, t_eval=X[:,0].)
+            The coordinates of the m evaluation points. (Default: t_eval=None. 
+            Then, t_eval=X[:,0].)
             
         h,b: float
-            The bandwidth parameters for the treatment/exposure variable and confounding variables. 
-            (Default: h=None, b=None. Then, the rule-of-thumb bandwidth selector in Eq.(A1) of 
-             Yang and Tschernig (1999) is used.)
+            The bandwidth parameters for the treatment/exposure variable and 
+            confounding variables. (Default: h=None, b=None. Then, the rule-of-thumb 
+            bandwidth selector in Eq.(A1) of Yang and Tschernig (1999) is used
+            with additional scaling factors C_h and C_b, respectively.)
             
         degree: int
             Degree of local polynomials. (Default: degree=2.)
             
         deriv_ord: int
-            The order of the estimated derivative of the conditional mean outcome function. 
-            (Default: deriv_ord=0. Then, it estimates the conditional mean outcome function itself.)
+            The order of the estimated derivative of the conditional mean outcome 
+            function. (Default: deriv_ord=0. Then, it estimates the conditional 
+            mean outcome function itself.)
             
         kernT, kernS: str
-            The names of kernel functions for the treatment/exposure variable and confounding variables.
-            (Default: "epanechnikov".)
+            The names of kernel functions for the treatment/exposure variable 
+            and confounding variables. (Default: "epanechnikov".)
             
         parallel: boolean
             The indicator of whether the function should be parallel executed by
             multi-processing. (Default: parallel=False.)
             
         processes: int
             The number of processes for parallel execution. (Default: processes=20.)
+            
+    Return
+    ----------
+        m_est: (m,)-array
+            The estimated dose-response curve evaluated at points "t_eval".
     '''
     
     if t_eval is None: 
         t_eval = X[:,0].copy()
     
     n = X.shape[0]  ## Number of data points
     
     if parallel:
         with Pool(processes=processes) as pool:
             part_fun = partial(LocalPolyReg_Fs, Y=Y, X=X, degree=degree, deriv_ord=deriv_ord, 
-                               h=h, b=b, kernT=kernT, kernS=kernS)
+                               h=h, b=b, C_h=C_h, C_b=C_b, kernT=kernT, kernS=kernS)
             beta_mat = pool.map(part_fun, [np.concatenate([t_eval[i]*np.ones((n,1)), X[:,1:]], axis=1) for i in range(t_eval.shape[0])])
             beta_mat = np.concatenate(beta_mat, axis=0).reshape(t_eval.shape[0], n).T
     else:
         beta_mat = np.zeros((n, t_eval.shape[0]))
         for i in range(t_eval.shape[0]):
             X_mat = np.concatenate([t_eval[i]*np.ones((n,1)), X[:,1:]], axis=1)
-            beta_mat[:,i] = LocalPolyReg(Y, X, x_eval=X_mat, degree=degree, deriv_ord=deriv_ord, 
-                                         h=h, b=b, kernT=kernT, kernS=kernS)
+            beta_mat[:,i] = LocalPolyReg(Y, X, x_eval=X_mat, degree=degree, 
+                                         deriv_ord=deriv_ord, h=h, b=b, C_h=C_h, 
+                                         C_b=C_b, kernT=kernT, kernS=kernS)
     m_est = np.mean(beta_mat, axis=0)
     return m_est
```

### Comparing `npdoseresponse-0.0.3/npDoseResponse/utils.py` & `npdoseresponse-0.0.4/npDoseResponse/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 # Author: Yikun Zhang
-# Last Editing: May 12, 2024
+# Last Editing: May 19, 2024
 
 # Description: This script contains the utility functions for the main functions 
 # in our package.
 
 import numpy as np
 from .rbf import KernelRetrieval
 
@@ -13,27 +13,38 @@
 
 
 def RoTBWLocalPoly(Y, X, kernT="epanechnikov", kernS="epanechnikov", C_h=7, C_b=3):
     '''
     Compute the rule-of-thumb bandwidth selector in Eq.(A1) of 
     Yang and Tschernig (1999).
     
-    
     Parameters
     ----------
         Y: (n,)-array
             The outcomes of n observations.
         
         X: (n,d+1)-array
             The first column of X is the treatment/exposure variable, while 
             the other d columns are confounding variables of n observations.
             
         kernT, kernS: str
             The names of kernel functions for the treatment/exposure variable 
             and confounding variables. (Default: "epanechnikov".)
+            
+        C_h,C_b: float
+            The scaling factors for the rule-of-thumb bandwidth parameters. 
+            (Default: C_h=7, C_b=3.)
+    
+    Return
+    ----------
+        h: float
+            The rule-of-thumb bandwidth parameter for the treatment/exposure variable.
+            
+        b: (d,)-array
+            The rule-of-thumb bandwidth vector for the confounding variables.
     '''
     n = X.shape[0]  ## Number of data points
     d = X.shape[1] - 1
     
     kernT, sigmaK_sq, K_sq = KernelRetrieval(kernT)
     # Apply the rule-of-thumb bandwidth selector in Eq.(A1) of Yang and Tschernig (1999)
     p_coeff = np.polyfit(X[:,0], Y, 4)
@@ -69,15 +80,14 @@
 
 
 def HatMatrix(X, degree=2, deriv_ord=1, h=None, b=None, kernT="epanechnikov", kernS="epanechnikov"):
     '''
     Compute the hat matrix of the local polynomial regression when it is viewed 
     as a linear smoother.
     
-    
     Parameters
     ----------
         X: (n,d+1)-array
             The first column of X is the treatment/exposure variable, while 
             the other d columns are confounding variables of n observations.
             
         degree: int
@@ -85,19 +95,25 @@
             
         deriv_ord: int
             The order of the estimated derivative the conditional mean outcome function. 
             (Default: deriv_ord=1. Then, it estimates the partial derivative of the 
             conditional mean outcome function with respect to the treatment variable.)
             
         h,b: float
-            The bandwidth parameters for the treatment/exposure variable and confounding variables. 
+            The bandwidth parameters for the treatment/exposure variable and 
+            confounding variables. 
             
         kernT, kernS: str
-            The names of kernel functions for the treatment/exposure variable and confounding variables.
-            (Default: "epanechnikov".)
+            The names of kernel functions for the treatment/exposure variable 
+            and confounding variables. (Default: "epanechnikov".)
+            
+    Return
+    ----------
+        hat_mat: (n,n)-array
+            The hat matrix.
     '''
     n = X.shape[0]  ## Number of data points
     d = X.shape[1] - 1
     x_eval = X.copy()
     
     print("The current bandwidth for treament variable in the local polynomial regression is "+ str(h) + ".\n")
     print("The current bandwidth for confounding variables in the local polynomial regression is "+ str(b) + ".\n")
@@ -120,8 +136,8 @@
         try:
             hat_mat_samp = np.dot(np.linalg.inv(design_mat), np.dot(X_dat.T, W))
         except:
             # Add some small quantities to the diagonal matrix to prevent the singularity of the matrix
             design_mat = design_mat + 1e-16*np.eye(design_mat.shape[0])
             hat_mat_samp = np.dot(np.linalg.inv(design_mat), np.dot(X_dat.T, W))
         hat_mat[i,inds] = hat_mat_samp[deriv_ord,:]
-    return hat_mat
+    return hat_mat
```

### Comparing `npdoseresponse-0.0.3/npDoseResponse.egg-info/PKG-INFO` & `npdoseresponse-0.0.4/npDoseResponse.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npDoseResponse
-Version: 0.0.3
+Version: 0.0.4
 Summary: Nonparametric Estimation and Inference on Dose-Response Curves
 Home-page: https://github.com/zhangyk8/npDoseResponse
 Author: Yikun Zhang
 Author-email: yikunzhang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,9 +38,9 @@
 ```
 pip install npDoseResponse
 ```
 
 References
 --------
 
-
+<a name="npdoseresponse">[1]</a> Y. Zhang, Y.-C. Chen, and A. Giessing (2024+) Nonparametric Inference on Dose-Response Curves Without the Positivity Condition [arXiv:2405.09003](https://arxiv.org/abs/2405.09003).
```

### Comparing `npdoseresponse-0.0.3/setup.py` & `npdoseresponse-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="npDoseResponse",
-    version="0.0.3",
+    version="0.0.4",
     author="Yikun Zhang",
     author_email="yikunzhang@foxmail.com",
     description="Nonparametric Estimation and Inference on Dose-Response Curves",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zhangyk8/npDoseResponse",
     classifiers=[
```

