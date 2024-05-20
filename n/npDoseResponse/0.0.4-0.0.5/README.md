# Comparing `tmp/npdoseresponse-0.0.4.tar.gz` & `tmp/npdoseresponse-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npdoseresponse-0.0.4.tar", last modified: Sun May 19 23:03:32 2024, max compression
+gzip compressed data, was "npdoseresponse-0.0.5.tar", last modified: Sun May 19 23:48:18 2024, max compression
```

## Comparing `npdoseresponse-0.0.4.tar` & `npdoseresponse-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-19 23:03:32.984838 npdoseresponse-0.0.4/
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1070 2024-05-07 04:36:16.000000 npdoseresponse-0.0.4/LICENSE
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     2141 2024-05-19 23:03:32.983833 npdoseresponse-0.0.4/PKG-INFO
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1641 2024-05-18 23:50:54.000000 npdoseresponse-0.0.4/README.md
-drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-19 23:03:32.978672 npdoseresponse-0.0.4/npDoseResponse/
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)      211 2024-05-19 22:54:58.000000 npdoseresponse-0.0.4/npDoseResponse/__init__.py
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)    24960 2024-05-19 22:39:45.000000 npdoseresponse-0.0.4/npDoseResponse/npDoseResponse.py
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     5934 2024-05-19 22:45:09.000000 npdoseresponse-0.0.4/npDoseResponse/rbf.py
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     5929 2024-05-19 22:42:14.000000 npdoseresponse-0.0.4/npDoseResponse/utils.py
-drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-19 23:03:32.983206 npdoseresponse-0.0.4/npDoseResponse.egg-info/
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     2141 2024-05-19 23:03:32.000000 npdoseresponse-0.0.4/npDoseResponse.egg-info/PKG-INFO
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)      321 2024-05-19 23:03:32.000000 npdoseresponse-0.0.4/npDoseResponse.egg-info/SOURCES.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)        1 2024-05-19 23:03:32.000000 npdoseresponse-0.0.4/npDoseResponse.egg-info/dependency_links.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)       12 2024-05-19 23:03:32.000000 npdoseresponse-0.0.4/npDoseResponse.egg-info/requires.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)       15 2024-05-19 23:03:32.000000 npdoseresponse-0.0.4/npDoseResponse.egg-info/top_level.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)       38 2024-05-19 23:03:32.984962 npdoseresponse-0.0.4/setup.cfg
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)      805 2024-05-19 22:54:36.000000 npdoseresponse-0.0.4/setup.py
+drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-19 23:48:18.485605 npdoseresponse-0.0.5/
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1070 2024-05-07 04:36:16.000000 npdoseresponse-0.0.5/LICENSE
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     2141 2024-05-19 23:48:18.484815 npdoseresponse-0.0.5/PKG-INFO
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1641 2024-05-19 23:42:02.000000 npdoseresponse-0.0.5/README.md
+drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-19 23:48:18.478806 npdoseresponse-0.0.5/npDoseResponse/
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)      211 2024-05-19 23:48:13.000000 npdoseresponse-0.0.5/npDoseResponse/__init__.py
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)    26152 2024-05-19 23:40:04.000000 npdoseresponse-0.0.5/npDoseResponse/npDoseResponse.py
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     5934 2024-05-19 22:45:09.000000 npdoseresponse-0.0.5/npDoseResponse/rbf.py
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     6165 2024-05-19 23:40:58.000000 npdoseresponse-0.0.5/npDoseResponse/utils.py
+drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-19 23:48:18.483948 npdoseresponse-0.0.5/npDoseResponse.egg-info/
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     2141 2024-05-19 23:48:18.000000 npdoseresponse-0.0.5/npDoseResponse.egg-info/PKG-INFO
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)      321 2024-05-19 23:48:18.000000 npdoseresponse-0.0.5/npDoseResponse.egg-info/SOURCES.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)        1 2024-05-19 23:48:18.000000 npdoseresponse-0.0.5/npDoseResponse.egg-info/dependency_links.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)       12 2024-05-19 23:48:18.000000 npdoseresponse-0.0.5/npDoseResponse.egg-info/requires.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)       15 2024-05-19 23:48:18.000000 npdoseresponse-0.0.5/npDoseResponse.egg-info/top_level.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)       38 2024-05-19 23:48:18.485724 npdoseresponse-0.0.5/setup.cfg
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)      805 2024-05-19 23:48:00.000000 npdoseresponse-0.0.5/setup.py
```

### Comparing `npdoseresponse-0.0.4/LICENSE` & `npdoseresponse-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `npdoseresponse-0.0.4/PKG-INFO` & `npdoseresponse-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npDoseResponse
-Version: 0.0.4
+Version: 0.0.5
 Summary: Nonparametric Estimation and Inference on Dose-Response Curves
 Home-page: https://github.com/zhangyk8/npDoseResponse
 Author: Yikun Zhang
 Author-email: yikunzhang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `npdoseresponse-0.0.4/README.md` & `npdoseresponse-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `npdoseresponse-0.0.4/npDoseResponse/npDoseResponse.py` & `npdoseresponse-0.0.5/npDoseResponse/npDoseResponse.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from multiprocessing import Pool
 from functools import partial
 from .utils import *
 
 #=======================================================================================#
 
 def LocalPolyReg(Y, X, x_eval=None, degree=2, deriv_ord=1, h=None, b=None, C_h=7, 
-                 C_b=3, kernT="epanechnikov", kernS="epanechnikov", 
+                 C_b=3, print_bw=True, kernT="epanechnikov", kernS="epanechnikov", 
                  h_lst=np.linspace(0.5, 15, 30), b_lst=np.linspace(0.2, 6, 30)):
     '''
     (Partial) Local polynomial regression for estimating the conditional mean outcome 
     function and its partial derivatives. We use higher order local monomials for 
     the treatment variable and first-order local monomials for the confounding variables.
     
     
@@ -47,14 +47,18 @@
             
         h,b: float
             The bandwidth parameters for the treatment/exposure variable and 
             confounding variables. (Default: h=None, b=None. Then, the rule-of-thumb 
             bandwidth selector in Eq.(A1) of Yang and Tschernig (1999) is used 
             with additional scaling factors C_h and C_b, respectively.)
             
+        print_bw: boolean
+            The indicator of whether the current bandwidth parameters should be
+            printed to the console. (Default: print_bw=True.)
+            
         kernT, kernS: str
             The names of kernel functions for the treatment/exposure variable 
             and confounding variables. (Default: "epanechnikov".)
             
         h_lst, b_lst: (k1,)-array and (k2,)-array
             Candidate searching values of h,b for LOOCV.
             
@@ -86,17 +90,18 @@
                 hat_mat = HatMatrix(X, degree=2, deriv_ord=1, h=h_lst[i], b=b_lst[i], kernT=kernT, kernS=kernS)
                 cv_mse[i,j] = np.mean(((Y - Y_reg_est) / (1 - np.diag(hat_mat)))**2)
         argmin_ind = np.unravel_index(cv_mse.argmin(), cv_mse.shape)
         h_opt = h_lst[argmin_ind[0]]
         b_opt = b_lst[argmin_ind[1]]
         h = h_opt
         b = b_opt
-        
-    print("The current bandwidth for treament variable in the local polynomial regression is "+ str(h) + ".\n")
-    print("The current bandwidth for confounding variables in the local polynomial regression is "+ str(b) + ".\n")
+    
+    if print_bw:
+        print("The current bandwidth for treament variable in the local polynomial regression is "+ str(h) + ".\n")
+        print("The current bandwidth for confounding variables in the local polynomial regression is "+ str(b) + ".\n")
     
     Y_est = LocalPolyRegMain(Y, X, x_eval=x_eval, degree=degree, deriv_ord=deriv_ord, 
                              h=h, b=b, kernT=kernT, kernS=kernS)
     return Y_est
 
 
 def LocalPolyRegMain(Y, X, x_eval=None, degree=2, deriv_ord=0, h=None, b=None, 
@@ -162,15 +167,15 @@
         rcond = np.finfo(lhs.dtype).eps * max(*lhs.shape)
         beta = np.linalg.lstsq(lhs, rhs, rcond=rcond)[0]
         Y_est[i] = np.math.factorial(deriv_ord)*beta[deriv_ord]
     return Y_est
 
 
 def LocalPolyReg_Fs(x_eval, Y, X, degree=2, deriv_ord=1, h=None, b=None, C_h=7, 
-                    C_b=3, kernT="epanechnikov", kernS="epanechnikov", 
+                    C_b=3, print_bw=True, kernT="epanechnikov", kernS="epanechnikov", 
                     h_lst=np.linspace(0.5, 15, 30), b_lst=np.linspace(0.2, 6, 30)):
     '''
     (Partial) Local polynomial regression for estimating the conditional mean outcome 
     function and its partial derivatives. We use higher order local monomials for 
     the treatment variable and first-order local monomials for the confounding variables.
     (This function is for multi-process execution only.)
     
@@ -198,14 +203,18 @@
             
         h,b: float
             The bandwidth parameters for the treatment/exposure variable and 
             confounding variables. (Default: h=None, b=None. Then, the rule-of-thumb 
             bandwidth selector in Eq.(A1) of Yang and Tschernig (1999) is used
             with additional scaling factors C_h and C_b, respectively.)
             
+        print_bw: boolean
+            The indicator of whether the current bandwidth parameters should be
+            printed to the console. (Default: print_bw=True.)
+            
         kernT, kernS: str
             The names of kernel functions for the treatment/exposure variable 
             and confounding variables. (Default: "epanechnikov".)
             
         h_lst, b_lst: (k1,)-array and (k2,)-array
             Candidate searching values of h,b for LOOCV.
             
@@ -237,25 +246,26 @@
                 hat_mat = HatMatrix(X, degree=2, deriv_ord=1, h=h_lst[i], b=b_lst[i], kernT=kernT, kernS=kernS)
                 cv_mse[i,j] = np.mean(((Y - Y_reg_est) / (1 - np.diag(hat_mat)))**2)
         argmin_ind = np.unravel_index(cv_mse.argmin(), cv_mse.shape)
         h_opt = h_lst[argmin_ind[0]]
         b_opt = b_lst[argmin_ind[1]]
         h = h_opt
         b = b_opt
-        
-    print("The current bandwidth for treament variable in the local polynomial regression is "+ str(h) + ".\n")
-    print("The current bandwidth for confounding variables in the local polynomial regression is "+ str(b) + ".\n")
+    
+    if print_bw:
+        print("The current bandwidth for treament variable in the local polynomial regression is "+ str(h) + ".\n")
+        print("The current bandwidth for confounding variables in the local polynomial regression is "+ str(b) + ".\n")
     
     Y_est = LocalPolyRegMain(Y, X, x_eval=x_eval, degree=degree, deriv_ord=deriv_ord, 
                              h=h, b=b, kernT=kernT, kernS=kernS)
     return Y_est
 
 
 def DerivEffect(Y, X, t_eval=None, h_bar=None, kernT_bar="gaussian", h=None, b=None, 
-                C_h=7, C_b=3, degree=2, deriv_ord=1, kernT="epanechnikov", 
+                C_h=7, C_b=3, print_bw=True, degree=2, deriv_ord=1, kernT="epanechnikov", 
                 kernS="epanechnikov", parallel=False, processes=20):
     '''
     Estimating the derivative of the dose-response curve via Nadaraya-Watson 
     conditional CDF estimator.
     
     
     Parameters
@@ -282,14 +292,18 @@
             
         h,b: float
             The bandwidth parameters for the treatment/exposure variable and 
             confounding variables. (Default: h=None, b=None. Then, the rule-of-thumb 
             bandwidth selector in Eq.(A1) of Yang and Tschernig (1999) is used
             with additional scaling factors C_h and C_b, respectively.)
             
+        print_bw: boolean
+            The indicator of whether the current bandwidth parameters should be
+            printed to the console. (Default: print_bw=True.)
+            
         degree: int
             Degree of local polynomials. (Default: degree=2.)
             
         deriv_ord: int
             The order of the estimated derivative the conditional mean outcome function. 
             (Default: deriv_ord=1. Then, it estimates the partial derivative of the 
             conditional mean outcome function with respect to the treatment variable.)
@@ -326,30 +340,31 @@
         
     weight_mat = kernT_bar((t_eval - X[:,0].reshape(-1,1)) / h_bar)
     weight_mat = weight_mat / np.sum(weight_mat, axis=0)
     weight_mat[np.isnan(weight_mat)] = 0
     if parallel:
         with Pool(processes=processes) as pool:
             part_fun = partial(LocalPolyReg_Fs, Y=Y, X=X, degree=degree, deriv_ord=deriv_ord, 
-                               h=h, b=b, C_h=C_h, C_b=C_b, kernT=kernT, kernS=kernS)
+                               h=h, b=b, C_h=C_h, C_b=C_b, print_bw=print_bw, kernT=kernT, kernS=kernS)
             beta_mat = pool.map(part_fun, [np.concatenate([t_eval[i]*np.ones((n,1)), X[:,1:]], axis=1) for i in range(t_eval.shape[0])])
             beta_mat = np.concatenate(beta_mat, axis=0).reshape(t_eval.shape[0], n).T
     else:
         beta_mat = np.zeros((n, t_eval.shape[0]))
         for i in range(t_eval.shape[0]):
             X_mat = np.concatenate([t_eval[i]*np.ones((n,1)), X[:,1:]], axis=1)
             beta_mat[:,i] = LocalPolyReg(Y, X, x_eval=X_mat, degree=degree, deriv_ord=deriv_ord, 
-                                         h=h, b=b, C_h=C_h, C_b=C_b, kernT=kernT, kernS=kernS)
+                                         h=h, b=b, C_h=C_h, C_b=C_b, print_bw=print_bw, 
+                                         kernT=kernT, kernS=kernS)
     
     theta_C = np.sum(weight_mat * beta_mat, axis=0)
     return theta_C
 
 
 def IntegEst(Y, X, t_eval=None, h_bar=None, kernT_bar="gaussian", h=None, b=None, 
-             C_h=7, C_b=3, degree=2, deriv_ord=1, kernT="epanechnikov", 
+             C_h=7, C_b=3, print_bw=True, degree=2, deriv_ord=1, kernT="epanechnikov", 
              kernS="epanechnikov", parallel=False, processes=20):
     '''
     Estimating the dose-response curve via our integral estimator with linear 
     interpolation approximation.
     
     
     Parameters
@@ -376,14 +391,18 @@
             
         h,b: float
             The bandwidth parameters for the treatment/exposure variable and 
             confounding variables. (Default: h=None, b=None. Then, the rule-of-thumb 
             bandwidth selector in Eq.(A1) of Yang and Tschernig (1999) is used
             with additional scaling factors C_h and C_b, respectively.)
             
+        print_bw: boolean
+            The indicator of whether the current bandwidth parameters should be
+            printed to the console. (Default: print_bw=True.)
+            
         degree: int
             Degree of local polynomials. (Default: degree=2.)
             
         deriv_ord: int
             The order of the estimated derivative the conditional mean outcome function. 
             (Default: deriv_ord=1. Then, it estimates the partial derivative of the 
             conditional mean outcome function with respect to the treatment variable.)
@@ -409,31 +428,31 @@
         t_eval = X[:,0].copy()
     
     T_sort = np.sort(X[:,0])
     n = X.shape[0]  ## Number of data points
     
     # Compute theta_C at the order statistics of T
     theta_est = DerivEffect(Y, X, t_eval=T_sort, h_bar=h_bar, kernT_bar=kernT_bar, 
-                            h=h, b=b, C_h=C_h, C_b=C_b, degree=degree, 
-                            deriv_ord=deriv_ord, kernT=kernT, kernS=kernS,
-                            parallel=parallel, processes=processes)
+                            h=h, b=b, C_h=C_h, C_b=C_b, print_bw=print_bw, 
+                            degree=degree, deriv_ord=deriv_ord, kernT=kernT, 
+                            kernS=kernS, parallel=parallel, processes=processes)
     T_delta = T_sort[1:] - T_sort[:(n-1)]
     
     int_mat_up = np.ones((n,)) * (T_delta*(np.arange(1, n)*theta_est[:(n-1)])).reshape(-1,1)
     int_mat_up = int_mat_up * (np.arange(n-1).reshape(-1,1) < np.arange(n))
     
     int_mat_down = np.ones((n,)) * (T_delta*((n-np.arange(1, n))*theta_est[1:])).reshape(-1,1)
     int_mat_down = int_mat_down * (np.arange(n-1).reshape(-1,1) >= np.arange(n))
     m_samp = np.mean(Y) + np.sum(int_mat_up - int_mat_down, axis=0)/n
     
     m_est = np.interp(t_eval, T_sort, m_samp)
     return m_est
 
 
-def LocalPolyReg1D(Y, X, h=None, x_eval=None, degree=3, deriv_ord=0, kernel="epanechnikov"):
+def LocalPolyReg1D(Y, X, h=None, x_eval=None, degree=2, deriv_ord=0, kernel="epanechnikov"):
     '''
     Local polynomial regression in one dimension.
     
     Parameters
     ----------
         Y: (m,)-array
             The y coordinates of m data points.
@@ -497,17 +516,17 @@
         rcond = np.finfo(lhs.dtype).eps * max(*lhs.shape)
         beta = np.linalg.lstsq(lhs, rhs, rcond=rcond)[0]
         Y_est[i] = np.math.factorial(deriv_ord)*beta[deriv_ord]
     return Y_est
 
 
 
-def RegAdjust(Y, X, t_eval=None, h=None, b=None, C_h=7, C_b=3, degree=2, deriv_ord=0, 
-              kernT="epanechnikov", kernS="epanechnikov", parallel=False, 
-              processes=20):
+def RegAdjust(Y, X, t_eval=None, h=None, b=None, C_h=7, C_b=3, print_bw=True, 
+              degree=2, deriv_ord=0, kernT="epanechnikov", kernS="epanechnikov", 
+              parallel=False, processes=20):
     '''
     Estimating the dose-response curve via simple integral estimator with linear 
     interpolation approximation.
     
     Parameters
     ----------
         Y: (n,)-array
@@ -523,14 +542,18 @@
             
         h,b: float
             The bandwidth parameters for the treatment/exposure variable and 
             confounding variables. (Default: h=None, b=None. Then, the rule-of-thumb 
             bandwidth selector in Eq.(A1) of Yang and Tschernig (1999) is used
             with additional scaling factors C_h and C_b, respectively.)
             
+        print_bw: boolean
+            The indicator of whether the current bandwidth parameters should be
+            printed to the console. (Default: print_bw=True.)
+            
         degree: int
             Degree of local polynomials. (Default: degree=2.)
             
         deriv_ord: int
             The order of the estimated derivative of the conditional mean outcome 
             function. (Default: deriv_ord=0. Then, it estimates the conditional 
             mean outcome function itself.)
@@ -555,21 +578,22 @@
     if t_eval is None: 
         t_eval = X[:,0].copy()
     
     n = X.shape[0]  ## Number of data points
     
     if parallel:
         with Pool(processes=processes) as pool:
-            part_fun = partial(LocalPolyReg_Fs, Y=Y, X=X, degree=degree, deriv_ord=deriv_ord, 
-                               h=h, b=b, C_h=C_h, C_b=C_b, kernT=kernT, kernS=kernS)
+            part_fun = partial(LocalPolyReg_Fs, Y=Y, X=X, degree=degree, 
+                               deriv_ord=deriv_ord, h=h, b=b, C_h=C_h, C_b=C_b, 
+                               print_bw=print_bw, kernT=kernT, kernS=kernS)
             beta_mat = pool.map(part_fun, [np.concatenate([t_eval[i]*np.ones((n,1)), X[:,1:]], axis=1) for i in range(t_eval.shape[0])])
             beta_mat = np.concatenate(beta_mat, axis=0).reshape(t_eval.shape[0], n).T
     else:
         beta_mat = np.zeros((n, t_eval.shape[0]))
         for i in range(t_eval.shape[0]):
             X_mat = np.concatenate([t_eval[i]*np.ones((n,1)), X[:,1:]], axis=1)
             beta_mat[:,i] = LocalPolyReg(Y, X, x_eval=X_mat, degree=degree, 
                                          deriv_ord=deriv_ord, h=h, b=b, C_h=C_h, 
-                                         C_b=C_b, kernT=kernT, kernS=kernS)
+                                         C_b=C_b, print_bw=print_bw, kernT=kernT, kernS=kernS)
     m_est = np.mean(beta_mat, axis=0)
     return m_est
```

