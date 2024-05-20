# Comparing `tmp/pyPPG-1.0.8.tar.gz` & `tmp/pyPPG-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPPG-1.0.8.tar", last modified: Wed Aug  9 06:10:27 2023, max compression
+gzip compressed data, was "pyPPG-1.0.9.tar", last modified: Mon Aug 14 08:19:44 2023, max compression
```

## Comparing `pyPPG-1.0.8.tar` & `pyPPG-1.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-08-09 06:10:27.689567 pyPPG-1.0.8/
--rw-rw-rw-   0        0        0      105 2023-05-03 11:40:28.000000 pyPPG-1.0.8/AUTHORS.rst
--rw-rw-rw-   0        0        0    35972 2023-07-18 09:12:28.000000 pyPPG-1.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0     4509 2023-08-09 06:10:27.688571 pyPPG-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3888 2023-08-08 21:55:51.000000 pyPPG-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-08-09 06:10:27.677959 pyPPG-1.0.8/pyPPG/
--rw-rw-rw-   0        0        0     3593 2023-08-08 17:27:20.000000 pyPPG-1.0.8/pyPPG/Biomarkers.py
--rw-rw-rw-   0        0        0    11223 2023-08-08 14:17:10.000000 pyPPG-1.0.8/pyPPG/DataHandling.py
--rw-rw-rw-   0        0        0     3567 2023-08-08 21:27:20.000000 pyPPG-1.0.8/pyPPG/EXAMPLE.py
--rw-rw-rw-   0        0        0    49739 2023-08-07 10:37:58.000000 pyPPG-1.0.8/pyPPG/FiducialPoints.py
--rw-rw-rw-   0        0        0     1846 2023-07-31 14:32:01.000000 pyPPG-1.0.8/pyPPG/Preprocessing.py
--rw-rw-rw-   0        0        0     1907 2023-07-31 14:33:15.000000 pyPPG-1.0.8/pyPPG/Statistics.py
--rw-rw-rw-   0        0        0        0 2023-07-23 10:03:08.000000 pyPPG-1.0.8/pyPPG/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-09 06:10:27.685521 pyPPG-1.0.8/pyPPG/pack_ppg/
--rw-rw-rw-   0        0        0      487 2022-11-08 13:38:06.000000 pyPPG-1.0.8/pyPPG/pack_ppg/_ErrorHandler.py
--rw-rw-rw-   0        0        0        0 2023-07-23 10:03:08.000000 pyPPG-1.0.8/pyPPG/pack_ppg/__init__.py
--rw-rw-rw-   0        0        0     4963 2023-07-31 14:33:15.000000 pyPPG-1.0.8/pyPPG/ppgSQI.py
-drwxrwxrwx   0        0        0        0 2023-08-09 06:10:27.688571 pyPPG-1.0.8/pyPPG/ppg_bm/
--rw-rw-rw-   0        0        0        0 2023-07-21 19:27:04.000000 pyPPG-1.0.8/pyPPG/ppg_bm/__init__.py
--rw-rw-rw-   0        0        0    49162 2023-08-08 15:59:12.000000 pyPPG-1.0.8/pyPPG/ppg_bm/biomarker_extractor.py
--rw-rw-rw-   0        0        0     5213 2023-08-08 17:30:48.000000 pyPPG-1.0.8/pyPPG/ppg_bm/get_bm_derivs_ratios.py
--rw-rw-rw-   0        0        0     3567 2023-08-08 18:05:34.000000 pyPPG-1.0.8/pyPPG/ppg_bm/get_bm_ppg_derivs.py
--rw-rw-rw-   0        0        0     6670 2023-08-08 17:35:55.000000 pyPPG-1.0.8/pyPPG/ppg_bm/get_bm_ppg_sig.py
--rw-rw-rw-   0        0        0     4727 2023-08-08 17:30:48.000000 pyPPG-1.0.8/pyPPG/ppg_bm/get_bm_sig_ratios.py
-drwxrwxrwx   0        0        0        0 2023-08-09 06:10:27.684536 pyPPG-1.0.8/pyPPG.egg-info/
--rw-rw-rw-   0        0        0     4509 2023-08-09 06:10:27.000000 pyPPG-1.0.8/pyPPG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      617 2023-08-09 06:10:27.000000 pyPPG-1.0.8/pyPPG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-09 06:10:27.000000 pyPPG-1.0.8/pyPPG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-09 06:10:27.000000 pyPPG-1.0.8/pyPPG.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2023-08-09 06:10:27.000000 pyPPG-1.0.8/pyPPG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      190 2023-07-27 13:48:40.000000 pyPPG-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-09 06:10:27.689567 pyPPG-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1079 2023-08-09 06:09:21.000000 pyPPG-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-14 08:19:44.855933 pyPPG-1.0.9/
+-rw-rw-rw-   0        0        0      105 2023-05-03 11:40:28.000000 pyPPG-1.0.9/AUTHORS.rst
+-rw-rw-rw-   0        0        0    35972 2023-07-18 09:12:28.000000 pyPPG-1.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     4509 2023-08-14 08:19:44.854751 pyPPG-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3888 2023-08-08 21:55:51.000000 pyPPG-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-08-14 08:19:44.818497 pyPPG-1.0.9/pyPPG/
+-rw-rw-rw-   0        0        0     5662 2023-08-14 08:12:28.000000 pyPPG-1.0.9/pyPPG/__init__.py
+-rw-rw-rw-   0        0        0     2190 2023-08-14 07:54:11.000000 pyPPG-1.0.9/pyPPG/biomarkers.py
+-rw-rw-rw-   0        0        0    10698 2023-08-14 07:15:33.000000 pyPPG-1.0.9/pyPPG/datahandling.py
+-rw-rw-rw-   0        0        0     3814 2023-08-14 07:54:11.000000 pyPPG-1.0.9/pyPPG/example.py
+-rw-rw-rw-   0        0        0    49171 2023-08-14 08:12:28.000000 pyPPG-1.0.9/pyPPG/fiducials.py
+drwxrwxrwx   0        0        0        0 2023-08-14 08:19:44.849037 pyPPG-1.0.9/pyPPG/pack_ppg/
+-rw-rw-rw-   0        0        0      487 2022-11-08 13:38:06.000000 pyPPG-1.0.9/pyPPG/pack_ppg/_ErrorHandler.py
+-rw-rw-rw-   0        0        0        0 2023-07-23 10:03:08.000000 pyPPG-1.0.9/pyPPG/pack_ppg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-14 08:19:44.854751 pyPPG-1.0.9/pyPPG/ppg_bm/
+-rw-rw-rw-   0        0        0        0 2023-07-21 19:27:04.000000 pyPPG-1.0.9/pyPPG/ppg_bm/__init__.py
+-rw-rw-rw-   0        0        0    48365 2023-08-14 07:57:41.000000 pyPPG-1.0.9/pyPPG/ppg_bm/bm_extraction.py
+-rw-rw-rw-   0        0        0     4169 2023-08-14 07:49:48.000000 pyPPG-1.0.9/pyPPG/ppg_bm/derivs_ratios.py
+-rw-rw-rw-   0        0        0     2531 2023-08-14 07:49:48.000000 pyPPG-1.0.9/pyPPG/ppg_bm/ppg_derivs.py
+-rw-rw-rw-   0        0        0     5632 2023-08-14 07:49:48.000000 pyPPG-1.0.9/pyPPG/ppg_bm/ppg_sig.py
+-rw-rw-rw-   0        0        0     3689 2023-08-14 07:49:48.000000 pyPPG-1.0.9/pyPPG/ppg_bm/sig_ratios.py
+-rw-rw-rw-   0        0        0     1911 2023-08-13 09:42:51.000000 pyPPG-1.0.9/pyPPG/ppg_bm/statistics.py
+-rw-rw-rw-   0        0        0     5024 2023-08-13 10:54:11.000000 pyPPG-1.0.9/pyPPG/ppg_sqi.py
+-rw-rw-rw-   0        0        0     1846 2023-07-31 14:32:01.000000 pyPPG-1.0.9/pyPPG/preproc.py
+drwxrwxrwx   0        0        0        0 2023-08-14 08:19:44.848031 pyPPG-1.0.9/pyPPG.egg-info/
+-rw-rw-rw-   0        0        0     4509 2023-08-14 08:19:44.000000 pyPPG-1.0.9/pyPPG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      580 2023-08-14 08:19:44.000000 pyPPG-1.0.9/pyPPG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-14 08:19:44.000000 pyPPG-1.0.9/pyPPG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-14 08:19:44.000000 pyPPG-1.0.9/pyPPG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2023-08-14 08:19:44.000000 pyPPG-1.0.9/pyPPG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      190 2023-07-27 13:48:40.000000 pyPPG-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-14 08:19:44.855933 pyPPG-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1079 2023-08-14 08:19:05.000000 pyPPG-1.0.9/setup.py
```

### Comparing `pyPPG-1.0.8/LICENSE.txt` & `pyPPG-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.8/PKG-INFO` & `pyPPG-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPPG
-Version: 1.0.8
+Version: 1.0.9
 Summary: pyPPG: a python toolbox for PPG morphological analysis.
 Home-page: https://github.com/godamartonaron/GODA_pyPPG
 Author: Marton A. Goda, PhD
 Author-email: marton.goda@campus.technion.ac.il
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `pyPPG-1.0.8/README.md` & `pyPPG-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.8/pyPPG/DataHandling.py` & `pyPPG-1.0.9/pyPPG/datahandling.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,48 @@
-import pandas as pd
-
-from Preprocessing import*
+import pyPPG
+from preproc import*
 
 import matplotlib.pyplot as plt
 import scipy.io
 import numpy as np
 from dotmap import DotMap
 from tkinter import filedialog
 import mne
 from matplotlib.backends.backend_agg import FigureCanvasAgg as FigureCanvas
 import os
 
 ###########################################################################
 ####################### Data Acquisition from Files #######################
 ###########################################################################
-def load_data(data_path:str,filtering: bool):
+def load_data(data_path: str, start = 0, end = 0, filtering = True):
     """
     Load PPG data function load the raw PPG data.
 
     :param data_path: path of the PPG signal
     :type data_path: str
+    :param start: beginning the of signal in sample
+    :type start: int
+    :param end: end of the signal in sample
+    :type end: int
     :param filtering: a bool for filtering
     :type filtering: bool
 
     :return s: a struct of PPG signal:
-        - s.v: a vector of PPG values
-        - s.fs: the sampling frequency of the PPG in Hz
-        - s.name: name of the record
-        - s.v: 1-d array, a vector of PPG values
-        - s.fs: the sampling frequency of the PPG in Hz
-        - s.filt_sig: 1-d array, a vector of the filtered PPG values
-        - s.filt_d1: 1-d array, a vector of the filtered PPG' values
-        - s.filt_d2: 1-d array, a vector of the filtered PPG" values
-        - s.filt_d3: 1-d array, a vector of the filtered PPG'" values
+
+        * s.start: beginning of the signal in sample
+        * s.end: end of the signal in sample
+        * s.v: a vector of PPG values
+        * s.fs: the sampling frequency of the PPG in Hz
+        * s.name: name of the record
+        * s.v: 1-d array, a vector of PPG values
+        * s.fs: the sampling frequency of the PPG in Hz
+        * s.filt_sig: 1-d array, a vector of the filtered PPG values
+        * s.filt_d1: 1-d array, a vector of the filtered PPG' values
+        * s.filt_d2: 1-d array, a vector of the filtered PPG" values
+        * s.filt_d3: 1-d array, a vector of the filtered PPG'" values
     """
 
     if data_path=="":
         sig_path = filedialog.askopenfilename(title='Select SIGNAL file', filetypes=[("Input Files", ".mat .csv .edf .pkl .txt")])
     else:
         sig_path=data_path
 
@@ -51,74 +57,72 @@
     try:
         sig_format=sig_path[len(sig_path)-sig_path[::-1].index('.'):]
     except:
         print('Invalid signal path!')
 
     if sig_format=='mat':
         input_sig = scipy.io.loadmat(sig_path)
-        hr = np.float64(np.squeeze(input_sig.get("Data")))[0:]
+        sig = np.float64(np.squeeze(input_sig.get("Data")))[0:]
         try:
             fs = np.squeeze(input_sig.get("Fs"))
         except:
             fs = 100
             print('The default sampling frequency is 100 Hz for .mat.')
     elif sig_format=='csv':
         input_sig = np.loadtxt(sig_path, delimiter=',').astype(int)
-        hr = input_sig
+        sig = input_sig
         fs = 75
         print('The default sampling frequency is 75 Hz for .csv.')
     elif sig_format=='txt':
         try:
             input_sig = np.loadtxt(sig_path, delimiter='\t').astype(int)
         except:
             try:
                 input_sig = np.loadtxt(sig_path, delimiter=' ').astype(int)
             except:
                 print('ERROR! The data separator is not supported for .txt.')
-        hr = input_sig
+        sig = input_sig
         fs = 1000
         print('The default sampling frequency is 1 kHz for .txt.')
     elif sig_format == 'edf':
         input_sig = mne.io.read_raw_edf(sig_path)
-        hr = -input_sig['Pleth'][0][0]
+        sig = -input_sig['Pleth'][0][0]
         try:
             fs = int(np.round(input_sig.info['sfreq']))
         except:
             fs = 256
             print('The default sampling frequency is 256 Hz for .edf.')
 
     s = DotMap()
-    s.v=hr
+
+    s.start = start
+    if start<end:
+        s.end = end
+    else:
+        s.end = len(sig)
+
+    s.v=sig[s.start:s.end]
     s.fs=fs
     s.name=rec_name
-
-    s.filt_sig, s.filt_d1, s.filt_d2, s.filt_d3 = Preprocessing(s, True)
+    s.filt_sig, s.filt_d1, s.filt_d2, s.filt_d3 = Preprocessing(s, filtering = True)
 
     return s
 
 ###########################################################################
 ########################### Plot Fiducial points ##########################
 ###########################################################################
-def plot_fiducials(s: DotMap, fiducials: pd.DataFrame):
+def plot_fiducials(s: pyPPG.PPG, fp: pyPPG.Fiducials, savingfolder: str):
     """
     Plot fiducial points of the filtered PPG signal.
 
-    :param s: a struct of PPG signal:
-        - s.v: a vector of PPG values
-        - s.fs: the sampling frequency of the PPG in Hz
-        - s.name: name of the record
-        - s.v: 1-d array, a vector of PPG values
-        - s.fs: the sampling frequency of the PPG in Hz
-        - s.filt_sig: 1-d array, a vector of the filtered PPG values
-        - s.filt_d1: 1-d array, a vector of the filtered PPG' values
-        - s.filt_d2: 1-d array, a vector of the filtered PPG" values
-        - s.filt_d3: 1-d array, a vector of the filtered PPG'" values
-    :type s: DotMap
-    :param fiducials: a dictionary where the key is the name of the fiducial pints and the value is the list of fiducial points.
-    :type fiducials: DataFrame
+    :param s: a struct of PPG signal
+    :type s: pyPPG.PPG object
+    :param fp: a struct of fiducial points
+    :type fp: pyPPG.Fiducials object
+    :param savingfolder: location of the saved figure
     """
 
     fig = plt.figure(figsize=(20, 12))
     ax1 = plt.subplot(411)
     plt.plot(s.filt_sig, 'k', label=None)
     ax2 = plt.subplot(412, sharex=ax1)
     plt.plot(s.filt_d1, 'k', label=None)
@@ -155,15 +159,15 @@
             plt.subplot(411)
             plt.title(s.name, fontsize=20)
         else:
             plt_num = int(s_type[ind][-1]) + 1
 
 
         ax = plt.subplot(4, 1, plt_num)
-        tmp_pnt=eval("fiducials['" + n + "'].values")
+        tmp_pnt=eval("fp." + n + ".values")
         tmp_pnt=tmp_pnt[~np.isnan(tmp_pnt)].astype(int)
         tmp_sig=eval("s." + s_type[ind])
         exec("plt.scatter(tmp_pnt, tmp_sig[tmp_pnt], s=60,linewidth=2, marker = marker[ind],facecolors='none', color=color[ind], label=n)")
         plt.ylabel(ylabe_names[plt_num - 1], fontsize=20)
 
         exec("plt.xlim([str_sig,end_sig])")
         leg = plt.legend(loc='upper right', fontsize=20, ncol=2,facecolor="orange",frameon=True)
@@ -180,97 +184,91 @@
         plt.yticks([])
 
     plt.xlabel('Time [s]', fontsize=20)
     plt.xticks(major_ticks,major_ticks_names, fontsize=20)
     plt.show()
 
     canvas = FigureCanvas(fig)
-    tmp_dir='temp_dir'+os.sep+'PPG_Figures'+os.sep
-    os.makedirs(tmp_dir, exist_ok=True)
+    tmp_dir=savingfolder+os.sep+'PPG_Figures'+os.sep
+    if not os.path.exists(tmp_dir):
+        os.mkdir(tmp_dir)
 
-    canvas.print_png((tmp_dir+'%s.png') % (s.name))
-    print('Figure has been saved in the "temp_dir".')
+    canvas.print_png((tmp_dir+'%s_btwn_%s-%s.png') % (s.name,s.start,s.end))
+    print('Figure has been saved in the "'+savingfolder+'".')
 
 ###########################################################################
 ################################# Save Data ###############################
 ###########################################################################
 
-def save_data(s: DotMap, fiducials: pd.DataFrame, biomarkers_vals: dict, biomarkers_defs: dict, ppg_statistics: dict, savingformat: str,savingfolder: str):
+def save_data(s: pyPPG.PPG, fp: pyPPG.Fiducials, bm: pyPPG.Biomarkers, savingformat: str, savingfolder: str):
     """
     Save the results of the filtered PPG analysis.
 
-    :param s: a struct of PPG signal:
-        - s.v: a vector of PPG values
-        - s.fs: the sampling frequency of the PPG in Hz
-        - s.name: name of the record
-        - s.v: 1-d array, a vector of PPG values
-        - s.fs: the sampling frequency of the PPG in Hz
-        - s.filt_sig: 1-d array, a vector of the filtered PPG values
-        - s.filt_d1: 1-d array, a vector of the filtered PPG' values
-        - s.filt_d2: 1-d array, a vector of the filtered PPG" values
-        - s.filt_d3: 1-d array, a vector of the filtered PPG'" values
+    :param s: a struct of PPG signal
+    :type s: pyPPG.PPG object
     :type s: DotMap
-    :param fiducials: a dictionary where the key is the name of the fiducial pints and the value is the list of fiducial points
-    :type fiducials: DataFrame
-    :param biomarkers_vals: dictionary of biomarkers in different categories:
-        - PPG signal
-        - Signal ratios
-        - PPG derivatives
-        - Derivatives ratios
-    :type biomarkers_vals: dict
-    :param biomarkers_defs: dictionary of biomarkers with name, definition and unit:
-        - PPG signal
-        - Signal ratios
-        - PPG derivatives
-        - Derivatives ratios
-    :type biomarkers_defs: dict
-    :param Statistics: data frame with summary of PPG features
-    :type Statistics: dict
+    :param fp: a struct of fiducial points
+    :type fp: pyPPG.Fiducial object
+    :param bm: a dictionary of biomarkers
+    :type bm: pyPPG.Biomarkers object
     :param savingformat: file format of the saved date, the provided file formats .mat and .csv
     :type savingformat: str
     :param savingfolder: location of the saved data
     :type savingfolder: str
     """
 
     tmp_dir = savingfolder
     os.makedirs(tmp_dir, exist_ok=True)
 
-    temp_dirs= ['Fiducials','Biomarkers','Statistics','Biomarkers_defs']
+    temp_dirs = ['Fiducial_points', 'Biomarker_vals', 'Biomarker_stats', 'Biomarker_defs', 'PPG_struct']
     for i in temp_dirs:
-        temp_dir = tmp_dir+os.sep+i+os.sep
+        temp_dir = tmp_dir + os.sep + i + os.sep
         if not os.path.exists(temp_dir):
             os.mkdir(temp_dir)
 
-    BM_keys = biomarkers_vals.keys()
+
+    keys=s.__dict__.keys()
+    keys_list = list(keys)
+    sc=DotMap()
+    for i in keys_list:
+        exec('sc.'+i+' = s.'+i)
+
+    file_name = (r'.' + os.sep + tmp_dir + os.sep + temp_dirs[4] + os.sep + s.name + '_data_btwn_%s-%s.mat')%(s.start,s.end)
+    scipy.io.savemat(file_name, sc)
+
+    BM_keys = bm.bm_vals.keys()
 
     if savingformat=="csv":
-        file_name = (r'.'+os.sep+tmp_dir+os.sep+temp_dirs[0]+os.sep+s.name+'_'+'Fiducial.csv')
-        fiducials.to_csv(file_name)
+        file_name = (r'.'+os.sep+tmp_dir+os.sep+temp_dirs[0]+os.sep+s.name+'_'+'Fiducials_btwn_%s-%s.csv')%(s.start,s.end)
+        fp.get_fp().to_csv(file_name)
 
         for key in BM_keys:
-            file_name = (r'.'+os.sep+tmp_dir+os.sep+temp_dirs[1]+os.sep+'%s.csv')% (s.name+'_'+key)
-            biomarkers_vals[key].to_csv(file_name,index=True,header=True)
+            file_name = (r'.'+os.sep+tmp_dir+os.sep+temp_dirs[1]+os.sep+'%s_btwn_%s-%s.csv')%(s.name+'_'+key,s.start,s.end)
+            bm.bm_vals[key].to_csv(file_name,index=True,header=True)
+
+            file_name = (r'.'+os.sep+tmp_dir+os.sep+temp_dirs[2]+os.sep+'%s_btwn_%s-%s.csv')%(s.name+'_'+key,s.start,s.end)
+            bm.bm_stats[key].to_csv(file_name, index=True, header=True)
 
-            file_name = (r'.'+os.sep+tmp_dir+os.sep+temp_dirs[2]+os.sep+'%s.csv') % (s.name+'_'+key)
-            ppg_statistics[key].to_csv(file_name, index=True, header=True)
+            file_name = (r'.'+os.sep+tmp_dir+os.sep+temp_dirs[3]+os.sep+'%s_btwn_%s-%s.csv')%(s.name+'_'+key,s.start,s.end)
+            bm.bm_defs[key].to_csv(file_name, index=True, header=True)
 
     elif savingformat=="mat":
-        matlab_struct = fiducials.to_dict(orient='list')
-        file_name = (r'.'+os.sep+tmp_dir+os.sep+temp_dirs[0]+os.sep+s.name+'_'+'Fiducial.mat')
+        matlab_struct = fp.get_fp().to_dict(orient='list')
+        file_name = (r'.'+os.sep+tmp_dir+os.sep+temp_dirs[0]+os.sep+s.name+'_'+'Fiducials_btwn_%s-%s.mat')%(s.start,s.end)
         scipy.io.savemat(file_name,matlab_struct)
 
         for key in BM_keys:
-            matlab_struct = biomarkers_defs[key].to_dict(orient='list')
-            file_name = (r'.'+os.sep+tmp_dir+os.sep+temp_dirs[3]+os.sep+'%s.mat')% (key)
-            scipy.io.savemat(file_name,matlab_struct)
 
-            matlab_struct = biomarkers_vals[key].to_dict(orient='list')
-            file_name = (r'.'+os.sep+tmp_dir+os.sep+temp_dirs[1]+os.sep+'%s.mat')% (s.name+'_'+key)
+            matlab_struct = bm.bm_vals[key].to_dict(orient='list')
+            file_name = (r'.'+os.sep+tmp_dir+os.sep+temp_dirs[1]+os.sep+'%s_btwn_%s-%s.mat')%(s.name+'_'+key,s.start,s.end)
             scipy.io.savemat(file_name,matlab_struct)
 
-            file_name = (r'.'+os.sep+tmp_dir+os.sep+temp_dirs[2]+os.sep+'%s.mat') % (s.name+'_'+key)
-            ppg_statistics[key].to_csv(file_name, index=True, header=True)
-            scipy.io.savemat(file_name, matlab_struct)
+            file_name = (r'.'+os.sep+tmp_dir+os.sep+temp_dirs[2]+os.sep+'%s_btwn_%s-%s.mat')%(s.name+'_'+key,s.start,s.end)
+            scipy.io.savemat(file_name, bm.bm_stats[key])
+
+            matlab_struct = bm.bm_defs[key].to_dict(orient='list')
+            file_name = (r'.'+os.sep+tmp_dir+os.sep+temp_dirs[3]+os.sep+'%s_btwn_%s-%s.mat')%(s.name+'_'+key,s.start,s.end)
+            scipy.io.savemat(file_name,matlab_struct)
     else:
         print('The file format is not suported for data saving! You can use "mat" or "csv" file formats.')
 
     print('Results have been saved into the "'+tmp_dir+'".')
```

