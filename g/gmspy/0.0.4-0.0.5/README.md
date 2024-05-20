# Comparing `tmp/gmspy-0.0.4.tar.gz` & `tmp/gmspy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmspy-0.0.4.tar", last modified: Wed Mar 15 02:12:32 2023, max compression
+gzip compressed data, was "gmspy-0.0.5.tar", last modified: Mon May 20 03:39:46 2024, max compression
```

## Comparing `gmspy-0.0.4.tar` & `gmspy-0.0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-03-15 02:12:32.328241 gmspy-0.0.4/
--rw-rw-rw-   0        0        0    34817 2022-12-02 05:00:10.000000 gmspy-0.0.4/LICENCE.txt
--rw-rw-rw-   0        0        0       43 2023-01-06 06:13:22.000000 gmspy-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1567 2023-03-15 02:12:32.328241 gmspy-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1119 2023-01-13 13:14:25.000000 gmspy-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-15 02:12:32.310294 gmspy-0.0.4/gmspy/
--rw-rw-rw-   0        0        0       23 2023-03-15 02:12:01.000000 gmspy-0.0.4/gmspy/__about__.py
--rw-rw-rw-   0        0        0      795 2023-02-26 13:35:00.000000 gmspy-0.0.4/gmspy/__init__.py
--rw-rw-rw-   0        0        0     2662 2023-01-06 07:06:18.000000 gmspy-0.0.4/gmspy/_baseline_corr.py
--rw-rw-rw-   0        0        0     8291 2023-01-14 04:46:30.000000 gmspy-0.0.4/gmspy/_const_duct_spec.py
--rw-rw-rw-   0        0        0     2500 2023-01-06 06:49:26.000000 gmspy-0.0.4/gmspy/_elas_resp_spec.py
--rw-rw-rw-   0        0        0     2620 2023-01-06 06:49:39.000000 gmspy-0.0.4/gmspy/_fou_pow_spec.py
--rw-rw-rw-   0        0        0     3851 2023-01-06 07:12:44.000000 gmspy-0.0.4/gmspy/_freq_filt.py
--rw-rw-rw-   0        0        0     5414 2023-01-06 06:50:00.000000 gmspy-0.0.4/gmspy/_lin_dyna_resp.py
--rw-rw-rw-   0        0        0     1580 2022-12-17 17:16:02.000000 gmspy-0.0.4/gmspy/_load_gm_examples.py
--rw-rw-rw-   0        0        0     1758 2023-02-17 15:54:44.000000 gmspy-0.0.4/gmspy/_load_peer.py
--rw-rw-rw-   0        0        0     6992 2023-02-26 13:42:00.000000 gmspy-0.0.4/gmspy/_load_peer_batch.py
--rw-rw-rw-   0        0        0     1171 2023-01-06 06:50:21.000000 gmspy-0.0.4/gmspy/_resample.py
-drwxrwxrwx   0        0        0        0 2023-03-15 02:12:32.328241 gmspy-0.0.4/gmspy/accelerograms/
--rw-rw-rw-   0        0        0    70397 2013-01-09 12:28:22.000000 gmspy-0.0.4/gmspy/accelerograms/ChiChi.dat
--rw-rw-rw-   0        0        0    59176 2013-01-09 12:30:44.000000 gmspy-0.0.4/gmspy/accelerograms/Friuli.dat
--rw-rw-rw-   0        0        0    65064 2013-01-09 12:41:24.000000 gmspy-0.0.4/gmspy/accelerograms/Hollister.dat
--rw-rw-rw-   0        0        0    64402 2013-01-09 12:44:22.000000 gmspy-0.0.4/gmspy/accelerograms/Imperial_Valley.dat
--rw-rw-rw-   0        0        0    66706 2013-01-09 12:46:26.000000 gmspy-0.0.4/gmspy/accelerograms/Kobe.dat
--rw-rw-rw-   0        0        0    56868 2013-01-09 12:48:54.000000 gmspy-0.0.4/gmspy/accelerograms/Kocaeli.dat
--rw-rw-rw-   0        0        0    78564 2013-01-09 12:51:40.000000 gmspy-0.0.4/gmspy/accelerograms/Landers.dat
--rw-rw-rw-   0        0        0    65026 2013-01-09 12:53:26.000000 gmspy-0.0.4/gmspy/accelerograms/Loma_Prieta.dat
--rw-rw-rw-   0        0        0    65123 2013-01-21 16:07:08.000000 gmspy-0.0.4/gmspy/accelerograms/Northridge.dat
--rw-rw-rw-   0        0        0    34501 2013-01-21 16:06:58.000000 gmspy-0.0.4/gmspy/accelerograms/Trinidad.dat
--rw-rw-rw-   0        0        0    42354 2023-03-15 02:05:55.000000 gmspy-0.0.4/gmspy/seismo.py
--rw-rw-rw-   0        0        0      486 2023-02-26 13:43:07.000000 gmspy-0.0.4/gmspy/test.py
-drwxrwxrwx   0        0        0        0 2023-03-15 02:12:32.310294 gmspy-0.0.4/gmspy.egg-info/
--rw-rw-rw-   0        0        0     1567 2023-03-15 02:12:32.000000 gmspy-0.0.4/gmspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      820 2023-03-15 02:12:32.000000 gmspy-0.0.4/gmspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-15 02:12:32.000000 gmspy-0.0.4/gmspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-03-15 02:12:32.000000 gmspy-0.0.4/gmspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-15 02:12:32.000000 gmspy-0.0.4/gmspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-15 02:12:32.328241 gmspy-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      906 2023-01-06 06:14:04.000000 gmspy-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 03:39:46.818643 gmspy-0.0.5/
+-rw-rw-rw-   0        0        0    34817 2022-12-02 05:00:10.000000 gmspy-0.0.5/LICENCE.txt
+-rw-rw-rw-   0        0        0       43 2023-01-06 06:13:22.000000 gmspy-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1702 2024-05-20 03:39:46.802430 gmspy-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1119 2023-01-13 13:14:25.000000 gmspy-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 03:39:46.629832 gmspy-0.0.5/gmspy/
+-rw-rw-rw-   0        0        0       23 2024-05-20 03:34:04.000000 gmspy-0.0.5/gmspy/__about__.py
+-rw-rw-rw-   0        0        0      795 2023-02-26 13:35:00.000000 gmspy-0.0.5/gmspy/__init__.py
+-rw-rw-rw-   0        0        0     2945 2023-07-08 16:26:56.000000 gmspy-0.0.5/gmspy/_artif_gm.py
+-rw-rw-rw-   0        0        0     2662 2023-01-06 07:06:18.000000 gmspy-0.0.5/gmspy/_baseline_corr.py
+-rw-rw-rw-   0        0        0     8434 2024-05-20 03:00:44.000000 gmspy-0.0.5/gmspy/_const_duct_spec.py
+-rw-rw-rw-   0        0        0     2650 2024-05-20 03:25:09.000000 gmspy-0.0.5/gmspy/_elas_resp_spec.py
+-rw-rw-rw-   0        0        0     2814 2024-05-20 03:01:39.000000 gmspy-0.0.5/gmspy/_fou_pow_spec.py
+-rw-rw-rw-   0        0        0     3901 2024-05-20 02:52:08.000000 gmspy-0.0.5/gmspy/_freq_filt.py
+-rw-rw-rw-   0        0        0     5762 2023-04-28 11:33:27.000000 gmspy-0.0.5/gmspy/_lin_dyna_resp.py
+-rw-rw-rw-   0        0        0     1580 2022-12-17 17:16:02.000000 gmspy-0.0.5/gmspy/_load_gm_examples.py
+-rw-rw-rw-   0        0        0     1758 2023-02-17 15:54:44.000000 gmspy-0.0.5/gmspy/_load_peer.py
+-rw-rw-rw-   0        0        0     6992 2023-02-26 13:42:00.000000 gmspy-0.0.5/gmspy/_load_peer_batch.py
+-rw-rw-rw-   0        0        0     1225 2024-05-20 02:59:54.000000 gmspy-0.0.5/gmspy/_resample.py
+drwxrwxrwx   0        0        0        0 2024-05-20 03:39:46.786793 gmspy-0.0.5/gmspy/accelerograms/
+-rw-rw-rw-   0        0        0    70397 2013-01-09 12:28:22.000000 gmspy-0.0.5/gmspy/accelerograms/ChiChi.dat
+-rw-rw-rw-   0        0        0    59176 2013-01-09 12:30:44.000000 gmspy-0.0.5/gmspy/accelerograms/Friuli.dat
+-rw-rw-rw-   0        0        0    65064 2013-01-09 12:41:24.000000 gmspy-0.0.5/gmspy/accelerograms/Hollister.dat
+-rw-rw-rw-   0        0        0    64402 2013-01-09 12:44:22.000000 gmspy-0.0.5/gmspy/accelerograms/Imperial_Valley.dat
+-rw-rw-rw-   0        0        0    66706 2013-01-09 12:46:26.000000 gmspy-0.0.5/gmspy/accelerograms/Kobe.dat
+-rw-rw-rw-   0        0        0    56868 2013-01-09 12:48:54.000000 gmspy-0.0.5/gmspy/accelerograms/Kocaeli.dat
+-rw-rw-rw-   0        0        0    78564 2013-01-09 12:51:40.000000 gmspy-0.0.5/gmspy/accelerograms/Landers.dat
+-rw-rw-rw-   0        0        0    65026 2013-01-09 12:53:26.000000 gmspy-0.0.5/gmspy/accelerograms/Loma_Prieta.dat
+-rw-rw-rw-   0        0        0    65123 2013-01-21 16:07:08.000000 gmspy-0.0.5/gmspy/accelerograms/Northridge.dat
+-rw-rw-rw-   0        0        0    34501 2013-01-21 16:06:58.000000 gmspy-0.0.5/gmspy/accelerograms/Trinidad.dat
+-rw-rw-rw-   0        0        0    44021 2024-05-20 03:30:29.000000 gmspy-0.0.5/gmspy/seismo.py
+drwxrwxrwx   0        0        0        0 2024-05-20 03:39:46.802430 gmspy-0.0.5/gmspy.egg-info/
+-rw-rw-rw-   0        0        0     1702 2024-05-20 03:39:46.000000 gmspy-0.0.5/gmspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      825 2024-05-20 03:39:46.000000 gmspy-0.0.5/gmspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 03:39:46.000000 gmspy-0.0.5/gmspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-20 03:39:46.000000 gmspy-0.0.5/gmspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-20 03:39:46.000000 gmspy-0.0.5/gmspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 03:39:46.818643 gmspy-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      857 2024-05-20 03:39:36.000000 gmspy-0.0.5/setup.py
```

### Comparing `gmspy-0.0.4/LICENCE.txt` & `gmspy-0.0.5/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `gmspy-0.0.4/PKG-INFO` & `gmspy-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: gmspy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Ground Motions Signal Processing for Python
 Home-page: https://github.com/yexiang1992
 Author: Yexiang Yan
 Author-email: yexiang_yan@outlook.com
 License: GPL Licence
 Keywords: Ground Motions Seismic IMs response spectra
 Platform: any
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8.*
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: joblib
+Requires-Dist: numba
+Requires-Dist: rich
 
 [![PyPI](https://img.shields.io/pypi/v/gmspy)](https://pypi.org/project/gmspy/)
 [![Downloads](https://static.pepy.tech/badge/gmspy)](https://pepy.tech/project/gmspy)
 [![Documentation Status](https://readthedocs.org/projects/gmspy/badge/?version=latest)](https://gmspy.readthedocs.io/en/latest/?badge=latest)
 ![license](https://img.shields.io/github/license/yexiang1992/gmspy)
 [![CodeFactor](https://www.codefactor.io/repository/github/yexiang1992/gmspy/badge)](https://www.codefactor.io/repository/github/yexiang1992/gmspy)
```