### Comparing `npdoseresponse-0.0.4/npDoseResponse/rbf.py` & `npdoseresponse-0.0.5/npDoseResponse/rbf.py`

 * *Files identical despite different names*

### Comparing `npdoseresponse-0.0.4/npDoseResponse/utils.py` & `npdoseresponse-0.0.5/npDoseResponse/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,16 @@
     sigmaK_sq = sigmaK_sq**2
     K_sq = K_sq**d
     b = ((K_sq*d*resid)/(4*n*sigmaK_sq*C_fun))**(1/(d+5)) * C_b
     
     return h, b
 
 
-def HatMatrix(X, degree=2, deriv_ord=1, h=None, b=None, kernT="epanechnikov", kernS="epanechnikov"):
+def HatMatrix(X, degree=2, deriv_ord=1, h=None, b=None, print_bw=True, 
+              kernT="epanechnikov", kernS="epanechnikov"):
     '''
     Compute the hat matrix of the local polynomial regression when it is viewed 
     as a linear smoother.
     
     Parameters
     ----------
         X: (n,d+1)-array
@@ -98,29 +99,34 @@
             (Default: deriv_ord=1. Then, it estimates the partial derivative of the 
             conditional mean outcome function with respect to the treatment variable.)
             
         h,b: float
             The bandwidth parameters for the treatment/exposure variable and 
             confounding variables. 
             
+        print_bw: boolean
+            The indicator of whether the current bandwidth parameters should be
+            printed to the console. (Default: print_bw=True.)
+            
         kernT, kernS: str
             The names of kernel functions for the treatment/exposure variable 
             and confounding variables. (Default: "epanechnikov".)
             
     Return
     ----------
         hat_mat: (n,n)-array
             The hat matrix.
     '''
     n = X.shape[0]  ## Number of data points
     d = X.shape[1] - 1
     x_eval = X.copy()
     
