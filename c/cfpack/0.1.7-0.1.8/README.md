# Comparing `tmp/cfpack-0.1.7.tar.gz` & `tmp/cfpack-0.1.8.tar.gz`

## Comparing `cfpack-0.1.7.tar` & `cfpack-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 cfpack-0.1.7/cfpack.browser_control.html
--rw-r--r--   0        0        0    16950 2020-02-02 00:00:00.000000 cfpack-0.1.7/cfpack.html
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.1.7/pyproject.toml.new
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.1.7/pyproject.toml.old
--rw-r--r--   0        0        0    49822 2020-02-02 00:00:00.000000 cfpack-0.1.7/cfpack/__init__.py
--rwxr-xr-x   0        0        0     6551 2020-02-02 00:00:00.000000 cfpack-0.1.7/cfpack/automator.py
--rwxr-xr-x   0        0        0     5236 2020-02-02 00:00:00.000000 cfpack-0.1.7/cfpack/browser_control.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 cfpack-0.1.7/cfpack/constants.py
--rwxr-xr-x   0        0        0     3077 2020-02-02 00:00:00.000000 cfpack-0.1.7/cfpack/hdfio.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 cfpack-0.1.7/cfpack/matplotlibrc.py
--rwxr-xr-x   0        0        0     2772 2020-02-02 00:00:00.000000 cfpack-0.1.7/cfpack/tests.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cfpack-0.1.7/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cfpack-0.1.7/LICENSE
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 cfpack-0.1.7/README.md
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 cfpack-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 cfpack-0.1.8/cfpack.browser_control.html
+-rw-r--r--   0        0        0    16950 2020-02-02 00:00:00.000000 cfpack-0.1.8/cfpack.html
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.1.8/pyproject.toml.new
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.1.8/pyproject.toml.old
+-rw-r--r--   0        0        0    57571 2020-02-02 00:00:00.000000 cfpack-0.1.8/cfpack/__init__.py
+-rwxr-xr-x   0        0        0     6551 2020-02-02 00:00:00.000000 cfpack-0.1.8/cfpack/automator.py
+-rwxr-xr-x   0        0        0     5236 2020-02-02 00:00:00.000000 cfpack-0.1.8/cfpack/browser_control.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 cfpack-0.1.8/cfpack/constants.py
+-rwxr-xr-x   0        0        0     3077 2020-02-02 00:00:00.000000 cfpack-0.1.8/cfpack/hdfio.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 cfpack-0.1.8/cfpack/matplotlibrc.py
+-rwxr-xr-x   0        0        0     2772 2020-02-02 00:00:00.000000 cfpack-0.1.8/cfpack/tests.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cfpack-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cfpack-0.1.8/LICENSE
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 cfpack-0.1.8/README.md
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 cfpack-0.1.8/PKG-INFO
```

### Comparing `cfpack-0.1.7/cfpack.browser_control.html` & `cfpack-0.1.8/cfpack.browser_control.html`

 * *Files identical despite different names*

### Comparing `cfpack-0.1.7/cfpack.html` & `cfpack-0.1.8/cfpack.html`

 * *Files identical despite different names*

### Comparing `cfpack-0.1.7/pyproject.toml.new` & `cfpack-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cfpack"
-version = "0.1.5"
+version = "0.1.8"
 authors = [
   { name="Christoph Federrath", email="christoph.federrath@anu.edu.au" },
 ]
 description = "Christoph Federrath (CF) python package (cfpack)"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3"
```

### Comparing `cfpack-0.1.7/pyproject.toml.old` & `cfpack-0.1.8/pyproject.toml.new`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cfpack"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Christoph Federrath", email="christoph.federrath@anu.edu.au" },
 ]
 description = "Christoph Federrath (CF) python package (cfpack)"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3"
```

### Comparing `cfpack-0.1.7/cfpack/__init__.py` & `cfpack-0.1.8/cfpack/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -135,54 +135,69 @@
                 plt.pause(pause)
         plt.clf(); plt.cla(); plt.close(); plt = None # clear figure after use
     return plt
 # === END plot ===
 
 # === START plot_map ===
 # function to plot a map (of a 2D numpy array)