### Comparing `gmspy-0.0.4/README.md` & `gmspy-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gmspy-0.0.4/gmspy/__init__.py` & `gmspy-0.0.5/gmspy/__init__.py`

 * *Files identical despite different names*

### Comparing `gmspy-0.0.4/gmspy/_baseline_corr.py` & `gmspy-0.0.5/gmspy/_baseline_corr.py`

 * *Files identical despite different names*

### Comparing `gmspy-0.0.4/gmspy/_const_duct_spec.py` & `gmspy-0.0.5/gmspy/_const_duct_spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+from typing import Union
+
 import numpy as np
 from joblib import Parallel, delayed
 from numba import jit
 
 from ._lin_dyna_resp import lida
 from ._resample import resample
 
 
 def const_duct_spec(dt: float,
-                    acc: list,
-                    Ts: list,
+                    acc: Union[list, tuple, np.ndarray],
+                    Ts: Union[list, tuple, np.ndarray],
                     harden_ratio: float = 0.02,
                     damp_ratio: float = 0.05,
                     analy_dt: float = None,
                     mu: float = 5,
                     niter: int = 100,
                     tol: float = 0.01,
                     n_jobs: int = 0
@@ -60,23 +62,25 @@
     """
     acc = np.array(acc)
     if analy_dt is None:
         analy_dt = dt
     else:
         _, acc = resample(dt, acc, analy_dt)
     Ts = np.atleast_1d(Ts)
+    if np.abs(Ts[0] - 0) < 1e-8:
+        Ts[0] = 1e-6
     omegas = 2 * np.pi / Ts
     omegas = omegas[::-1]
     mass = 1.0
     # file_dir = os.path.abspath(os.path.dirname(__file__))
     # filename = 'temp_f.txt'  # file_dir.replace("\\", '/') + '/temp_f.txt'
     # Fdata = -mass * acc
     # np.savetxt(filename, Fdata, fmt="%f")
 
-    def run(omegai):
+    def run(omegai: float):
         k = mass * omegai ** 2
         ue, ve, ae = lida(dt, acc, omegai, damp_ratio)
         upeak = np.max(np.abs(ue))
         fpeak = k * upeak
         # mumin
         maxuy = np.max(np.abs(ue))
         fy = k * maxuy
```

### Comparing `gmspy-0.0.4/gmspy/_elas_resp_spec.py` & `gmspy-0.0.5/gmspy/_elas_resp_spec.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+from typing import Union
+
 import numpy as np
 from joblib import Parallel, delayed
 
 from ._lin_dyna_resp import lida
 
 
 def elas_resp_spec(dt: float,
-                   acc: list,
-                   Ts: list,
+                   acc: Union[list, tuple, np.ndarray],
+                   Ts: Union[list, tuple, np.ndarray],
                    damp_ratio: float = 0.05,
                    method: str = "nigam_jennings",
-                   n_jobs: int = 0):
+                   n_jobs: int = 0) -> np.ndarray:
     """Computing the Elastic Response Spectrum.
 
     Parameters
     ----------
     dt : float
         Time step.
     acc : 1D ArrayLike
@@ -41,14 +43,16 @@
     -------
     output: (len(Ts), 5) ArrayLike.
         Each column is the *pseudo-acceleration spectrum*, *pseudo-velocity spectrum*,
         *acceleration spectrum*, *velocity spectrum* and *displacement spectrum* in turn.
     """
     acc = np.array(acc)
     Ts = np.atleast_1d(Ts)
+    if np.abs(Ts[0] - 0) < 1e-8:
+        Ts[0] = 1e-6
     omegas = 2 * np.pi / Ts
 
     def spec(wn):
         d, v, a = lida(dt, acc, wn, damp_ratio, method=method)
         sd = np.max(np.abs(d))
         sv = np.max(np.abs(v))
         sa = np.max(np.abs(a))
```

### Comparing `gmspy-0.0.4/gmspy/_fou_pow_spec.py` & `gmspy-0.0.5/gmspy/_fou_pow_spec.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,18 @@
+from typing import Union
+
 import matplotlib.pyplot as plt
 import numpy as np
+from scipy.fft import fft, fftfreq
 
 
-def fou_pow_spec(ts: list, acc: list, plot: bool = False):
+def fou_pow_spec(
+        ts: Union[list, tuple, np.ndarray],
+        acc: Union[list, tuple, np.ndarray],
+        plot: bool = False):
     """The Fourier Amplitude Spectrum and the Power Spectrum (or Power Spectral Density Function)
     are computed by means of Fast Fourier Transformation (FFT) of the input time-history.
 
     * Fourier Amplitude is computed as the square root of the sum of the squares of the real and imaginary parts of the
       Fourier transform: SQRT (Re^2+Im^2);
     * Fourier Phase is computed as the angle given by the real and imaginary parts of
       the Fourier transform: ATAN (Re/Im);
@@ -31,39 +37,38 @@
     phase: 1D ArrayLike
         Fourier Phase.
     pow_amp: 1D ArrayLike
         Power Spectral Amplitude.
     """
     n = len(acc)
     dt = ts[1] - ts[0]
-    Nfft = int(2 ** np.ceil(np.log2(n)))
-    af = np.fft.fft(acc, Nfft, norm='ortho')
-    freq = np.fft.fftfreq(Nfft, d=dt)
-    # freq = freq[np.argsort(freq)]
-    # af = af[np.argsort(freq)]
-    idx = freq > 0
-    af = af[idx]
-    freq = freq[idx]
-    # Fourier amplitudes
-    amp = np.abs(af)
-    # Fourier Phase
-    phase = np.arctan(af.real / af.imag)
+    af = fft(acc)[:n//2] / n
+    amp = 2.0 * np.abs(af)
+    freq = fftfreq(n, d=dt)[:n//2]
+    df = freq[1] - freq[0]
+    phase = np.angle(af)  # Fourier Phase
     # Power Spectral Amplitude
-    Arms = np.sqrt(np.trapz(acc ** 2, ts) / ts[-1])
-    pow_amp = amp ** 2 / (np.pi * ts[-1] * Arms**2)
+    # Arms = np.sqrt(np.trapz(acc ** 2, ts) / ts[-1])
+    pow_amp = 2 * np.abs(af) ** 2 / df  # / (np.pi * ts[-1] * Arms**2)
 
     if plot:
-        fig, axs = plt.subplots(3, 1, figsize=(10, 10))
-        plot_x = [ts, freq, freq]
-        plot_y = [acc, amp, pow_amp]
-        xlabels = ['Time(s)', "frequency(Hz)", "frequency(Hz)"]
-        ylabels = ['acceleration', "Fourier Amplitude", "Power Amplitude"]
-        for i in range(3):
+        fig, axs = plt.subplots(4, 1, figsize=(10, 15))
+        plot_x = [ts, freq, freq, freq]
+        plot_y = [acc, amp, pow_amp, phase]
+        xlabels = ['Time(s)', "frequency(Hz)",
+                   "frequency(Hz)", "frequency(Hz)"]
+        ylabels = ['acceleration', "Fourier Amplitude",
+                   "Power Amplitude", "Phase Angle"]
+        for i in range(4):
             ax = axs[i]
-            ax.plot(plot_x[i], plot_y[i], c='k', lw=1)
+            if i < 3:
+                ax.plot(plot_x[i], plot_y[i], c='k', lw=1)
+            else:
+                ax.plot(plot_x[i], plot_y[i], 'o', c='k', )
+                ax.set_aspect('equal')
             ax.set_xlabel(xlabels[i], fontsize=15)
             ax.set_ylabel(ylabels[i], fontsize=15)
             ax.tick_params(labelsize=12)
             if i == 0:
                 ax.set_xlim(np.min(plot_x[i]), np.max(plot_x[i]))
             else:
                 ax.set_xlim(np.min(plot_x[i]), 15)
```

### Comparing `gmspy-0.0.4/gmspy/_freq_filt.py` & `gmspy-0.0.5/gmspy/_freq_filt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy import signal
-
+from typing import Union
 
 def freq_filt(dt: float,
-              acc: list,
+              acc: Union[list, tuple, np.ndarray],
               ftype: str = "Butterworth",
               btype: str = "bandpass",
               order: int = 4,
               freq1: float = 0.1,
               freq2: float = 24.99,
               rp: float = 3,
               plot: bool = False
```

### Comparing `gmspy-0.0.4/gmspy/_lin_dyna_resp.py` & `gmspy-0.0.5/gmspy/_lin_dyna_resp.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from numba import jit
 
 
-def lida(dt: float,
-         acc: list,
-         omega: float,
-         damp_ratio: float = 0.05,
-         method: str = "nigam_jennings",
-         plot: bool = False):
+def lida(
+    dt: float,
+    acc: list,
+    omega: float,
+    damp_ratio: float = 0.05,
+    method: str = "nigam_jennings",
+    plot: bool = False,
+):
     """Linear Dynamic Time-History Analysis of Single Degree of Freedom Systems via Fast Fourier Transform.
 
     Parameters
     ----------
     dt : float
         Time step.
     acc : 1D ArrayLike
@@ -45,72 +47,106 @@
         a, v, u = _newmark(dt, acc, omega, damp_ratio, gamma=0.5, beta=0.25)
     elif method.lower() == "newmark1":
         a, v, u = _newmark(dt, acc, omega, damp_ratio, gamma=0.5, beta=1 / 6)
     else:
         raise ValueError(f"Not supported method {method}!")
 
     if plot:
-        fig, axs = plt.subplots(3, 1, figsize=(9, 9), sharex='all')
+        fig, axs = plt.subplots(3, 1, figsize=(9, 9), sharex="all")
         plot_y = [a, v, u]
-        y_labels = ['acc', 'vel', 'disp']
+        y_labels = ["acc", "vel", "disp"]
         ts = np.arange(len(acc)) * dt
         for i in range(3):
             ax = axs[i]
-            ax.plot(ts, plot_y[i], c='k', lw=1.2)
+            ax.plot(ts, plot_y[i], c="k", lw=1.2)
             ax.set_ylabel(y_labels[i], fontsize=15)
             ax.grid(False)
             ax.tick_params(labelsize=12)
             ax.set_xlim(np.min(ts), np.max(ts))
-        axs[-1].set_xlabel('Time (s)', fontsize=15)
+        axs[-1].set_xlabel("Time (s)", fontsize=15)
         plt.show()
     return u, v, a
 
 
 def _sodf_fft(dt, acc, omega, damp_ratio):
     n = len(acc)
     Nfft = int(2 ** np.ceil(np.log2(n)))
     af = np.fft.fft(acc, Nfft)
     f = np.fft.fftfreq(Nfft, d=dt)
     ws = 2.0 * np.pi * f
     H = 1 / (ws**2 - 2 * ws * damp_ratio * omega * 1j - omega**2)
     u = np.fft.ifft(af * H).real
     v = np.fft.ifft(af * ws * H * 1j).real
-    a = np.fft.ifft(-af * ws ** 2 * H).real
+    a = np.fft.ifft(-af * ws**2 * H).real
     u = u[:n]
     v = v[:n]
     a = a[:n]
     a = a + acc
     return a, v, u
 
 
 @jit(nopython=True)
 def _nigam_jennings(dt, acc, omega, damp_ratio):
     xi = damp_ratio
     wn = omega
-    wd = wn * np.sqrt(1 - xi ** 2)
-    a11 = (np.exp(-xi * wn * dt) * (xi / np.sqrt(1 - xi**2)
-           * np.sin(wd * dt) + np.cos(wd * dt)))
+    wd = wn * np.sqrt(1 - xi**2)
+    a11 = np.exp(-xi * wn * dt) * (
+        xi / np.sqrt(1 - xi**2) * np.sin(wd * dt) + np.cos(wd * dt)
+    )
     a12 = np.exp(-xi * wn * dt) / wd * np.sin(wd * dt)
-    a21 = - wn / np.sqrt(1 - xi**2) * np.exp(-xi * wn * dt) * np.sin(wd * dt)
-    a22 = (np.exp(-xi * wn * dt) * (np.cos(wd * dt) -
-           xi / np.sqrt(1 - xi**2) * np.sin(wd * dt)))
-    b11 = np.exp(-xi * wn * dt) * (((2 * xi**2 - 1) / wn**2 / dt + xi / wn) * np.sin(wd * dt) /
-                                   wd + (2 * xi / wn**3 / dt + 1 / wn**2) * np.cos(wd * dt)) - 2 * xi / wn ** 3 / dt
-    b12 = -np.exp(-xi * wn * dt) * (((2 * xi**2 - 1) / wn ** 2 / dt) * np.sin(wd * dt) /
-                                    wd + 2 * xi / wn**3 / dt * np.cos(wd * dt)) - 1 / wn**2 + 2 * xi / wn**3 / dt
-    b21 = (-1 / wn**2 * (-1 / dt + np.exp(-xi * wn * dt) * ((wn / np.sqrt(1 - xi**2) +
-           xi / dt / np.sqrt(1 - xi**2)) * np.sin(wd * dt) + 1 / dt * np.cos(wd * dt))))
-    b22 = (-1 / wn**2 / dt * (1 - np.exp(-xi * wn * dt) *
-           (xi / np.sqrt(1 - xi**2) * np.sin(wd * dt) + np.cos(wd * dt))))
+    a21 = -wn / np.sqrt(1 - xi**2) * np.exp(-xi * wn * dt) * np.sin(wd * dt)
+    a22 = np.exp(-xi * wn * dt) * (
+        np.cos(wd * dt) - xi / np.sqrt(1 - xi**2) * np.sin(wd * dt)
+    )
+    b11 = (
+        np.exp(-xi * wn * dt)
+        * (
+            ((2 * xi**2 - 1) / wn**2 / dt + xi / wn) * np.sin(wd * dt) / wd
+            + (2 * xi / wn**3 / dt + 1 / wn**2) * np.cos(wd * dt)
+        )
+        - 2 * xi / wn**3 / dt
+    )
+    b12 = (
+        -np.exp(-xi * wn * dt)
+        * (
+            ((2 * xi**2 - 1) / wn**2 / dt) * np.sin(wd * dt) / wd
+            + 2 * xi / wn**3 / dt * np.cos(wd * dt)
+        )
+        - 1 / wn**2
+        + 2 * xi / wn**3 / dt
+    )
+    b21 = (
+        -1
+        / wn**2
+        * (
+            -1 / dt
+            + np.exp(-xi * wn * dt)
+            * (
+                (wn / np.sqrt(1 - xi**2) + xi / dt / np.sqrt(1 - xi**2))
+                * np.sin(wd * dt)
+                + 1 / dt * np.cos(wd * dt)
+            )
+        )
+    )
+    b22 = (
+        -1
+        / wn**2
+        / dt
+        * (
+            1
+            - np.exp(-xi * wn * dt)
+            * (xi / np.sqrt(1 - xi**2) * np.sin(wd * dt) + np.cos(wd * dt))
+        )
+    )
     d = [0]
     v = [0]
     a = [-acc[0]]
     for i in range(len(acc) - 1):
-        d_ = a11 * d[i] + a12 * v[i] + b11 * acc[i] + b12 * acc[i+1]
-        v_ = a21 * d[i] + a22 * v[i] + b21 * acc[i] + b22 * acc[i+1]
+        d_ = a11 * d[i] + a12 * v[i] + b11 * acc[i] + b12 * acc[i + 1]
+        v_ = a21 * d[i] + a22 * v[i] + b21 * acc[i] + b22 * acc[i + 1]
         a_ = -acc[i + 1] - wn**2 * d_ - 2 * xi * wn * v_
         d.append(d_)
         v.append(v_)
         a.append(a_)
     return np.array(a) + acc, np.array(v), np.array(d)
 
 
@@ -125,12 +161,18 @@
     k_hat = wn**2 + a1
     d = [0]
     v = [0]
     a = [acc0]
     for i in range(len(acc) - 1):
         acc_temp = -acc[i + 1] + a1 * d[i] + a2 * v[i] + a3 * a[i]
         d.append(acc_temp / k_hat)
-        v.append(gamma / beta / dt * (d[i + 1] - d[i]) +
-                 (1 - gamma / beta) * v[i] + dt * (1 - gamma / 2 / beta) * a[i])
-        a.append(1 / beta / dt**2 * (d[i + 1] - d[i]) -
-                 1 / beta / dt * v[i] - (1 / 2 / beta - 1) * a[i])
+        v.append(
+            gamma / beta / dt * (d[i + 1] - d[i])
+            + (1 - gamma / beta) * v[i]
+            + dt * (1 - gamma / 2 / beta) * a[i]
+        )
+        a.append(
+            1 / beta / dt**2 * (d[i + 1] - d[i])
+            - 1 / beta / dt * v[i]
+            - (1 / 2 / beta - 1) * a[i]
+        )
     return np.array(a) + acc, np.array(v), np.array(d)
```

### Comparing `gmspy-0.0.4/gmspy/_load_gm_examples.py` & `gmspy-0.0.5/gmspy/_load_gm_examples.py`

 * *Files identical despite different names*

### Comparing `gmspy-0.0.4/gmspy/_load_peer.py` & `gmspy-0.0.5/gmspy/_load_peer.py`

 * *Files identical despite different names*

### Comparing `gmspy-0.0.4/gmspy/_load_peer_batch.py` & `gmspy-0.0.5/gmspy/_load_peer_batch.py`

 * *Files identical despite different names*

### Comparing `gmspy-0.0.4/gmspy/_resample.py` & `gmspy-0.0.5/gmspy/_resample.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import fractions
+from typing import Union
+
 import numpy as np
 from scipy import signal
 
 
-def resample(dt: float, acc: list, dti: float):
+def resample(dt: float, acc: Union[list, tuple, np.ndarray], dti: float):
     """Resampling the signal.
 
     Parameters
     ----------
     dt: float
         The size of the time step of the input acceleration time history.
     acc: 1D ArrayLike
```

### Comparing `gmspy-0.0.4/gmspy/accelerograms/ChiChi.dat` & `gmspy-0.0.5/gmspy/accelerograms/ChiChi.dat`

 * *Files identical despite different names*

### Comparing `gmspy-0.0.4/gmspy/accelerograms/Friuli.dat` & `gmspy-0.0.5/gmspy/accelerograms/Friuli.dat`

 * *Files identical despite different names*

### Comparing `gmspy-0.0.4/gmspy/accelerograms/Hollister.dat` & `gmspy-0.0.5/gmspy/accelerograms/Hollister.dat`

 * *Files identical despite different names*

### Comparing `gmspy-0.0.4/gmspy/accelerograms/Imperial_Valley.dat` & `gmspy-0.0.5/gmspy/accelerograms/Imperial_Valley.dat`

 * *Files identical despite different names*

### Comparing `gmspy-0.0.4/gmspy/accelerograms/Kobe.dat` & `gmspy-0.0.5/gmspy/accelerograms/Kobe.dat`

 * *Files identical despite different names*

### Comparing `gmspy-0.0.4/gmspy/accelerograms/Kocaeli.dat` & `gmspy-0.0.5/gmspy/accelerograms/Kocaeli.dat`

 * *Files identical despite different names*

### Comparing `gmspy-0.0.4/gmspy/accelerograms/Landers.dat` & `gmspy-0.0.5/gmspy/accelerograms/Landers.dat`

 * *Files identical despite different names*

### Comparing `gmspy-0.0.4/gmspy/accelerograms/Loma_Prieta.dat` & `gmspy-0.0.5/gmspy/accelerograms/Loma_Prieta.dat`

 * *Files identical despite different names*

### Comparing `gmspy-0.0.4/gmspy/accelerograms/Northridge.dat` & `gmspy-0.0.5/gmspy/accelerograms/Northridge.dat`

 * *Files identical despite different names*

### Comparing `gmspy-0.0.4/gmspy/accelerograms/Trinidad.dat` & `gmspy-0.0.5/gmspy/accelerograms/Trinidad.dat`

 * *Files identical despite different names*

### Comparing `gmspy-0.0.4/gmspy/seismo.py` & `gmspy-0.0.5/gmspy/seismo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Union
 
-import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 from rich import print
 from rich.console import Console
-from rich.table import Column, Table
+from rich.table import Table
 from scipy.integrate import cumulative_trapezoid, trapz
 
 from ._const_duct_spec import const_duct_spec
 from ._elas_resp_spec import elas_resp_spec
 from ._fou_pow_spec import fou_pow_spec
 from ._freq_filt import freq_filt
 
@@ -26,26 +25,25 @@
     acc: 1D ArrayLike
         The acceleration time history.
     unit: str, optional, one of ('g', 'm', 'cm', 'mm', 'in', 'ft')
         Unit of input acceleration time-history, by default "g", ignoring time unit /s2.
 
     """
 
-    def __init__(self,
-                 dt: float,
-                 acc: list,
-                 unit: str = 'g'
-                 ) -> None:
+    def __init__(self, dt: float, acc: Union[list, tuple, np.ndarray], unit: str = "g") -> None:
         self.dt = dt
         self.acc = np.array(acc)
         if np.abs(self.acc[0]) > 1e-5:
             self.acc = np.insert(self.acc, 0, 0)
         self.nacc = len(self.acc)
         self.time = np.arange(self.nacc) * dt
 
+        self.disp = None
+        self.vel = None
+
         # Arias IMs
         self.Arias = None
         self.AriasSeries = None
         self.AriasPercent = None
         # Tsp
         self.Tsp = None
         self.Spec_sp = None
@@ -55,106 +53,152 @@
         self.vel_unit = None
         self.disp_unit = None
         self.acc_factor = None
         self.vel_factor = None
         self.disp_factor = None
         self.unit_factors = {
             "g-g": 1.0,
-            "g-m": 9.81, "g-cm": 981, "g-mm": 9810, "g-in": 9.81 * 39.3701, "g-ft": 9.81 * 3.28084,
-            "m-m": 1, "m-cm": 100, "m-mm": 1000, "m-in": 39.3701, "m-ft": 3.28084, "m-g": 1 / 9.81,
-            "cm-m": 0.01, "cm-cm": 1, "cm-mm": 10, "cm-in": 0.393701, "cm-ft": 0.0328084, "cm_g": 1 / 981,
-            "mm-m": 0.001, "mm-cm": 0.1, "mm-mm": 1, "mm-in": 0.0393701, "mm-ft": 0.00328084, "mm-g": 1 / 9810,
-            "in-m": 0.0254, "in-cm": 2.54, "in-mm": 25.4, "in-in": 1, "in-ft": 0.0833333, "in-g": 1 / (9.81 * 39.3701),
-            "ft-m": 0.3048, "ft-cm": 30.48, "ft-mm": 304.8, "ft-in": 12, "ft-ft": 1, "ft-g": 1 / (9.81 * 3.28084),
+            "g-m": 9.81,
+            "g-cm": 981,
+            "g-mm": 9810,
+            "g-in": 9.81 * 39.3701,
+            "g-ft": 9.81 * 3.28084,
+            "m-m": 1,
+            "m-cm": 100,
+            "m-mm": 1000,
+            "m-in": 39.3701,
+            "m-ft": 3.28084,
+            "m-g": 1 / 9.81,
+            "cm-m": 0.01,
+            "cm-cm": 1,
+            "cm-mm": 10,
+            "cm-in": 0.393701,
+            "cm-ft": 0.0328084,
+            "cm_g": 1 / 981,
+            "mm-m": 0.001,
+            "mm-cm": 0.1,
+            "mm-mm": 1,
+            "mm-in": 0.0393701,
+            "mm-ft": 0.00328084,
+            "mm-g": 1 / 9810,
+            "in-m": 0.0254,
+            "in-cm": 2.54,
+            "in-mm": 25.4,
+            "in-in": 1,
+            "in-ft": 0.0833333,
+            "in-g": 1 / (9.81 * 39.3701),
+            "ft-m": 0.3048,
+            "ft-cm": 30.48,
+            "ft-mm": 304.8,
+            "ft-in": 12,
+            "ft-ft": 1,
+            "ft-g": 1 / (9.81 * 3.28084),
         }
-        self.set_units(acc=unit, vel='cm', disp='cm')
+        self.set_units(acc=unit, vel="cm", disp="cm", verbose=False)
 
         # colors
-        self.colors = ['#037ef3', '#f85a40',
-                       '#00c16e', '#7552cc', '#0cb9c1', '#f48924']
+        self.colors = [
+            "#037ef3", "#f85a40", "#00c16e", "#7552cc", "#0cb9c1", "#f48924"
+        ]
 
     def set_units(self,
                   acc: str = "g",
                   vel: str = "cm",
-                  disp: str = "cm"):
+                  disp: str = "cm",
+                  verbose: bool = True):
         """Specify the unit of input acceleration time-history and the units of output velocity and displacement.
 
         Parameters
         ----------
         acc : str, optional, one of ('g', 'm', 'cm', 'mm', 'in', 'ft')
             Unit of input acceleration time-history, by default "g",  ignoring time unit /s2.
         vel : str, optional, one of ('m', 'cm', 'mm', 'in', 'ft')
             Unit of output velocity, by default "cm",  ignoring time unit /s.
         disp : str, optional, one of ('m', 'cm', 'mm', 'in', 'ft')
             Unit of output displacement, by default "cm".
+        verbose: bool, default=True
+            Print info.
         """
         self.acc_factor = self.unit_factors[f"{self.acc_unit}-{acc}"]
         self.acc_unit = acc
         self.acc *= self.acc_factor
         self.vel = cumulative_trapezoid(self.acc, self.time, initial=0)
         self.disp = cumulative_trapezoid(self.vel, self.time, initial=0)
         self.vel_factor = self.unit_factors[f"{acc}-{vel}"]
         self.disp_factor = self.unit_factors[f"{acc}-{disp}"]
         self.vel_unit = vel
         self.disp_unit = disp
         self.vel *= self.vel_factor
         self.disp *= self.disp_factor