### Comparing `pyPPG-1.0.8/pyPPG/EXAMPLE.py` & `pyPPG-1.0.9/pyPPG/example.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,19 @@
-from DataHandling import*
-import FiducialPoints as Fp
-import Biomarkers as Bm
-from Statistics import*
-
-import matplotlib.pyplot as plt
-import numpy as np
-from dotmap import DotMap
-import time
+from pyPPG import*
+from datahandling import*
+import pyPPG.fiducials as FP
+import pyPPG.biomarkers as BM
 
 import sys
 import json
 
 ###########################################################################
 ################################## EXAMPLE ################################
 ###########################################################################
-def ppg_example(data_path="",filtering=True,correct=True, savefig=True, savedata=True, savingformat="mat",savingfolder="temp_dir"):
+def ppg_example(data_path="",start = 0, end = 0, filtering=True, correct=True, savingfolder="temp_dir", savefig=True, savedata=True, savingformat="csv"):
     '''
     This is an example code for PPG analysis. The main parts:
         1) Loading a raw PPG signal: various file formats such as .mat, .csv, .txt, or .edf.
         2) Get Fiducial points: extract the fiducial points of PPG, PPG', PPG'' and PPG'" signals
         3) Plot Fiducials Points
         4) Get Biomarkers: extract 74 PPG biomarkers in four categories:
             - PPG signal
@@ -26,52 +21,66 @@
             - PPG derivatives
             - Derivatives ratios
         5) Get Statistics: summary of the 74 PPG biomarkers
         6) Save data: save the extracted Fiducial points, Biomarkers, and Statistics into .csv file
 
     :param data_path: path of the PPG signal
     :type data_path: str
+    :param start: beginning the of signal in sample
+    :type start: int
+    :param end: end of the signal in sample
+    :type end: int
     :param filtering: a bool for filtering
     :type filtering: bool
-    :param savefig: a bool for current figure saving
-    :type savefig: bool
     :param correct: a bool for fiducials points corretion
     :type correct: bool
+    :param savingfolder: location of the saved data
+    :type savingfolder: str
+    :param savefig: a bool for current figure saving
+    :type savefig: bool
     :param savedata: a bool for saving fiducial points, biomarkers, and statistics
     :type savedata: bool
     :param savingformat: file format of the saved date, the provided file formats .mat and .csv
     :type savingformat: str
-    :param savingfolder: location of the saved data
-    :type savingfolder: str
 
     :return: fiducial points, a dictionary where the key is the name of the fiducial pints and the value is the list of fiducial points
-    '''
 
 
+    Example:
+
+        .. code-block:: python
+
+            from pyPPG import ppg_example
+
+            # run example code
+            ppg_example(savedata=True, savefig=True)
+
+    '''
+
     ## Loading a raw PPG signal
-    s=load_data(data_path,filtering)
+    ppg_data = load_data(data_path,start,end,filtering)
+    s = PPG(ppg_data)
 
     ## Get Fiducial points
-    fp = Fp.FiducialPoints(s)
-    fiducials=fp.getFiducialPoints(correct)
+    fpex = FP.FpCollection(s)
+    fiducials=fpex.get_fiducials(s,correct)+s.start
+    fp = Fiducials(fiducials)
 
     if savefig:
         ## Plot Fiducials Points
-        plot_fiducials(s, fiducials)
+        plot_fiducials(s, fp, savingfolder)
 
     if savedata:
-        ## Get Biomarkers
-        bm = Bm.Biomarkers(s, fiducials)
-        biomarkers_vals, biomarkers_defs = bm.getBiomarkers()
-
-        ## Get Statistics
-        statistics = Statistics(fiducials['sp'], fiducials['on'], biomarkers_vals)
+        ## Get Biomarkers and Statistics
+        bmex = BM.BmCollection(s, fp)
+        bm_defs, bm_vals, bm_stats = bmex.get_biomarkers()
+        bm = Biomarkers(bm_defs, bm_vals , bm_stats)
 
         ## Save data
-        save_data(s,fiducials,biomarkers_vals,biomarkers_defs,statistics,savingformat,savingfolder)
+        save_data(s, fp, bm, savingformat, savingfolder)
 
     print('Program finished')
     return fiducials
 
 
 ###########################################################################
 ############################## RUN EXAMPLE CODE ###########################
@@ -87,8 +96,8 @@
             fiducials = ppg_example(**function_args)
             json_data = fiducials.to_json(orient="split")
             print(json.dumps(json_data))
         else:
             print("Invalid function name")
     else:
         print("Please provide function name and arguments as JSON string")
-        ppg_example(savedata=True, savefig=True)
+        ppg_example(savedata=True, savefig=True)
```

### Comparing `pyPPG-1.0.8/pyPPG/FiducialPoints.py` & `pyPPG-1.0.9/pyPPG/fiducials.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,77 +1,66 @@
 import copy
 import pandas as pd
 
-from pack_ppg._ErrorHandler import _check_shape_, WrongParameter
+import pyPPG
 import numpy as np
 from dotmap import DotMap
 from scipy.signal import kaiserord, firwin, filtfilt, detrend, periodogram, lfilter, find_peaks, firls, resample
-import matplotlib.pyplot as plt
-import time
 from scipy import signal
 
-class FiducialPoints:
+class FpCollection:
 
     ###########################################################################
     ###################### Initialization of Fiducial Points ##################
     ###########################################################################
-    def __init__(self, s: DotMap):
+    def __init__(self, s: pyPPG.PPG):
         """
         The purpose of the FiducialPoints class is to calculate the fiducial points.
 
-        :param s: a struct of PPG signal:
-            - s.v: a vector of PPG values
-            - s.fs: the sampling frequency of the PPG in Hz
-            - s.name: name of the record
-            - s.v: 1-d array, a vector of PPG values
-            - s.fs: the sampling frequency of the PPG in Hz
-            - s.filt_sig: 1-d array, a vector of the filtered PPG values
-            - s.filt_d1: 1-d array, a vector of the filtered PPG' values
-            - s.filt_d2: 1-d array, a vector of the filtered PPG" values
-            - s.filt_d3: 1-d array, a vector of the filtered PPG'" values
-        :type s: DotMap
-
-        """
-        if s.fs <= 0:
-            raise WrongParameter("Sampling frequency should be strictly positive")
-        _check_shape_(s.v, s.fs)
+        :param s: object of PPG signal
+        :type s: pyPPG.PPG object
 
-        keys=s.keys()
+        """
+
+        keys=s.__dict__.keys()
         keys_list = list(keys)
         for i in keys_list:
-            exec('self.'+i+' = s[i]')
+            exec('self.'+i+' = s.'+i)
 
     ###########################################################################
     ############################ Get Fiducial Points ##########################
     ###########################################################################
-    def getFiducialPoints(self,correct: bool):
+    def get_fiducials(self, s: pyPPG.PPG, correct=True):
         '''The function calculates the PPG Fiducial Points.
