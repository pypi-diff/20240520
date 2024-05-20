# Comparing `tmp/svsa-0.0.8.tar.gz` & `tmp/svsa-0.0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svsa-0.0.8.tar", last modified: Mon May 20 16:11:48 2024, max compression
+gzip compressed data, was "svsa-0.0.8.1.tar", last modified: Mon May 20 16:23:21 2024, max compression
```

## Comparing `svsa-0.0.8.tar` & `svsa-0.0.8.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2024-05-20 16:11:48.888291 svsa-0.0.8/
--rw-rw-r--   0 greg      (1000) greg      (1000)     1633 2024-05-20 16:11:48.888291 svsa-0.0.8/PKG-INFO
--rw-rw-r--   0 greg      (1000) greg      (1000)      951 2024-05-20 16:04:49.000000 svsa-0.0.8/README.md
--rw-rw-r--   0 greg      (1000) greg      (1000)       38 2024-05-20 16:11:48.888291 svsa-0.0.8/setup.cfg
--rw-r--r--   0 greg      (1000) greg      (1000)      883 2024-05-20 16:08:15.000000 svsa-0.0.8/setup.py
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2024-05-20 16:11:48.888291 svsa-0.0.8/svsa/
--rw-rw-r--   0 greg      (1000) greg      (1000)      146 2024-05-20 16:04:49.000000 svsa-0.0.8/svsa/__init__.py
--rwxrwxr-x   0 greg      (1000) greg      (1000)     3222 2024-05-20 16:04:49.000000 svsa-0.0.8/svsa/crbs6.py
--rwxrwxr-x   0 greg      (1000) greg      (1000)     3770 2024-05-20 16:04:49.000000 svsa-0.0.8/svsa/crbs7.py
--rw-rw-r--   0 greg      (1000) greg      (1000)     1033 2024-05-20 16:04:49.000000 svsa-0.0.8/svsa/gen_spectra.py
--rw-rw-r--   0 greg      (1000) greg      (1000)     3329 2024-05-20 16:04:49.000000 svsa-0.0.8/svsa/support_vector_spectrum.py
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2024-05-20 16:11:48.888291 svsa-0.0.8/svsa.egg-info/
--rw-rw-r--   0 greg      (1000) greg      (1000)     1633 2024-05-20 16:11:48.000000 svsa-0.0.8/svsa.egg-info/PKG-INFO
--rw-rw-r--   0 greg      (1000) greg      (1000)      277 2024-05-20 16:11:48.000000 svsa-0.0.8/svsa.egg-info/SOURCES.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)        1 2024-05-20 16:11:48.000000 svsa-0.0.8/svsa.egg-info/dependency_links.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)       32 2024-05-20 16:11:48.000000 svsa-0.0.8/svsa.egg-info/requires.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)        5 2024-05-20 16:11:48.000000 svsa-0.0.8/svsa.egg-info/top_level.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)        1 2024-05-20 16:11:48.000000 svsa-0.0.8/svsa.egg-info/zip-safe
+drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2024-05-20 16:23:21.100589 svsa-0.0.8.1/
+-rw-rw-r--   0 greg      (1000) greg      (1000)     1635 2024-05-20 16:23:21.100589 svsa-0.0.8.1/PKG-INFO
+-rw-rw-r--   0 greg      (1000) greg      (1000)      951 2024-05-20 16:04:49.000000 svsa-0.0.8.1/README.md
+-rw-rw-r--   0 greg      (1000) greg      (1000)       38 2024-05-20 16:23:21.100589 svsa-0.0.8.1/setup.cfg
+-rw-r--r--   0 greg      (1000) greg      (1000)      885 2024-05-20 16:23:12.000000 svsa-0.0.8.1/setup.py
+drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2024-05-20 16:23:21.100589 svsa-0.0.8.1/svsa/
+-rw-rw-r--   0 greg      (1000) greg      (1000)      146 2024-05-20 16:04:49.000000 svsa-0.0.8.1/svsa/__init__.py
+-rwxrwxr-x   0 greg      (1000) greg      (1000)     3222 2024-05-20 16:04:49.000000 svsa-0.0.8.1/svsa/crbs6.py
+-rwxrwxr-x   0 greg      (1000) greg      (1000)     3770 2024-05-20 16:04:49.000000 svsa-0.0.8.1/svsa/crbs7.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)     1033 2024-05-20 16:19:20.000000 svsa-0.0.8.1/svsa/gen_spectra.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)     3329 2024-05-20 16:21:23.000000 svsa-0.0.8.1/svsa/support_vector_spectrum.py
+drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2024-05-20 16:23:21.100589 svsa-0.0.8.1/svsa.egg-info/
+-rw-rw-r--   0 greg      (1000) greg      (1000)     1635 2024-05-20 16:23:21.000000 svsa-0.0.8.1/svsa.egg-info/PKG-INFO
+-rw-rw-r--   0 greg      (1000) greg      (1000)      277 2024-05-20 16:23:21.000000 svsa-0.0.8.1/svsa.egg-info/SOURCES.txt
+-rw-rw-r--   0 greg      (1000) greg      (1000)        1 2024-05-20 16:23:21.000000 svsa-0.0.8.1/svsa.egg-info/dependency_links.txt
+-rw-rw-r--   0 greg      (1000) greg      (1000)       32 2024-05-20 16:23:21.000000 svsa-0.0.8.1/svsa.egg-info/requires.txt
+-rw-rw-r--   0 greg      (1000) greg      (1000)        5 2024-05-20 16:23:21.000000 svsa-0.0.8.1/svsa.egg-info/top_level.txt
+-rw-rw-r--   0 greg      (1000) greg      (1000)        1 2024-05-20 16:11:48.000000 svsa-0.0.8.1/svsa.egg-info/zip-safe
```

### Comparing `svsa-0.0.8/PKG-INFO` & `svsa-0.0.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svsa
-Version: 0.0.8
+Version: 0.0.8.1
 Summary: Fast approximations of scattering spectra with SVR.
 Home-page: https://gjhunt.github.io/svsa/
 Author: Gregory J. Hunt
 Author-email: ghunt@wm.edu
 License: GPL3
 Description: <img src="ex_u.jpg" width="75%">