-        acc_end = '' if self.acc_unit == 'g' else "/s2"
-        print(f"[#0099e5]acc-unit: {self.acc_unit}{acc_end};[/]\n"
-              f"[#ff4c4c]vel-unit；{self.vel_unit}/s;[/]\n"
-              f"[#34bf49]disp-unit: {self.disp_unit}[/]")
+        acc_end = "" if self.acc_unit == "g" else "/s2"
+        if verbose:
+            print(f"[#0099e5]acc-unit: {self.acc_unit}{acc_end};[/]\n"
+                  f"[#ff4c4c]vel-unit；{self.vel_unit}/s;[/]\n"
+                  f"[#34bf49]disp-unit: {self.disp_unit}[/]")
 
     def plot_hist(self):
-        acc_unit_end = '' if self.acc_unit == 'g' else "/$s^2$"
-        vel_unit_end = '/s'
-        ylabels = [f'acc ({self.acc_unit}{acc_unit_end})',
-                   f'vel ({self.vel_unit}{vel_unit_end})',
-                   f'disp ({self.disp_unit})'
-                   ]
-        fig, axs = plt.subplots(3, 1, figsize=(9, 9), sharex='all')
+        acc_unit_end = "" if self.acc_unit == "g" else "/$s^2$"
+        vel_unit_end = "/s"
+        ylabels = [
+            f"acc ({self.acc_unit}{acc_unit_end})",
+            f"vel ({self.vel_unit}{vel_unit_end})",
+            f"disp ({self.disp_unit})",
+        ]
+        fig, axs = plt.subplots(3, 1, figsize=(9, 9), sharex="all")
         plot_y = [self.acc, self.vel, self.disp]
         for i in range(3):
             ax = axs[i]
             ax.plot(self.time, plot_y[i], lw=1.5, c=self.colors[i])
             ax.set_xlim(np.min(self.time), np.max(self.time))
             ax.grid(False)
             ax.set_ylabel(ylabels[i], fontsize=15)
             ax.tick_params(labelsize=12)
         axs[-1].set_xlabel("Time (s)", fontsize=15)
         plt.show()
 
     def get_acc(self):