-            - Original signal: List of pulse onset, pea and dicrotic notch
+            - Original signal: List of systolic peak, pulse onset, dicrotic notch, and diastolic peak
             - 1st derivative: List of points of 1st maximum and minimum in 1st derivitive between the onset to onset intervals (u,v)
             - 2nd derivative: List of maximum and minimum points in 2nd derivitive between the onset to onset intervals (a, b, c, d, e)
 
+        :param s: object of PPG signal
+        :type s: pyPPG.PPG object
         :param correct: a bool for fiducials points corretion
         :type correct: bool
 
-        :return: fiducial points, a dictionary where the key is the name of the fiducial pints and the value is the list of fiducial points
+        :param fiducials: a DataFrame where the key is the name of the fiducial pints and the value is the list of fiducial points PPG Fiducials Points.
+        :type fiducials: DataFrame
         '''
 
-        # 'abp' refers the improved Aboy++, and 'aby' refers the original Aboy peak detector
-        peak_detector='abp'
+        # 'ABD' refers the original Aboy peak detectorm and 'PPGdet' refers the improved version.
+        peak_detector='PPGdet'
 
         # Extract Fiducial Points
         drt0_fp=pd.DataFrame()
-        peaks, onsets = self.abdp_beat_detector(peak_detector)
-        dicroticnotch = self.getDicroticNotch(peaks, onsets)
+        peaks, onsets = self.get_peak_onset(peak_detector)
+        dicroticnotch = self.get_dicrotic_notch(peaks, onsets)
 
-        drt1_fp = self.getFirstDerivitivePoints(onsets)
-        drt2_fp = self.getSecondDerivitivePoints(onsets, peaks)
-        drt3_fp = self.getThirdDerivitivePoints(onsets, drt2_fp)
+        drt1_fp = self.get_1st_drt_fiducials(onsets)
+        drt2_fp = self.get_2nd_drt_fiducials(onsets, peaks)
+        drt3_fp = self.get_3rd_drt_fiducials(onsets, drt2_fp)
 
-        diastolicpeak = self.getDiastolicPeak(onsets, dicroticnotch, drt2_fp.e)
+        diastolicpeak = self.get_diastolic_peak(onsets, dicroticnotch, drt2_fp.e)
 
         # Merge Fiducial Points
         keys=('on', 'sp', 'dn','dp')
         dummy = np.empty(len(peaks))
         dummy.fill(np.NaN)
         n=0
         for temp_val in (onsets,peaks,dicroticnotch,diastolicpeak):
@@ -84,25 +73,25 @@
             for key in list(temp_drt.keys()):
                 fiducials[key] = dummy
                 temp_val = temp_drt[key].values
                 fiducials[key][0:len(temp_val)]=temp_val
 
         # Correct Fiducial Points
         if correct:
-            fiducials=self.CorrectFiducialPoints(fiducials)
+            fiducials=self.correct_fiducials(fiducials)
 
         fiducials=fiducials.astype('Int64')
         return fiducials
 
 
     ###########################################################################
     ############################ PPG beat detector ############################
     ###########################################################################
-    def abdp_beat_detector(self, peak_detector: str):
-        '''ABDP_BEAT_DETECTOR detects beats in a photoplethysmogram (PPG) signal
+    def get_peak_onset(self, peak_detector: str):
+        '''PPGdet detects beats in a photoplethysmogram (PPG) signal
         using the improved 'Automatic Beat Detection' of Aboy M et al.
 
         :param peak_detector: type of peak detector
         :type peak_detector: str
 
         :return:
             - peaks, 1-d array: indices of detected systolic peaks
@@ -137,25 +126,25 @@
         '''
 
         # inputs
         x = copy.deepcopy(self.filt_sig)                    #signal
         fso=self.fs
         fs = 75
         x = resample(x, int(len(self.filt_sig)*(fs/fso)))
-        up = self.setup_up_abdp_algorithm()                 #settings
+        up = self.set_beat_detection()                 #settings
         win_sec=10
         w = fs * win_sec                                    #window length(number of samples)
         win_starts = np.array(list(range(0,len(x),round(0.8*w))))
         win_starts = win_starts[0:min(np.where([win_starts >= len(x) - w])[1])]
         win_starts = np.insert(win_starts,len(win_starts), len(x) + 1 - w)
 
         # before pre-processing
         hr_win=0  #the estimated systolic peak-to-peak distance, initially it is 0
         hr_win_v=[]
-        px = self.DetectMaxima(x, 0, hr_win, peak_detector) # detect all maxima
+        px = self.detect_maxima(x, 0, hr_win, peak_detector) # detect all maxima
         if len(px)==0:
             peaks = []
             onsets = []
             return peaks, onsets
 
         # detect peaks in windows
         all_p4 = []
@@ -164,56 +153,56 @@
         hr_past = 0 # the actual heart rate
         hrvi = 0    # heart rate variability index
 
         for win_no in range(0,len(win_starts) - 1):
             curr_els = range(win_starts[win_no],win_starts[win_no] + w)
             curr_x = x[curr_els]
 
-            y1 = self.Bandpass(curr_x, fs, 0.9 * up.fl_hz, 3 * up.fh_hz)   # Filter no.1
-            hr = self.EstimateHeartRate(y1, fs, up, hr_past)               # Estimate HR from weakly filtered signal
+            y1 = self.def_bandpass(curr_x, fs, 0.9 * up.fl_hz, 3 * up.fh_hz)   # Filter no.1
+            hr = self.estimate_HR(y1, fs, up, hr_past)               # Estimate HR from weakly filtered signal
             hr_past=hr
             all_hr[win_no] = hr
 
-            if (peak_detector=='abp') and (hr>40):
+            if (peak_detector=='PPGdet') and (hr>40):
                 if win_no==0:
-                    p1 = self.DetectMaxima(y1, 0, hr_win, peak_detector)
+                    p1 = self.detect_maxima(y1, 0, hr_win, peak_detector)
                     tr = np.percentile(np.diff(p1), 50)
                     pks_diff = np.diff(p1)
                     pks_diff = pks_diff[pks_diff>=tr]
                     hrvi = np.std(pks_diff) / np.mean(pks_diff) * 5
 
                 hr_win = fs / ((1 + hrvi) * 3)
                 hr_win_v.append(hr_win)
             else:
                 hr_win=0
 
