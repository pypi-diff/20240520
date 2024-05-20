# Comparing `tmp/npdoseresponse-0.0.5.tar.gz` & `tmp/npdoseresponse-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npdoseresponse-0.0.5.tar", last modified: Sun May 19 23:48:18 2024, max compression
+gzip compressed data, was "npdoseresponse-0.0.6.tar", last modified: Mon May 20 00:39:41 2024, max compression
```

## Comparing `npdoseresponse-0.0.5.tar` & `npdoseresponse-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-19 23:48:18.485605 npdoseresponse-0.0.5/
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1070 2024-05-07 04:36:16.000000 npdoseresponse-0.0.5/LICENSE
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     2141 2024-05-19 23:48:18.484815 npdoseresponse-0.0.5/PKG-INFO
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1641 2024-05-19 23:42:02.000000 npdoseresponse-0.0.5/README.md
-drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-19 23:48:18.478806 npdoseresponse-0.0.5/npDoseResponse/
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)      211 2024-05-19 23:48:13.000000 npdoseresponse-0.0.5/npDoseResponse/__init__.py
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)    26152 2024-05-19 23:40:04.000000 npdoseresponse-0.0.5/npDoseResponse/npDoseResponse.py
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     5934 2024-05-19 22:45:09.000000 npdoseresponse-0.0.5/npDoseResponse/rbf.py
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     6165 2024-05-19 23:40:58.000000 npdoseresponse-0.0.5/npDoseResponse/utils.py
-drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-19 23:48:18.483948 npdoseresponse-0.0.5/npDoseResponse.egg-info/
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     2141 2024-05-19 23:48:18.000000 npdoseresponse-0.0.5/npDoseResponse.egg-info/PKG-INFO
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)      321 2024-05-19 23:48:18.000000 npdoseresponse-0.0.5/npDoseResponse.egg-info/SOURCES.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)        1 2024-05-19 23:48:18.000000 npdoseresponse-0.0.5/npDoseResponse.egg-info/dependency_links.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)       12 2024-05-19 23:48:18.000000 npdoseresponse-0.0.5/npDoseResponse.egg-info/requires.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)       15 2024-05-19 23:48:18.000000 npdoseresponse-0.0.5/npDoseResponse.egg-info/top_level.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)       38 2024-05-19 23:48:18.485724 npdoseresponse-0.0.5/setup.cfg
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)      805 2024-05-19 23:48:00.000000 npdoseresponse-0.0.5/setup.py
+drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-20 00:39:41.364735 npdoseresponse-0.0.6/
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1070 2024-05-07 04:36:16.000000 npdoseresponse-0.0.6/LICENSE
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     2141 2024-05-20 00:39:41.362358 npdoseresponse-0.0.6/PKG-INFO
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1641 2024-05-19 23:42:02.000000 npdoseresponse-0.0.6/README.md
+drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-20 00:39:41.340759 npdoseresponse-0.0.6/npDoseResponse/
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)      242 2024-05-20 00:38:45.000000 npdoseresponse-0.0.6/npDoseResponse/__init__.py
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)    33722 2024-05-20 00:33:47.000000 npdoseresponse-0.0.6/npDoseResponse/npDoseResponse.py
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     5934 2024-05-19 22:45:09.000000 npdoseresponse-0.0.6/npDoseResponse/rbf.py
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     6165 2024-05-19 23:40:58.000000 npdoseresponse-0.0.6/npDoseResponse/utils.py
+drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-20 00:39:41.360654 npdoseresponse-0.0.6/npDoseResponse.egg-info/
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     2141 2024-05-20 00:39:41.000000 npdoseresponse-0.0.6/npDoseResponse.egg-info/PKG-INFO
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)      321 2024-05-20 00:39:41.000000 npdoseresponse-0.0.6/npDoseResponse.egg-info/SOURCES.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)        1 2024-05-20 00:39:41.000000 npdoseresponse-0.0.6/npDoseResponse.egg-info/dependency_links.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)       12 2024-05-20 00:39:41.000000 npdoseresponse-0.0.6/npDoseResponse.egg-info/requires.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)       15 2024-05-20 00:39:41.000000 npdoseresponse-0.0.6/npDoseResponse.egg-info/top_level.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)       38 2024-05-20 00:39:41.365049 npdoseresponse-0.0.6/setup.cfg
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)      805 2024-05-20 00:38:14.000000 npdoseresponse-0.0.6/setup.py
```

### Comparing `npdoseresponse-0.0.5/LICENSE` & `npdoseresponse-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `npdoseresponse-0.0.5/PKG-INFO` & `npdoseresponse-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npDoseResponse
-Version: 0.0.5
+Version: 0.0.6
 Summary: Nonparametric Estimation and Inference on Dose-Response Curves
 Home-page: https://github.com/zhangyk8/npDoseResponse
 Author: Yikun Zhang
 Author-email: yikunzhang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `npdoseresponse-0.0.5/README.md` & `npdoseresponse-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `npdoseresponse-0.0.5/npDoseResponse/npDoseResponse.py` & `npdoseresponse-0.0.6/npDoseResponse/npDoseResponse.py`

 * *Files 10% similar despite different names*