-def plot_map(image=None, dims=None, vmin=None, vmax=None, log=False, colorbar=True, cmap='magma', cmap_label=None, xlabel=None, ylabel=None,
-             extent=None, dpi=200, show=False, pause=None, xlog=False, ylog=False, xlim=None, ylim=None, save=None, *args, **kwargs):
+def plot_map(image, xedges=None, yedges=None, dims=None, vmin=None, vmax=None, log=False, colorbar=True, cmap='magma', cmap_label=None,
+             xlabel=None, ylabel=None, xlog=False, ylog=False, xlim=None, ylim=None, aspect='auto',
+             dpi=200, show=False, pause=None, save=None, *args, **kwargs):
     import matplotlib.pyplot as plt
     import matplotlib.colors as mpl_colors
-    if image is not None:
-        if dims is not None: image = congrid(image, (dims[0], dims[1])) # re-sample image
-        # define how to normalise colours
-        norm = mpl_colors.Normalize(vmin=vmin, vmax=vmax)
-        if log: norm = mpl_colors.LogNorm(vmin=vmin, vmax=vmax)
-        # plot map
-        plt.imshow(image, cmap=cmap, origin='lower', interpolation='none', norm=norm, extent=extent, *args, **kwargs)
-    if show or save:
-        # add colorbar
-        if colorbar:
-            cb = plt.colorbar(label=cmap_label, pad=0.01, aspect=25)
-            if not log: cb.ax.minorticks_on()
-            cb.ax.yaxis.set_offset_position('left')
-        # plot map
-        ax = plt.gca()
-        ax.set_xlabel(xlabel)
-        ax.set_ylabel(ylabel)
-        if xlim is not None: plt.xlim(xlim)
-        if ylim is not None: plt.ylim(ylim)
-        if xlog: ax.set_xscale('log')
-        if ylog: ax.set_yscale('log')
-        plt.gcf().set_dpi(dpi)
-        plt.tight_layout(pad=0.0)
-        # save
-        if save:
-            plt.savefig(save, bbox_inches='tight')
-            print(save+' written.', color='magenta')
-        # show
-        if show:
-            block = None
-            if pause: block = False
-            plt.show(block=block)
-            if pause:
-                plt.draw()
-                plt.pause(pause)
-        plt.clf(); plt.cla(); plt.close(); plt = None # clear figure after use
+    ax = plt.gca()
+    if dims is not None: image = congrid(image, (dims[0], dims[1])) # re-sample image
+    # define how to normalise colours
+    norm = mpl_colors.Normalize(vmin=vmin, vmax=vmax)
+    if log: norm = mpl_colors.LogNorm(vmin=vmin, vmax=vmax)
+    # define the coordinates of the map
+    shape = np.array(image.shape)
+    xrange = [0.5, shape[0]+0.5]
+    yrange = [0.5, shape[1]+0.5]
+    if xlim is not None:
+        xrange = [xlim[0], xlim[1]]
+    if ylim is not None:
+        yrange = [ylim[0], ylim[1]]
+    plt.xlim(xrange)
+    plt.ylim(yrange)
+    if xlog: ax.set_xscale('log')
+    if ylog: ax.set_yscale('log')
+    ax.set_xlabel(xlabel)
+    ax.set_ylabel(ylabel)
+    if aspect != "auto":
+        ax.set_aspect(aspect)
+    if xedges is not None and yedges is not None:
+        x_edges, y_edges = np.meshgrid(xedges, yedges, indexing='ij')
+    else:
+        x_edges, y_edges = get_2d_coords([xrange[0], yrange[0]], [xrange[1], yrange[1]], shape+1, cell_centred=False)
+        if aspect == "auto" and xlim is None and ylim is None:
+            ax.set_aspect((yrange[1]-yrange[0])/(xrange[1]-xrange[0]))
+    # plot map
+    pc = ax.pcolormesh(x_edges, y_edges, image, cmap=cmap, norm=norm, *args, **kwargs)
+    #pc = plt.imshow(image, cmap=cmap, norm=norm, origin='lower', interpolation='none', extent=[xrange[0], xrange[1], yrange[0], yrange[1]], *args, **kwargs)
+    # add colorbar
+    if colorbar:
+        cb = plt.colorbar(pc, label=cmap_label, pad=0.01, aspect=25)
+        if not log: cb.ax.minorticks_on()
+        cb.ax.yaxis.set_offset_position('left')
+    plt.gcf().set_dpi(dpi)
+    plt.tight_layout(pad=0.0)
+    # save
+    if save:
+        plt.savefig(save, bbox_inches='tight')
+        print(save+' written.', color='magenta')
+    # show
+    if show:
+        block = None
+        if pause: block = False
+        plt.show(block=block)
+        if pause:
+            plt.draw()
+            plt.pause(pause)
+    plt.clf(); plt.cla(); plt.close(); plt = None # clear figure after use
     return plt
 # === END plot_map ===
 
 # === START rgba2data ===
 # Given a RGBA colour image (2D array) plotted with a colourbar 'cmap', and vmin/vmax values on the colourbar.
 # Return the interpolated data values in the RGBA colour image.
 # Adopted from http://stackoverflow.com/questions/3720840/how-to-reverse-color-map-image-to-scalar-values/3722674#3722674