-            y2 = self.Bandpass(curr_x, fs, 0.9 * up.fl_hz, 2.5 * hr / 60)              # Filter no.2
-            y2_deriv = self.EstimateDeriv(y2)                                          # Estimate derivative from highly filtered signal
-            p2 = self.DetectMaxima(y2_deriv, up.deriv_threshold,hr_win, peak_detector) # Detect maxima in derivative
-            y3 = self.Bandpass(curr_x, fs, 0.9 * up.fl_hz, 10 * hr / 60)
-            p3 = self.DetectMaxima(y3, 50, hr_win, peak_detector)                      # Detect maxima in moderately filtered signal
+            y2 = self.def_bandpass(curr_x, fs, 0.9 * up.fl_hz, 2.5 * hr / 60)           # Filter no. 2
+            y2_deriv = self.estimate_deriv(y2)                                          # Estimate derivative from highly filtered signal
+            p2 = self.detect_maxima(y2_deriv, up.deriv_threshold,hr_win, peak_detector) # Detect maxima in derivative
+            y3 = self.def_bandpass(curr_x, fs, 0.9 * up.fl_hz, 10 * hr / 60)
+            p3 = self.detect_maxima(y3, 50, hr_win, peak_detector)                      # Detect maxima in moderately filtered signal
             p4 = self.find_pulse_peaks(p2, p3)
             p4 = np.unique(p4)
 
-            if peak_detector=='abp':
+            if peak_detector=='PPGdet':
                 if len(p4)>round(win_sec/2):
                     pks_diff = np.diff(p4)
                     tr = np.percentile(pks_diff, 30)
                     pks_diff = pks_diff[pks_diff >= tr]
 
                     med_hr=np.median(all_hr[np.where(all_hr>0)])
                     if ((med_hr*0.5<np.mean(pks_diff)) and (med_hr*1.5<np.mean(pks_diff))):
                         hrvi = np.std(pks_diff) / np.mean(pks_diff)*10
 
             all_p4 = np.concatenate((all_p4, win_starts[win_no] + p4), axis=None)
 
         all_p4=all_p4.astype(int)
         all_p4 = np.unique(all_p4)
 
-        peaks, fn = self.IBICorrect(all_p4, px, np.median(all_hr), fs, up)
+        peaks, fn = self.correct_IBI(all_p4, px, np.median(all_hr), fs, up)
 
         peaks = (all_p4/fs*fso).astype(int)
         onsets, peaks = self.find_onsets(self.filt_sig, fso, up, peaks,60/np.median(all_hr)*fs)
 
         # Correct Peaks
         for i in range(0, len(peaks) - 1):
             max_loc = np.argmax(self.filt_sig[onsets[i]:onsets[i + 1]]) + onsets[i]
@@ -234,15 +223,15 @@
             onsets = np.delete(onsets, temp_i)
 
         return peaks, onsets
 
     ###########################################################################
     ############################# Maximum detector ############################
     ###########################################################################
-    def DetectMaxima(self, sig: np.array, percentile: int ,hr_win: int, peak_detector: str):
+    def detect_maxima(self, sig: np.array, percentile: int ,hr_win: int, peak_detector: str):
         #Table VI pseudocode
         """
         Detect Maxima function detects all peaks in the raw and also in the filtered signal to find.
 
         :param sig: array of signal with shape (N,) where N is the length of the signal
         :type sig: 1-d array
         :param percentile: in each signal partition, a rank filter detects the peaks above a given percentile
@@ -254,21 +243,21 @@
 
         :return: maximum peaks of signal, 1-d array.
 
         """
 
         tr = np.percentile(sig, percentile)
 
-        if peak_detector=='aby':
+        if peak_detector=='ABD':
 
             s1,s2,s3 = sig[2:], sig[1:-1],sig[0:-2]
             m = 1 + np.array(np.where((s1 < s2) & (s3 < s2)))
             max_pks = m[sig[m] > tr]
 
-        if peak_detector=='abp':
+        if peak_detector=='PPGdet':
             s1,s2,s3 = sig[2:], sig[1:-1],sig[0:-2]
 
             max_loc = []
             min_loc = []
             max_pks=[]
             intensity_v = []
             if hr_win == 0:
@@ -280,29 +269,29 @@
 
                 for i in range(0,len(max_loc)):
                     values = abs(max_loc[i] - min_loc)
                     min_v = min(values)
                     min_i = np.where(min_v==values)[0][0]
                     intensity_v.append(sig[max_loc[i]] - sig[min_loc[min_i]])
 
-                # improvements:
-                #   - adaptive threshold
-                #   - probability density of maximum
+                # possible improvements:
+                #   - using adaptive thresholding for the maximum
+                #   - estimate probability density of the maximum
 
                 tr2 = np.mean(intensity_v)*0.25
                 max_pks = find_peaks(sig+min(sig),prominence=tr2,distance=hr_win)[0]
 
         return max_pks
 
     ###########################################################################
     ############################ Bandpass filtering ###########################
     ###########################################################################
-    def Bandpass(self, sig: np.array, fs: int, lower_cutoff: float, upper_cutoff: float):
+    def def_bandpass(self, sig: np.array, fs: int, lower_cutoff: float, upper_cutoff: float):
         """
-        Bandpass filter function detects all peaks in the raw and also in the filtered signal to find.
+        def_bandpass filter function detects all peaks in the raw and also in the filtered signal to find.
 
         :param sig: array of signal with shape (N,) where N is the length of the signal
         :type sig: 1-d array
         :param fs: sampling frequency
         :type fs: int
         :param lower_cutoff: lower cutoff frequency
         :type lower_cutoff: float
@@ -337,15 +326,15 @@
         bpf_sig = filtfilt(b, 1, s.v)
 
         return bpf_sig
 
     ###########################################################################
     ################### Filter the high frequency components  #################
     ###########################################################################
-    def elim_vlfs_abd(self, s: np.array, up: DotMap, lower_cutoff: float):
+    def elim_vlfs(self, s: np.array, up: DotMap, lower_cutoff: float):
         """
         This function filter the high frequency components.
 
         :param s: array of signal with shape (N,) where N is the length of the signal
         :type s: 1-d array
         :param up: setup up parameters of the algorithm
         :type up: DotMap
@@ -428,15 +417,15 @@
         s_filt.v = filtfilt(AMfilter, 1, s_dt)
 
         return s_filt
 
     ###########################################################################
     ########################### Heart Rate estimation #########################
     ###########################################################################
-    def EstimateHeartRate(self, sig: np.array, fs: int, up: DotMap, hr_past: int):
+    def estimate_HR(self, sig: np.array, fs: int, up: DotMap, hr_past: int):
         """
         Heart Rate Estimation function estimate the heart rate according to the previous heart rate in given time window
 
         :param sig: array of signal with shape (N,) where N is the length of the signal
         :type sig: 1-d array
         :type fs: int
         :param up: setup up parameters of the algorithm
@@ -467,35 +456,35 @@
         hr = int(hr[0])
 
         return hr
 
     ###########################################################################
     ############# Estimate derivative from highly filtered signal #############
     ###########################################################################
-    def EstimateDeriv(self, sig: np.array):
+    def estimate_deriv(self, sig: np.array):
         """
         Derivative Estimation function estimate derivative from highly filtered signal based on the
         General least-squares smoothing and differentiation by the convolution (Savitzky Golay) method
 
         :param sig: array of signal with shape (N,) where N is the length of the signal
         :type sig: 1-d array
 
         :return: derivative, 1-d array.
 
         """
 
         #Savitzky Golay
         deriv_no = 1
         win_size = 5
-        deriv = self.savitzky_golay_abd(sig, deriv_no, win_size)
+        deriv = self.savitzky_golay(sig, deriv_no, win_size)
 
         return deriv
 
 
-    def savitzky_golay_abd(self, sig: np.array, deriv_no: int, win_size: int):
+    def savitzky_golay(self, sig: np.array, deriv_no: int, win_size: int):
         """
         This function estimate the Savitzky Golay derivative from highly filtered signal
 
         :param sig: array of signal with shape (N,) where N is the length of the signal
         :type sig: 1-d array
         :param deriv_no: number of derivative
         :type deriv_no: int
@@ -619,17 +608,17 @@
         p4 = p4[np.where(~np.isnan(p4))]
         p4 = p4.astype(int)
         return p4
 
     ###########################################################################
     ####################### Correct peaks' location error #####################
     ###########################################################################
-    def  IBICorrect(self, p: np.array, m: np.array, hr: float, fs: int, up: DotMap):
+    def  correct_IBI(self, p: np.array, m: np.array, hr: float, fs: int, up: DotMap):
         """
-        This function corrects the peaks' location error
+        This function corrects the peaks' location (interbeat intervals) error
 
         :param p: systolic peaks of the PPG signal
         :type p: 1-d array
         :param m: all maxima of the PPG signal
         :type m: 1-d array
         :param hr: heart rate
         :type hr: float
@@ -705,15 +694,15 @@
         fn = IBIs > IBI_thresh
 
         return fn
 
     ###########################################################################
     ####################### Setup up the beat detector ########################
     ###########################################################################
-    def setup_up_abdp_algorithm(self):
+    def set_beat_detection(self):
         """
         This function setups the filter parameters of the algorithm
 
         :return: filter parameters of the algorithm, DotMap
 
         """
         # plausible HR limits
@@ -751,15 +740,15 @@
         :param med_hr: median heart rate
         :type med_hr: float
 
         :return: onsets, 1-d array
 
         """
 
-        Y1=self.Bandpass(sig, fs, 0.9*up.fl_hz, 3*up.fh_hz)
+        Y1=self.def_bandpass(sig, fs, 0.9*up.fl_hz, 3*up.fh_hz)
         temp_oi0=find_peaks(-Y1,distance=med_hr*0.3)[0]
 
         null_indexes = np.where(temp_oi0<peaks[0])
         if len(null_indexes[0])!=0:
             if len(null_indexes[0])==1:
                 onsets = [null_indexes[0][0]]
             else:
@@ -787,15 +776,15 @@
                 peaks = np.delete(peaks, i)
 
         return onsets,peaks
 
     ###########################################################################
     ########################## Detect dicrotic notch ##########################
     ###########################################################################
-    def getDicroticNotch (self, peaks: np.array, onsets: list):
+    def get_dicrotic_notch (self, peaks: np.array, onsets: list):
         """
         Dicrotic Notch function estimate the location of dicrotic notch in between the systolic and diastolic peak
 
         :param peaks: peaks of the signal
         :type peaks: 1-d array
         :param onsets: onsets of the signal
         :type onsets: list
@@ -813,15 +802,15 @@
         FcD = FcU + 5                               # Transition Frequency: 5 Hz
 
         n = 21                                      # Filter order
         f = [0, (FcU / Fn), (FcD / Fn), 1]          # Frequency band edges
         a = [1, 1, 0, 0]                            # Amplitudes
         b = firls(n, f, a)
 
-        lp_filt_sig = filtfilt(b, 1,  dxx)    # Low pass filtered signal with 20 cut off Frequency and 5 Hz Transition width
+        lp_filt_sig = filtfilt(b, 1,  dxx)          # Low pass filtered signal with 20 cut off Frequency and 5 Hz Transition width
 
         ## The weighting is calculated and applied to each beat individually
         def t_wmax(i, peaks,onsets):
             if i < 3:
                 HR = np.mean(np.diff(peaks))/fs
                 t_wmax = -0.1 * HR + 0.45
             else:
@@ -872,15 +861,15 @@
             dic_not.append(max_pp_i+onsets[i]+shift)
 
         return dic_not
 
     ###########################################################################
     ########################## Detect diastolic peak ##########################
     ###########################################################################
-    def getDiastolicPeak(self, onsets: list, dicroticnotch: list, e_point: pd.Series):
+    def get_diastolic_peak(self, onsets: list, dicroticnotch: list, e_point: pd.Series):
         """
         Dicrotic Notch function estimate the location of dicrotic notch in between the systolic and diastolic peak
 
         :param onsets: onsets of the signal
         :type onsets: list
         :param dicroticnotches: dicrotic notches of the signal
         :type dicroticnotches: list
@@ -917,15 +906,15 @@
                 pass
 
         return diastolicpeak
 
     ###########################################################################
     ####################### Get First Derivitive Points #######################
     ###########################################################################
