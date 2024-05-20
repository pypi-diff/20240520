# Comparing `tmp/pyihm-1.0.0.tar.gz` & `tmp/pyihm-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyihm-1.0.0.tar", last modified: Thu Mar 21 16:32:41 2024, max compression
+gzip compressed data, was "pyihm-1.1.0.tar", last modified: Thu May 16 13:12:23 2024, max compression
```

## Comparing `pyihm-1.0.0.tar` & `pyihm-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-03-21 16:32:41.549779 pyihm-1.0.0/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1481 2024-03-18 15:02:14.000000 pyihm-1.0.0/LICENSE.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       30 2023-07-19 13:41:44.000000 pyihm-1.0.0/MANIFEST.in
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1452 2024-03-21 16:32:41.549779 pyihm-1.0.0/PKG-INFO
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      976 2024-03-21 16:28:55.000000 pyihm-1.0.0/README.md
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-03-21 16:32:41.545779 pyihm-1.0.0/docs/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)  1688479 2024-03-21 16:24:38.000000 pyihm-1.0.0/docs/pyihm.pdf
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-03-21 16:32:41.549779 pyihm-1.0.0/pyihm/
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    15893 2024-03-21 15:59:05.000000 pyihm-1.0.0/pyihm/GUIs.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)      124 2024-03-21 16:31:21.000000 pyihm-1.0.0/pyihm/__init__.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     4200 2024-03-21 15:46:10.000000 pyihm-1.0.0/pyihm/__main__.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    23260 2024-03-21 15:51:26.000000 pyihm-1.0.0/pyihm/fit_mixture.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     8161 2024-03-21 15:47:55.000000 pyihm-1.0.0/pyihm/gen_param.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    11133 2024-03-21 16:11:14.000000 pyihm-1.0.0/pyihm/input_reading.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     8600 2024-01-30 17:34:50.000000 pyihm-1.0.0/pyihm/plots.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    10523 2024-03-21 15:47:03.000000 pyihm-1.0.0/pyihm/spectra_reading.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-03-21 16:32:41.549779 pyihm-1.0.0/pyihm.egg-info/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1452 2024-03-21 16:32:41.000000 pyihm-1.0.0/pyihm.egg-info/PKG-INFO
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      409 2024-03-21 16:32:41.000000 pyihm-1.0.0/pyihm.egg-info/SOURCES.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        1 2024-03-21 16:32:41.000000 pyihm-1.0.0/pyihm.egg-info/dependency_links.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       64 2024-03-21 16:32:41.000000 pyihm-1.0.0/pyihm.egg-info/requires.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        6 2024-03-21 16:32:41.000000 pyihm-1.0.0/pyihm.egg-info/top_level.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       85 2023-07-19 13:41:44.000000 pyihm-1.0.0/pyproject.toml
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       38 2024-03-21 16:32:41.549779 pyihm-1.0.0/setup.cfg
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)      950 2024-03-21 16:31:03.000000 pyihm-1.0.0/setup.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-03-21 16:32:41.549779 pyihm-1.0.0/test/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4460 2024-03-19 13:28:35.000000 pyihm-1.0.0/test/mix.out
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      375 2024-03-19 11:43:32.000000 pyihm-1.0.0/test/pyihm_input
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-16 13:12:23.512815 pyihm-1.1.0/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1481 2024-03-18 15:02:14.000000 pyihm-1.1.0/LICENSE.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       30 2023-07-19 13:41:44.000000 pyihm-1.1.0/MANIFEST.in
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1470 2024-05-16 13:12:23.512815 pyihm-1.1.0/PKG-INFO
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      976 2024-05-16 10:47:16.000000 pyihm-1.1.0/README.md
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-16 13:12:23.512815 pyihm-1.1.0/docs/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)  1689405 2024-05-16 13:02:12.000000 pyihm-1.1.0/docs/pyihm.pdf
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-16 13:12:23.512815 pyihm-1.1.0/pyihm/
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)    15893 2024-03-21 15:59:05.000000 pyihm-1.1.0/pyihm/GUIs.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)      124 2024-05-16 13:12:00.000000 pyihm-1.1.0/pyihm/__init__.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     5222 2024-05-16 12:51:02.000000 pyihm-1.1.0/pyihm/__main__.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)    24811 2024-05-14 13:13:03.000000 pyihm-1.1.0/pyihm/fit_mixture.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     8161 2024-03-21 15:47:55.000000 pyihm-1.1.0/pyihm/gen_param.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)    11630 2024-05-14 13:13:03.000000 pyihm-1.1.0/pyihm/input_reading.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     8600 2024-01-30 17:34:50.000000 pyihm-1.1.0/pyihm/plots.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)    10523 2024-03-21 15:47:03.000000 pyihm-1.1.0/pyihm/spectra_reading.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-16 13:12:23.512815 pyihm-1.1.0/pyihm.egg-info/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1470 2024-05-16 13:12:23.000000 pyihm-1.1.0/pyihm.egg-info/PKG-INFO
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      409 2024-05-16 13:12:23.000000 pyihm-1.1.0/pyihm.egg-info/SOURCES.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        1 2024-05-16 13:12:23.000000 pyihm-1.1.0/pyihm.egg-info/dependency_links.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       64 2024-05-16 13:12:23.000000 pyihm-1.1.0/pyihm.egg-info/requires.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        6 2024-05-16 13:12:23.000000 pyihm-1.1.0/pyihm.egg-info/top_level.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       85 2023-07-19 13:41:44.000000 pyihm-1.1.0/pyproject.toml
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       38 2024-05-16 13:12:23.516815 pyihm-1.1.0/setup.cfg
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)      968 2024-05-16 11:22:45.000000 pyihm-1.1.0/setup.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-05-16 13:12:23.512815 pyihm-1.1.0/test/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4460 2024-03-19 13:28:35.000000 pyihm-1.1.0/test/mix.out
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      375 2024-03-19 11:43:32.000000 pyihm-1.1.0/test/pyihm_input
```

### Comparing `pyihm-1.0.0/LICENSE.txt` & `pyihm-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyihm-1.0.0/PKG-INFO` & `pyihm-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyihm
-Version: 1.0.0
+Version: 1.1.0
 Summary: Indirect Hard Modelling, in Python
 Home-page: https://github.com/MetallerTM/pyihm