@@ -405,14 +420,37 @@
         # compute time difference in seconds
         self.dt = self.stop_time-self.start_time
     def report(self):
         self.stop()
         if self.dt is None: self.get_dt()
         print("=== timer('"+self.name+"'): start = "+str(self.start_time)+", stop = "+str(self.stop_time)+", runtime = "+str(self.dt), highlight=1, no_prefix=True)
 
+# === class to monitor loop progress ===
+class monitor:
+    from datetime import datetime
+    # ============= __init__ =============
+    def __init__(self, loop_size, signature=""):
+        self.loop_size = loop_size
+        self.signature = signature # label
+        self.report_status = 0.01
+        self.start_time = self.datetime.now()
+    def report(self, loop_index):
+        frac_done = (loop_index+1)/self.loop_size
+        if (frac_done >= 0.01) and (self.report_status==0.01):
+            dt = int((self.datetime.now()-self.start_time).total_seconds()*100)/100
+            print(self.signature+"...  1% done in "+str(dt)+"s...")
+            self.report_status = 0.10
+        if (frac_done >= 0.10) and (self.report_status==0.10):
+            dt = int((self.datetime.now()-self.start_time).total_seconds()*100)/100
+            print(self.signature+"... 10% done in "+str(dt)+"s...")
+            self.report_status = 1.00
+        if (frac_done >= 1.00) and (self.report_status==1.00):
+            dt = int((self.datetime.now()-self.start_time).total_seconds()*100)/100
+            print(self.signature+"...100% done in "+str(dt)+"s...")
+
 # === executes a shell command: input string 'cmd'
 def run_shell_command(cmd, quiet=False, print_only=False, capture=False, **kargs):
     from subprocess import run
     if (not quiet) or print_only:
         if 'color' not in kargs.keys():
             kargs['color'] = 'magenta' # set default colour for shell command print
         print(cmd, **kargs)
@@ -578,77 +616,164 @@
         bin_edges = x_edges
         bin_center = x_mid_points
     return ret
 
 # === bin data with bin_values (same size as data) into bins (number or array of bin edges) ===
 def get_binned_stats(data, bin_values, bins=None, statistic='mean', **kwargs):
     from scipy.stats import binned_statistic
+    if bins is None: bins = 100
     binned_stats = binned_statistic(bin_values.flatten(), data.flatten(), bins=bins, statistic=statistic)
     return binned_stats.statistic, binned_stats.bin_edges
 
-# === get the Fourier (k-space) spectrum of data with ncmp components in axis=0 ===
-# === e.g., for a 64^3 dataset and 3 vector components, data.shape must be (3, 64, 64, 64) ===
-# === e.g., for a 32^2 dataset with only 1 component, data.shape must be (32, 32) ===
-def get_spectrum(data_in, ncmp=1):
-    data = np.copy(data_in) # flatten to strip any possible extra dimensions
+# === bin data with 2 bin_values (each with the same size as data) into 2D bins (number or array of bin edges) ===
+def get_binned_stats_2d(data, bin_values_1, bin_values_2, bins=None, statistic='sum', **kwargs):
+    from scipy.stats import binned_statistic_2d
+    if bins is None: bins = 100
+    binned_stats = binned_statistic_2d(bin_values_1.flatten(), bin_values_2.flatten(), data.flatten(), bins=bins, statistic=statistic)
+    return binned_stats.statistic, binned_stats.x_edge, binned_stats.y_edge
+
+# === Compute the Fourier (k-space) spectrum of 'data_in' with ncmp components in axis=0 ===
+# E.g., for a 64^3 dataset and 3 vector components, data.shape must be (3, 64, 64, 64).
+# E.g., for a 32^2 dataset with only 1 component, data.shape must be (32, 32).
+# Note that if 'data_in' is 2D or 3D, then the indices are in order data_in[x,[y,[z]]].
+# Binning can be 'spherical' (default ->1D) or 'cylindrical' (->2D).
+# If binning='cylindrical' (only for 3D input): r_cyl^2=x^2+y^2 -> k_perp; z_cyl=z -> k_para.
+# If sum=True, then bininng uses 'sum' instead of 'mean' and integral_factor = 1.
+# Results should be similar with either sum=True or sum=False.
+# If return_ft_data=True, it also returns the full Fourier-transformed dataset.
+# Use verbose=0 to switch off any status prints from this function.
+def get_spectrum(data_in, ncmp=1, binning='spherical', sum=False, return_ft_data=False, verbose=1):
+    # check binning type
+    supported_binning = ["spherical", "cylindrical"]
+    if binning not in supported_binning:
+        print("binning='"+binning+"' not supported; binning must be any of ", supported_binning, error=True)
+    # check statistic type
+    if sum:
+        statistic = 'sum'
+        normalise = False
+    else:
+        statistic = 'mean'
+        normalise = True
+    # flatten to strip any possible extra dimensions
+    data = np.copy(data_in)
     if (ncmp == 1) and (data.shape[0] > 1):
         data = np.array([data]) # add an extra (fake) index, so we can index as if there were components
     num = np.array(data[0].shape) # number of points in data
     ndim = len(num) # number of dimensions