-    def getFirstDerivitivePoints(self, onsets: list):
+    def get_1st_drt_fiducials(self, onsets: list):
         """Calculate first derivitive points u and v from the PPG' signal
 
         :param onsets: onsets of the signal
         :type onsets: list
 
         :return:
             - u: The highest amplitude between the pulse onset and systolic peak on PPG'
@@ -965,15 +954,15 @@
         drt1_fp = pd.DataFrame({"u":[], "v":[], "w":[]})
         drt1_fp.u, drt1_fp.v, drt1_fp.w = u, v, w
         return drt1_fp
 
     ###########################################################################
     ####################### Get Second Derivitive Points ######################
     ###########################################################################
-    def getSecondDerivitivePoints(self, onsets: list, peaks: np.array):
+    def get_2nd_drt_fiducials(self, onsets: list, peaks: np.array):
         """Calculate Second derivitive points a, b, c, d, e, and f from the PPG" signal
 
         :param onsets: onsets of the signal
         :type onsets: list
         :param peaks: peaks of the signal
         :param types: 1-d array
 
@@ -1077,15 +1066,15 @@
             except:
                 pass
 
         drt2_fp = pd.DataFrame({"a":[], "b":[], "c":[],"d":[], "e":[], "f":[]})
         drt2_fp.a, drt2_fp.b, drt2_fp.c, drt2_fp.d, drt2_fp.e, drt2_fp.f = a, b, c, d, e, f
         return drt2_fp
 
-    def getThirdDerivitivePoints(self, onsets: list, drt2_fp: pd.DataFrame):
+    def get_3rd_drt_fiducials(self, onsets: list, drt2_fp: pd.DataFrame):
         """Calculate third derivitive points p1 and p2 from the PPG'" signal
 
             :param onsets: onsets of the signal
             :type onsets: list
             :param drt2_fp: fiducial points of PPG" signal
             :type drt2_fp: DataFrame
 
@@ -1146,15 +1135,15 @@
                 pass
 
         drt3_fp = pd.DataFrame({"p1": [], "p2": []})
         drt3_fp.p1, drt3_fp.p2 = p1, p2
 
         return drt3_fp
 
-    def CorrectFiducialPoints(self,fiducials: pd.DataFrame):
+    def correct_fiducials(self,fiducials: pd.DataFrame):
         """Correct the Fiducial Points
 
             :param fiducials: a dictionary where the key is the name of the fiducial pints and the value is the list of fiducial points.
             :type fiducials: DataFrame
 
             :return:
                 - fiducials: a dictionary where the key is the name of the fiducial pints and the value is the list of fiducial points
@@ -1241,12 +1230,12 @@
                     fiducials.f[i] = min_f
             except:
                 pass
 
 
         # Correct diastolic peak
         try:
-            fiducials.dp = self.getDiastolicPeak(fiducials.on, fiducials.dn, fiducials.e)
+            fiducials.dp = self.get_diastolic_peak(fiducials.on, fiducials.dn, fiducials.e)
         except:
             pass
 
         return fiducials
```

### Comparing `pyPPG-1.0.8/pyPPG/Preprocessing.py` & `pyPPG-1.0.9/pyPPG/preproc.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.8/pyPPG/Statistics.py` & `pyPPG-1.0.9/pyPPG/ppg_bm/statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pandas as pd
 import scipy.stats
 
 ###########################################################################
 ###################### Statistics of PPG Biomarkers #######################
 ###########################################################################
 
-def Statistics(peaks: pd.Series, onsets: pd.Series, ppg_biomarkers: dict):
+def get_statistics(peaks: pd.Series, onsets: pd.Series, ppg_biomarkers: dict):
     """
     The function compares the different biomedical features of PPG signal.
 
     :param peaks: 1-d array, peaks of the signal
     :type peaks: Series
     :param onsets: 1-d array, onsets of the signal
     :type onsets: Series
```

### Comparing `pyPPG-1.0.8/pyPPG/ppgSQI.py` & `pyPPG-1.0.9/pyPPG/ppg_sqi.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 import numpy as np
 from scipy.signal import detrend, find_peaks, correlate
 from numpy.fft import fft, ifft, fftshift
 
-def ppgSQI(ppg, fs, ann_ppg):
+def get_ppgSQI(ppg: list, fs: int, annotation: list):
     '''
     PPG Signal Quality Index based on beat template correlation.
 
-    :param ppg: PPG data
+    :param ppg: a vector of PPG values
+    :type ppg: int
     :param fs: Samples frequency
-    :param ann_ppg: PPG annotation time(samples)
+    :type fs: int
+    :param annotation: PPG annotation time(samples)
+    :type annotation: list
+
     :return: psqi: PPG Signal Quality Index
 
-    Reference
-    ---------
-    Li, Qiao, and Gari D. Clifford. "Dynamic time warping and machine learning for signal quality assessment of pulsatile signals."
-    Physiological measurement 33.9 (2012): 1491.
 
-    Author:
-    Marton A. Goda – Faculty of Biomedical Engineering,
-    Technion – Israel Institute of Technology, Haifa, Israel (August 2022)
+    Reference:
+    ----------
 
     Original Matlab implementation:
     Qiao Li, November 10, 2014.
     https://github.com/MIT-LCP/PhysioNetChallengePublic/blob/master/2015/sample-submission/ppgSQI.m
+
+    Author:
+    Marton A. Goda – Faculty of Biomedical Engineering,
+    Technion – Israel Institute of Technology, Haifa, Israel (August 2022)
     '''
 
     Fs = fs
     # Create PPG template
-    t,v = template(ppg, ann_ppg-1, fs)
+    t,v = use_template(ppg, annotation-1, fs)
 
-    c1 = np.empty(len(ann_ppg)-1)
+    c1 = np.empty(len(annotation)-1)
     c1[:] = np.NaN
-    psqi = np.empty(len(ann_ppg)-1)
+    psqi = np.empty(len(annotation)-1)
     psqi[:] = np.NaN
 
-    for j in range (0,len(ann_ppg) - 1):
+    for j in range (0,len(annotation) - 1):
         # Calculate correlation coefficients based on the template length
-        beatbegin = ann_ppg[j]-1
-        beatend = ann_ppg[j + 1]-1
+        beatbegin = annotation[j]-1
+        beatend = annotation[j + 1]-1
         if beatend - beatbegin > 3 * Fs:
             beatend = beatbegin + 3 * Fs
 
         templatelength = len(t)
         if (beatbegin + templatelength - 1 > len(ppg)) or (beatend > len(ppg)) or (beatbegin < 1):
             continue
 
@@ -51,132 +54,136 @@
         if (c1[j] < 0):
             c1[j] = 0
 
         psqi[currentb] = c1[j]
 
     return psqi
 
-def template(wave, anntime, samp_freq):
-    # PPG waveform template creation.
-    # Written by Qiao Li, February 21, 2011.
-    #
-    # input:
-    #   wave: PPG data
-    #   anntime: PPG annotation time(sample)
-    #   samp_freq: sampling frequency, default is 125 Hz
-    # output:
-    #   t: PPG waveform template based on normal - length beats
-    #   valid:  1 for valid template
-    #           0 for invalid template
+def use_template(wave, annotation: list, fs: int):
+    '''
+    PPG waveform template creation.
+    Written by Qiao Li, February 21, 2011
+
+    :param wave: a vector of PPG wave
+    :type ppg: int
+    :param fs: Samples frequency
+    :type fs: int
+    :param annotation: PPG annotation time(sample)
+    :type ann_ppg: list
+
+    :return:
+        - template: PPG waveform template based on normal - length beats
+        - valid: 1 for valid template, 0 for invalid template
+    '''
 
-    t = []
+    template = []
     valid = 0
 
     # according to heart rate max(300 bpm) and min(20 bpm) to get max and min beat - by - beat interval
     hr_max = 300
-    bb_interval_min = samp_freq * 60 / hr_max
+    bb_interval_min = fs * 60 / hr_max
     hr_min = 20
-    bb_interval_max = samp_freq * 60 / hr_min
+    bb_interval_max = fs * 60 / hr_min
 
     # Normal beat thresholds
     normal_beat_length_min = 0.7
     normal_beat_lentth_max = 1.5
     normal_beat_percent_threshold = 0.5
 
     # using correlate to get the basic period of the PPG as the length of template
     data = detrend(wave)
 
     y = correlate(data, data, 'full', method='fft')
     lenw = len(wave)
-    lena = len(anntime)
+    lena = len(annotation)
     i = lenw
 
     locs = find_peaks(y[i:])[0]
     pks = y[locs]
     if len(pks)==0:
         return
 
     max_v=max(pks)
     max_i=np.where(pks==max_v)[0][0]
     i = locs[max_i]
 
-    cycle = samp_freq
+    cycle = fs
     if i < lenw - 1:
         cycle = i
 
     # cumulate the beats with reasonable length to get template
     if lena < 2:
         return
 
     p0 = 1
-    i = anntime[p0]
+    i = annotation[p0]
 
     temp_ahead=0
     while i - temp_ahead < 1:
         p0 = p0 + 1
         if (p0 > lena):
-            t = wave
+            template = wave
             valid = 0
             return
 
-        i = anntime[p0]
+        i = annotation[p0]
 
     if p0 + 1 >= lena:
         return
 
-    beat_interval = np.diff(anntime[p0:len(anntime)])
+    beat_interval = np.diff(annotation[p0:len(annotation)])
     median_bi = np.median(beat_interval)
 
     if median_bi!='NaN':
         temp_peak = abs(locs - median_bi)
         m = min(temp_peak)
         i = np.where(temp_peak==m)[0][0]
         cycle = locs[i]+1
     else:
         return
 
     # the length of template valid detection
     valid = 1
     if (cycle > bb_interval_max) or (cycle < bb_interval_min):
         valid = 0
-        t = np.zeros(cycle)
+        template = np.zeros(cycle)
         return
 
     n = 0
     d1 = 0
     invalidn = 0
-    currentbeatlength = anntime[p0 + 1] - anntime[p0]
+    currentbeatlength = annotation[p0 + 1] - annotation[p0]
     if currentbeatlength > 0:
         d1 = wave[i - temp_ahead:i + cycle]
         n = 1
     else:
         invalidn = invalidn + 1
         d1 = np.zeros(cycle + temp_ahead)
 
     p0 = p0
     if p0 < lena - 1:
-        i = anntime[p0]
+        i = annotation[p0]
         n = 1
         invalidn = 0
         while (i < lenw - cycle) and (p0 < lena - 1):
-            currentbeatlength = anntime[p0 + 1] - anntime[p0]
+            currentbeatlength = annotation[p0 + 1] - annotation[p0]
             if currentbeatlength > 0:
                 d1 = d1 + wave[i - temp_ahead:i + cycle]
                 n = n + 1
             else:
                 invalidn = invalidn + 1
 
             p0 = p0 + 1
-            i = anntime[p0]
+            i = annotation[p0]
 
         d1 = d1/n
         # normal beat is less than the reasonable percentage of all beats
         if (n / (n + invalidn)) < normal_beat_percent_threshold:
             valid = 0
         else:
             valid = 0
     else:
         valid=0
 
-    t = d1
+    template = d1
 
-    return t,valid
+    return template,valid
```

### Comparing `pyPPG-1.0.8/pyPPG/ppg_bm/biomarker_extractor.py` & `pyPPG-1.0.9/pyPPG/ppg_bm/bm_extraction.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import numpy as np
 from dotmap import DotMap
 import pandas as pd
 from scipy.signal import find_peaks
 
+import pyPPG
+
 ###########################################################################
 ####################### PPG biomarkers extraction #########################
 ###########################################################################
 
-class BmExtractor:
+class BmExctator:
     """
     Class that extracts the PPG biomarkers.
     """
 
     def __init__(self, data: DotMap, peak_value: float, peak_time: float, next_peak_value: float, next_peak_time: float, onsets_values: np.array, onsets_times: np.array,
                  sample_rate: int, list_biomarkers: list, fiducials: pd.DataFrame):
         """
 
         :param data: struct of PPG,PPG', PPG", PPG'":
+
             - data.sig: segment of PPG timeseries to analyse and extract biomarkers as a np array
             - data.d1: segment of PPG'
             - data.d2: segment of PPG"
             - data.d3: segment of PPG'"
         :type data: DotMap
         :param peak_value: PPG peak value
         :type peak_value: float