-Author: Francesco Bruno
+Author: Francesco Bruno, Letizia Fiorucci
 Author-email: bruno@cerm.unifi.it
 License: LICENSE.txt
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.10
```

### Comparing `pyihm-1.0.0/README.md` & `pyihm-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyihm-1.0.0/docs/pyihm.pdf` & `pyihm-1.1.0/docs/pyihm.pdf`

 * *Files 4% similar despite different names*

#### Comparing `pyihm-1.0.0/docs/pyihm.pdf` & `pyihm-1.1.0/docs/pyihm.pdf`

 * *Document info*

```diff
@@ -1,10 +1,10 @@
 Author: ''
-CreationDate: "D:20240321172434+01'00'"
+CreationDate: "D:20240516150204+02'00'"
 Creator: 'LaTeX with hyperref'
 Keywords: ''
-ModDate: "D:20240321172434+01'00'"
+ModDate: "D:20240516150204+02'00'"
 PTEX.Fullbanner: 'This is pdfTeX, Version 3.141592653-2.6-1.40.22 (TeX Live 2022/dev/Debian) kpathsea version 6.3.4/dev'
 Producer: 'pdfTeX-1.40.22'
 Subject: ''
 Title: ''
 Trapped: '/False'
```

#### pdftotext {} -

```diff
@@ -1,12 +1,12 @@
 Author:
-Francesco Bruno
-Version: 0.1.0
+Francesco Bruno, Letizia Fiorucci
+Version: 1.1.0
 Documentation release date:
-March 21, 2024
+May 16, 2024
 
 i
 
 ii
 
 Contents
 1
@@ -181,15 +181,15 @@
 2.2
 
 Make the deconvolution of the spectra
 
 A script for the deconvolution of the spectra is provided in table 2.1. It uses the KLASSEZ package
 to read, process and deconvolve the spectrum. The script must be edited in order to adapt the
 specific user’s need. At the end of the run, the .fvf file will be saved in the folder of the spectrum.