-    print("The current bandwidth for treament variable in the local polynomial regression is "+ str(h) + ".\n")
-    print("The current bandwidth for confounding variables in the local polynomial regression is "+ str(b) + ".\n")
+    if print_bw:
+        print("The current bandwidth for treament variable in the local polynomial regression is "+ str(h) + ".\n")
+        print("The current bandwidth for confounding variables in the local polynomial regression is "+ str(b) + ".\n")
     
     kernT, sigmaK_sq, K_sq = KernelRetrieval(kernT)
     kernS, sigmaK_sq, K_sq = KernelRetrieval(kernS)
     hat_mat = np.zeros((n, n))
     for i in range(x_eval.shape[0]):
         weights = kernT((X[:,0] - x_eval[i,0])/h) * np.prod(kernS((X[:,1:] - x_eval[i,1:])/b), axis=1)
         # Filter out the data points with zero weights to speed up regressions with kernels of compact support
```

### Comparing `npdoseresponse-0.0.4/npDoseResponse.egg-info/PKG-INFO` & `npdoseresponse-0.0.5/npDoseResponse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npDoseResponse
-Version: 0.0.4
+Version: 0.0.5
 Summary: Nonparametric Estimation and Inference on Dose-Response Curves
 Home-page: https://github.com/zhangyk8/npDoseResponse
 Author: Yikun Zhang
 Author-email: yikunzhang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `npdoseresponse-0.0.4/setup.py` & `npdoseresponse-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="npDoseResponse",
-    version="0.0.4",
+    version="0.0.5",
     author="Yikun Zhang",
     author_email="yikunzhang@foxmail.com",
     description="Nonparametric Estimation and Inference on Dose-Response Curves",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zhangyk8/npDoseResponse",
     classifiers=[
```