@@ -60,15 +63,15 @@
         self.u, self.v, self.w, self.Tu, self.Tv, self.Tw = self._getFirstDerivitivePoints()
         self.a, self.b, self.c, self.d, self.e, self.f, self.Ta, self.Tb, self.Tc, self.Td, self.Te, self.Tf = self._getSecondDerivitivePoints()
         self.p1, self.p2, self.Tp1, self.Tp2 = self._getThirdDerivitivePoints()
 
     def map_func(self):
         """ This function assign for each name of biomarkers a function that calculates it
 
-        :returns my_funcs: a dictionary where the key is the name of the feature and the value is the function to call
+        :returns my_funcs: a dictionary where the key is the name of the biomarker and the value is the function to call
         """
         my_funcs = {#PPG signal
                     "Tpi": self.getTpi(),
                     "Tpp": self.getTpp(),
                     "Tsys": self.getTsys(),
                     "Tdia": self.getTdia(),
                     "Tsp": self.getTsp(),
@@ -183,23 +186,23 @@
                     "RIp1": self.getRIp2(),
                     "RIp2": self.getRIp2(),
                     "SC": self.getSC(),
                     "IPAD": self.getIPAD(),
         }
         return my_funcs
 
-    def get_feature_extract_func(self):
-        """ This function go through the list of biomarkers and call the function that is relevant to calculate it each feature takes two spots in the feature vector: one for the average value and one for its standard deviation.
+    def get_biomarker_extract_func(self):
+        """ This function go through the list of biomarkers and call the function that is relevant to calculate it each biomarker takes two spots in the biomarker vector: one for the average value and one for its standard deviation.
 
-            :returns biomarkers_vec: a vector of each feature avg value and std of the patient"""
+            :returns biomarkers_vec: a vector of each biomarker avg value and std of the patient"""
         my_funcs = self.map_func()
         biomarkers_vec = []
 
-        for feature in self.list_biomarkers:
-            func_to_call = my_funcs[feature]
+        for biomarker in self.list_biomarkers:
+            func_to_call = my_funcs[biomarker]
             biomarkers_vec.append(func_to_call)
         return biomarkers_vec
 
     def _getPeaksOnsets(self,x):
         """Find the peaks and onsets of a short FILTERED segment of PPG
 
         :return: peaks
@@ -366,151 +369,151 @@
         right_onset_value = self.onsets_values[1]
         cst = right_onset_value - left_onset_value
         return cst
 
     def getTpi(self):
         """ Tpi which means the Pulse Interval, the time between the pulse onset and pulse offset.
 
-            :return: Tpi feature
+            :return: Tpi biomarker
         """
         return self.onsets_times[1] - self.onsets_times[0]
     def getTpp(self):
         """ Tpp means the Peak-to-Peak Interval, the time between two consecutive systolic peaks.
 
-            :return:  Tpp feature
+            :return:  Tpp biomarker
         """
         cardiac_period = self.next_peak_time - self.peak_time
         return cardiac_period
 
     def getTsys(self):
         """ Tsys means the Systolic Time, the time between the pulse onset and dicrotic notch.
 
-        :return: Tsys feature
+        :return: Tsys biomarker
         """
 
         Tsys = self.Tdn
         return Tsys
 
     def getTdia(self):
         """ Tdia means the Diastolic Time, the time between the dicrotic notch and pulse offset.
 
-        :return: Tdia feature
+        :return: Tdia biomarker
         """
 
         Tdia = self.getTpi()-self.Tdp
         return Tdia
 
     def getTsp(self):
         """ Tsp means the Systolic Peak Time, the time between the pulse onset and systolic peak.
 
-        :return: Tsp feature
+        :return: Tsp biomarker
         """
         left_onset = self.onsets_times[0]
         Tsp = self.peak_time - left_onset
         return Tsp
 
     def getTdp(self):
         """ Tdp means the Diastolic Peak Time, the time between the pulse onset and diastolic peak.
 
-        :return: Tdp feature
+        :return: Tdp biomarker
         """
 
         Tdp = self.Tdp
         return Tdp
 
     def get_deltaT(self):
         """ deltaT means the Time Delay, the time between the systolic peak and diastolic peak.
 
-        :return: deltaT feature
+        :return: deltaT biomarker
         """
 
         deltaT = self.Tdp-self.getTsp()
         return deltaT
 
     def getSystolicWidth_d_percent(self, d):
         """ The function calculates the Systolic Width,
             the width at x% of the Systolic Peak Amplitude between the pulse onset and systolic peak.
 
             :param d: the percentage chosen to calculate the width
 
-            :return: Tswx feature
+            :return: Tswx biomarker
         """
         # value in segment corresponding to d percent of pulse height
         d_percent_val = (d/100)*(self.peak_value - self.onsets_values[0]) + self.onsets_values[0]
         time_of_d = self._getSysTime_from_val(d_percent_val)
         Tswx = self.peak_time - (time_of_d/self.sample_rate)
         return Tswx
 
 
     def getDiastolicWidth_d_percent(self, d):
         """ The function calculates the Diastolic Width,
             the width at x% of the Systolic Peak Amplitude between the systolic peak and pulse offset.
 
             :param d: the percentage chosen to calculate the width
 
-            :return: Tdwx feature
+            :return: Tdwx biomarker
         """
         # value in segment corresponding to d percent of pulse height
         d_percent_val = (d/100)*(self.peak_value - self.onsets_values[1]) + self.onsets_values[1]
         time_of_d = self._getDiaTime_from_val(d_percent_val)
         Tdwx = (time_of_d/self.sample_rate) - self.peak_time
         return Tdwx
 
     def getSumSW_DW(self, d):
         """ The function calculates Pulse Width,
             the sum of the Systolic Width and Diastolic Width at x%.
 
             :param d: the percentage chosen to calculate the width
 
-            :return: Tpwx feature
+            :return: Tpwx biomarker
         """
         Tswx = self.getSystolicWidth_d_percent(d)
         Tdwx = self.getDiastolicWidth_d_percent(d)
         return Tswx + Tdwx
 
     def getSystolicPeak(self):
         """ The function calculates the Systolic Peak Amplitude, the difference in amplitude between the pulse onset and systolic peak.
 
-            :return: Systolic Peak Amplitude feature
+            :return: Systolic Peak Amplitude biomarker
         """
         sys_peak = self.peak_value - self.onsets_values[0]
         return sys_peak
     def getDicroticNotchAmplitude(self):
         """ The function calculates the Dicrotic Notch Amplitude, the difference in amplitude between the pulse onset and the dicrotic notch.
 
-            :return: Dicrotic Notch Amplitude feature
+            :return: Dicrotic Notch Amplitude biomarker
         """
         dn_value = self.segment[self.dn]
         dn_amp = dn_value - self.onsets_values[0]
         return dn_amp
 
     def getDiastolicPeak(self):
         """ The function calculates the Diastolic Peak Amplitude, the difference in amplitude between the pulse onset and the diastolic peak.
 
-            :return: Diastolic Peak Amplitude feature
+            :return: Diastolic Peak Amplitude biomarker
         """
         ## temp solution 04/04/2023 --> if DN==DP
         dp_value = self.segment[self.dp+20]
         dia_peak = dp_value - self.onsets_values[0]
         return dia_peak
 
     def getPulseOffsetAmplitude(self):
         """ The function calculates the Pulse Offset Amplitude, the difference in amplitude between the pulse onset and pulse offset.
 
-            :return: Pulse Offset Amplitude feature
+            :return: Pulse Offset Amplitude biomarker
         """
 
         offset_value = self.onsets_values[1]
         Aoff = offset_value - self.onsets_values[0]
         return Aoff
 
     def getAUCpi(self):
         """ The function the Area Under Pulse Interval Curve, the area under the pulse wave between pulse onset and pulse offset.
 
-            :return: AUCpi feature
+            :return: AUCpi biomarker
         """
         left_onset_time = self.onsets_times[0]*self.sample_rate
         right_onset_time = self.onsets_times[1]*self.sample_rate
         baseline_shift_slope = self._getBaselineSlope()
         baseline_cst = self._getBaselineCst()
         vec_value_between_ons = self.segment
         num_t = len(vec_value_between_ons)
@@ -521,15 +524,15 @@
         AUCpi = 10*sum/((self.peak_value - baseline) * (right_onset_time - left_onset_time))
 
         return AUCpi
 
     def getAUCsys(self):
         """ The function calculates the Area Under Systolic Curve, the area under the pulse wave between the pulse onset and dicrotic notch.
 
-            :return: AUCsys feature
+            :return: AUCsys biomarker
         """
         left_onset_time = self.onsets_times[0]*self.sample_rate
         right_onset_time = self.onsets_times[1]*self.sample_rate
         baseline_shift_slope = self._getBaselineSlope()
         baseline_cst = self._getBaselineCst()
         vec_value_between_ons = self.segment
         num_t = self.dn
@@ -540,116 +543,116 @@
         AUCsys = 10*sum/((self.peak_value - baseline) * (right_onset_time - left_onset_time))
 
         return AUCsys
 
     def getAUCdia(self):
         """ The function calculates Area Under Diastolic Curve, the area under the pulse wave between the dicrotic notch and pulse offset.
 
-            :return: AUCdia feature
+            :return: AUCdia biomarker
         """
         AUCdia = self.getAUCpi()-self.getAUCsys()
         return AUCdia
 
     def getIPR(self):
         """ The function calculates the Instantaneous Pulse Rate, 60/CP.
 
-            :return: IPR feature
+            :return: IPR biomarker
         """
         IPR = 60/self.getTpp()
         return IPR
 
     def get_ratio_Tsys_Tdia(self):
         """ The function calculates the ratio of the Systolic Time to the Diastolic Time.
 
-            :return: Tsys/Tdia feature
+            :return: Tsys/Tdia biomarker
         """
         Tsys_Tdia = self.getTsys()/self.getTdia()
         return Tsys_Tdia
 
     def get_ratio_Tpwx_Tpi(self, d):
         """ The function calculates the ratio of the Pulse Width at x% of the Systolic Peak Amplitude to the Systolic Peak Time.
 
             :param d: the percentage chosen to calculate the width
 
-            :return: The ratio of the Tpi to the Pulse Width feature
+            :return: The ratio of the Tpi to the Pulse Width biomarker
         """
         sys_width = self.getSystolicWidth_d_percent(d)
         dia_width = self.getDiastolicWidth_d_percent(d)
         width = sys_width + dia_width
         Tpi = self.getTpi()
         return width/Tpi
 
     def get_ratio_Tpwx_Tsp(self, d):
         """ The function calculates the ratio of the Pulse Width at x% of the Systolic Peak Amplitude to the Systolic Peak Time.
 
             :param d: the percentage chosen to calculate the width
 
-            :return: Tpwx/Tsp feature
+            :return: Tpwx/Tsp biomarker
         """
         Tswx = self.getSystolicWidth_d_percent(d)
         Tdwx = self.getDiastolicWidth_d_percent(d)
         Tpwx = Tswx + Tdwx
         Tsp = self.getSystolicPeakTime()
         return Tpwx/Tsp
 
     def get_ratio_Tdwx_Tswx(self, d):
         """ The function calculates the ratio of the Diastolic Width to the Systolic Width at x% width.
 
             :param d: the percentage chosen to calculate the width
 
-            :return: Tdwx/Tswx feature
+            :return: Tdwx/Tswx biomarker
         """
         Tswx = self.getSystolicWidth_d_percent(d)
         Tdwx = self.getDiastolicWidth_d_percent(d)
         return Tdwx/Tswx
 
     def get_ratio_Tsp_Tpi(self):
         """ The function calculates the ratio of the Systolic Peak Time to the Pulse Interval
 
-            :return: Tsp/Tpi feature
+            :return: Tsp/Tpi biomarker
         """
         Tsp = self.getSystolicPeakTime()
         Tpi = self.getTpi()
         return Tsp/Tpi
 
     def get_ratio_Asp_Aoff(self):
         """ The function calculates the ratio of the Systolic Peak Time to the Pulse Interval
 
-            :return: Asp/Aoff feature
+            :return: Asp/Aoff biomarker
         """
         Asp = self.getSystolicPeak()
         Aoff = self.onsets_values[1]
         return Asp/Aoff
 
     def get_ratio_Adp_Asp(self):
         """ The function calculates Reflection Index, the ratio of the Diastolic Peak Amplitude to the Systolic Peak Amplitude.
 
-            :return: Reflection Index feature
+            :return: Reflection Index biomarker
         """
         RI = self.getDiastolicPeak()/self.getSystolicPeak()
         return RI
     def getIPA(self):
         """ The function calculates the Inflection Point Area, the ratio of the Area Under Diastolic Curve to the Area Under Systolic Curve.
 
-            :return: IPA feature
+            :return: IPA biomarker
         """
         IPA = self.getAUCdia()/self.getAUCsys()
         return IPA
 
     def get_ratio_Tsp_Asp(self):
         """ The function calculates the ratio of the Systolic Peak Time to the Systolic Peak Amplitude.
 