-        """return acceleration time history.
-        """
+        """return acceleration time-history."""
         return self.acc
 
     def get_vel(self):
-        """return velocity time history.
-        """
+        """return velocity time-history."""
         return self.vel
 
     def get_disp(self):
-        """return displacement time history.
-        """
+        """return displacement time-history."""
         return self.disp
 
     def get_time(self):
-        """return time array.
-        """
+        """return time array."""
         return self.time
 
     def get_time_hists(self):
         """return acceleration, velocity, and displacement time history.
 
         Returns
         --------
             A length 3 tuple of acceleration, velocity, and displacement time histories.
         """
         return self.acc, self.vel, self.disp
 
+    def get_truncate_hists(self):
+        """Returns the truncated time-histories for 5%-95% Arias intensity.
+
+        Returns
+        -------
+        (acc, vel, disp): 1D Array like.
+        """
+        if self.Arias is None:
+            _ = self.get_ia()
+        Arias = self.Arias
+        series = self.AriasSeries
+        # elements of the time vector which are within the significant duration
+        idx = (series >= 0.05 * Arias) & (series <= 0.95 * Arias)
+        return self.acc[idx], self.vel[idx], self.disp[idx]
+
     def get_ims(self, display_results: bool = False):
         """return various IMs independent of response spectra.
 
         display_results: bool
             If True, display the results.
 
         Returns
@@ -205,113 +249,129 @@
         cav, cad, cai = self.get_cavdi()
         cavstd = self.get_cavstd()
         ip = self.get_ip()
         tsig_5_95, _ = self.get_t_5_95()
         tsig_5_75, _ = self.get_t_5_75()
         t_bd = self.get_brac_td()
         t_ud = self.get_unif_td()
-        output = dict(PGA=pga,
-                      PGV=pgv,
-                      PGD=pgd,
-                      V_A=v_a,
-                      D_V=d_v,
-                      EDA=eda,
-                      Ia=arias,
-                      Ima=arias_corr,
-                      MIV=miv,
-                      Arms=arms,
-                      Vrms=vrms,
-                      Drms=drms,
-                      Pa=pa,
-                      Pv=pv,
-                      Pd=pd,
-                      Ra=ra,
-                      Rv=rv,
-                      Rd=rd,
-                      SED=sed,
-                      If=fi,
-                      Ic=ic,
-                      Icm=icm,
-                      CAV=cav,
-                      CAD=cad,
-                      CAI=cai,
-                      CAVstd=cavstd,
-                      Ip=ip,
-                      Tsig_5_95=tsig_5_95,
-                      Tsig_5_75=tsig_5_75,
-                      Tbd=t_bd,
-                      Tud=t_ud
-                      )
+        output = dict(
+            PGA=pga,
+            PGV=pgv,
+            PGD=pgd,
+            V_A=v_a,
+            D_V=d_v,
+            EDA=eda,
+            Ia=arias,
+            Ima=arias_corr,
+            MIV=miv,
+            Arms=arms,
+            Vrms=vrms,
+            Drms=drms,
+            Pa=pa,
+            Pv=pv,
+            Pd=pd,
+            Ra=ra,
+            Rv=rv,
+            Rd=rd,
+            SED=sed,
+            If=fi,
+            Ic=ic,
+            Icm=icm,
+            CAV=cav,
+            CAD=cad,
+            CAI=cai,
+            CAVstd=cavstd,
+            Ip=ip,
+            Tsig_5_95=tsig_5_95,
+            Tsig_5_75=tsig_5_75,
+            Tbd=t_bd,
+            Tud=t_ud,
+        )
         units, IMnames = _get_ims_unit(self)
         if display_results:
             console = Console()
             table = Table(title="")  # IMs Independent of Spectra
             table.add_column("IM", justify="left", style="bold", no_wrap=True)
             table.add_column("Value", justify="center", style="bold")
             table.add_column("Unit", justify="center", style="bold")
             table.add_column("Name", justify="right", style="bold")
             for key, values in output.items():
                 # c = next(colors)
-                table.add_row(f"[#0099e5]{key}[/]",
-                              f"[#ff4c4c]{values:>.3f}[/]",
-                              f"[#34bf49]{units[key]}[/]",
-                              f"[#0cb9c1]{IMnames[key]}[/]")
+                table.add_row(
+                    f"[#0099e5]{key}[/]",
+                    f"[#ff4c4c]{values:>.3f}[/]",
+                    f"[#34bf49]{units[key]}[/]",
+                    f"[#0cb9c1]{IMnames[key]}[/]",
+                )
             console.print(table)
         return output
 
     def get_pga(self):
-        """return peak ground values of acceleration (PGA).
-        """
+        """return peak ground values of acceleration (PGA)."""
         return np.max(np.abs(self.acc))
 
     def get_pgv(self):
-        """return peak ground values of velocity (PGV).
-        """
+        """return peak ground values of velocity (PGV)."""
         return np.max(np.abs(self.vel))
 
     def get_pgd(self):
-        """return peak ground values of displacement (PGD).
-        """
+        """return peak ground values of displacement (PGD)."""
         return np.max(np.abs(self.disp))
 
     def get_v_a(self):
-        """Peak velocity and acceleration ratio (PGV/PGA).
-        """
+        """Peak velocity and acceleration ratio (PGV/PGA)."""
         v_a = self.get_pgv() / self.get_pga() / self.vel_factor
         return v_a
 
     def get_d_v(self):
-        """Peak displacement and velocity ratio (PGD/PGV).
-        """
-        d_v = self.get_pgd() / self.disp_factor / (self.get_pgv() / self.vel_factor)
+        """Peak displacement and velocity ratio (PGD/PGV)."""
+        d_v = self.get_pgd() / self.disp_factor / (self.get_pgv() /
+                                                   self.vel_factor)
         return d_v
 
     def get_eda(self, freq=9):
         """EDA，Effective design acceleration,
         defined as the peak acceleration value found after lowpass filtering the input time history
         with a cut-off frequency of 9 Hz [Benjamin and Associates, 1988].
 
         Parameters
         -----------
         freq: float, default=9HZ
             Frequency threshold.
         """
-        acc_filter = freq_filt(self.dt, self.acc,
-                               ftype='Butterworth', btype='lowpass',
-                               order=5, freq1=freq)
+        acc_filter = freq_filt(self.dt,
+                               self.acc,
+                               ftype="Butterworth",
+                               btype="lowpass",
+                               order=5,
+                               freq1=freq)
         eda = np.max(np.abs(acc_filter))
         return eda
 
     def get_ia(self):
-        """return Arias intensity Ia.
+        """return Arias intensity IA.
+        The Arias intensity (IA) is a measure of the strength of a ground motion.
+        It determines the intensity of shaking by measuring the acceleration of transient seismic waves.
+        It has been found to be a fairly reliable parameter to describe earthquake shaking necessary
+        to trigger landslides. It was proposed by Chilean engineer Arturo Arias in 1970.
+
+        It is defined as the time-integral of the square of the ground acceleration:
+
+        .. math::
+
+            I_{A}={\frac{\\pi}{2g}}\\int_{0}^{T_{d}}a(t)^{2}dt} (m/s)
+
+        where g is the acceleration due to gravity and Td is the duration of signal above threshold.
+        The Arias Intensity could also alternatively be defined as the sum of all the squared acceleration
+        values from seismic strong motion records.
         """
         # time history of Arias Intensity