-    ks = -num//2 # k start
-    ke = np.array([np.min([-ks[d], num[d]//2-1]) for d in range(ndim)]) # k end
+    if binning == 'cylindrical': # error checking
+        if ndim != 3:
+            print("Parallel-perpendicular binning currently only works for 3D datasets!", error=True)
+        if (num[0] != num[1]) or (num[0] != num[2]):
+            print("Parallel-perpendicular binning currently only works for cubic datasets!", error=True)
+    # print info about real-space field
+    mean_sq = 0.0
+    std_sq = 0.0
+    for d in range(ncmp):
+        mean_sq += data[d].mean()**2
+        std_sq += np.std(data[d])**2
+    if verbose: print("data mean squared = "+eform(mean_sq)+", data std squared = "+eform(std_sq))
+    # construct wave numbers and bins
+    ks = -(num//2) # k start
+    ke = np.array([num[d]//2+(num[2]%2-1) for d in range(ndim)]) # k end
     k = get_coords(ks, ke, num, cell_centred=False) # get k vector with k=0 in the center
+    if binning == 'cylindrical':
+        k_perp = k[0:2] # split the k array into perpendicular and parallel components
+        k_para = k[2] # the z axis is the parallel direction
     if ndim == 1: k_abs = np.abs(k) # length of k vector
     if ndim  > 1: k_abs = np.sqrt((k**2).sum(axis=0)) # length of k vector
-    bins = np.arange(np.max(num)//2) - 0.5 # k bins for 1D spectrum
+    if binning == 'cylindrical': # construct absolute k_perp and k_para for binning below
+        k_abs_perp = np.sqrt((k_perp**2).sum(axis=0))
+        k_abs_para = np.abs(k_para)
+    bins = np.arange(np.max(ke)+2) - 0.5 # k bins for 1D spectrum
+    # do Fourier transformation
     data_ft = []
     for d in range(ncmp):
-        data_ft.append(np.fft.fftn(data[d], norm='forward')) # FFT
-        data_ft[d] = np.fft.fftshift(data_ft[d]) # shift k=0 to center
+        data_ft.append(np.fft.fftn(data[d].T, norm='forward')) # FFT (note that we transpose before FFT, to get data[x,[y,[z]]] -> data[[[z],y],x])
+        data_ft[d] = np.fft.fftshift(data_ft[d]).T # shift k=0 to center and transpose back, so we have data_ft[kx,[ky,[kz]]]
     data_ft = np.array(data_ft)
     # get total power
     power_tot = (np.abs(data_ft)**2).sum(axis=0)
-    # Helmholtz decomposition
+    P0 = power_tot[k_abs==0][0] # extract k=0 value of power spectrum
+    norm = power_tot.sum()-P0 # integral over all k!=0
+    if verbose: print("           P(k=0) = "+eform(P0)+",      total power = "+eform(norm))
+    # bin in k shells
+    if binning == 'spherical':
+        spect_tot, bins = get_binned_stats(power_tot, k_abs, bins=bins, statistic=statistic)
+        bin_centers = bins[:-1]+0.5
+        if statistic == "mean":
+            integral_factor = bin_centers**(ndim-1)
+            if ndim > 1: integral_factor *= np.pi*2*(ndim-1)
+    if binning == 'cylindrical':
+        spect_tot, bins_perp, bins_para = get_binned_stats_2d(power_tot, k_abs_perp, k_abs_para, bins=[bins,bins], statistic=statistic)
+        bin_centers_perp = bins_perp[:-1]+0.5
+        bin_centers_para = bins_para[:-1]+0.5
+        # construct 2D array with k values
+        k2d = get_2d_coords(cmin=[bin_centers_perp[0],bin_centers_para[0]], cmax=[bin_centers_perp[-1],bin_centers_para[-1]], ndim=[len(bin_centers_perp),len(bin_centers_para)], cell_centred=False)
+        bin_centers = np.sqrt((k2d**2).sum(axis=0))
+        if statistic == "mean":
+            integral_factor = 2*2**np.pi*k2d[0] # 2 pi k_perp is the circumference when integrating over phi, and the additional factor 2 is because we fold k_para
+            integral_factor[0,:] = 1.0 # set the entire k_perp = 0 axis to an integral factor of 1, so we don't destroy the power on that axis when multiplying below
+    # integral factor and normalisation if needed
+    if statistic == "sum": integral_factor = np.ones(spect_tot.shape)
+    spect_tot[bin_centers!=0] *= integral_factor[bin_centers!=0] # k=0 stays
+    if normalise: spect_tot[bin_centers!=0] = spect_tot[bin_centers!=0] / spect_tot[bin_centers!=0].sum() * norm # normalise
+    # construct return dict (more added below)
+    if binning == 'spherical':
+        ret = {'k': bin_centers, 'P_tot': spect_tot}
+    if binning == 'cylindrical':
+        # integrate over k_para -> P_perp and integrate over k_perp -> P_para
+        spect_tot[bin_centers==0] = 0.0 # temporarily set P(k=0)=0 for easier summation
+        spect_tot_perp = np.sum(spect_tot, axis=1)
+        spect_tot_para = np.sum(spect_tot, axis=0)
+        spect_tot[bin_centers==0] = P0 # restore P(k=0)
+        ret = {'k': bin_centers, 'P_tot': spect_tot, 'k_perp': bin_centers_perp, 'k_para': bin_centers_para, 'P_tot_perp': spect_tot_perp, 'P_tot_para': spect_tot_para}
+    # # Helmholtz decomposition
     if ncmp > 1: # there is more than 1 component
         power_lgt = np.zeros(num, dtype=complex)
         if ndim == 1: power_lgt += k*data_ft[0] # 1D case: scalar product (k is a 1D array and we only use x-component data for the longitudinal power)
         if ndim >= 2: # 2D and 3D cases: scalar product (get power along k); if ndim < ncmp (i.e., 2.5D), the z-component does not enter the scalar product
-            for d in range(ndim): power_lgt += k[d]*data_ft[d].T # scalar product
+            for d in range(ndim): power_lgt += k[d]*data_ft[d] # scalar product
         power_lgt = np.abs(power_lgt/np.maximum(k_abs,1e-99))**2
         power_trv = power_tot - power_lgt
-        print("tot power = "+str(power_tot.sum()/ncmp))
-        print("lgt power = "+str(power_lgt.sum()/ncmp)+", relative to tot: "+str(power_lgt.sum()/power_tot.sum()))
-        print("trv power = "+str(power_trv.sum()/ncmp)+", relative to tot: "+str(power_trv.sum()/power_tot.sum()))
-    # bin in k shells
-    spect_tot, bins = get_binned_stats(power_tot, k_abs, bins=bins)
-    bin_centers = bins[:-1]+0.5
-    integral_factor = bin_centers**(ndim-1)
-    if ndim > 1: integral_factor *= np.pi*2*(ndim-1)
-    ret = {'k': bin_centers, 'P_tot': spect_tot*integral_factor}
-    if ncmp > 1:
-        spect_lgt, bins = get_binned_stats(power_lgt, k_abs, bins=bins)
-        spect_trv, bins = get_binned_stats(power_trv, k_abs, bins=bins)
-        ret['P_lgt'] = spect_lgt*integral_factor
-        ret['P_trv'] = spect_trv*integral_factor
-    # return dict
-    return ret
+        power_trv[k_abs==0] = 0.0 # remove k=0 mode from decomposed spectra
+        norm_lgt = power_lgt.sum(); norm_trv = power_trv.sum()
+        if verbose:
+            print("longitudinal (lgt) power = "+eform(norm_lgt)+", relative to total: "+str(norm_lgt/norm))
+            print("  transverse (trv) power = "+eform(norm_trv)+", relative to total: "+str(norm_trv/norm))
+        if binning == 'spherical':
+            spect_lgt, bins = get_binned_stats(power_lgt, k_abs, bins=bins, statistic=statistic)
+            spect_trv, bins = get_binned_stats(power_trv, k_abs, bins=bins, statistic=statistic)
+        if binning == 'cylindrical':
+            spect_lgt, bins_perp, bins_para = get_binned_stats_2d(power_lgt, k_abs_perp, k_abs_para, bins=[bins,bins], statistic=statistic)
+            spect_trv, bins_perp, bins_para = get_binned_stats_2d(power_trv, k_abs_perp, k_abs_para, bins=[bins,bins], statistic=statistic)
+        spect_lgt[bin_centers!=0] *= integral_factor[bin_centers!=0] # k=0 stays
+        spect_trv[bin_centers!=0] *= integral_factor[bin_centers!=0] # k=0 stays
+        if normalise: spect_lgt[bin_centers!=0] = spect_lgt[bin_centers!=0] / spect_lgt[bin_centers!=0].sum() * norm_lgt # normalise
+        if normalise: spect_trv[bin_centers!=0] = spect_trv[bin_centers!=0] / spect_trv[bin_centers!=0].sum() * norm_trv # normalise
+        ret['P_lgt'] = spect_lgt
+        ret['P_trv'] = spect_trv
+    if return_ft_data: ret['Power_tot'] = power_tot # if the user wants to have the Fourier-transformed data (power) returned
+    return ret # return dict with power spectrum data
 
+# === return a KDE'd version of 'data' ===
 def get_kde_sample(data, n=1000, seed=1, show=False):
     from scipy.stats import gaussian_kde
     kernel = gaussian_kde(data)
     data_resampled = kernel.resample(size=n, seed=seed)
     if show:
         import matplotlib.pyplot as plt
-        pdf_original, x = get_pdf(data)
-        pdf_resampled, x = get_pdf(data_resampled)
-        plt.plot(x, pdf_original, label='original')
-        plt.plot(x, kernel(x), label='KDE')
-        plt.plot(x, pdf_resampled, label='resampled')
-        plt.legend()
-        plt.show(block=True)
+        pdf_obj = get_pdf(data)
+        pdf_original = pdf_obj.pdf
+        pdf_obj = get_pdf(data_resampled)
+        pdf_resampled = pdf_obj.pdf
+        x = pdf_obj.bin_center
+        plot(x=x, y=pdf_original, label='original')
+        plot(x=x, y=kernel.pdf(x), label='KDE')
+        plot(x=x, y=pdf_resampled, label='resampled')
+        plot(show=True)
     return data_resampled
 
 # === return x rounded to nfigs significant figures ===
 def round(x, nfigs=3, str_ret=False):
     # prepare function for scalar or array input and copy x into ret
     ret = np.array(x)
     scalar_input = False
```

### Comparing `cfpack-0.1.7/cfpack/automator.py` & `cfpack-0.1.8/cfpack/automator.py`

 * *Files identical despite different names*

### Comparing `cfpack-0.1.7/cfpack/browser_control.py` & `cfpack-0.1.8/cfpack/browser_control.py`

 * *Files identical despite different names*

### Comparing `cfpack-0.1.7/cfpack/constants.py` & `cfpack-0.1.8/cfpack/constants.py`

 * *Files identical despite different names*

### Comparing `cfpack-0.1.7/cfpack/hdfio.py` & `cfpack-0.1.8/cfpack/hdfio.py`

 * *Files identical despite different names*

### Comparing `cfpack-0.1.7/cfpack/matplotlibrc.py` & `cfpack-0.1.8/cfpack/matplotlibrc.py`

 * *Files identical despite different names*

### Comparing `cfpack-0.1.7/cfpack/tests.py` & `cfpack-0.1.8/cfpack/tests.py`

 * *Files identical despite different names*

### Comparing `cfpack-0.1.7/LICENSE` & `cfpack-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cfpack-0.1.7/pyproject.toml` & `cfpack-0.1.8/pyproject.toml.old`

 * *Files identical despite different names*

### Comparing `cfpack-0.1.7/PKG-INFO` & `cfpack-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cfpack
-Version: 0.1.7
+Version: 0.1.8
 Summary: Christoph Federrath (CF) python package (cfpack)
 Project-URL: Homepage, https://www.mso.anu.edu.au/~chfeder/codes/cfpack/cfpack.html
 Author-email: Christoph Federrath <christoph.federrath@anu.edu.au>
 License: MIT License
         
         Copyright (c) 2022 Christoph Federrath
```