```

### Comparing `svsa-0.0.8/README.md` & `svsa-0.0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `svsa-0.0.8/setup.py` & `svsa-0.0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='svsa',
-      version='0.0.8',
+      version='0.0.8.1',
       url='https://gjhunt.github.io/svsa/',
       author='Gregory J. Hunt',
       author_email='ghunt@wm.edu',
       description='Fast approximations of scattering spectra with SVR.',
       long_description=long_description,
       long_description_content_type="text/markdown",
       license='GPL3',
```

### Comparing `svsa-0.0.8/svsa/crbs6.py` & `svsa-0.0.8.1/svsa/crbs6.py`

 * *Files identical despite different names*

### Comparing `svsa-0.0.8/svsa/crbs7.py` & `svsa-0.0.8.1/svsa/crbs7.py`

 * *Files identical despite different names*

### Comparing `svsa-0.0.8/svsa/gen_spectra.py` & `svsa-0.0.8.1/svsa/gen_spectra.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 from .crbs6 import crbs6
 from .crbs7 import crbs7
 
 def gen_spectra(y_seq,ri_seq,ef_seq,ci_seq,ct_seq,x_seq,scatter_type="sptsig",model="s6",file=None):
 
     all_combs = itertools.product(y_seq,ri_seq,ef_seq,ci_seq,ct_seq)
-    if model is "s6":
+    if model == "s6":
         all_signals = [crbs6(p[0],p[1],p[2],p[3],p[4],x_seq) for p in all_combs]
-    if model is "s7":
+    if model == "s7":
         all_signals = [crbs7(p[0],p[1],p[2],p[3],p[4],x_seq) for p in all_combs]
 
     lineshapes = [out[scatter_type] for out in all_signals]
     lineshape_df = pd.DataFrame(np.array(lineshapes))
     
     params = [(out['y'],out['rlx_int'],out['eukenf'],out['c_int'],out['c_tr'])
               for out in all_signals]
```

### Comparing `svsa-0.0.8/svsa/support_vector_spectrum.py` & `svsa-0.0.8.1/svsa/support_vector_spectrum.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,22 +66,22 @@
         
             alpha0 = np.array([mod.intercept_ for mod in self.mods])
             alpha0 = alpha0.reshape(1,-1)
 
         return sv_mat, alpha, alpha0
 
     def save_fit(self,fname='fit',type='csv'):
-        if type is "csv":
+        if type == "csv":
             np.savetxt(fname+'_beta0'+'.csv',np.array(self.beta0),delimiter=',')
             np.savetxt(fname+'_beta'+'.csv',np.array(self.beta),delimiter=',')
             np.savetxt(fname+'_sigma'+'.csv',np.array(self.sigma),delimiter=',')
             np.savetxt(fname+'_sigmabar'+'.csv',np.array(self.sigmabar),delimiter=',')
             np.savetxt(fname+'_gamma'+'.csv',np.array([self.gamma]),delimiter=',')
             np.savetxt(fname+'_x'+'.csv',np.array([self.x]),delimiter=',')
-        elif type is "mat":
+        elif type == "mat":
             d = {'beta0':self.beta0,
                  'beta':self.beta,
                  'sigma':self.sigma,
                  'sigmabar':self.sigmabar,
                  'gamma':self.gamma,
                  'x':self.x
             }
```

### Comparing `svsa-0.0.8/svsa.egg-info/PKG-INFO` & `svsa-0.0.8.1/svsa.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svsa
-Version: 0.0.8
+Version: 0.0.8.1
 Summary: Fast approximations of scattering spectra with SVR.
 Home-page: https://gjhunt.github.io/svsa/
 Author: Gregory J. Hunt
 Author-email: ghunt@wm.edu
 License: GPL3
 Description: <img src="ex_u.jpg" width="75%">
```