-        acc = self.acc * self.unit_factors[f'{self.acc_unit}-m']
+        acc = self.acc * self.unit_factors[f"{self.acc_unit}-m"]
         series = np.pi / 2 / 9.81 * cumulative_trapezoid(
-            acc ** 2, self.time, initial=0)
+            acc**2, self.time, initial=0)
         # Total Arias Intensity at the end of the ground motion
         arias = series[-1]
         # time history of the normalized Arias Intensity
         arias_percent = series / arias
         # ----------------------------------------------------
         self.Arias = arias
         self.AriasSeries = series
@@ -334,31 +394,33 @@
         above = accsig >= y0
         kth1 = below[0:-1] & above[1:]
         kth2 = above[0:-1] & below[1:]
         kp1 = np.array([*kth1, False])
         kp11 = np.array([False, *kth1])
         kp2 = np.array([False, *kth2])
         kp22 = np.array([*kth2, False])
-        timed01 = np.abs(y0 - accsig[kp1]) * np.abs(timed[kp11] - timed[kp1]) / np.abs(
-            accsig[kp11] - accsig[kp1]) + timed[kp1]
-        timed02 = np.abs(y0 - accsig[kp22]) * np.abs(timed[kp2] - timed[kp22]) / np.abs(
-            accsig[kp2] - accsig[kp22]) + timed[kp22]
+        timed01 = (
+            np.abs(y0 - accsig[kp1]) * np.abs(timed[kp11] - timed[kp1]) /
+            np.abs(accsig[kp11] - accsig[kp1]) + timed[kp1])
+        timed02 = (
+            np.abs(y0 - accsig[kp22]) * np.abs(timed[kp2] - timed[kp22]) /
+            np.abs(accsig[kp2] - accsig[kp22]) + timed[kp22])
         timed0 = np.hstack((timed01, timed02))
         timed0 = np.sort(timed0)
         nzero = len(timed0) / (timed[-1] - timed[0] + self.dt)
-        arias_m = self.Arias / nzero ** 2
+        arias_m = self.Arias / nzero**2
         return arias_m
 
     @staticmethod
     def __iv_aid(time1, time2, acc):
         iv = np.zeros(len(time1) - 1)
         for i in range(len(time1) - 1):
-            idxzero1 = np.argwhere(np.abs(time2 - time1[i]) <= 1E-8)
-            idxzero2 = np.argwhere(
-                np.abs(time2 - time1[i + 1]) <= 1E-8)  # locate zero point
+            idxzero1 = np.argwhere(np.abs(time2 - time1[i]) <= 1e-8)
+            # locate zero point
+            idxzero2 = np.argwhere(np.abs(time2 - time1[i + 1]) <= 1e-8)
             idxzero1 = idxzero1[0, 0]
             idxzero2 = idxzero2[0, 0]
             iv[i] = np.trapz(acc[idxzero1:idxzero2 + 1],
                              time2[idxzero1:idxzero2 + 1])
         return iv
 
     def get_miv(self):
@@ -377,130 +439,128 @@
         above = accsigDura >= y0
         kth1 = below[0:-1] & above[1:]
         kth2 = above[0:-1] & below[1:]
         kp1 = np.array([*kth1, False])
         kp11 = np.array([False, *kth1])
         kp2 = np.array([False, *kth2])
         kp22 = np.array([*kth2, False])
-        timed01 = np.abs(y0 - accsigDura[kp1]) * np.abs(timed[kp11] - timed[kp1]) / np.abs(
-            accsigDura[kp11] - accsigDura[kp1]) + timed[kp1]
-        timed02 = np.abs(y0 - accsigDura[kp22]) * np.abs(timed[kp2] - timed[kp22]) / np.abs(
-            accsigDura[kp2] - accsigDura[kp22]) + timed[kp22]
+        timed01 = (
+            np.abs(y0 - accsigDura[kp1]) * np.abs(timed[kp11] - timed[kp1]) /
+            np.abs(accsigDura[kp11] - accsigDura[kp1]) + timed[kp1])
+        timed02 = (
+            np.abs(y0 - accsigDura[kp22]) * np.abs(timed[kp2] - timed[kp22]) /
+            np.abs(accsigDura[kp2] - accsigDura[kp22]) + timed[kp22])
         timed0 = np.hstack((timed01, timed02))
         timed0 = np.sort(timed0)
         Y0 = np.zeros(len(timed0)) + y0
         accdnew0 = np.array([*accsigDura, *Y0])
         timedNew1 = np.array([*timed, *timed0])
         idxMIV = np.argsort(timedNew1)
         timedNew = timedNew1[idxMIV]
         accdnew = accdnew0[idxMIV]
         IV = self.__iv_aid(timed0, timedNew, accdnew)
         miv = np.max(np.abs(IV))
         return miv * self.vel_factor
 
     def get_sed(self):
-        """Specific Energy Density (SED).
-        """
-        sed = trapz(self.vel ** 2, self.time)
+        """Specific Energy Density (SED)."""
+        sed = trapz(self.vel**2, self.time)
         return sed
 
     def get_rms(self):
-        """Root-mean-square (RMS) of acceleration, velocity and displacement.
-        """
-        Arms = np.sqrt(trapz(self.acc ** 2, self.time) / self.time[-1])
-        Vrms = np.sqrt(trapz(self.vel ** 2, self.time) / self.time[-1])
-        Drms = np.sqrt(trapz(self.disp ** 2, self.time) / self.time[-1])
+        """Root-mean-square (RMS) of acceleration, velocity and displacement."""
+        Arms = np.sqrt(trapz(self.acc**2, self.time) / self.time[-1])
+        Vrms = np.sqrt(trapz(self.vel**2, self.time) / self.time[-1])
+        Drms = np.sqrt(trapz(self.disp**2, self.time) / self.time[-1])
         return Arms, Vrms, Drms
 
     def get_pavd(self):
         """Housner earthquake power index, Pa, Pv, Pd"""
         if self.Arias is None:
             _ = self.get_ia()
         Arias = self.Arias
         series = self.AriasSeries
         idx_5_95 = (series >= 0.05 * Arias) & (series <= 0.95 * Arias)
         timed = self.time[idx_5_95]
         accsigDura = self.acc[idx_5_95]
-        Pa = trapz(accsigDura ** 2, timed) / (timed[-1] - timed[0])
-        Pv = trapz(self.vel[idx_5_95] ** 2, timed) / (timed[-1] - timed[0])
-        Pd = trapz(self.disp[idx_5_95] ** 2, timed) / (timed[-1] - timed[0])
+        Pa = trapz(accsigDura**2, timed) / (timed[-1] - timed[0])
+        Pv = trapz(self.vel[idx_5_95]**2, timed) / (timed[-1] - timed[0])
+        Pd = trapz(self.disp[idx_5_95]**2, timed) / (timed[-1] - timed[0])
         return Pa, Pv, Pd
 
     def get_ravd(self):
         """Riddell index，Ra, Rv, Rd"""
         Td_5_95, _ = self.get_t_5_95()
         PGA = self.get_pga()
         PGV = self.get_pgv()
         PGD = self.get_pgd()