-Alternatively, one can set a custom filename, for saving the.fvf files in different locations.
+Alternatively, one can set a custom filename, for saving the .fvf files in different locations.
 If you do not have an experimental spectrum of one (or more) component, you can simulate it
 with KLASSEZ. You have to produce an input file like the one in table 2.2, then use it in the given
 script. This generates a .fvf in the current working directory.
 
 3
 
 Table 2.1: Script for creating a .fvf file, to be used as input for pyIHM.
@@ -389,28 +389,35 @@
 8
 
 2.4
 
 Starting the fit
 
 The software can be operated from the command line by typing:
-python3 -m pyihm <input_file> <options>
+python3 -m pyihm --input <input_file> <options>
 
 where <input_file> is the path to the input file that contains the parameters for the run, and
 <options> are flags for specific functions (see below).
 Multiple input files can be given at once, writing their paths in sequence without punctuation
 signs between them.
-python3 -m pyihm <input_file_1> <input_file_2> <input_file_3>
+python3 -m pyihm --input <input_file_1> <input_file_2> <input_file_3> <options>
 
-There are two possible options for a PYIHM run:
-• –debug: during the fitting routines, a figure that shows how the optimization process is going
+Here, the possible options for a PYIHM run follow:
+• --debug: during the fitting routines, a figure that shows how the optimization process is going
 is saved in the current working directory and updated every 20 iterations.
-• –cal: before to start the fit, the initial guess can be refined with a dedicated GUI, that allows
+• --cal: before to start the fit, the initial guess can be refined with a dedicated GUI, that allows
 to shift the spectra to correct for field drifts, and provide a better estimation of the starting
 intensities.
+• --opt_method: optimization method for the core fit of pyIHM
+– tight (default): two-step optimization, first with Nelder-Mead simplex and then with
+Levenberg-Marquardt least-squares
+– fast: single-step optimization with Levenberg-Marquardt least-squares
+– custom: reads the 'FIT_KWS' section of the input file, and performs the optimization
+accordingly
+• --help: displays this message on the terminal.
 
 9
 
 2.5
 
 Results
```

### Comparing `pyihm-1.0.0/pyihm/GUIs.py` & `pyihm-1.1.0/pyihm/GUIs.py`

 * *Files identical despite different names*

### Comparing `pyihm-1.0.0/pyihm/fit_mixture.py` & `pyihm-1.1.0/pyihm/fit_mixture.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import klassez as kz
 import lmfit as l
 
 from .gen_param import main as gen_param
 from . import plots
 from . import GUIs
 
+
 def calc_spectra(param, N_spectra, acqus, N):
     """
     Computes the spectra to be used as components for the fitting procedure, in form of lists of 1darrays. Each array is the sum of all the peaks.
     This function is called at each iteration of the fit.
     ---------
     Parameters:
     - param: lmfit.Parameters object
@@ -253,15 +254,15 @@
     # Reset the "vary" status of the parameters to the original one
     for p in param:
         popt[p].set(vary=vary_dict[p])
 
     return popt
 
 
-def f2min(param, N_spectra, acqus, N, exp, I, plims, cnvg_path, method='leastsq', debug=False):
+def f2min(param, N_spectra, acqus, N, exp, I, plims, cnvg_path, debug=False):
     """
     Function to compute the quantity to be minimized by the fit.
     ----------
     Parameters:
     - param: lmfit.Parameters object
         actual parameters
     - N_spectra: int
@@ -278,16 +279,15 @@
         Delimiters for the fitting region. The residuals are computed only in this regio. They must be given as point indices
     - cnvg_path: str
         Path for the file where to save the convergence path
     - debug: bool
         If True, saves a figurte of the ongoing fit in the current working directory every 20 iterations
     ----------
     Returns:
-    - target: float or 1darray
-        For Levenberg-Marquardt (method='leastsq'), array of the residuals, else \sum [ (exp - I*calc)^2 ]
+    - target: 1darray
     """
     param['count'].value += 1
     count = param['count'].value
     # Compute the trace for each spectrum
     x = np.arange(N)
     spectra = calc_spectra(param, N_spectra, acqus, N)
     spectra_T = [np.concatenate([spectrum[w] for w in plims]) for spectrum in spectra]
@@ -304,18 +304,15 @@
             kz.figures.ongoing_fit(exp/I, total, t_residual, filename='ongoing_fit', dpi=200)
 
     # Print how the fit is going, both in the file and in standart output
     with open(cnvg_path, 'a', buffering=1) as cnvg:
         cnvg.write(f'{count:5.0f}\t{target:10.5e}\n')
     print(f'Iteration step: {count:5.0f}; Target: {target:10.5e}', end='\r')
 
-    if method == 'leastsq':
-        return t_residual
-    else:
-        return target
+    return t_residual
 
 
 def write_output(M, I, K, spectra, n_comp, lims, filename='fit.report'):
     """
     Write a report of the performed fit in a file.
     The parameters of the single peaks are saved using the kz.fit.write_vf function.
     -----------