-            :return: Tsp/Asp feature
+            :return: Tsp/Asp biomarker
         """
 
         return self.getTsp()/self.getSystolicPeak()
     def get_ratio_Asp_deltaT(self):
         """ The function calculates the Stiffness Index, the ratio of the Systolic Peak Amplitude to the Time Delay.
 
-            :return: Stiffness Index feature
+            :return: Stiffness Index biomarker
         """
         SI = self.getSystolicPeak()/(self.getTdp()-self.getTsp())
         return SI
 
     def get_ratio_Asp_TpiTsp(self):
         """ The function calculates the ratio of the Systolic Peak Amplitude to the difference between the Pulse Interval and Systolic Peak Time.
 
@@ -660,261 +663,261 @@
         Asp = self.getSystolicPeak()
         return Asp/(Tpi-Tsp)
 
 
     def get_u(self):
         """ u means the u-point sample, the sample between the pulse onset and u-point.
 
-            :return: u feature
+            :return: u biomarker
         """
         return self.u
 
 
     def get_v(self):
         """ v means the v-point sample, the sample between the pulse onset and v-point.
 
-            :return: v feature
+            :return: v biomarker
         """
         return self.v
 
     def get_w(self):
         """ w means the w-point sample, the sample between the pulse onset and w-point.
 
-            :return: w feature
+            :return: w biomarker
         """
         return self.w
 
     def get_a(self):
         """ a means the a-point sample, the sample between the pulse onset and a-point.
 
-            :return: a feature
+            :return: a biomarker
         """
         return self.a
 
     def get_b(self):
         """ b means the b-point sample, the sample between the pulse onset and b-point.
 
-            :return: b feature
+            :return: b biomarker
         """
         return self.b
 
     def get_c(self):
         """ c means the c-point sample, the sample between the pulse onset and c-point.
 
-            :return: c feature
+            :return: c biomarker
         """
         return self.c
 
     def get_d(self):
         """ d means the d-point sample, the sample between the pulse onset and d-point.
 
-            :return: d feature
+            :return: d biomarker
         """
         return self.d
 
     def get_e(self):
         """ e means the e-point sample, the sample between the pulse onset and e-point.
 
-            :return: e feature
+            :return: e biomarker
         """
         return self.e
 
     def get_f(self):
         """ f means the f-point sample, the sample between the pulse onset and f-point.
 
-            :return: f feature
+            :return: f biomarker
         """
         return self.f
 
     def get_Tu(self):
         """ Tu means the u-point time, the time between the pulse onset and u-point.
 
-            :return: Tu feature
+            :return: Tu biomarker
         """
         return self.Tu
 
     def get_Tv(self):
         """ Tv means the v-point time, the time between the pulse onset and v-point.
 
-            :return: Tv feature
+            :return: Tv biomarker
         """
         return self.Tv
 
     def get_Tw(self):
         """ Tw means the v-point time, the time between the pulse onset and w-point.
 
-            :return: Tw feature
+            :return: Tw biomarker
         """
         return self.Tw
 
     def get_Ta(self):
         """ Ta means the a-point time, the time between the pulse onset and a-point.
 
-            :return: Ta feature
+            :return: Ta biomarker
         """
         return self.Ta
 
     def get_Tb(self):
         """ Tb means the b-point time, the time between the pulse onset and b-point.
 
-            :return: Tb feature
+            :return: Tb biomarker
         """
         return self.Tb
 
     def get_Tc(self):
         """ Tc means the c-point time, the time between the pulse onset and c-point.
 
-            :return: Tb feature
+            :return: Tb biomarker
         """
         return self.Tc
 
     def get_Td(self):
         """ Td means the d-point time, the time between the pulse onset and d-point.
 
-            :return: Td feature
+            :return: Td biomarker
         """
         return self.Td
 
 
     def get_Te(self):
         """ Te means the e-point time, the time between the pulse onset and e-point.
 
-            :return: Te feature
+            :return: Te biomarker
         """
         return self.Te
 
     def get_Tf(self):
         """ Tf means the f-point time, the time between the pulse onset and f-point.
 
-            :return: Tf feature
+            :return: Tf biomarker
         """
         return self.Tf
 
     def get_Tbc(self):
         """ Tbc means the b–c time, the time between the b-point and c-point.
 
-            :return: Tbc feature
+            :return: Tbc biomarker
         """
         return self.Tc-self.Tb
 
     def get_Tbd(self):
         """ Tbd means the b–d time, the time between the b-point and d-point.
 
-            :return: Tbd feature
+            :return: Tbd biomarker
         """
         return self.Td - self.Tb
 
     def get_Tp1(self):
         """ Tp1 means the p1-point time, the time between the pulse onset and p1-point.
 
-            :return: Tp1 feature
+            :return: Tp1 biomarker
         """
         return self.Tp1
 
     def get_Tp2(self):
         """ Tp2 means the p1-point time, the time between the pulse onset and p2-point.
 
-            :return: Tp2 feature
+            :return: Tp2 biomarker
         """
         return self.Tp2
 
     def get_Tp1_dp(self):
         """ The function calculatesthe p1–dia time, the time between the p1-point and diastolic peak.
 
-            :return: Tdia-Tp1 feature
+            :return: Tdia-Tp1 biomarker
         """
         Tp1_dia=(self.dp-self.p1)/self.sample_rate
         return Tp1_dia
 
     def get_Tp2_dp(self):
         """ The function calculatesthe p2–dia time, the time between the p2-point and diastolic peak.
 
-            :return: Tdia-Tp2 feature
+            :return: Tdia-Tp2 biomarker
         """
         Tp2_dia=(self.dp-self.p2)/self.sample_rate
         return Tp2_dia
 
 
     def get_ratio_Tu_Tpi(self):
         """ The function calculates the ratio of the u-point time to the Pulse Interval.
 
-            :return: Tu/Tpi feature
+            :return: Tu/Tpi biomarker
         """
         T1 = self.get_Tu()
         return T1 / self.getTpp()
 
 
     def get_ratio_Tv_Tpi(self):
         """ The function calculates the ratio of the v-point time to the Pulse Interval.
 
-            :return: Tv/Tpi feature
+            :return: Tv/Tpi biomarker
         """
         Tv = self.get_Tv()
         return Tv / self.getTpp()
 
     def get_ratio_Tw_Tpi(self):
         """ The function calculates the ratio of the w-point time to the Pulse Interval.
 
-            :return: Tw/Tpi feature
+            :return: Tw/Tpi biomarker
         """
         Tw = self.get_Tw()
         return Tw / self.getTpp()
 
     def get_ratio_Ta_Tpi(self):
         """ The function calculates the ratio of the a-point time to the Pulse Interval.
 
-            :return: Ta/Tpi feature
+            :return: Ta/Tpi biomarker
         """
         Ta = self.get_Ta()
         return Ta / self.getTpp()
 
     def get_ratio_Tb_Tpi(self):
         """ The function calculates the ratio of the b-point time to the Pulse Interval.
 
-            :return: Tb/Tpi feature
+            :return: Tb/Tpi biomarker
         """
         Tb = self.get_Tb()
         return Tb / self.getTpp()
 
     def get_ratio_Tc_Tpi(self):
         """ The function calculates the ratio of the c-point time to the Pulse Interval.
 
-            :return: Tc/Tpi feature
+            :return: Tc/Tpi biomarker
         """
         Tc = self.get_Tc()
         return Tc / self.getTpp()
 
     def get_ratio_Td_Tpi(self):
         """ The function calculates the ratio of the d-point time to the Pulse Interval.
 
-            :return: Td/Tpi feature
+            :return: Td/Tpi biomarker
         """
         Td = self.get_Td()
         return Td / self.getTpp()
 
     def get_ratio_Te_Tpi(self):
         """ The function calculates the ratio of the e-point time to the Pulse Interval.
 
-            :return: Te/Tpi feature
+            :return: Te/Tpi biomarker
         """
         Te = self.get_Te()
         return Te / self.getTpp()
 
     def get_ratio_Tf_Tpi(self):
         """ The function calculates the ratio of the f-point time to the Pulse Interval.
 
-            :return: Tf/Tpi feature
+            :return: Tf/Tpi biomarker
         """
         Tf = self.get_Tf()
         return Tf / self.getTpp()
 
     def get_ratio_TuTa_Tpi(self):
         """ The function calculates the ratio of the difference between the u-point time and a-point time to the Pulse Interval.
 
-            :return: (Tu-Ta)/Tpi feature
+            :return: (Tu-Ta)/Tpi biomarker
         """
         Ta = self.get_Ta()
         Tu = self.get_Tu()
         Tpi = self.getTpi()
         return (Tu - Ta) / Tpi
 
     def get_ratio_TvTb_Tpi(self):