-        Ra = PGA * Td_5_95 ** (1 / 3)
-        Rv = PGV ** (2 / 3) * Td_5_95 ** (1 / 3)
-        Rd = PGD * Td_5_95 ** (1 / 3)
+        Ra = PGA * Td_5_95**(1 / 3)
+        Rv = PGV**(2 / 3) * Td_5_95**(1 / 3)
+        Rd = PGD * Td_5_95**(1 / 3)
         return Ra, Rv, Rd
 
     def get_if(self):
         """Fajfar index."""
         Td_5_95, _ = self.get_t_5_95()
         PGV = self.get_pgv()
-        If = PGV * Td_5_95 ** 0.25
+        If = PGV * Td_5_95**0.25
         return If
 
     def get_ic(self):
-        """Characteristic Intensity (Ic).
-        """
+        """Characteristic Intensity (Ic)."""
         Arms = self.get_rms()[0]
-        Ic = Arms ** 1.5 * np.sqrt(self.time[-1])
+        Ic = Arms**1.5 * np.sqrt(self.time[-1])
         return Ic
 
     def get_icm(self):
-        """Cosenza–Manfredi Intensity.
-        """
+        """Cosenza–Manfredi Intensity."""
         if self.Arias is None:
             _ = self.get_ia()
-        PGA = self.get_pga() * self.unit_factors[f'{self.acc_unit}-m']
-        PGV = self.get_pgv() * self.unit_factors[f'{self.vel_unit}-m']
+        PGA = self.get_pga() * self.unit_factors[f"{self.acc_unit}-m"]
+        PGV = self.get_pgv() * self.unit_factors[f"{self.vel_unit}-m"]
         Icm = 2 * 9.81 * self.Arias / (np.pi * PGA * PGV)
         return Icm
 
     def get_cavdi(self):
-        """Cumulative Absolute Velocity (CAV) ，Displacement (CAD) and Impetus(CAI).
-        """
+        """Cumulative Absolute Velocity (CAV) ，Displacement (CAD) and Impetus(CAI)."""
         CAV = trapz(np.abs(self.acc), self.time)
         CAD = trapz(np.abs(self.vel), self.time)
         CAI = trapz(np.abs(self.disp), self.time)
         return CAV * self.vel_factor, CAD, CAI
 
     def get_cavstd(self):
-        """Standardized Cumulative Absolute Velocity (CAVSTD) [Campbell and Bozorgnia 2011].
-        """
+        """Standardized Cumulative Absolute Velocity (CAVSTD) [Campbell and Bozorgnia 2011]."""
         ts = np.arange(np.floor(self.time[-1]) + 1)
-        acc = self.acc / self.unit_factors[f'g-{self.acc_unit}']
+        acc = self.acc / self.unit_factors[f"g-{self.acc_unit}"]
         idxs = []
         for t in ts:
             idx = np.argmin(np.abs(self.time - t))
             idxs.append(idx)
         idxs.append(len(self.time) - 1)
         cavs = []
         for i in range(len(idxs) - 1):
-            p = trapz(np.abs(acc[idxs[i]:idxs[i + 1] + 1]),
-                      self.time[idxs[i]:idxs[i + 1] + 1])
+            p = trapz(
+                np.abs(acc[idxs[i]:idxs[i + 1] + 1]),
+                self.time[idxs[i]:idxs[i + 1] + 1],
+            )
             pgai = np.max(np.abs(acc[idxs[i]:idxs[i + 1] + 1]))
             a = 0 if pgai - 0.025 < 0 else 1
             cavs.append(a * p)
         cavstd = np.sum(cavs)
         return cavstd
 
     def get_ip(self):
         """Impulsivity Index (IP) [Panella et al., 2017].
         An indicator of the impulsive character of the ground motion and is calculated as
         the developed length of velocity of the velocity time-series divided by the Peak Ground Velocity.
         """
         PGV = self.get_pgv()
         vel1 = self.vel[0:-1]
         vel2 = self.vel[1:]
-        Ldv = np.sum(np.sqrt((vel2 - vel1) ** 2 + self.dt ** 2))
+        Ldv = np.sum(np.sqrt((vel2 - vel1)**2 + self.dt**2))
         Ip = Ldv / PGV
         return Ip
 
     def get_t_5_95(self):
         if self.Arias is None:
             _ = self.get_ia()
         Arias = self.Arias
@@ -546,30 +606,34 @@
         above = acc > y0
         kth1 = below[0:-1] & above[1:]
         kth2 = above[0:-1] & below[1:]
         kp1 = np.array([*kth1, False])
         kp11 = np.array([False, *kth1])
         kp2 = np.array([False, *kth2])
         kp22 = np.array([*kth2, False])
-        timed01 = np.abs(y0 - acc[kp1]) * np.abs(self.time[kp11] - self.time[kp1]) / np.abs(
-            acc[kp11] - acc[kp1]) + self.time[kp1]
-        timed02 = np.abs(y0 - acc[kp22]) * np.abs(self.time[kp2] - self.time[kp22]) / np.abs(
-            acc[kp2] - acc[kp22]) + self.time[kp22]
+        timed01 = (
+            np.abs(y0 - acc[kp1]) * np.abs(self.time[kp11] - self.time[kp1]) /
+            np.abs(acc[kp11] - acc[kp1]) + self.time[kp1])
+        timed02 = (
+            np.abs(y0 - acc[kp22]) * np.abs(self.time[kp2] - self.time[kp22]) /
+            np.abs(acc[kp2] - acc[kp22]) + self.time[kp22])
         T_ud = np.sum(timed02 - timed01)
         return T_ud
 
     # -----------------------------------------------------
     # ---- response spectrum and IMs ----------------------
     # -----------------------------------------------------
-    def get_elas_spec(self,
-                      Ts: Union[float, list],
-                      damp_ratio: float = 0.05,
-                      method: str = "nigam_jennings",
-                      n_jobs: int = 0,
-                      plot: bool = False):
+    def get_elas_spec(
+        self,
+        Ts: Union[float, list, np.ndarray],
+        damp_ratio: float = 0.05,
+        method: str = "nigam_jennings",
+        n_jobs: int = 0,
+        plot: bool = False,
+    ):
         """Computing the Elastic Response Spectrum.
 
         Parameters
         ----------
         Ts : Union[float, ArrayLike]
             Eigenperiods for which the response spectra are requested.
         damp_ratio : float, optional
@@ -594,49 +658,60 @@
         Returns
         -------
         output: (len(Ts), 5) ArrayLike.
             Each column is the *pseudo-acceleration spectrum*, *pseudo-velocity spectrum*,
             *acceleration spectrum*, *velocity spectrum* and *displacement spectrum* in turn.
         """
         Ts = np.atleast_1d(Ts)
-        output = elas_resp_spec(self.dt, self.acc, Ts,
-                                damp_ratio=damp_ratio, method=method, n_jobs=n_jobs)
-        output *= np.array([1, self.vel_factor, 1,
-                            self.vel_factor, self.disp_factor])
-
+        output = elas_resp_spec(self.dt,
+                                self.acc,
+                                Ts,
+                                damp_ratio=damp_ratio,
+                                method=method,
+                                n_jobs=n_jobs)
+        output *= np.array(
+            [1, self.vel_factor, 1, self.vel_factor, self.disp_factor]
+        )
         if plot:
-            acc_unit_end = '' if self.acc_unit == 'g' else "/$s^2$"
-            vel_unit_end = '/s'
-            ylabels = [f'PSa ({self.acc_unit}{acc_unit_end})',
-                       f'PSv ({self.vel_unit}{vel_unit_end})',
-                       f'Sa ({self.acc_unit}{acc_unit_end})',
-                       f'Sv ({self.vel_unit}{vel_unit_end})',
-                       f'Sd ({self.disp_unit})']
-            fig, axs = plt.subplots(5, 1, figsize=(9, 15), sharex='all')
+            acc_unit_end = "" if self.acc_unit == "g" else "/$s^2$"
+            vel_unit_end = "/s"
+            ylabels = [
+                f"PSa ({self.acc_unit}{acc_unit_end})",
+                f"PSv ({self.vel_unit}{vel_unit_end})",
+                f"Sa ({self.acc_unit}{acc_unit_end})",
+                f"Sv ({self.vel_unit}{vel_unit_end})",
+                f"Sd ({self.disp_unit})",
+            ]
+            fig, axs = plt.subplots(5, 1, figsize=(9, 15), sharex="all")
             for i in range(5):
                 ax = axs[i]
                 ax.plot(Ts, output[:, i], lw=1.5, c=self.colors[i])
                 ax.set_xlim(0, np.max(Ts))
                 ax.grid(False)
                 ax.set_ylabel(ylabels[i], fontsize=15)
                 ax.tick_params(labelsize=12)
             axs[-1].set_xlabel("Ts (s)", fontsize=15)
             plt.show()
-        return output
+        if len(output) == 1:
+            return output[0]
+        else:
+            return output
 
-    def get_const_duct_spec(self,
-                            Ts: list,
-                            harden_ratio: float = 0.02,
-                            damp_ratio: float = 0.05,
-                            analy_dt: float = None,
-                            mu: float = 5,
-                            niter: int = 100,
-                            tol: float = 0.01,
-                            n_jobs: int = 0,
-                            plot: int = False):
+    def get_const_duct_spec(
+        self,
+        Ts: Union[float, list, np.ndarray],
+        harden_ratio: float = 0.02,
+        damp_ratio: float = 0.05,
+        analy_dt: float = None,
+        mu: float = 5,
+        niter: int = 100,
+        tol: float = 0.01,
+        n_jobs: int = 0,
+        plot: int = False,
+    ) -> np.ndarray:
         """Constant-ductility inelastic spectra.
         See
 
         * section 7.5 in Anil K. Chopra (DYNAMICS OF STRUCTURES, Fifth Edition, 2020) and
         * the notes "Inelastic Response Spectra" (CEE 541. Structural Dynamics) by Henri P. Gavin.
         * Papazafeiropoulos, George, and Vagelis Plevris."OpenSeismoMatlab: A new open-source software for strong
           ground motion data processing."Heliyon 4.9 (2018): e00784.
@@ -667,39 +742,53 @@
 
         Returns
         -------
         Size (len(Ts), 6) numpy array
             Each column corresponds to acceleration Sa, velocity Sv, displacement Sd spectra,
             yield displacement Dy, strength reduction factor Ry, and yield strength factor Cy (1/Ry).
         """
-        output = const_duct_spec(self.dt, self.acc, Ts, harden_ratio, damp_ratio,
-                                 analy_dt, mu, niter, tol, n_jobs)
-        output *= np.array([1, self.vel_factor, self.disp_factor,
-                            self.disp_factor, 1, 1])
+        output = const_duct_spec(
+            self.dt,
+            self.acc,
+            Ts,
+            harden_ratio,
+            damp_ratio,
+            analy_dt,
+            mu,
+            niter,
+            tol,
+            n_jobs,
+        )
+        output *= np.array(
+            [1, self.vel_factor, self.disp_factor, self.disp_factor, 1, 1])
         if plot:
-            acc_unit_end = '' if self.acc_unit == 'g' else "/$s^2$"
-            vel_unit_end = '/s'
-            ylabels = [f'Sa ({self.acc_unit}{acc_unit_end})',
-                       f'Sv ({self.vel_unit}{vel_unit_end})',
-                       f'Sd ({self.disp_unit})',
-                       f'yield displacement\nDy ({self.disp_unit})',
-                       'strength reduction factor\nRy',
-                       'yield strength factor\nCy (1/Ry)',
-                       ]
-            fig, axs = plt.subplots(6, 1, figsize=(9, 18), sharex='all')
+            acc_unit_end = "" if self.acc_unit == "g" else "/$s^2$"
+            vel_unit_end = "/s"
+            ylabels = [
+                f"Sa ({self.acc_unit}{acc_unit_end})",
+                f"Sv ({self.vel_unit}{vel_unit_end})",
+                f"Sd ({self.disp_unit})",
+                f"yield displacement\nDy ({self.disp_unit})",
+                "strength reduction factor\nRy",
+                "yield strength factor\nCy (1/Ry)",
+            ]
+            fig, axs = plt.subplots(6, 1, figsize=(9, 18), sharex="all")
             for i in range(6):
                 ax = axs[i]
                 ax.plot(Ts, output[:, i], lw=1.5, c=self.colors[i])
                 ax.set_xlim(0, np.max(Ts))
                 ax.grid(False)
                 ax.set_ylabel(ylabels[i], fontsize=15)
                 ax.tick_params(labelsize=12)
             axs[-1].set_xlabel("Ts (s)", fontsize=15)
             plt.show()
-        return output
+        if len(output) == 1:
+            return output[0]
+        else:
+            return output
 
     def get_fou_pow_spec(self, plot: bool = False):
         """The Fourier Amplitude Spectrum and the Power Spectrum (or Power Spectral Density Function)
         are computed by means of Fast Fourier Transformation (FFT) of the input time-history.
         The Fourier amplitude spectrum shows how the amplitude of the ground motion is distributed
         with respect to frequency (or period), effectively meaning that the frequency content of
         the given accelerogram can be fully determined. The power spectral density function,
@@ -727,20 +816,21 @@
         phase: 1D ArrayLike
             Fourier Phase.
         pow_amp: 1D ArrayLike
             Power Spectral Amplitude.
         """
         return fou_pow_spec(self.time, self.acc, plot=plot)
 
-    def get_sac(self,
-                T1: Union[float, list],
-                damp_ratio: float = 0.05,
-                alpha: float = 0.5,
-                beta: float = 0.5
-                ):
+    def get_sac(
+        self,
+        T1: Union[float, list, np.ndarray],
+        damp_ratio: float = 0.05,
+        alpha: float = 0.5,
+        beta: float = 0.5,
+    ):
         """Cordova Intensity.
 
         Parameters
         ----------
         T1 : Union[float, ArrayLike]
             The 1st order natural period of the structure.
         damp_ratio : float, optional
@@ -758,28 +848,29 @@
         if alpha + beta != 1.0:
             raise ValueError("alpha + beta must be 1 !")
         T1 = np.atleast_1d(T1)
         output1 = self.get_elas_spec(T1, damp_ratio)
         output2 = self.get_elas_spec(T1 * 2, damp_ratio)
         sa1 = output1[:, 2]
         sa2 = output2[:, 2]
-        sac = sa1 ** alpha * sa2 ** beta
+        sac = sa1**alpha * sa2**beta
         if len(sac) == 1:
             sac = sac[0]
         return sac
 
-    def get_savam(self,
-                  T1: Union[float, list],
-                  T2: Union[float, list],
-                  T3: Union[float, list] = None,
-                  damp_ratio: float = 0.05,
-                  alpha: float = 1 / 3,
-                  beta: float = 1 / 3,
-                  gamma: float = 1 / 3
-                  ):
+    def get_savam(
+        self,
+        T1: Union[float, list, np.ndarray],
+        T2: Union[float, list, np.ndarray],
+        T3: Union[float, list, np.ndarray] = None,
+        damp_ratio: float = 0.05,
+        alpha: float = 1 / 3,
+        beta: float = 1 / 3,
+        gamma: float = 1 / 3,
+    ):
         """Vamvatsikos Intensity.
 
         Parameters
         ----------
         T1 : Union[float, ArrayLike]
             The 1st order natural period of the structure.
         T2 : Union[float, ArrayLike]
@@ -808,25 +899,27 @@
             raise ValueError("length of T1 and T2 must same!")
         if T3 is None:
             T3 = 2 * T1
         output1 = self.get_elas_spec(T1, damp_ratio)
         output2 = self.get_elas_spec(T2, damp_ratio)
         output3 = self.get_elas_spec(T3, damp_ratio)
         sa1, sa2, sa3 = output1[:, 2], output2[:, 2], output3[:, 2]
-        sa_vam = sa1 ** alpha * sa2 ** beta * sa3 ** gamma
+        sa_vam = sa1**alpha * sa2**beta * sa3**gamma
         if len(sa_vam) == 1:
             sa_vam = sa_vam[0]
         return sa_vam
 
-    def get_samp(self,
-                 T1: Union[float, list],
-                 T2: Union[float, list],
-                 m1: Union[float, list],
-                 m2: Union[float, list],
-                 damp_ratio: float = 0.05):
+    def get_samp(
+        self,
+        T1: Union[float, list, np.ndarray],
+        T2: Union[float, list, np.ndarray],
+        m1: Union[float, list, np.ndarray],
+        m2: Union[float, list, np.ndarray],
+        damp_ratio: float = 0.05,
+    ):
         """Multiple-Period Intensities.
 
         Parameters
         -----------
         T1 : Union[float, ArrayLike]
             The 1st order natural period of the structure.
         T2 : Union[float, ArrayLike]
@@ -842,21 +935,21 @@
         -------
         Sa_mp: Union[float, ArrayLike]
             Multiple-Period Intensity.
         """
         output1 = self.get_elas_spec(T1, damp_ratio)
         output2 = self.get_elas_spec(T2, damp_ratio)
         sa1, sa2 = output1[:, 2], output2[:, 2]
-        sa_mp = sa1 ** (m1 / (m1 + m2)) * sa2 ** (m2 / (m1 + m2))
+        sa_mp = sa1**(m1 / (m1 + m2)) * sa2**(m2 / (m1 + m2))
         if len(sa_mp) == 1:
             sa_mp = sa_mp[0]
         return sa_mp
 
     def get_avgsavd(self,
-                    Tavg: list,
+                    Tavg: Union[list, tuple, np.ndarray],
                     damp_ratio: float = 0.05,
                     n_jobs: int = 0):
         """Average Spectral Acceleration, Velocity and Displacement.
         They are computed as the geometric mean.
 
         Parameters
         ----------
@@ -886,16 +979,15 @@
         """Response spectrum calculation for calculating spectral intensity."""
         self.Tsp = np.arange(0.0, 4.02, 0.02)
         self.Tsp[0] = 0.001
         output = self.get_elas_spec(self.Tsp, damp_ratio, n_jobs=0)
         self.Spec_sp = output
         return output
 
-    def get_savdp(self,
-                  damp_ratio: float = 0.05):
+    def get_savdp(self, damp_ratio: float = 0.05):
         """The peak of the response spectra.
 
         Parameters
         ----------
         damp_ratio : float, optional
             Damping ratio, by default 0.05.
 
@@ -907,16 +999,15 @@
         if self.Tsp is None:
             output = self._spectrum_prefit(damp_ratio)
         else:
             output = self.Spec_sp
         Savd_p = np.max(np.abs(output[:, 2:]), axis=0)
         return Savd_p
 
-    def get_avdsi(self,
-                  damp_ratio: float = 0.05):
+    def get_avdsi(self, damp_ratio: float = 0.05):
         """Acceleration (ASI)，Velocity (VSI) and Displacement(DSI) Spectrum Intensity.
 
         Parameters
         ----------
         damp_ratio : float, optional
             Damping ratio, by default 0.05.
 
@@ -925,26 +1016,25 @@
         AVD_SI: 1D ArrayLike
             Each element is in the order of acceleration, velocity and displacement.
         """
         if self.Tsp is None:
             output = self._spectrum_prefit(damp_ratio)
         else:
             output = self.Spec_sp
-        SIidx1 = np.argwhere(np.abs(self.Tsp - 0.1) <= 1E-8).item()
-        SIidx2 = np.argwhere(np.abs(self.Tsp - 0.5) <= 1E-8).item()
-        SIidx3 = np.argwhere(np.abs(self.Tsp - 2.5) <= 1E-8).item()
-        SIidx4 = np.argwhere(np.abs(self.Tsp - 4.0) <= 1E-8).item()
+        SIidx1 = np.argwhere(np.abs(self.Tsp - 0.1) <= 1e-8).item()
+        SIidx2 = np.argwhere(np.abs(self.Tsp - 0.5) <= 1e-8).item()
+        SIidx3 = np.argwhere(np.abs(self.Tsp - 2.5) <= 1e-8).item()
+        SIidx4 = np.argwhere(np.abs(self.Tsp - 4.0) <= 1e-8).item()
         Sasp, Svsp, Sdsp = output[:, 2], output[:, 3], output[:, 4]
         ASI = trapz(Sasp[SIidx1:SIidx2], self.Tsp[SIidx1:SIidx2])
         VSI = trapz(Svsp[SIidx1:SIidx3], self.Tsp[SIidx1:SIidx3])
         DSI = trapz(Sdsp[SIidx3:SIidx4], self.Tsp[SIidx3:SIidx4])
         return np.array([ASI, VSI, DSI])
 
-    def get_hsi(self,
-                damp_ratio: float = 0.05):
+    def get_hsi(self, damp_ratio: float = 0.05):
         """Housner Spectra Intensity (HSI).
 
         Parameters
         ----------
         damp_ratio : float, optional
             Damping ratio, by default 0.05.
 
@@ -954,16 +1044,16 @@
             Housner Spectra Intensity (HSI)
         """
         if self.Tsp is None:
             output = self._spectrum_prefit(damp_ratio)
         else:
             output = self.Spec_sp
         PSv = output[:, 1]