@@ -387,15 +384,15 @@
     # Transpose to make it column_wise
     data_arr = np.array(data).T
     # Save the file. "comments=''" is needed because header appears as a comment, therefore adds a column
     np.savetxt(f'{filename}.csv', data_arr, header=' '.join(header), comments='')
 
         
 
-def main(M, N_spectra, Hs, param, lims=None, fit_kws={}, filename='fit', CAL_FLAG=False, DEBUG_FLAG=False, ext='tiff', dpi=600):
+def main(M, N_spectra, Hs, param, lims=None, fit_kws={}, filename='fit', CAL_FLAG=False, DEBUG_FLAG=False, METHOD_FLAG='fast', ext='tiff', dpi=600):
     """
     Core of the fitting procedure.
     It computes the initial guess, save the figure, then starts the fit.
     After the fit, writes the output file and saves the figures of the result.
     Summary of saved files:
     > "<filename>.out": fit report
     > "<filename>_iguess.<ext>": figure of the initial guess
@@ -418,14 +415,16 @@
         Additional parameters for the lmfit.Minimizer.minimize function
     - filename: str
         Root of the names for the names of the files that will be saved.
     - CAL_FLAG: bool
         True for adjusting the initial guess before starting the fit
     - DEBUG_FLAG: bool
         True for saving a figure of the ongoing fit every 20 iterations
+    - METHOD_FLAG: str
+        Method to be used for the fit. Can be 'fast', 'tight', 'custom'
     - ext: str
         Format of the figures
     - dpi: int
         Resolution of the figures, in dots per inches
     """
     # Get the parameters for building the spectra
     acqus = dict(M.acqus)
@@ -503,26 +502,48 @@
 
     # Clear it and write the header
     with open(cnvg_path, 'w') as cnvg:
         cnvg.write('# Step \t Target\n')
 
     # Do the fit
     @kz.cron
-    def start_fit():
-        if fit_kws['method'] == 'leastsq':
-            tol = fit_kws.pop('tol')
-            fit_kws['xtol'] = tol
-            fit_kws['ftol'] = tol
-            fit_kws['gtol'] = tol
-        minner = l.Minimizer(f2min, param, fcn_args=(N_spectra, acqus, N, exp_T, I, plims, cnvg_path, fit_kws['method'], DEBUG_FLAG))
-        print(f'This fit has {len([key for key in param if param[key].vary])} parameters.\nStarting fit...')
-        result = minner.minimize(**fit_kws)
-        print(f'\n{result.message} Number of function evaluations: {result.nfev}.')
+    def start_fit(flag):
+        print(f'This fit has {len([key for key in param if param[key].vary])} parameters.')
+        if flag == 'fast':
+            print('Default fitting method: fast')
+            minner = l.Minimizer(f2min, param, fcn_args=(N_spectra, acqus, N, exp_T, I, plims, cnvg_path, DEBUG_FLAG))
+            print(f'Fitting n. 1 of 1, method: leastsq\nStarting fit...')
+            result = minner.minimize(method='leastsq', max_nfev=5000, xtol=1e-8, ftol=1e-8, gtol=1e-8)
+            print(f'\n{result.message} Number of function evaluations: {result.nfev}.')
+        elif flag == 'tight':
+            print('Default fitting method: tight')
+            minner = l.Minimizer(f2min, param, fcn_args=(N_spectra, acqus, N, exp_T, I, plims, cnvg_path, DEBUG_FLAG))
+            print(f'Fitting n. 1 of 2, method: Nelder\nStarting fit...')
+            result = minner.minimize(method='Nelder', max_nfev=10000)
+            print(f'\n{result.message} Number of function evaluations: {result.nfev}.')
+            params = result.params
+            print(f'Fitting n. 2 of 2, method: leastsq\nStarting fit...')
+            result = minner.minimize(method='leastsq', params=params, max_nfev=10000, xtol=1e-8, ftol=1e-8, gtol=1e-8)
+            print(f'\n{result.message} Number of function evaluations: {result.nfev}.')
+        elif flag == 'custom':
+            for idx in range(len(fit_kws.keys())):  # for each fitting round...
+                if idx == 0:
+                    minner = l.Minimizer(f2min, param, fcn_args=(N_spectra, acqus, N, exp_T, I, plims, cnvg_path, DEBUG_FLAG))
+                if fit_kws[idx]['method'] == 'leastsq':
+                    tol = fit_kws[idx].pop('tol')
+                    fit_kws[idx]['xtol'] = tol
+                    fit_kws[idx]['ftol'] = tol
+                    fit_kws[idx]['gtol'] = tol
+                print(f'Fitting n. {idx+1} of {len(fit_kws.keys())}, method: {fit_kws[idx]["method"]}\nStarting fit...')
+                if idx != 0:
+                    fit_kws[idx]['params'] = result.params
+                result = minner.minimize(**fit_kws[idx])
+                print(f'\n{result.message} Number of function evaluations: {result.nfev}.')
         return result