@@ -926,210 +929,210 @@
         Tv = self.get_Tv()
         Tpi = self.getTpi()
         return (Tv-Tb)/Tpi
 
     def get_ratio_Au_Asp(self):
         """ This function calculates the ratio of the u-point amplitude to the Systolic Peak Amplitude.
 
-            :return: Au/Asp feature
+            :return: Au/Asp biomarker
         """
         u_max = self.segment_d1[self.get_u()]
         sp_amp = self.peak_value
         return u_max / sp_amp
 
     def get_ratio_Av_Au(self):
         """ This function calculates the ratio of the v-point amplitude to the u-point amplitude.
 
-            :return: Av/Au feature
+            :return: Av/Au biomarker
         """
         u_max = self.segment_d1[self.get_u()]
         v_min = self.segment_d1[self.get_v()]
         return v_min / u_max
 
     def get_ratio_Aw_Au(self):
         """ This function calculates the ratio of the w-point amplitude to the u-point amplitude.
 
-            :return: Aw/Au feature
+            :return: Aw/Au biomarker
         """
         u_max = self.segment_d1[self.get_u()]
         w_max = self.segment_d1[self.get_w()]
         return w_max / u_max
 
     def get_ratio_Ab_Aa(self):
         """ This function calculates the ratio of the b-point amplitude to the a-point amplitude.
 
-            :return: Ab/Aa feature
+            :return: Ab/Aa biomarker
         """
         a_max = self.segment_d2[self.get_a()]
         b_min = self.segment_d2[self.get_b()]
         return b_min / a_max
 
     def get_ratio_Ac_Aa(self):
         """ This function calculates the ratio of the c-point amplitude to the a-point amplitude.
 
-            :return: Ac/Aa feature
+            :return: Ac/Aa biomarker
         """
         a_max = self.segment_d2[self.get_a()]
         c_max = self.segment_d2[self.get_c()]
         return c_max / a_max
 
     def get_ratio_Ad_Aa(self):
         """ This function calculates the ratio of the d-point amplitude to the a-point amplitude.
 
-            :return: Ad/Aa feature
+            :return: Ad/Aa biomarker
         """
         a_max = self.segment_d2[self.get_a()]
         d_min = self.segment_d2[self.get_d()]
         return d_min / a_max
 
     def get_ratio_Ae_Aa(self):
         """ This function calculates the ratio of the e-point amplitude to the a-point amplitude.
 
-            :return: Ae/Aa feature
+            :return: Ae/Aa biomarker
         """
         a_max = self.segment_d2[self.get_a()]
         e_max = self.segment_d2[self.get_e()]
         return e_max / a_max
 
     def get_ratio_Af_Aa(self):
         """ This function calculates the ratio of the f-point amplitude to the a-point amplitude.
 
-            :return: Af/Aa feature
+            :return: Af/Aa biomarker
         """
         a_max = self.segment_d2[self.get_a()]
         f_min = self.segment_d2[self.get_f()]
         return f_min / a_max
 
     def get_ratio_Ap2_Ap1(self):
         """ The function calculates the ratio of the p2-point amplitude to the p1-point amplitude.
 
-            :return: Ap2/Ap1 feature
+            :return: Ap2/Ap1 biomarker
         """
         Rp2p1 = self.segment[self.p2]/self.segment[self.p1]
         return Rp2p1
 
     def get_ratio_AcAb_Aa(self):
         """ The function calculates the ratio of the difference between the b-point amplitude and c-point amplitude to the a-point amplitude.
 
-            :return: (Ac-Ab)/Aa feature
+            :return: (Ac-Ab)/Aa biomarker
         """
         Aa = self.segment_d2[self.get_a()]
         Ab = self.segment_d2[self.get_b()]
         Ac = self.segment_d2[self.get_c()]
         return (Ac-Ab)/Aa
 
     def get_ratio_AdAb_Aa(self):
         """ The function calculates the ratio of the difference between the b-point amplitude and d-point amplitude to the a-point amplitude.
 
-            :return: (Ad-Ab)/Aa feature
+            :return: (Ad-Ab)/Aa biomarker
         """
         Aa = self.segment_d2[self.get_a()]
         Ab = self.segment_d2[self.get_b()]
         Ad = self.segment_d2[self.get_d()]
         return (Ad-Ab)/Aa
 
     def getAGI(self):
         """ The function calculates the Aging Index.
 
-            :return: (Ab-Ac-Ad-Ae)/Aa feature
+            :return: (Ab-Ac-Ad-Ae)/Aa biomarker
         """
         Aa = self.segment_d2[self.get_a()]
         Ab = self.segment_d2[self.get_b()]
         Ac = self.segment_d2[self.get_c()]
         Ad = self.segment_d2[self.get_d()]
         Ae = self.segment_d2[self.get_e()]
         return (Ab-Ac-Ad-Ae)/Aa
 
     def getAGImod(self):
         """ The function calculates the Modified Aging Index.
 
-            :return: (Ab-Ac-Ad)/Aa feature
+            :return: (Ab-Ac-Ad)/Aa biomarker
         """
         Aa = self.segment_d2[self.get_a()]
         Ab = self.segment_d2[self.get_b()]
         Ac = self.segment_d2[self.get_c()]
         Ad = self.segment_d2[self.get_d()]
         return (Ab-Ac-Ad)/Aa
 
     def getAGIinf(self):
         """ The function calculates the Informal Aging Index.
 
-            :return: (Ab-Ae)/Aa feature
+            :return: (Ab-Ae)/Aa biomarker
         """
         Aa = self.segment_d2[self.get_a()]
         Ab = self.segment_d2[self.get_b()]
         Ae = self.segment_d2[self.get_e()]
         return (Ab-Ae)/Aa
 
     def getAI(self):
         """ The function calculates the Augmentation Index, (PPG(Tp2) − PPG(Tp1))/Asp.
 
-            :return: AI feature
+            :return: AI biomarker
         """
         AI = (self.segment[self.p2]-self.segment[self.p1])/self.peak_value
         return AI
 
     def getRIp1(self):
         """ The function calculates the Reflection Index of p1, Adp/(PPG(Tp1) − PPG(Tpi(0))).
 
-            :return: RIp1 feature
+            :return: RIp1 biomarker
         """
         RIp1 = self.getDiastolicPeak()/self.segment[self.p1]
         return RIp1
 
     def getRIp2(self):
         """ The function calculates the Reflection Index of p2, Adp/(PPG(Tp2) − PPG(Tpi(0))).
 
-            :return: RIp2 feature
+            :return: RIp2 biomarker
         """
         RIp2 = self.getDiastolicPeak()/self.segment[self.p2]
         return RIp2
 
     def getSC(self):
         """ The function calculates the Spring Constant, PPG"(Tsp)/((Asp-Au)/Asp).
 
-            :return: SC feature
+            :return: SC biomarker
         """
         ddxSPA=self.segment_d2[(self.getTsp()*self.sample_rate).astype(int)]
         SPA=self.getSystolicPeak()
         MS=self.segment[self.u]
         SC = ddxSPA/((SPA-MS)/SPA)
         return SC
 
     def getIPAD(self):
         """ The function calculates the Inflection point area plus normalised d-point amplitude, AUCdia/AUCsys+Ad/Aa.
 
-            :return: IPAD feature
+            :return: IPAD biomarker
         """
         IPAD = self.getAUCdia()/self.getAUCsys()+self.get_ratio_Ad_Aa()
         return IPAD
     def getRatioSW_DW(self, d):
         """ The function calculates the ratio of systolic and diastolic width at d percent of the pulse height
 
             :param d: the percentage chosen to calculate the width
 
-            :return: ratio feature
+            :return: ratio biomarker
         """
         sw_d = self.getSystolicWidth_d_percent(d)
         dw_d = self.getDiastolicWidth_d_percent(d)
         ratio = dw_d/sw_d
         return ratio
 
     def getPIR(self):
         """ The function calculates the ratio between the peak value and the right onset value
 
-            :return: pir feature
+            :return: pir biomarker
         """
         pir = self.peak_value/self.onsets_values[1]
         return pir
 
     def getMS(self):
         """ The function calculates Maximum slope, PPG'(u)/(PPG(systolic peak) − PPG(systolic onset))
 
-            :return: MS feature
+            :return: MS biomarker
         """
         MS = self.segment_d1[self.u]
         return MS
 
     def getUpslope(self):
         """ The function calculates Systolic Upslope between the left onset and the systolic peak.
 
@@ -1149,15 +1152,15 @@
         left_onset_value = self.onsets_values[0]
         diff = self.peak_value - left_onset_value
         return diff
 
     def getSTT(self):
         """ STT means slope transit time, which based on geometrical considerations of the PPG pulse wave to account for simultaneous.
 
-            :return: STT feature
+            :return: STT biomarker
         """
         upslope = self.getUpslope()
         A = self.getdiffVal()
         return A/upslope
 
     def getSystolicPeakTime(self):
         """ Systolic Peak Time means the distance between the consecutive Systolic Peaks
@@ -1174,103 +1177,87 @@
         sys_peak_time = self.getSystolicPeakTime()
         sys_amplitude = self.getSystolicPeak()
         return sys_peak_time/sys_amplitude
 
     def getAGIext(self):
         """ The function calculates the Extended Aging Index.
 
-            :return: (Ab-Ac-Ad-Ae-Af)/Aa feature
+            :return: (Ab-Ac-Ad-Ae-Af)/Aa biomarker
         """
         Aa = self.segment_d2[self.get_a()]
         Ab = self.segment_d2[self.get_b()]
         Ac = self.segment_d2[self.get_c()]
         Ad = self.segment_d2[self.get_d()]
         Ae = self.segment_d2[self.get_e()]
         Af = self.segment_d2[self.get_e()]
         return (Ab-Ac-Ad-Ae-Af)/Aa
 
 ###########################################################################
-############################# Get PPG biomarkers ############################
+############################ Get PPG biomarkers ###########################
 ###########################################################################
-def get_biomarkers(s, fiducials, biomarkers_lst):
+def get_biomarkers(s: pyPPG.PPG, fp: pyPPG.Fiducials, biomarkers_lst):
     """
     The function calculates the biomedical biomarkers of PPG signal.
 
-    :param s: a struct of PPG signal:
-        - s.v: a vector of PPG values
-        - s.fs: the sampling frequency of the PPG in Hz
-        - s.name: name of the record
-        - s.v: 1-d array, a vector of PPG values
-        - s.fs: the sampling frequency of the PPG in Hz
-        - s.filt_sig: 1-d array, a vector of the filtered PPG values
-        - s.filt_d1: 1-d array, a vector of the filtered PPG' values
-        - s.filt_d2: 1-d array, a vector of the filtered PPG" values
-        - s.filt_d3: 1-d array, a vector of the filtered PPG'" values
-    :param fiducials: M-d Dateframe, where M is the number of fiducial points
-    :param biomarkers_lst: list of biomarkers
+    :param s: object of PPG signal
+    :type s: pyPPG.PPG object
+    :param fp: object of fiducial points
+    :type fp: pyPPG.Fiducials object
 
     :return:
         - df: data frame with onsets, offset and peaks
         - df_biomarkers: data frame with PPG signal biomarkers
     """
 
     fs=s.fs
     ppg=s.filt_sig
     data = DotMap()
 
     df = pd.DataFrame()
     df_biomarkers = pd.DataFrame(columns=biomarkers_lst)
-    peaks = fiducials.sp.values
-    onsets = fiducials.on.values
+    peaks = fp.sp.values
+    onsets = fp.on.values
 
-    # display(df_biomarkers)
     for i in range(len(onsets) - 1):
-        #   print(f'i is {i}')
         onset = onsets[i]
         offset = onsets[i + 1]
         data.sig = ppg[int(onset):int(offset)]
         data.d1 = s.filt_d1[int(onset):int(offset)]
         data.d2 = s.filt_d2[int(onset):int(offset)]
         data.d3 = s.filt_d3[int(onset):int(offset)]
         peak = peaks[(peaks > onset) * (peaks < offset)]
         if len(peak) != 1:
             continue
         peak = peak[0]
 
-        temp_fiducials = fiducials.iloc[[i]]
+        temp_fiducials = fp.get_row(i)
 
         peak_value = ppg[peak]
         peak_time = peak / fs
         onset_value = ppg[onset]
         onset_time = onset / fs
 
         if (peak_value - onset_value) == 0:
             continue
-        #     print(onset_time)
+
         offset_value = ppg[offset]
         offset_time = offset / fs
-        #     print(offset_time)
+
         idx_array = np.where(peaks == peak)
         idx = idx_array[0]
         onsets_values = np.array([onset_value, offset_value])
         onsets_times = np.array([onset_time, offset_time])
-        #     print(onset,peak, offset)
         if (idx + 1) < len(peaks):
             next_peak_value = ppg[peaks[idx + 1].astype('int64')][0]
             next_peak_time = peaks[idx + 1] / fs
             next_peak_time = next_peak_time[0]
-            #         plt.plot(data.sig)
-            #         plt.show()
-            #         print(peak_value,peak_time,next_peak_value,next_peak_time,onsets_values,onsets_times)
             try:
-                biomarkers_extractor = BmExtractor(data, peak_value, peak_time, next_peak_value, next_peak_time,
-                                                          onsets_values, onsets_times, fs, biomarkers_lst,temp_fiducials)
-                biomarkers_vec = biomarkers_extractor.get_feature_extract_func()
+                biomarkers_extractor = BmExctator(data, peak_value, peak_time, next_peak_value, next_peak_time, onsets_values, onsets_times, fs, biomarkers_lst,temp_fiducials)
+                biomarkers_vec = biomarkers_extractor.get_biomarker_extract_func()
                 lst = list(biomarkers_vec)
                 df_biomarkers.loc[len(df_biomarkers.index)] = lst
-                #         display(df_biomarkers)
                 df = pd.concat({'onset': onset, 'offset': offset, 'peak': peak}, ignore_index=True)
             except:
                 pass
         else:
             print("no more peaks")
     return df, df_biomarkers
```

### Comparing `pyPPG-1.0.8/pyPPG.egg-info/PKG-INFO` & `pyPPG-1.0.9/pyPPG.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPPG
-Version: 1.0.8
+Version: 1.0.9
 Summary: pyPPG: a python toolbox for PPG morphological analysis.
 Home-page: https://github.com/godamartonaron/GODA_pyPPG
 Author: Marton A. Goda, PhD
 Author-email: marton.goda@campus.technion.ac.il
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `pyPPG-1.0.8/pyPPG.egg-info/SOURCES.txt` & `pyPPG-1.0.9/pyPPG.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 AUTHORS.rst
 LICENSE.txt
 README.md
 pyproject.toml
 setup.py
-pyPPG/Biomarkers.py
-pyPPG/DataHandling.py
-pyPPG/EXAMPLE.py
-pyPPG/FiducialPoints.py
-pyPPG/Preprocessing.py
-pyPPG/Statistics.py
 pyPPG/__init__.py
-pyPPG/ppgSQI.py
+pyPPG/biomarkers.py
+pyPPG/datahandling.py
+pyPPG/example.py
+pyPPG/fiducials.py
+pyPPG/ppg_sqi.py
+pyPPG/preproc.py
 pyPPG.egg-info/PKG-INFO
 pyPPG.egg-info/SOURCES.txt
 pyPPG.egg-info/dependency_links.txt
 pyPPG.egg-info/requires.txt
 pyPPG.egg-info/top_level.txt
 pyPPG/pack_ppg/_ErrorHandler.py
 pyPPG/pack_ppg/__init__.py
 pyPPG/ppg_bm/__init__.py
-pyPPG/ppg_bm/biomarker_extractor.py
-pyPPG/ppg_bm/get_bm_derivs_ratios.py
-pyPPG/ppg_bm/get_bm_ppg_derivs.py
-pyPPG/ppg_bm/get_bm_ppg_sig.py
-pyPPG/ppg_bm/get_bm_sig_ratios.py
+pyPPG/ppg_bm/bm_extraction.py
+pyPPG/ppg_bm/derivs_ratios.py
+pyPPG/ppg_bm/ppg_derivs.py
+pyPPG/ppg_bm/ppg_sig.py
+pyPPG/ppg_bm/sig_ratios.py
+pyPPG/ppg_bm/statistics.py
```

### Comparing `pyPPG-1.0.8/setup.py` & `pyPPG-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import io
 
 with io.open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pyPPG',
-    version='1.0.8',
+    version='1.0.9',
     description='pyPPG: a python toolbox for PPG morphological analysis.',
     author='Marton A. Goda, PhD',
     author_email="marton.goda@campus.technion.ac.il",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/godamartonaron/GODA_pyPPG",
     project_urls={"Bug Tracker": "https://github.com/pypa/sampleproject/issues",},
```