```diff
@@ -330,14 +330,15 @@
         t_eval = X[:,0].copy()
         
     n = X.shape[0]  ## Number of data points
     d = 1
     if h_bar is None:
         # Apply the Silverman's rule of thumb bandwidth in Chen et al.(2016).
         h_bar = (4/(d+2))**(1/(d+4))*(n**(-1/(d+4)))*np.std(X[:,0])
+    if print_bw:
         print("The current bandwidth for the conditional CDF estimator is "+ str(h_bar) + ".\n")
     
     kernT_bar, sigmaK_sq, K_sq = KernelRetrieval(kernT_bar)
         
     weight_mat = kernT_bar((t_eval - X[:,0].reshape(-1,1)) / h_bar)
     weight_mat = weight_mat / np.sum(weight_mat, axis=0)
     weight_mat[np.isnan(weight_mat)] = 0
@@ -355,22 +356,108 @@
                                          h=h, b=b, C_h=C_h, C_b=C_b, print_bw=print_bw, 
                                          kernT=kernT, kernS=kernS)
     
     theta_C = np.sum(weight_mat * beta_mat, axis=0)
     return theta_C
 
 
+def DerivEffectBoot(Y, X, t_eval=None, h_bar=None, kernT_bar="gaussian", h=None, 
+                    b=None, C_h=7, C_b=3, print_bw=True, degree=2, deriv_ord=1, 
+                    kernT="epanechnikov", kernS="epanechnikov", boot_num=500, 
+                    parallel=False, processes=20):
+    '''
+    Conduct inference on the derivative of the dose-response curve via Nadaraya-Watson 
+    conditional CDF estimator and nonparametric bootstrap.
+    
+    Parameters
+    ----------
+        Y: (n,)-array
+            The outcomes of n observations.
+            
+        X: (n,d+1)-array
+            The first column of X is the treatment/exposure variable, while 
+            the other d columns are confounding variables of n observations.
+            
+        t_eval: (m,)-array
+            The coordinates of the m evaluation points. (Default: t_eval=None. 
+            Then, t_eval=X[:,0], which consists of the observed treatment variables.)
+            
+        h_bar: float
+            The bandwidth parameters for the Nadaraya-Watson conditional CDF estimator. 
+            (Default: h_bar=None. Then, the Silverman's rule of thumb is applied. 
+            See Chen et al.(2016) for details.)
+            
+        kernT_bar: str
+            The name of the kernel function for Nadaraya-Watson conditional CDF 
+            estimator. (Default: "gaussian".)
+            
+        h,b: float
+            The bandwidth parameters for the treatment/exposure variable and 
+            confounding variables. (Default: h=None, b=None. Then, the rule-of-thumb 
+            bandwidth selector in Eq.(A1) of Yang and Tschernig (1999) is used
+            with additional scaling factors C_h and C_b, respectively.)
+            
+        print_bw: boolean
+            The indicator of whether the current bandwidth parameters should be
+            printed to the console. (Default: print_bw=True.)
+            
+        degree: int
+            Degree of local polynomials. (Default: degree=2.)
+            
+        deriv_ord: int
+            The order of the estimated derivative the conditional mean outcome function. 
+            (Default: deriv_ord=1. Then, it estimates the partial derivative of the 
+            conditional mean outcome function with respect to the treatment variable.)
+            
+        kernT, kernS: str
+            The names of kernel functions for the treatment/exposure variable 
+            and confounding variables. (Default: "epanechnikov".)
+            
+        boot_num: int
+            The number of bootstrapping times. (Default: bootstrap_num=500.) 
+            
+        parallel: boolean
+            The indicator of whether the function should be parallel executed by
+            multi-processing. (Default: parallel=False.)
+            
+        processes: int
+            The number of processes for parallel execution. (Default: processes=20.)
+    
+    Return
+    ----------
+        theta_C_boot: (m,)-array
+            The estimated derivatives of the dose-response curve on bootstrap samples 
+            evaluated at points "t_eval".
+    '''
+    
+    if t_eval is None: 
+        t_eval = X[:,0].copy()
+        
+    n = X.shape[0]  ## Number of data points
+    
+    theta_C_boot = np.zeros((boot_num, t_eval.shape[0]))
+    for b in range(boot_num):
+        ind = np.random.choice(n, size=n, replace=True)
+        X_boot = X[ind,:]
+        Y_boot = Y[ind]
+        theta_C_boot[b,:] = DerivEffect(Y_boot, X_boot, t_eval=t_eval, h_bar=h_bar, 
+                                   kernT_bar=kernT_bar, h=h, b=b, C_h=C_h, C_b=C_b, 
+                                   print_bw=print_bw, degree=degree, deriv_ord=deriv_ord, 
+                                   kernT=kernT, kernS=kernS, parallel=parallel, 
+                                   processes=processes)
+    return theta_C_boot
+
+
 def IntegEst(Y, X, t_eval=None, h_bar=None, kernT_bar="gaussian", h=None, b=None, 
              C_h=7, C_b=3, print_bw=True, degree=2, deriv_ord=1, kernT="epanechnikov", 
              kernS="epanechnikov", parallel=False, processes=20):
     '''
     Estimating the dose-response curve via our integral estimator with linear 
     interpolation approximation.
     
-    
     Parameters
     ----------
         Y: (n,)-array
             The outcomes of n observations.
             
         X: (n,d+1)-array
             The first column of X is the treatment/exposure variable, while 
@@ -441,17 +528,103 @@
     int_mat_up = int_mat_up * (np.arange(n-1).reshape(-1,1) < np.arange(n))
     
     int_mat_down = np.ones((n,)) * (T_delta*((n-np.arange(1, n))*theta_est[1:])).reshape(-1,1)
     int_mat_down = int_mat_down * (np.arange(n-1).reshape(-1,1) >= np.arange(n))
     m_samp = np.mean(Y) + np.sum(int_mat_up - int_mat_down, axis=0)/n
     
     m_est = np.interp(t_eval, T_sort, m_samp)
+            
     return m_est
 
 
+def IntegEstBoot(Y, X, t_eval=None, h_bar=None, kernT_bar="gaussian", h=None, b=None, 
+             C_h=7, C_b=3, print_bw=True, degree=2, deriv_ord=1, kernT="epanechnikov", 
+             kernS="epanechnikov", boot_num=500, parallel=False, processes=20):
+    '''
+    Conduct inference on the dose-response curve via our integral estimator and
+    nonparametric bootstrap.
+    
+    Parameters
+    ----------
+        Y: (n,)-array
+            The outcomes of n observations.
+            
+        X: (n,d+1)-array
+            The first column of X is the treatment/exposure variable, while 
+            the other d columns are confounding variables of n observations.
+            
+        t_eval: (m,)-array
+            The coordinates of the m evaluation points. (Default: t_eval=None. 
+            Then, t_eval=X[:,0].)
+            
+        h_bar: float
+            The bandwidth parameters for the Nadaraya-Watson conditional CDF estimator. 
+            (Default: h_bar=None. Then, the Silverman's rule of thumb is applied. 
+            See Chen et al.(2016) for details.)
+            
+        kernT_bar: str
+            The name of the kernel function for Nadaraya-Watson conditional CDF estimator.
+            (Default: "gaussian".)
+            
+        h,b: float
+            The bandwidth parameters for the treatment/exposure variable and 
+            confounding variables. (Default: h=None, b=None. Then, the rule-of-thumb 
+            bandwidth selector in Eq.(A1) of Yang and Tschernig (1999) is used
+            with additional scaling factors C_h and C_b, respectively.)
+            
+        print_bw: boolean
+            The indicator of whether the current bandwidth parameters should be
+            printed to the console. (Default: print_bw=True.)
+            
+        degree: int
+            Degree of local polynomials. (Default: degree=2.)
+            
+        deriv_ord: int
+            The order of the estimated derivative the conditional mean outcome function. 
+            (Default: deriv_ord=1. Then, it estimates the partial derivative of the 
+            conditional mean outcome function with respect to the treatment variable.)
+            
+        kernT, kernS: str
+            The names of kernel functions for the treatment/exposure variable 
+            and confounding variables. (Default: "epanechnikov".)
+            
+        boot_num: int
+            The number of bootstrapping times. (Default: bootstrap_num=500.) 
+        
+        parallel: boolean
+            The indicator of whether the function should be parallel executed by
+            multi-processing. (Default: parallel=False.)
+            
+        processes: int
+            The number of processes for parallel execution. (Default: processes=20.)
+            
+    Return
+    ----------
+        m_est_boot: (boot_num, m)-array
+            The estimated dose-response curves (or their derivatives) on the bootstrap 
+            samples evaluated at points "t_eval".
+    '''
+    
+    if t_eval is None: 
+        t_eval = X[:,0].copy()
+    
+    n = X.shape[0]  ## Number of data points
+    m_est_boot = np.zeros((boot_num, t_eval.shape[0]))
+    for b in range(boot_num):
+        ind = np.random.choice(n, size=n, replace=True)
+        X_boot = X[ind,:]
+        Y_boot = Y[ind]
+        m_est_boot[b,:] = IntegEst(Y_boot, X_boot, t_eval=t_eval, h_bar=h_bar, 
+                                   kernT_bar=kernT_bar, h=h, b=b, C_h=C_h, C_b=C_b, 
+                                   print_bw=print_bw, degree=degree, deriv_ord=deriv_ord, 
+                                   kernT=kernT, kernS=kernS, parallel=parallel, 
+                                   processes=processes)
+    return m_est_boot
+
+
 def LocalPolyReg1D(Y, X, h=None, x_eval=None, degree=2, deriv_ord=0, kernel="epanechnikov"):
     '''
     Local polynomial regression in one dimension.
     
     Parameters
     ----------
         Y: (m,)-array
@@ -568,15 +741,16 @@
             
         processes: int
             The number of processes for parallel execution. (Default: processes=20.)
             
     Return
     ----------
         m_est: (m,)-array
-            The estimated dose-response curve evaluated at points "t_eval".
+            The estimated dose-response curve (or its derivative) evaluated 
+            at points "t_eval".
     '''
     
     if t_eval is None: 
         t_eval = X[:,0].copy()
     
     n = X.shape[0]  ## Number of data points
     
@@ -591,9 +765,10 @@
         beta_mat = np.zeros((n, t_eval.shape[0]))
         for i in range(t_eval.shape[0]):
             X_mat = np.concatenate([t_eval[i]*np.ones((n,1)), X[:,1:]], axis=1)
             beta_mat[:,i] = LocalPolyReg(Y, X, x_eval=X_mat, degree=degree, 
                                          deriv_ord=deriv_ord, h=h, b=b, C_h=C_h, 
                                          C_b=C_b, print_bw=print_bw, kernT=kernT, kernS=kernS)
     m_est = np.mean(beta_mat, axis=0)
+    
     return m_est
```

### Comparing `npdoseresponse-0.0.5/npDoseResponse/rbf.py` & `npdoseresponse-0.0.6/npDoseResponse/rbf.py`

 * *Files identical despite different names*

### Comparing `npdoseresponse-0.0.5/npDoseResponse/utils.py` & `npdoseresponse-0.0.6/npDoseResponse/utils.py`

 * *Files identical despite different names*

### Comparing `npdoseresponse-0.0.5/npDoseResponse.egg-info/PKG-INFO` & `npdoseresponse-0.0.6/npDoseResponse.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npDoseResponse
-Version: 0.0.5
+Version: 0.0.6
 Summary: Nonparametric Estimation and Inference on Dose-Response Curves
 Home-page: https://github.com/zhangyk8/npDoseResponse
 Author: Yikun Zhang
 Author-email: yikunzhang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `npdoseresponse-0.0.5/setup.py` & `npdoseresponse-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="npDoseResponse",
-    version="0.0.5",
+    version="0.0.6",
     author="Yikun Zhang",
     author_email="yikunzhang@foxmail.com",
     description="Nonparametric Estimation and Inference on Dose-Response Curves",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zhangyk8/npDoseResponse",
     classifiers=[
```