-    result = start_fit()
+    result = start_fit(METHOD_FLAG)
 
     # Get the optimized parameters
     popt = result.params
     # Calculate the optimized spectra
     #   ...as arrays
     opt_spectra = calc_spectra(popt, N_spectra, acqus, N)
     #   ...as kz.fit.Peak objects
@@ -574,12 +595,12 @@
 
     # Make the figures
     print('Saving figures...')
     plots.plot_output(M.ppm, exp, I*opt_total, [I*s for s in opt_spectra], 
             lims=(np.max(np.array(lims)), np.min(np.array(lims))), 
             plims=plims,
             X_label=X_label, filename=os.path.join(base_dir, f'{name}-FIGURES', filename), ext=ext, dpi=dpi)
-    save_data(os.path.join(base_dir, f'{name}-DATA', f'{filename}-result'), M.ppm, M.r, *[I*y for y in algn_spectra])
+    save_data(os.path.join(base_dir, f'{name}-DATA', f'{filename}-result'), M.ppm, M.r, *[I*y for y in opt_spectra])
     print('Done.\n')
```

### Comparing `pyihm-1.0.0/pyihm/gen_param.py` & `pyihm-1.1.0/pyihm/gen_param.py`

 * *Files identical despite different names*

### Comparing `pyihm-1.0.0/pyihm/input_reading.py` & `pyihm-1.1.0/pyihm/input_reading.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #! /usr/bin/env python3
 
 import sys
 import os
 import numpy as np
 from .GUIs import select_regions
 