-        HSIidxLow = np.argwhere(np.abs(self.Tsp - 0.1) <= 1E-8).item()
-        HSIidxTop = np.argwhere(np.abs(self.Tsp - 2.5) <= 1E-8).item()
+        HSIidxLow = np.argwhere(np.abs(self.Tsp - 0.1) <= 1e-8).item()
+        HSIidxTop = np.argwhere(np.abs(self.Tsp - 2.5) <= 1e-8).item()
         hsi = 1 / 2.4 * trapz(PSv[HSIidxLow:HSIidxTop],
                               self.Tsp[HSIidxLow:HSIidxTop])
         return hsi
 
     def get_epavd(self, damp_ratio: float = 0.05):
         """Effective peak acceleration (EPA), velocity (EPV) and displacement (EPD).
 
@@ -978,69 +1068,95 @@
             Each element is in the order of acceleration, velocity and displacement.
         """
         if self.Tsp is None:
             output = self._spectrum_prefit(damp_ratio)
         else:
             output = self.Spec_sp
         Tsp = self.Tsp
-        EPidx1 = np.argwhere(np.abs(Tsp - 0.1) <= 1E-8).item()
-        EPidx2 = np.argwhere(np.abs(Tsp - 0.5) <= 1E-8).item()
-        EPidx3 = np.argwhere(np.abs(Tsp - 0.8) <= 1E-8).item()
-        EPidx4 = np.argwhere(np.abs(Tsp - 2.0) <= 1E-8).item()
-        EPidx5 = np.argwhere(np.abs(Tsp - 2.5) <= 1E-8).item()
-        EPidx6 = np.argwhere(np.abs(Tsp - 4.0) <= 1E-8).item()
+        EPidx1 = np.argwhere(np.abs(Tsp - 0.1) <= 1e-8).item()
+        EPidx2 = np.argwhere(np.abs(Tsp - 0.5) <= 1e-8).item()
+        EPidx3 = np.argwhere(np.abs(Tsp - 0.8) <= 1e-8).item()
+        EPidx4 = np.argwhere(np.abs(Tsp - 2.0) <= 1e-8).item()
+        EPidx5 = np.argwhere(np.abs(Tsp - 2.5) <= 1e-8).item()
+        EPidx6 = np.argwhere(np.abs(Tsp - 4.0) <= 1e-8).item()
         Sa, Sv, Sd = output[:, 2], output[:, 3], output[:, 4]
         EPA = np.sum(Sa[EPidx1:EPidx2]) / (EPidx2 - EPidx1 + 1) / 2.5
         EPV = np.sum(Sv[EPidx3:EPidx4]) / (EPidx4 - EPidx3 + 1) / 2.5
         EPD = np.sum(Sd[EPidx5:EPidx6]) / (EPidx6 - EPidx5 + 1) / 2.5
         return np.array([EPA, EPV, EPD])
 
 
 def _get_ims_unit(self):
-    acc_end = '' if self.acc_unit == 'g' else "/s2"
-    units = dict(PGA=f"{self.acc_unit}{acc_end}", PGV=f"{self.vel_unit}/s", PGD=f"{self.disp_unit}",
-                 V_A="s", D_V="s",
-                 EDA=f"{self.acc_unit}{acc_end}",
-                 Ia="m/s", Ima="m/s", MIV=f"{self.vel_unit}/s",
-                 Arms=f"{self.acc_unit}{acc_end}", Vrms=f"{self.vel_unit}/s", Drms=f"{self.disp_unit}",
-                 Pa=f"({self.acc_unit}{acc_end})^2", Pv=f"({self.vel_unit}/s)^2", Pd=f"({self.disp_unit})^2",
-                 Ra=f"{self.acc_unit}{acc_end}*s^(1/3)",
-                 Rv=f"({self.vel_unit}/s)^(2/3)*s^(1/3)",
-                 Rd=f"{self.disp_unit}*s^(1/3)",
-                 SED=f"{self.vel_unit}2/s",
-                 If=f"({self.vel_unit}/s)*s^(1/4)",
-                 Ic=f"({self.acc_unit}{acc_end})^(2/3)*s^(1/2)",
-                 Icm='--', CAV=f"{self.vel_unit}/s", CAD=f"{self.vel_unit}", CAI=f"{self.disp_unit}*s",
-                 CAVstd="g*s", Ip='--', Tsig_5_95='s', Tsig_5_75='s', Tbd='s', Tud='s')
-    name = dict(PGA="Peak ground acceleration", PGV="Peak ground velocity", PGD="Peak ground displacement",
-                V_A="PGV/PGA", D_V="PGD/PGV",
-                EDA="Effective Design Acceleration ",
-                Ia="Arias Intensity", Ima="Modified Arias Intensity", MIV="Maximum Incremental Velocity",
-                Arms="Root-mean-square of acceleration",
-                Vrms="Root-mean-square of velocity",
-                Drms="Root-mean-square of displacement",
-                Pa="Housner earthquake power index of acceleration",
-                Pv="Housner earthquake power index of velocity",
-                Pd="Housner earthquake power index of displacement",
-                Ra="Riddell index of acceleration",
-                Rv="Riddell index of velocity",
-                Rd="Riddell index of displacement",
-                SED="Specific Energy Density",
-                If="Fajfar index",
-                Ic="Characteristic Intensity",
-                Icm='Cosenza–Manfredi Intensity',
-                CAV="Cumulative Absolute Velocity",
-                CAD="Cumulative Absolute Displacement",
-                CAI="Cumulative Absolute Impetus",
-                CAVstd="tandardized Cumulative Absolute Velocity",
-                Ip='Impulsivity Index',
-                Tsig_5_95=r'5%-95% Arias intensity duration',
-                Tsig_5_75=r'5%-75% Arias intensity duration',
-                Tbd='Bracketed duration',
-                Tud='Uniform duration')
+    acc_end = "" if self.acc_unit == "g" else "/s2"
+    units = dict(
+        PGA=f"{self.acc_unit}{acc_end}",
+        PGV=f"{self.vel_unit}/s",
+        PGD=f"{self.disp_unit}",
+        V_A="s",
+        D_V="s",
+        EDA=f"{self.acc_unit}{acc_end}",
+        Ia="m/s",
+        Ima="m/s",
+        MIV=f"{self.vel_unit}/s",
+        Arms=f"{self.acc_unit}{acc_end}",
+        Vrms=f"{self.vel_unit}/s",
+        Drms=f"{self.disp_unit}",
+        Pa=f"({self.acc_unit}{acc_end})^2",
+        Pv=f"({self.vel_unit}/s)^2",
+        Pd=f"({self.disp_unit})^2",
+        Ra=f"{self.acc_unit}{acc_end}*s^(1/3)",
+        Rv=f"({self.vel_unit}/s)^(2/3)*s^(1/3)",
+        Rd=f"{self.disp_unit}*s^(1/3)",
+        SED=f"{self.vel_unit}2/s",
+        If=f"({self.vel_unit}/s)*s^(1/4)",
+        Ic=f"({self.acc_unit}{acc_end})^(2/3)*s^(1/2)",
+        Icm="--",
+        CAV=f"{self.vel_unit}/s",
+        CAD=f"{self.vel_unit}",
+        CAI=f"{self.disp_unit}*s",
+        CAVstd="g*s",
+        Ip="--",
+        Tsig_5_95="s",
+        Tsig_5_75="s",
+        Tbd="s",
+        Tud="s",
+    )
+    name = dict(
+        PGA="Peak ground acceleration",
+        PGV="Peak ground velocity",
+        PGD="Peak ground displacement",
+        V_A="PGV/PGA",
+        D_V="PGD/PGV",
+        EDA="Effective Design Acceleration ",
+        Ia="Arias Intensity",
+        Ima="Modified Arias Intensity",
+        MIV="Maximum Incremental Velocity",
+        Arms="Root-mean-square of acceleration",
+        Vrms="Root-mean-square of velocity",
+        Drms="Root-mean-square of displacement",
+        Pa="Housner earthquake power index of acceleration",
+        Pv="Housner earthquake power index of velocity",
+        Pd="Housner earthquake power index of displacement",
+        Ra="Riddell index of acceleration",
+        Rv="Riddell index of velocity",
+        Rd="Riddell index of displacement",
+        SED="Specific Energy Density",
+        If="Fajfar index",
+        Ic="Characteristic Intensity",
+        Icm="Cosenza–Manfredi Intensity",
+        CAV="Cumulative Absolute Velocity",
+        CAD="Cumulative Absolute Displacement",
+        CAI="Cumulative Absolute Impetus",
+        CAVstd="tandardized Cumulative Absolute Velocity",
+        Ip="Impulsivity Index",
+        Tsig_5_95=r"5%-95% Arias intensity duration",
+        Tsig_5_75=r"5%-75% Arias intensity duration",
+        Tbd="Bracketed duration",
+        Tud="Uniform duration",
+    )
     return units, name
 
 
 # def _plot_comb_spec(Ts, Sa, Sv, Sd):
 #     ticks = []
 #     for i in np.arange(-5, 5.1, 1):
 #         for j in range(1, 10):
```

### Comparing `gmspy-0.0.4/gmspy.egg-info/PKG-INFO` & `gmspy-0.0.5/gmspy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: gmspy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Ground Motions Signal Processing for Python
 Home-page: https://github.com/yexiang1992
 Author: Yexiang Yan
 Author-email: yexiang_yan@outlook.com
 License: GPL Licence
 Keywords: Ground Motions Seismic IMs response spectra
 Platform: any
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8.*
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: joblib
+Requires-Dist: numba
+Requires-Dist: rich
 
 [![PyPI](https://img.shields.io/pypi/v/gmspy)](https://pypi.org/project/gmspy/)
 [![Downloads](https://static.pepy.tech/badge/gmspy)](https://pepy.tech/project/gmspy)
 [![Documentation Status](https://readthedocs.org/projects/gmspy/badge/?version=latest)](https://gmspy.readthedocs.io/en/latest/?badge=latest)
 ![license](https://img.shields.io/github/license/yexiang1992/gmspy)
 [![CodeFactor](https://www.codefactor.io/repository/github/yexiang1992/gmspy/badge)](https://www.codefactor.io/repository/github/yexiang1992/gmspy)
```

### Comparing `gmspy-0.0.4/gmspy.egg-info/SOURCES.txt` & `gmspy-0.0.5/gmspy.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 LICENCE.txt
 MANIFEST.in
 README.md
 setup.py
 gmspy/__about__.py
 gmspy/__init__.py
+gmspy/_artif_gm.py
 gmspy/_baseline_corr.py
 gmspy/_const_duct_spec.py
 gmspy/_elas_resp_spec.py
 gmspy/_fou_pow_spec.py
 gmspy/_freq_filt.py
 gmspy/_lin_dyna_resp.py
 gmspy/_load_gm_examples.py
 gmspy/_load_peer.py
 gmspy/_load_peer_batch.py
 gmspy/_resample.py
 gmspy/seismo.py
-gmspy/test.py
 gmspy.egg-info/PKG-INFO
 gmspy.egg-info/SOURCES.txt
 gmspy.egg-info/dependency_links.txt
 gmspy.egg-info/requires.txt
 gmspy.egg-info/top_level.txt
 gmspy/accelerograms/ChiChi.dat
 gmspy/accelerograms/Friuli.dat
```