+
 def read_input_file(filename):
     """
     Runs over the input file, looks for specific keywords, and interpret them accordingly.
     ----------
     Parameters:
     - filename: str
         Path to the input file
@@ -138,26 +139,28 @@
                 key, item = kw.split('=')
                 # Remove the spaces from the key
                 key = key.replace(' ', '')
                 dic['fit_bds'][key] = eval(item)    # This is always a number
 
         if 'FIT_KWS' in lines[0]:
             dic['fit_kws'] = {} # Placeholder
-            line = lines[1].split(',')  # Separates the various options
-            for kw in line:    # Loop on the parameters
-                if '=' not in kw:
-                    continue
-                # Separate the key from the actual value
-                key, item = kw.split('=')
-                # Remove the spaces from the key
-                key = key.replace(' ', '')
-                try:
-                    dic['fit_kws'][key] = eval(item)
-                except:
-                    dic['fit_kws'][key] = f'{item}'.replace(' ', '')
+            for il, l in enumerate(lines[1:]):
+                line = l.split(',')  # Separates the various options
+                dic['fit_kws'][il] = {} # Placeholder
+                for kw in line:    # Loop on the parameters
+                    if '=' not in kw:
+                        continue
+                    # Separate the key from the actual value
+                    key, item = kw.split('=')
+                    # Remove the spaces from the key
+                    key = key.replace(' ', '')
+                    try:
+                        dic['fit_kws'][il][key] = eval(item)
+                    except:
+                        dic['fit_kws'][il][key] = f'{item}'.replace(' ', '')
 
         # Options for saving the figures: format and resolution
         if 'PLT_OPTS' in lines:
             # Same thing as before
             dic['plt_opt'] = {}
             for kw in lines[1].split(','):
                 if '=' not in kw:
@@ -207,22 +210,28 @@
     if 'mix_spectrum_txt' not in dic.keys():    # This is an optional parameter: replacement for spectrum
         dic['mix_spectrum_txt'] = None
     if 'fit_lims' not in dic.keys():
         print('Fit limits not found in the input file.')
         dic['fit_lims'] = None
     if 'fit_kws' not in dic.keys():    # This is an optional parameter: parameters for the fit routine
         dic['fit_kws'] = {}
-    if 'method' not in dic['fit_kws'].keys():  # Algorithm to be used for the fit
-        dic['fit_kws']['method'] = 'leastsq'
-    if 'max_nfev' not in dic['fit_kws'].keys(): # Set default max_nfev
-        dic['fit_kws']['max_nfev'] = 10000
-    else:   # If it is set, make sure it is an integer
-        dic['fit_kws']['max_nfev'] = int(dic['fit_kws']['max_nfev'])
-    if 'tol' not in dic['fit_kws'].keys():      # Set default tolerance
-        dic['fit_kws']['tol'] = 1e-5
+    if len(dic['fit_kws'].keys()) == 0:    # If the dictionary is empty, it means that the user did not specify any parameter
+        dic['fit_kws'] = {0: {}}    # Create a dummy dictionary
+        dic['fit_kws'][0]['method'] = 'leastsq'
+        dic['fit_kws'][0]['max_nfev'] = 10000
+        dic['fit_kws'][0]['tol'] = 1e-5
+    # make sure that max_nfev is an integer
+    for key in dic['fit_kws'].keys():
+        if 'max_nfev' in dic['fit_kws'][key].keys():
+            dic['fit_kws'][key]['max_nfev'] = int(dic['fit_kws'][key]['max_nfev'])
+        if dic['fit_kws'][key]['method'] == 'leastsq':
+            if 'tol' not in dic['fit_kws'][key].keys():
+                dic['fit_kws'][key]['tol'] = 1e-5
+            if 'max_nfev' not in dic['fit_kws'][key].keys():
+                dic['fit_kws'][key]['max_nfev'] = 10000
     # Set the figures' options to .tiff 300 dpi, unless explicitely said
     if 'plt_opt' not in dic.keys():
         dic['plt_opt'] = {}
     if 'ext' not in dic['plt_opt'].keys():
         dic['plt_opt']['ext'] = 'tiff'
     if 'dpi' not in dic['plt_opt'].keys():
         dic['plt_opt']['dpi'] = 300
```

### Comparing `pyihm-1.0.0/pyihm/plots.py` & `pyihm-1.1.0/pyihm/plots.py`

 * *Files identical despite different names*

### Comparing `pyihm-1.0.0/pyihm/spectra_reading.py` & `pyihm-1.1.0/pyihm/spectra_reading.py`

 * *Files identical despite different names*

### Comparing `pyihm-1.0.0/pyihm.egg-info/PKG-INFO` & `pyihm-1.1.0/pyihm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyihm
-Version: 1.0.0
+Version: 1.1.0
 Summary: Indirect Hard Modelling, in Python
 Home-page: https://github.com/MetallerTM/pyihm
-Author: Francesco Bruno
+Author: Francesco Bruno, Letizia Fiorucci
 Author-email: bruno@cerm.unifi.it
 License: LICENSE.txt
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.10
```

### Comparing `pyihm-1.0.0/setup.py` & `pyihm-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
         name='pyihm',
-        version='1.0.0',
-        author='Francesco Bruno',
+        version='1.1.0',
+        author='Francesco Bruno, Letizia Fiorucci',
         author_email='bruno@cerm.unifi.it',
         description='Indirect Hard Modelling, in Python',
         url='https://github.com/MetallerTM/pyihm',
         long_description=long_description,
         long_description_content_type = 'text/markdown',
         classifiers = [
             'Programming Language :: Python :: 3',
```

### Comparing `pyihm-1.0.0/test/mix.out` & `pyihm-1.1.0/test/mix.out`

 * *Files identical despite different names*

