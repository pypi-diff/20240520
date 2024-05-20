# Comparing `tmp/msigen-0.1.0.tar.gz` & `tmp/msigen-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msigen-0.1.0.tar", max compression
+gzip compressed data, was "msigen-0.2.1.tar", max compression
```

## Comparing `msigen-0.1.0.tar` & `msigen-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,14 @@
--rw-r--r--   0        0        0     1070 2024-04-01 19:14:32.937425 msigen-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      178 2024-04-01 18:06:19.915046 msigen-0.1.0/MSIGen/__init__.py
--rw-r--r--   0        0        0    52726 2024-04-26 21:44:32.380107 msigen-0.1.0/MSIGen/D.py
--rw-r--r--   0        0        0    46609 2024-04-19 16:40:53.326262 msigen-0.1.0/MSIGen/GUI.py
--rw-r--r--   0        0        0    58172 2024-04-26 20:50:25.997330 msigen-0.1.0/MSIGen/msigen.py
--rw-r--r--   0        0        0    33676 2024-04-01 18:06:16.975885 msigen-0.1.0/MSIGen/mzml.py
--rw-r--r--   0        0        0    19263 2024-04-01 18:03:50.526230 msigen-0.1.0/MSIGen/raw.py
--rw-r--r--   0        0        0 12886552 2022-05-06 20:20:48.683786 msigen-0.1.0/MSIGen/timsdata.dll
--rw-r--r--   0        0        0     9568 2024-04-01 21:37:47.587353 msigen-0.1.0/MSIGen/tsf.py
--rw-r--r--   0        0        0    19069 2024-04-29 17:36:40.182207 msigen-0.1.0/MSIGen/visualization.py
--rw-r--r--   0        0        0     1329 2024-04-30 18:29:15.242296 msigen-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1652 2024-04-30 18:19:26.496352 msigen-0.1.0/README.md
--rw-r--r--   0        0        0     1817 2024-04-30 18:22:06.825507 msigen-0.1.0/tests/make GUI shortcut.py
--rw-r--r--   0        0        0     9634 2024-04-30 18:22:05.989120 msigen-0.1.0/tests/MSIGen_CLI.py
--rw-r--r--   0        0        0     8897 2024-04-30 18:22:03.999970 msigen-0.1.0/tests/MSIGen_jupyter.ipynb
--rw-r--r--   0        0        0     3035 1970-01-01 00:00:00.000000 msigen-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-05-16 19:53:18.606091 msigen-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0      178 2024-05-16 19:53:07.444990 msigen-0.2.1/MSIGen/__init__.py
+-rw-r--r--   0        0        0    52726 2024-05-16 19:53:03.628205 msigen-0.2.1/MSIGen/D.py
+-rw-r--r--   0        0        0    51238 2024-05-16 19:52:31.864409 msigen-0.2.1/MSIGen/GUI.py
+-rw-r--r--   0        0        0    58278 2024-05-16 19:53:10.557672 msigen-0.2.1/MSIGen/msigen.py
+-rw-r--r--   0        0        0    33676 2024-05-16 19:53:09.653091 msigen-0.2.1/MSIGen/mzml.py
+-rw-r--r--   0        0        0    19004 2024-05-16 19:53:08.655754 msigen-0.2.1/MSIGen/raw.py
+-rw-r--r--   0        0        0 12886552 2024-04-30 20:20:11.276935 msigen-0.2.1/MSIGen/timsdata.dll
+-rw-r--r--   0        0        0     9775 2024-05-16 19:53:12.647190 msigen-0.2.1/MSIGen/tsf.py
+-rw-r--r--   0        0        0    21985 2024-05-20 15:10:20.012509 msigen-0.2.1/MSIGen/visualization.py
+-rw-r--r--   0        0        0     1320 2024-05-20 15:23:06.551962 msigen-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2323 2024-05-14 23:34:29.375945 msigen-0.2.1/README.md
+-rw-r--r--   0        0        0     1077 2024-05-16 20:43:03.261270 msigen-0.2.1/tests/example_config_file.json
+-rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 msigen-0.2.1/PKG-INFO
```

### Comparing `msigen-0.1.0/LICENSE.txt` & `msigen-0.2.1/LICENSE.txt`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 EmersonHernly
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 EmersonHernly
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `msigen-0.1.0/MSIGen/D.py` & `msigen-0.2.1/MSIGen/D.py`

 * *Files identical despite different names*

### Comparing `msigen-0.1.0/MSIGen/GUI.py` & `msigen-0.2.1/MSIGen/GUI.py`

 * *Files 5% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         self.rawfile_paths = tk.StringVar(value="")
         self.mass_list_path = tk.StringVar(value="")
         self.output_file_path = tk.StringVar(value="")
         self.img_h = tk.StringVar(value="10")
         self.img_w = tk.StringVar(value="10")
         self.is_MS2_var = tk.IntVar()
         self.is_mob_var = tk.IntVar()
-        self.scale = tk.DoubleVar(value=0.999)
+        self.scale = tk.DoubleVar(value=100)
         self.threshold = tk.DoubleVar(value=0.)
 
         # left frame
         self.rawfiles_frame = tk.Frame(self)
         self.rawfiles_frame.pack(side = tk.LEFT, fill=tk.BOTH, expand=True, padx=10, pady=10)
     
         # selecting raw files
@@ -355,15 +355,15 @@
             try:
                 mass_tolerance_MS1, mass_tolerance_prec, mass_tolerance_frag, mobility_tolerance = [float(i.get()) for i in self.tolerance_value]
             except:
                 error_message = "Tolerance values must be numbers."
                 tk.messagebox.showerror("Argument error", error_message)
                 self.run_workflow_button['state'] = 'normal'
 
-            mass_tolerance_MS1_units, mass_tolerance_prec_units, mass_tolerance_frag_units, mobility_tolerance_units = [i.get() for i in self.tolerance_value]
+            mass_tolerance_MS1_units, mass_tolerance_prec_units, mass_tolerance_frag_units, mobility_tolerance_units = [i.get() for i in self.tolerance_units]
 
             try:
                 img_height, img_width = float(self.img_h.get()), float(self.img_w.get())
                 image_dimensions_units = "mm"
             except: 
                 error_message = "Image dimension values must be numbers."
                 tk.messagebox.showerror("Argument error", error_message)
@@ -394,15 +394,16 @@
             pass
         
         try:
             example_file, mass_list_dir, mass_tolerance_MS1, mass_tolerance_prec, mass_tolerance_frag, mobility_tolerance,\
                 mass_tolerance_MS1_units, mass_tolerance_prec_units, mass_tolerance_frag_units, mobility_tolerance_units,\
                 img_height, img_width, image_dimensions_units, is_MS2, is_mobility, normalize_img_sizes, output_file_loc,\
                     = self.get_input_vars()
-
+            print(mass_tolerance_MS1, mass_tolerance_prec, mass_tolerance_frag, mobility_tolerance)
+            print(mass_tolerance_MS1_units, mass_tolerance_prec_units, mass_tolerance_frag_units, mobility_tolerance_units)
             self.metadata = msigen.get_metadata_and_params(example_file, mass_list_dir, mass_tolerance_MS1, mass_tolerance_MS1_units, mass_tolerance_prec, \
                         mass_tolerance_prec_units, mass_tolerance_frag, mass_tolerance_frag_units, mobility_tolerance, mobility_tolerance_units,\
                         img_height, img_width, image_dimensions_units, is_MS2, is_mobility, normalize_img_sizes, output_file_loc, in_jupyter = False, testing = True)
 
             self.open_progessbar_window()
 
             self.results = {}
@@ -480,35 +481,40 @@
         self.notebook.add(self.tab2, text='Fractional Images')
         self.notebook.add(self.tab3, text='Ratio Images')
 
         # Tab 1: Ion images
         self.normalization1_label = tk.Label(self.tab1, text = "Normalization method:")
         self.normalization1_label.grid(row=0, column=0, sticky = "e")
         self.dropdown_normalization1_var = tk.StringVar(value="None")
-        self.dropdown_normalization1 = ttk.OptionMenu(self.tab1, self.dropdown_normalization1_var, "None", *["None", "TIC", "Internal Standard"])
+        self.dropdown_normalization1 = ttk.OptionMenu(self.tab1, self.dropdown_normalization1_var, \
+            "None", *["None", "TIC", "Internal Standard"], command=self.show_or_hide_std_idx_entry)
         self.dropdown_normalization1.grid(row=0, column=1, sticky = "w")
-        self.dropdown_normalization1_var.trace("w", self.show_or_hide_std_idx_entry)
 
         self.std_idx_var_label = tk.Label(self.tab1, text = "Index of internal standard from mass list:")
         self.std_idx_var_label.grid(row=1, column=0, sticky = "e")
         self.std_idx_var = tk.StringVar(value="1")
         self.std_idx_entry = tk.Entry(self.tab1, textvariable=self.std_idx_var)
         self.std_idx_entry.grid(row=1, column=1, sticky = "ew")
 
-        # self.scale_label = tk.Label(self.tab1, text = "Adjust max intensity to this quantile (0-1):")
-        # self.scale_label.grid(row=2, column=0, sticky = "e")
-        # self.scale_stringvar = tk.StringVar(value=str(self.scale.get()))
-        # self.scale_entry = tk.Entry(self.tab1, textvariable=self.scale_stringvar)
-        # self.scale_entry.grid(row=2, column=1, sticky = "ew")
-
-        self.threshold_label = tk.Label(self.tab1, text = "Adjust max intensity to this value:")
-        self.threshold_label.grid(row=2, column=0, sticky = "e")
-        self.threshold_stringvar = tk.StringVar(value="")
-        self.threshold_entry = tk.Entry(self.tab1, textvariable=self.threshold_stringvar)
-        self.threshold_entry.grid(row=2, column=1, sticky = "ew")
+        self.choose_scale_threshold_label1 = tk.Label(self.tab1, text = "Reduce max intensity to a percentile or an absolute value?")
+        self.choose_scale_threshold_label1.grid(row=2, column=0, sticky = "e")
+        self.choose_scale_threshold_var1 = tk.StringVar(value="Percentile")
+        self.choose_scale_threshold_dropdown1 = ttk.OptionMenu(self.tab1, self.choose_scale_threshold_var1, "Percentile", *["Percentile", "Absolute"],\
+            command = lambda selection: self.scale_or_threshold_display(selection, self.scale_label1, self.scale_entry1, self.threshold_label1, self.threshold_entry1, 3))
+        self.choose_scale_threshold_dropdown1.grid(row=2, column=1, sticky = "w")
+
+        self.scale_label1 = tk.Label(self.tab1, text = "Adjust max intensity to this percentile:")
+        self.scale_stringvar = tk.StringVar(value=str(self.scale.get()))
+        self.scale_entry1 = tk.Entry(self.tab1, textvariable=self.scale_stringvar)
+        self.scale_label1.grid(row=3, column=0, sticky = "e")
+        self.scale_entry1.grid(row=3, column=1, sticky = "ew")
+
+        self.threshold_label1 = tk.Label(self.tab1, text = "Adjust max intensity to this value:")
+        self.threshold_stringvar = tk.StringVar(value="1")
+        self.threshold_entry1 = tk.Entry(self.tab1, textvariable=self.threshold_stringvar)
 
         self.tab1.columnconfigure(0, weight=1, uniform = 'half')
         self.tab1.columnconfigure(1, weight=1, uniform = 'half')
 
         # Tab 2: Fractional Images
         self.normalization2_label = tk.Label(self.tab2, text = "Normalization method:")
         self.normalization2_label.grid(row=0, column=0, sticky = "e")
@@ -518,69 +524,94 @@
 
         self.frac_img_idxs_label = tk.Label(self.tab2, text = "Indices of ions to use from mass list:")
         self.frac_img_idxs_label.grid(row=1, column=0, sticky = "e")
         self.frac_img_idxs_var = tk.StringVar(value="1, 2")
         self.frac_img_idxs = tk.Entry(self.tab2, textvariable=self.frac_img_idxs_var)
         self.frac_img_idxs.grid(row=1, column=1, sticky = "ew")
 
+        self.choose_scale_threshold_label2 = tk.Label(self.tab2, text = "Reduce max intensity to a percentile or an absolute value?")
+        self.choose_scale_threshold_label2.grid(row=2, column=0, sticky = "e")
+        self.choose_scale_threshold_var2 = tk.StringVar(value="Percentile")
+        self.choose_scale_threshold_dropdown2 = ttk.OptionMenu(self.tab2, self.choose_scale_threshold_var2, "Percentile", *["Percentile", "Absolute"],\
+            command = lambda selection: self.scale_or_threshold_display(selection, self.scale_label2, self.scale_entry2, self.threshold_label2, self.threshold_entry2, 3))
+        self.choose_scale_threshold_dropdown2.grid(row=2, column=1, sticky = "w")
+
+        self.scale_label2 = tk.Label(self.tab2, text = "Adjust max intensity to this quantile (0-1):")
+        self.scale_label2.grid(row=3, column=0, sticky = "e")
+        self.scale_entry2 = tk.Entry(self.tab2, textvariable=self.scale_stringvar)
+        self.scale_entry2.grid(row=3, column=1, sticky = "ew")
+
+        self.threshold_label2 = tk.Label(self.tab2, text = "Adjust max intensity to this value:")
+        self.threshold_entry2 = tk.Entry(self.tab2, textvariable=self.threshold_stringvar)
+
         self.tab2.columnconfigure(0, weight=1, uniform = 'half')
         self.tab2.columnconfigure(1, weight=1, uniform = 'half')
 
         # Tab 3: Ratio Images
         self.normalization3_label = tk.Label(self.tab3, text = "Normalization method:")
         self.normalization3_label.grid(row=0, column=0, sticky = "e")
         self.dropdown_normalization3_var = tk.StringVar(value="None")
         self.dropdown_normalization3 = ttk.OptionMenu(self.tab3, self.dropdown_normalization3_var, "None", *["None", "Base Peak"])
         self.dropdown_normalization3.grid(row=0, column=1, sticky = "w")
 
-        self.handle_infinity_method_label = tk.Label(self.tab3, text = "How to handle divide by zero errors:")
-        self.handle_infinity_method_label.grid(row=1, column=0, sticky = "e")
-        self.handle_infinity_method_var = tk.StringVar(value="Maximum")
-        self.dropdown_handle_infinity_method = ttk.OptionMenu(self.tab3, self.handle_infinity_method_var, "Maximum", *['Maximum', 'Infinity', 'Zero'])
-        self.dropdown_handle_infinity_method.grid(row=1, column=1, sticky = "w")
-
         self.ratio_img_idxs_label = tk.Label(self.tab3, text = "Indices of ions to use from mass list:")
-        self.ratio_img_idxs_label.grid(row=2, column=0, sticky = "e")
+        self.ratio_img_idxs_label.grid(row=1, column=0, sticky = "e")
         self.ratio_img_idxs_var = tk.StringVar(value="1, 2")
         self.ratio_img_idxs = tk.Entry(self.tab3, textvariable=self.ratio_img_idxs_var)
-        self.ratio_img_idxs.grid(row=2, column=1, sticky = "ew")
+        self.ratio_img_idxs.grid(row=1, column=1, sticky = "ew")
 
-        # self.scale_label = tk.Label(self.tab3, text = "Adjust max intensity to this quantile (0-1):")
-        # self.scale_label.grid(row=4, column=0, sticky = "e")
-        # self.scale_entry = tk.Entry(self.tab3, textvariable=self.scale_stringvar)
-        # self.scale_entry.grid(row=4, column=1, sticky = "ew")
-
-        self.threshold_label = tk.Label(self.tab3, text = "Adjust max intensity to this value:")
-        self.threshold_label.grid(row=3, column=0, sticky = "e")
-        self.threshold_entry = tk.Entry(self.tab3, textvariable=self.threshold_stringvar)
-        self.threshold_entry.grid(row=3, column=1, sticky = "ew")
+        self.choose_scale_threshold_label3 = tk.Label(self.tab3, text = "Reduce max intensity to a percentile or an absolute value?")
+        self.choose_scale_threshold_label3.grid(row=2, column=0, sticky = "e")
+        self.choose_scale_threshold_var3 = tk.StringVar(value="Percentile")
+        self.choose_scale_threshold_dropdown3 = ttk.OptionMenu(self.tab3, self.choose_scale_threshold_var3, "Percentile", *["Percentile", "Absolute"],\
+            command = lambda selection: self.scale_or_threshold_display(selection, self.scale_label3, self.scale_entry3, self.threshold_label3, self.threshold_entry3, 3))
+        self.choose_scale_threshold_dropdown3.grid(row=2, column=1, sticky = "w")
+
+        self.scale_label3 = tk.Label(self.tab3, text = "Adjust max intensity to this quantile (0-1):")
+        self.scale_label3.grid(row=3, column=0, sticky = "e")
+        self.scale_entry3 = tk.Entry(self.tab3, textvariable=self.scale_stringvar)
+        self.scale_entry3.grid(row=3, column=1, sticky = "ew")
+
+        self.threshold_label3 = tk.Label(self.tab3, text = "Adjust max intensity to this value:")
+        self.threshold_entry3 = tk.Entry(self.tab3, textvariable=self.threshold_stringvar)
+
+        self.handle_infinity_method_label = tk.Label(self.tab3, text = "How to handle divide by zero errors:")
+        self.handle_infinity_method_label.grid(row=4, column=0, sticky = "e")
+        self.handle_infinity_method_var = tk.StringVar(value="Maximum")
+        self.dropdown_handle_infinity_method = ttk.OptionMenu(self.tab3, self.handle_infinity_method_var, "Maximum", *['Maximum', 'Infinity', 'Zero'])
+        self.dropdown_handle_infinity_method.grid(row=4, column=1, sticky = "w")
 
         self.log_scale_var = tk.IntVar()
         self.log_scale_ckbtn = tk.Checkbutton(self.tab3, text="Use log-scale for intensity", variable = self.log_scale_var)
-        self.log_scale_ckbtn.grid(row = 4, column = 0, columnspan = 2)
-
+        self.log_scale_ckbtn.grid(row = 5, column = 0, columnspan = 2)
 
         self.tab3.columnconfigure(0, weight=1, uniform = 'half')
         self.tab3.columnconfigure(1, weight=1, uniform = 'half')
 
         # Parameters applying to any image type
         self.general_img_params_frame = tk.Frame(self.image_maker_window)
         self.general_img_params_frame.pack(fill="x", expand=True, padx = 10)
         self.dropdown_colormap_label = tk.Label(self.general_img_params_frame, text = "Colormap to use:")
-        self.dropdown_colormap_label.grid(row=0, column=0, sticky = "w", padx = 5)
+        self.dropdown_colormap_label.grid(row=0, column=0, sticky = "e", padx = 5)
         self.dropdown_colormap_var = tk.StringVar(value="viridis")
         self.dropdown_colormap = ttk.OptionMenu(self.general_img_params_frame, self.dropdown_colormap_var, "viridis", *["viridis", "cividis", "hot", "jet", "seismic"])
-        self.dropdown_colormap.grid(row=1, column=0, sticky = "w", padx = 5)
+        self.dropdown_colormap.grid(row=0, column=1, sticky = "w", padx = 5)
+
+        self.dropdown_savetype_label = tk.Label(self.general_img_params_frame, text = "Save images as:")
+        self.dropdown_savetype_label.grid(row=1, column=0, sticky = "e", padx = 5)
+        self.dropdown_savetype_var = tk.StringVar(value="figure")
+        self.dropdown_savetype = ttk.OptionMenu(self.general_img_params_frame, self.dropdown_savetype_var, "figure", *["figure", "image", "array"])
+        self.dropdown_savetype.grid(row=1, column=1, sticky = "w", padx = 5)
 
         self.output_file_path_label2 = tk.Label(self.general_img_params_frame, text = "Path to save images to:")
-        self.output_file_path_label2.grid(row=0, column=1, sticky = "w", padx = 5)
+        self.output_file_path_label2.grid(row=2, column=0, sticky = "w", padx = 5)
         self.output_file_path_entry_box2 = tk.Entry(self.general_img_params_frame, textvariable=self.output_file_path)
-        self.output_file_path_entry_box2.grid(row=1, column=1, sticky = "ew", padx = 5)
+        self.output_file_path_entry_box2.grid(row=2, column=1, sticky = "ew", padx = 5)
         self.output_file_path_entry_button2 = MyButton(self.general_img_params_frame, text="Reselect Output Folder", command=self.select_output_file_path)
-        self.output_file_path_entry_button2.grid(row=2, column=1, sticky = "w", padx = 5)
+        self.output_file_path_entry_button2.grid(row=3, column=1, sticky = "w", padx = 5)
 
         self.general_img_params_frame.columnconfigure(1, weight=1, uniform = 'half')
 
         self.img_maker_buttons_frame = tk.Frame(self.image_maker_window)
         self.img_maker_buttons_frame.pack()
         
         self.generate_images_button = MyButton(self.img_maker_buttons_frame, text = 'Generate Images', command = self.generate_images)
@@ -591,79 +622,86 @@
 
         self.reselect_raw_files_button = MyButton(self.img_maker_buttons_frame, text = 'Reselect Raw Files', command = self.reselect_raw_files)
         self.reselect_raw_files_button.pack(side = tk.LEFT, padx = 5)
 
         # self.end_all_button = MyButton(self.img_maker_buttons_frame, text = 'Finish')
         # self.end_all_button.pack(side = tk.LEFT)
 
-    ## TODO make this call the correct image generation function and have a popup window with a clickable path to images
     def generate_images(self):
         active_nb_pg = self.notebook.tab(self.notebook.select(),"text")
         # ensure the threshold box is a positive number
-        print(self.threshold_stringvar.get())
+        
+        
 
-        try:
-            if self.threshold_stringvar.get().replace(' ','').lower() in ["","none"]:
-                threshold = float(0)
-            else:
-                threshold = float(self.threshold_stringvar.get().replace(' ',''))
-            assert threshold >= 0
-            self.threshold.set(threshold)
-        except:
-            error_message = 'The value of the box labelled "Adjust max intensity to this value" must be a positive number.'
-            tk.messagebox.showerror("Threshold value error", error_message)
+        # try:
+        #     if self.threshold_stringvar.get().replace(' ','').lower() in ["","none"]:
+        #         threshold = float(0)
+        #     else:
+        #         threshold = float(self.threshold_stringvar.get().replace(' ',''))
+        #     assert threshold >= 0
+        #     self.threshold.set(threshold)
+        # except:
+        #     error_message = 'The value of the box labelled "Adjust max intensity to this value" must be a positive number.'
+        #     tk.messagebox.showerror("Threshold value error", error_message)
         
-        else:
-            if active_nb_pg == "Ion Images":
-                try:
-                    std_idx = int(self.std_idx_var.get())
-                    assert std_idx > 0
-                except:
-                    std_idx = 0
-                    error_message = "The index of the internal standard must be a single positive integer."
-                    tk.messagebox.showerror("Internal standard index error", error_message)
-                
-                if std_idx:
-                    pixels_normed = vis.get_pixels_to_display(self.pixels, self.metadata, normalize = self.dropdown_normalization1_var.get(), std_idx = std_idx)
-                    vis.save_images(pixels_normed, self.metadata, MSI_data_output=self.output_file_path.get(), cmap=self.dropdown_colormap_var.get(), \
-                        threshold=self.threshold.get(), scale=self.scale.get())
-                    self.open_images_were_saved_dialog()
-
-            elif active_nb_pg == "Fractional Images":
-                try:
-                    idxs_list = [int(i) for i in self.frac_img_idxs_var.get().split(',')]
-                    assert all([i>0 for i in idxs_list])
-                except:
-                    idxs_list = []
-                    error_message = "The indices given must be positive integers separated by a ','."
-                    tk.messagebox.showerror("Index error", error_message)
-
-                if idxs_list:
-                    fract_imgs, titles = vis.get_fractional_abundance_imgs(self.pixels, self.metadata, idxs = idxs_list, \
-                        normalize = self.dropdown_normalization2_var.get())
-                    vis.display_fractional_images(fract_imgs, self.metadata, titles = titles, save_imgs = True, \
-                        MSI_data_output = self.output_file_path.get(), cmap = self.dropdown_colormap_var.get())
-                    self.open_images_were_saved_dialog()
-
-            elif active_nb_pg == "Ratio Images":
-                try:
-                    idxs_list = [int(i) for i in self.ratio_img_idxs_var.get().split(',')]
-                    assert all([i>0 for i in idxs_list]) and (len(idxs_list) == 2)
-                except:
-                    idxs_list = []
-                    error_message = "The indices given must be two positive integers separated by a ','."
-                    tk.messagebox.showerror("Index error", error_message)
-
-                if idxs_list:
-                    ratio_imgs, titles = vis.get_ratio_imgs(self.pixels, self.metadata, idxs = idxs_list, \
-                        normalize = self.dropdown_normalization3_var.get(), handle_infinity = self.handle_infinity_method_var.get())
-                    vis.display_ratio_images(ratio_imgs, self.metadata, titles = titles, save_imgs = True, \
-                        MSI_data_output = self.output_file_path.get(), cmap = self.dropdown_colormap_var.get(),\
-                        log_scale = bool(self.log_scale_var.get()), scale = self.scale.get(), threshold = self.threshold.get())
-                    self.open_images_were_saved_dialog()
+        if active_nb_pg == "Ion Images":
+            scale, threshold = self.get_scale_threshold_values(self.choose_scale_threshold_dropdown1, \
+                                                        self.scale_stringvar, self.threshold_stringvar)
+            print(scale, threshold)
+            try:
+                std_idx = int(self.std_idx_var.get())
+                assert std_idx > 0
+            except:
+                std_idx = 0
+                error_message = "The index of the internal standard must be a single positive integer."
+                tk.messagebox.showerror("Internal standard index error", error_message)
+            
+            if std_idx:
+                pixels_normed = vis.get_pixels_to_display(self.pixels, self.metadata, normalize = self.dropdown_normalization1_var.get(), std_idx = std_idx)
+                vis.display_images(pixels_normed, self.metadata, MSI_data_output=self.output_file_path.get(), cmap=self.dropdown_colormap_var.get(),\
+                    threshold=threshold, scale=scale, save_imgs=True, image_savetype=self.dropdown_savetype_var.get())
+                self.open_images_were_saved_dialog()
+
+        elif active_nb_pg == "Fractional Images":
+            scale, threshold = self.get_scale_threshold_values(self.choose_scale_threshold_dropdown2, \
+                                        self.scale_stringvar, self.threshold_stringvar)
+            try:
+                idxs_list = [int(i) for i in self.frac_img_idxs_var.get().split(',')]
+                assert all([i>0 for i in idxs_list])
+            except:
+                idxs_list = []
+                error_message = "The indices given must be positive integers separated by a ','."
+                tk.messagebox.showerror("Index error", error_message)
+
+            if idxs_list:
+                fract_imgs = vis.get_fractional_abundance_imgs(self.pixels, self.metadata, idxs = idxs_list, \
+                    normalize = self.dropdown_normalization2_var.get())
+                vis.display_fractional_images(fract_imgs, self.metadata, save_imgs = True, MSI_data_output = self.output_file_path.get(), \
+                    cmap = self.dropdown_colormap_var.get(), image_savetype=self.dropdown_savetype_var.get(), scale=scale, threshold=threshold)
+                self.open_images_were_saved_dialog()
+
+        elif active_nb_pg == "Ratio Images":
+            scale, threshold = self.get_scale_threshold_values(self.choose_scale_threshold_dropdown3, \
+                                        self.scale_stringvar, self.threshold_stringvar)
+            try:
+                idxs_list = [int(i) for i in self.ratio_img_idxs_var.get().split(',')]
+                assert all([i>0 for i in idxs_list]) and (len(idxs_list) == 2)
+            except:
+                idxs_list = []
+                error_message = "The indices given must be two positive integers separated by a ','."
+                tk.messagebox.showerror("Index error", error_message)
+
+            if idxs_list:
+                ratio_imgs = vis.get_ratio_imgs(self.pixels, self.metadata, idxs = idxs_list, \
+                    normalize = self.dropdown_normalization3_var.get(), handle_infinity = self.handle_infinity_method_var.get())
+                vis.display_ratio_images(ratio_imgs, self.metadata, save_imgs = True, \
+                    MSI_data_output = self.output_file_path.get(), cmap = self.dropdown_colormap_var.get(),\
+                    log_scale = bool(self.log_scale_var.get()), scale=scale, threshold=threshold, \
+                    image_savetype=self.dropdown_savetype_var.get())
+                self.open_images_were_saved_dialog()
 
     def open_images_were_saved_dialog(self):
         self.images_were_saved_dialog = tk.Toplevel(self.image_maker_window)
         self.images_were_saved_dialog.minsize(200,100)
         self.images_were_saved_dialog.protocol("WM_DELETE_WINDOW", self.images_were_saved_dialog.destroy)
 
         self.saved_imgs_label1 = tk.Label(self.images_were_saved_dialog, text="Your files were saved to:")
@@ -693,14 +731,42 @@
         if self.dropdown_normalization1_var.get() == "Internal Standard":
             self.std_idx_var_label.grid(row=1, column=0, sticky = "e")
             self.std_idx_entry.grid(row=1, column=1, sticky = "ew")
         else: 
             self.std_idx_var_label.grid_forget(row=1, column=0, sticky = "e")
             self.std_idx_entry.grid_forget(row=1, column=1, sticky = "ew")
 
+    def scale_or_threshold_display(self, selection, scale_label, scale_entry, threshold_label, threshold_entry, row):
+        if selection == "Percentile":
+            scale_label.grid(row=row, column=0, sticky = "e")
+            scale_entry.grid(row=row, column=1, sticky = "ew")
+            threshold_label.grid_forget()
+            threshold_entry.grid_forget()
+        else: 
+            threshold_label.grid(row=row, column=0, sticky = "e")
+            threshold_entry.grid(row=row, column=1, sticky = "ew")
+            scale_label.grid_forget()
+            scale_entry.grid_forget()
+
+    def get_scale_threshold_values(self, dropdown_menu, scale_stringvar, threshold_stringvar):
+        if dropdown_menu.get() == "Percentile":
+            scale = scale_stringvar.get()
+            threshold = None
+            try:
+                scale = float(scale)/100
+            except:
+                scale = 1
+        else:
+            scale = 1
+            threshold = threshold_stringvar.get()
+            try:
+                threshold = float(threshold)
+            except:
+                threshold = None
+        return scale, threshold
 
 class FileExplorerWindow(tk.Tk):
     def __init__(self, callback):
         super().__init__()
         self.title("Insert Listbox Example")
         self.geometry("400x300")  # Set a fixed size for the window
         self.callback = callback
```

### Comparing `msigen-0.1.0/MSIGen/msigen.py` & `msigen-0.2.1/MSIGen/msigen.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,19 +338,16 @@
     return MS1_units, prec_units, frag_units, mob_units
 
 def get_mass_or_mobility_window(upper_lims, lower_lims, val_list, tol, unit):
     '''Determines the upper and lower bounds for selection window'''
     if unit.lower() == 'ppm':
         lower_lims.append(np.clip(np.array(val_list) * (1-(tol/1000000)), 0, None))
         upper_lims.append(np.array(val_list) * (1+(tol/1000000)))
-    elif unit.lower() in ['mz','μs','1/K0']:
-        lower_lims.append(np.clip((np.array(val_list) - tol),0,None))
-        upper_lims.append(np.array(val_list) + tol)
     else:
-        lower_lims.append(np.clip((np.array(val_list) - tol),0,None))
+        lower_lims.append(np.clip((np.array(val_list) - tol), 0, None))
         upper_lims.append(np.array(val_list) + tol)
     return upper_lims, lower_lims
 
 def get_all_ms_and_mobility_windows(mass_lists, tolerances, tolerance_units):
     '''Determines the upper and lower bounds for each mass or mobility window'''
     # unpack variables
     MS1_list, MS1_mob_list, MS1_polarity_list, prec_list, frag_list, MS2_mob_list, MS2_polarity_list, mass_list_idxs = mass_lists
@@ -948,21 +945,25 @@
 
 def get_num_spe_per_group_aligned(scans_per_filter_grp, normalize_img_sizes=True):
     num_spe_per_group_aligned = np.ceil(np.max(np.array(scans_per_filter_grp), axis = 0)).astype(int)
     if normalize_img_sizes == True:
         num_spe_per_group_aligned = np.full(num_spe_per_group_aligned.shape, num_spe_per_group_aligned.max(), dtype = int)
     return num_spe_per_group_aligned
 
-def reorder_pixels(pixels, filters_grp_info, mz_idxs_per_filter, mass_list_idxs, line_list):
+def reorder_pixels(pixels, filters_grp_info, mz_idxs_per_filter, mass_list_idxs, line_list, filters_info = None):
+    # get the scan type/level 
     if line_list[0].lower().endswith('.raw'):
-        iterator = filters_grp_info[2]
+        iterator = [] 
+        for filter_grp in filters_grp_info:
+            iterator.append(filters_info[2][np.where(filter_grp[0]==filters_info[0])])
     else:
         iterator = [filtr[0][2] for filtr in filters_grp_info]
 
-    pixels_reordered = [None]*(len(mass_list_idxs[0])+len(mass_list_idxs[1])+1)
+    #put pixels into a list. If the window is MS1, its first mass will be assumed to be TIC.
+    pixels_reordered = [np.zeros((1,1))]*(len(mass_list_idxs[0])+len(mass_list_idxs[1])+1)
     for i, acq_type in enumerate(iterator):
         if acq_type in ['MS1', 1, '1', 'Full ms']:
             pixels_reordered[0] = pixels[i][:,:,0]
             for j in range(pixels[i].shape[-1]-1):
                 pixels_reordered[mass_list_idxs[0][mz_idxs_per_filter[i][j]]+1]=pixels[i][:,:,j+1]
         else:
             for j in range(pixels[i].shape[-1]-1):
```

### Comparing `msigen-0.1.0/MSIGen/mzml.py` & `msigen-0.2.1/MSIGen/mzml.py`

 * *Files identical despite different names*

### Comparing `msigen-0.1.0/MSIGen/raw.py` & `msigen-0.2.1/MSIGen/raw.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,16 @@
 # ==================================
 
 def raw_ms2_no_mob(line_list, mass_lists, lower_lims, upper_lims, experiment_type, metadata = {}, normalize_img_sizes = True, in_jupyter = True, testing = False, gui=False, tkinter_widgets = [None, None, None]):
     # variables for monitoring progress on gui
     if gui:
         tkinter_widgets[1]['text']="Preprocessing data"
         tkinter_widgets[1].update()
+    elif in_jupyter:
+        print("Preprocessing data...")
     
     MS1_list, _, MS1_polarity_list, prec_list, frag_list, _, MS2_polarity_list, mass_list_idxs = mass_lists
     
     acq_times, all_filters_list = check_dim_raw(line_list, experiment_type, ShowNumLineSpe = in_jupyter)
     metadata['average_start_time'] = np.mean([i[0] for i in acq_times])
     metadata['average_end_time'] = np.mean([i[-1] for i in acq_times])
     
@@ -244,15 +246,15 @@
     # for i, pixels_meta in enumerate(pixels_metas):
     #     for j, pixels_meta_grp in enumerate(pixels_meta):
     #         points = (all_TimeStamps_normed[i][j], np.arange(pixels_meta_grp.shape[1]))
     #         sampling_points = np.array(np.meshgrid(*(all_TimeStamps_aligned[j], np.arange(pixels_meta_grp.shape[1])), indexing = 'ij')).transpose(1,2,0)
     #         pixels[j][i] = interpn(points, pixels_meta_grp, sampling_points, method = 'nearest', bounds_error = False, fill_value=None)
     
     # Order the pixels in the way the mass list csv/excel file was ordered
-    pixels = msigen.reorder_pixels(pixels, filters_info, mzIndicesPerFilter, mass_list_idxs, line_list)    
+    pixels = msigen.reorder_pixels(pixels, consolidated_filter_list, mz_idxs_per_filter_grp, mass_list_idxs, line_list, filters_info)    
     if normalize_img_sizes:
         pixels = msigen.pixels_list_to_array(pixels, line_list, all_TimeStamps_aligned)
 
     return metadata, pixels 
 
 def check_dim_raw(line_list, experiment_type, ShowNumLineSpe=False):
     """Gets the times and other information about each scan to decide 
@@ -368,45 +370,40 @@
 
         if Name.lower().endswith('.raw'):
             # Get each filter
             for j in range(len(all_filters_list[i])):
                 Filter = all_filters_list[i][j]
 
                 # Get the filter index of the scan
-                idx = get_filter_idx_raw(Filter,polar_loc,types_loc,acq_types,acq_polars,mz_ranges,precursors)
+                idx = get_filter_idx_raw(Filter,polar_loc,types_loc,acq_types,acq_polars,mz_ranges,precursors,filter_list)
 
                 # count on 
                 Dims[idx] += 1
 
             # count on
             scans_per_filter = np.append(scans_per_filter, Dims.reshape((1, acq_polars.shape[0])), axis=0)
 
     return scans_per_filter
 
-def get_filter_idx_raw(Filter,polar_loc,types_loc,acq_types,acq_polars,mz_ranges,precursors):
+def get_filter_idx_raw(Filter,polar_loc,types_loc,acq_types,acq_polars,mz_ranges,precursors,filter_list):
     '''Gets the index of the current Thermo filter'''
     acq_polar = Filter.split(' ')[polar_loc]
 
     if acq_polar == '+':
         polarity_numeric = 1.0
     elif acq_polar == '-':
         polarity_numeric = -1.0
 
     acq_type = Filter.split(' ')[types_loc[0]] + ' ' + Filter.split(' ')[types_loc[1]]                
 
     if acq_type == 'Full ms':   # since filter name varies for ms, we just hard code this situation. 
         precursor = 0.0
         mz_range = [100.0, 950.0]
-    elif acq_type == 'Full ms2':
-        precursor = float(Filter.split('@')[0].split(' ')[-1])
-        mz_range = [float(Filter.split('[')[-1].split(',')[0].split('-')[0].split(' ')[0]),
-                    float(Filter.split(' ')[-1].split('-')[-1].split(',')[-1].split(']')[0])]
-    
-    mz_range_judge = np.array(mz_range).reshape(1, 2) == mz_ranges.astype(float)
+        mz_range_judge = np.array(mz_range).reshape(1, 2) == mz_ranges.astype(float)    
 
     # to match look-up table: acq_types, acq_polars, precursors
     if acq_type == 'Full ms':
         idx = (polarity_numeric == acq_polars)&(acq_type == acq_types)&(mz_range_judge[:,0])&(mz_range_judge[:,1])
+        idx = np.where(idx)[0]
     if acq_type == 'Full ms2': 
-        idx = (polarity_numeric == acq_polars)&(acq_type == acq_types)&(mz_range_judge[:,0])&(mz_range_judge[:,1])&(precursor == precursors)
-    idx = np.where(idx)[0]
+        idx = np.where(Filter == filter_list)
     return idx
```

### Comparing `msigen-0.1.0/MSIGen/timsdata.dll` & `msigen-0.2.1/MSIGen/timsdata.dll`

 * *Files identical despite different names*

### Comparing `msigen-0.1.0/MSIGen/tsf.py` & `msigen-0.2.1/MSIGen/tsf.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,208 +1,208 @@
-# =========================================================================
-# Allows for processing of .d data that uses Bruker .tsf data storage
-# =========================================================================
-import os
-import ctypes, sqlite3
-from pathlib import Path
-import pandas as pd
-import numpy as np
-
-# =========================================================================
-# initiate bruker dll for .tsf files
-# =========================================================================
-# on windows system, we will use .dll 
-try:
-    dll = ctypes.cdll.LoadLibrary(str((Path(Path(__file__).parent,"timsdata.dll"))))
-
-    ### settings
-    # .tsf Open
-    dll.tsf_open.argtypes = [ctypes.c_char_p, ctypes.c_uint32]
-    dll.tsf_open.restype = ctypes.c_uint64
-
-    # .tsf Close
-    dll.tsf_close.argtypes = [ctypes.c_uint64]
-    dll.tsf_close.restype = None
-
-    # Read in profile or line spectra
-    dll.tsf_read_line_spectrum.argtypes = [ctypes.c_uint64,
-                                                ctypes.c_int64,
-                                                ctypes.POINTER(ctypes.c_double),
-                                                ctypes.POINTER(ctypes.c_float),
-                                                ctypes.c_uint32]
-    dll.tsf_read_line_spectrum.restype = ctypes.c_uint32
-
-    dll.tsf_read_profile_spectrum.argtypes = [ctypes.c_uint64,
-                                                    ctypes.c_int64,
-                                                    ctypes.POINTER(ctypes.c_uint32),
-                                                    ctypes.c_uint32]
-    dll.tsf_read_profile_spectrum.restype = ctypes.c_uint32
-
-    # Get m/z values from indices.
-    dll.tsf_index_to_mz.argtypes = [ctypes.c_uint64,
-                                        ctypes.c_int64,
-                                        ctypes.POINTER(ctypes.c_double),
-                                        ctypes.POINTER(ctypes.c_double),
-                                        ctypes.c_uint32]
-    dll.tsf_index_to_mz.restype = ctypes.c_uint32
-
-
-    # =========================================================================
-    # Import definitions
-    # =========================================================================
-
-
-    class tsf_data(object):
-        def __init__(self, bruker_d_folder_name: str, tdf_sdk_dll, use_recalibrated_state=True):
-            self.dll = tdf_sdk_dll
-            self.handle = self.dll.tsf_open(bruker_d_folder_name.encode('utf-8'), 1 if use_recalibrated_state else 0)
-            if self.handle == 0:
-                raise RuntimeError("Cannot load this file. Is it a .tsf format Bruker file?")
-                
-            self.conn = sqlite3.connect(os.path.join(bruker_d_folder_name, 'analysis.tsf'))
-
-            # arbitrary size, from Bruker tsfdata.py
-            self.line_buffer_size = 1024
-            self.profile_buffer_size = 1024
-
-            self.meta_data = None
-            self.frames = None
-            #self.maldiframeinfo = None
-            self.framemsmsinfo = None
-            self.source_file = bruker_d_folder_name
-
-            self.get_global_metadata()       # to populate the .meta_data
-            self.get_frames_table()          # to pupulate the .frames
-            #self.get_maldiframeinfo_table() # to populate the .maldiframeinfo, skip it since there's no maldi info
-            self.get_framemsmsinfo_table()   # to populate the .framemsmsinfo
-
-            self.close_sql_connection()
-
-        # from Bruker tsfdata.py
-        # provided by Bruker
-        def __del__(self):
-            if hasattr(self, 'handle'):
-                self.dll.tsf_close(self.handle)
-
-        # from Bruker tsfdata.py
-        # provided by Bruker
-        def __call_conversion_func(self, frame_id, input_data, func):
-            if type(input_data) is np.ndarray and input_data.dtype == np.float64:
-                in_array = input_data
-            else:
-                in_array = np.array(input_data, dtype=np.float64)
-
-            cnt = len(in_array)
-            out = np.empty(shape=cnt, dtype=np.float64)
-            success = func(self.handle,
-                        frame_id,
-                        in_array.ctypes.data_as(ctypes.POINTER(ctypes.c_double)),
-                        out.ctypes.data_as(ctypes.POINTER(ctypes.c_double)),
-                        cnt)
-
-            if success == 0:
-                raise RuntimeError("Cannot load this file. Is it a .tsf format Bruker file?")
-
-            return out
-
-        # from Bruker tsfdata.py
-        # provided by Bruker
-        def index_to_mz(self, frame_id, indices):
-            return self.__call_conversion_func(frame_id, indices, self.dll.tsf_index_to_mz)
-
-        # modified from Bruker tsfdata.py
-        def read_line_spectrum(self, frame_id):
-            while True:
-                cnt = int(self.profile_buffer_size)
-                index_buf = np.empty(shape=cnt, dtype=np.float64)
-                intensity_buf = np.empty(shape=cnt, dtype=np.float32)
-
-                required_len = self.dll.tsf_read_line_spectrum(self.handle,
-                                                            frame_id,
-                                                            index_buf.ctypes.data_as(ctypes.POINTER(ctypes.c_double)),
-                                                            intensity_buf.ctypes.data_as(ctypes.POINTER(ctypes.c_float)),
-                                                            self.profile_buffer_size)
-
-                if required_len > self.profile_buffer_size:
-                    if required_len > 16777216:
-                        raise RuntimeError('Maximum expected frame size exceeded.')
-                    self.profile_buffer_size = required_len
-                else:
-                    break
-
-            return (index_buf[0:required_len], intensity_buf[0:required_len])
-
-        # provided by Bruker
-        def read_line_spectrum_with_width(self, frame_id):
-            while True:
-                cnt = int(self.profile_buffer_size)
-                index_buf = np.empty(shape=cnt, dtype=np.float64)
-                intensity_buf = np.empty(shape=cnt, dtype=np.float32)
-                width_buf = np.empty(shape=cnt, dtype=np.float32)
-
-                required_len = self.dll.tsf_read_line_spectrum_with_width(self.handle,
-                                                                        frame_id,
-                                                                        index_buf.ctypes.data_as(ctypes.POINTER(ctypes.c_double)),
-                                                                        intensity_buf.ctypes.data_as(ctypes.POINTER(ctypes.c_float)),
-                                                                        width_buf.ctypes.data_as(ctypes.POINTER(ctypes.c_float)),
-                                                                        self.profile_buffer_size)
-
-                if required_len > self.profile_buffer_size:
-                    if required_len > 16777216:
-                        raise RuntimeError('Maximum expected frame size exceeded.')
-                    self.profile_buffer_size = required_len
-                else:
-                    break
-
-            return (index_buf[0:required_len], intensity_buf[0:required_len], width_buf[0:required_len])
-
-        
-        # modified from Bruker tsfdata.py
-        def read_profile_spectrum(self, frame_id):
-            while True:
-                cnt = int(self.profile_buffer_size)
-                index_buf = np.empty(shape=cnt, dtype=np.float64)
-                intensity_buf = np.empty(shape=cnt, dtype=np.uint32)
-
-                required_len = self.dll.tsf_read_profile_spectrum(self.handle,
-                                                                frame_id,
-                                                                intensity_buf.ctypes.data_as(ctypes.POINTER(ctypes.c_uint32)),
-                                                                self.profile_buffer_size)
-
-                if required_len > self.profile_buffer_size:
-                    if required_len > 16777216:
-                        raise RuntimeError('Maximum expected frame size exceeded.')
-                    self.profile_buffer_size = required_len
-                else:
-                    break
-
-            return intensity_buf[0:required_len]
-
-        # Gets global metadata table as a dictionary.
-        def get_global_metadata(self):
-            metadata_query = 'SELECT * FROM GlobalMetadata'
-            metadata_df = pd.read_sql_query(metadata_query, self.conn)
-            metadata_dict = {}
-            for index, row in metadata_df.iterrows():
-                metadata_dict[row['Key']] = row['Value']
-            self.meta_data = metadata_dict
-
-        # Get Frames table from analysis.tsf SQL database.
-        def get_frames_table(self):
-            frames_query = 'SELECT * FROM Frames'
-            self.frames = pd.read_sql_query(frames_query, self.conn)
-
-        # Get MaldiFramesInfo table from analysis.tsf SQL database.
-        def get_maldiframeinfo_table(self):
-            maldiframeinfo_query = 'SELECT * FROM MaldiFrameInfo'
-            self.maldiframeinfo = pd.read_sql_query(maldiframeinfo_query, self.conn)
-
-        # Get FrameMsMsInfo table from analysis.tsf SQL database.
-        def get_framemsmsinfo_table(self):
-            framemsmsinfo_query = 'SELECT * FROM FrameMsMsInfo'
-            self.framemsmsinfo = pd.read_sql_query(framemsmsinfo_query, self.conn)
-
-        def close_sql_connection(self):
-            self.conn.close()
-
-except:
+# =========================================================================
+# Allows for processing of .d data that uses Bruker .tsf data storage
+# =========================================================================
+import os
+import ctypes, sqlite3
+from pathlib import Path
+import pandas as pd
+import numpy as np
+
+# =========================================================================
+# initiate bruker dll for .tsf files
+# =========================================================================
+# on windows system, we will use .dll 
+try:
+    dll = ctypes.cdll.LoadLibrary(str((Path(Path(__file__).parent,"timsdata.dll"))))
+
+    ### settings
+    # .tsf Open
+    dll.tsf_open.argtypes = [ctypes.c_char_p, ctypes.c_uint32]
+    dll.tsf_open.restype = ctypes.c_uint64
+
+    # .tsf Close
+    dll.tsf_close.argtypes = [ctypes.c_uint64]
+    dll.tsf_close.restype = None
+
+    # Read in profile or line spectra
+    dll.tsf_read_line_spectrum.argtypes = [ctypes.c_uint64,
+                                                ctypes.c_int64,
+                                                ctypes.POINTER(ctypes.c_double),
+                                                ctypes.POINTER(ctypes.c_float),
+                                                ctypes.c_uint32]
+    dll.tsf_read_line_spectrum.restype = ctypes.c_uint32
+
+    dll.tsf_read_profile_spectrum.argtypes = [ctypes.c_uint64,
+                                                    ctypes.c_int64,
+                                                    ctypes.POINTER(ctypes.c_uint32),
+                                                    ctypes.c_uint32]
+    dll.tsf_read_profile_spectrum.restype = ctypes.c_uint32
+
+    # Get m/z values from indices.
+    dll.tsf_index_to_mz.argtypes = [ctypes.c_uint64,
+                                        ctypes.c_int64,
+                                        ctypes.POINTER(ctypes.c_double),
+                                        ctypes.POINTER(ctypes.c_double),
+                                        ctypes.c_uint32]
+    dll.tsf_index_to_mz.restype = ctypes.c_uint32
+
+
+    # =========================================================================
+    # Import definitions
+    # =========================================================================
+
+
+    class tsf_data(object):
+        def __init__(self, bruker_d_folder_name: str, tdf_sdk_dll, use_recalibrated_state=True):
+            self.dll = tdf_sdk_dll
+            self.handle = self.dll.tsf_open(bruker_d_folder_name.encode('utf-8'), 1 if use_recalibrated_state else 0)
+            if self.handle == 0:
+                raise RuntimeError("Cannot load this file. Is it a .tsf format Bruker file?")
+                
+            self.conn = sqlite3.connect(os.path.join(bruker_d_folder_name, 'analysis.tsf'))
+
+            # arbitrary size, from Bruker tsfdata.py
+            self.line_buffer_size = 1024
+            self.profile_buffer_size = 1024
+
+            self.meta_data = None
+            self.frames = None
+            #self.maldiframeinfo = None
+            self.framemsmsinfo = None
+            self.source_file = bruker_d_folder_name
+
+            self.get_global_metadata()       # to populate the .meta_data
+            self.get_frames_table()          # to pupulate the .frames
+            #self.get_maldiframeinfo_table() # to populate the .maldiframeinfo, skip it since there's no maldi info
+            self.get_framemsmsinfo_table()   # to populate the .framemsmsinfo
+
+            self.close_sql_connection()
+
+        # from Bruker tsfdata.py
+        # provided by Bruker
+        def __del__(self):
+            if hasattr(self, 'handle'):
+                self.dll.tsf_close(self.handle)
+
+        # from Bruker tsfdata.py
+        # provided by Bruker
+        def __call_conversion_func(self, frame_id, input_data, func):
+            if type(input_data) is np.ndarray and input_data.dtype == np.float64:
+                in_array = input_data
+            else:
+                in_array = np.array(input_data, dtype=np.float64)
+
+            cnt = len(in_array)
+            out = np.empty(shape=cnt, dtype=np.float64)
+            success = func(self.handle,
+                        frame_id,
+                        in_array.ctypes.data_as(ctypes.POINTER(ctypes.c_double)),
+                        out.ctypes.data_as(ctypes.POINTER(ctypes.c_double)),
+                        cnt)
+
+            if success == 0:
+                raise RuntimeError("Cannot load this file. Is it a .tsf format Bruker file?")
+
+            return out
+
+        # from Bruker tsfdata.py
+        # provided by Bruker
+        def index_to_mz(self, frame_id, indices):
+            return self.__call_conversion_func(frame_id, indices, self.dll.tsf_index_to_mz)
+
+        # modified from Bruker tsfdata.py
+        def read_line_spectrum(self, frame_id):
+            while True:
+                cnt = int(self.profile_buffer_size)
+                index_buf = np.empty(shape=cnt, dtype=np.float64)
+                intensity_buf = np.empty(shape=cnt, dtype=np.float32)
+
+                required_len = self.dll.tsf_read_line_spectrum(self.handle,
+                                                            frame_id,
+                                                            index_buf.ctypes.data_as(ctypes.POINTER(ctypes.c_double)),
+                                                            intensity_buf.ctypes.data_as(ctypes.POINTER(ctypes.c_float)),
+                                                            self.profile_buffer_size)
+
+                if required_len > self.profile_buffer_size:
+                    if required_len > 16777216:
+                        raise RuntimeError('Maximum expected frame size exceeded.')
+                    self.profile_buffer_size = required_len
+                else:
+                    break
+
+            return (index_buf[0:required_len], intensity_buf[0:required_len])
+
+        # provided by Bruker
+        def read_line_spectrum_with_width(self, frame_id):
+            while True:
+                cnt = int(self.profile_buffer_size)
+                index_buf = np.empty(shape=cnt, dtype=np.float64)
+                intensity_buf = np.empty(shape=cnt, dtype=np.float32)
+                width_buf = np.empty(shape=cnt, dtype=np.float32)
+
+                required_len = self.dll.tsf_read_line_spectrum_with_width(self.handle,
+                                                                        frame_id,
+                                                                        index_buf.ctypes.data_as(ctypes.POINTER(ctypes.c_double)),
+                                                                        intensity_buf.ctypes.data_as(ctypes.POINTER(ctypes.c_float)),
+                                                                        width_buf.ctypes.data_as(ctypes.POINTER(ctypes.c_float)),
+                                                                        self.profile_buffer_size)
+
+                if required_len > self.profile_buffer_size:
+                    if required_len > 16777216:
+                        raise RuntimeError('Maximum expected frame size exceeded.')
+                    self.profile_buffer_size = required_len
+                else:
+                    break
+
+            return (index_buf[0:required_len], intensity_buf[0:required_len], width_buf[0:required_len])
+
+        
+        # modified from Bruker tsfdata.py
+        def read_profile_spectrum(self, frame_id):
+            while True:
+                cnt = int(self.profile_buffer_size)
+                index_buf = np.empty(shape=cnt, dtype=np.float64)
+                intensity_buf = np.empty(shape=cnt, dtype=np.uint32)
+
+                required_len = self.dll.tsf_read_profile_spectrum(self.handle,
+                                                                frame_id,
+                                                                intensity_buf.ctypes.data_as(ctypes.POINTER(ctypes.c_uint32)),
+                                                                self.profile_buffer_size)
+
+                if required_len > self.profile_buffer_size:
+                    if required_len > 16777216:
+                        raise RuntimeError('Maximum expected frame size exceeded.')
+                    self.profile_buffer_size = required_len
+                else:
+                    break
+
+            return intensity_buf[0:required_len]
+
+        # Gets global metadata table as a dictionary.
+        def get_global_metadata(self):
+            metadata_query = 'SELECT * FROM GlobalMetadata'
+            metadata_df = pd.read_sql_query(metadata_query, self.conn)
+            metadata_dict = {}
+            for index, row in metadata_df.iterrows():
+                metadata_dict[row['Key']] = row['Value']
+            self.meta_data = metadata_dict
+
+        # Get Frames table from analysis.tsf SQL database.
+        def get_frames_table(self):
+            frames_query = 'SELECT * FROM Frames'
+            self.frames = pd.read_sql_query(frames_query, self.conn)
+
+        # Get MaldiFramesInfo table from analysis.tsf SQL database.
+        def get_maldiframeinfo_table(self):
+            maldiframeinfo_query = 'SELECT * FROM MaldiFrameInfo'
+            self.maldiframeinfo = pd.read_sql_query(maldiframeinfo_query, self.conn)
+
+        # Get FrameMsMsInfo table from analysis.tsf SQL database.
+        def get_framemsmsinfo_table(self):
+            framemsmsinfo_query = 'SELECT * FROM FrameMsMsInfo'
+            self.framemsmsinfo = pd.read_sql_query(framemsmsinfo_query, self.conn)
+
+        def close_sql_connection(self):
+            self.conn.close()
+
+except:
     pass
```

### Comparing `msigen-0.1.0/MSIGen/visualization.py` & `msigen-0.2.1/MSIGen/visualization.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib import colors
 from skimage.transform import resize
 import os
+from PIL import Image
 
 
 # ===========================================================================================
 # Raw or normalized image visualization
 # ===========================================================================================
 
 def get_normalize_value(normalize, possible_entries = ['None','TIC','intl_std']):
     if normalize in [None, False]:
         normalize = 'None'
 
     elif type(normalize) == str:
         normalize_vals_dict = {
             'None': ['none', 'no', 'false'],
-            'TIC': ['tic', 'total ion current'],
+            'TIC': ['tic', 'total ion current', 'total_ion_current'],
             'intl_std': ['intl', 'internal', 'internal standard', "internal_standard", 'intl std', 'intl_std', 'standard', 'std'],
             'base_peak': ['base', 'base_peak', 'base peak', 'tallest_peak', 'tallest peak'],
         }
         # Check if the given value is in the dict
         for key in possible_entries:
             if normalize.lower() in normalize_vals_dict[key]:
                 normalize = key
                 break
         # raise error if not in dict
         if normalize not in possible_entries:
             raise ValueError(f"Value for 'normalize' should be in {possible_entries}")
-
     
     else:
-        raise ValueError(f"Value for 'normalize' should be in {possible_entries}")
+        raise ValueError(f"Value for 'normalize' should be one of the following:\n{possible_entries}")
     return normalize
 
 def match_to_mass_list(mass_list, std_idx = None, std_precursor = None, std_mass = None, std_fragment = None, std_mobility = None, std_charge = None):
     # use given std_idx if possible
     if std_idx != None:
         return std_idx
 
@@ -105,21 +105,21 @@
 
 def base_peak_normalize_pixels(pixels):
     for i, img in enumerate(pixels):
         if img.max():
             pixels[i]=img/img.max()
     return pixels
 
-
 def get_and_dispay_images(pixels, metadata, normalize = None, std_idx = None, std_precursor = None, std_mass = None, \
                         std_fragment = None, std_mobility = None, std_charge = None, aspect = None, scale = .999, \
                         how_many_images_to_display = 'all', save_imgs = False, MSI_data_output = None, cmap = 'viridis', \
-                        titles = None, threshold = None, title_fontsize = 10):
+                        titles = None, threshold = None, title_fontsize = 10, image_savetype = "figure", axis_tick_marks = False):
     pixels_normed = get_pixels_to_display(pixels, metadata, normalize, std_idx, std_precursor, std_mass, std_fragment, std_mobility, std_charge)
-    display_images(pixels_normed, metadata, aspect, scale, how_many_images_to_display, save_imgs, MSI_data_output, cmap, titles, threshold, title_fontsize)
+    display_images(pixels_normed, metadata, aspect, scale, how_many_images_to_display, save_imgs, MSI_data_output, cmap, titles, threshold, \
+                   title_fontsize, image_savetype=image_savetype, axis_tick_marks=axis_tick_marks)
 
 def get_pixels_to_display(pixels, metadata, normalize = None, std_idx = None, std_precursor = None, std_mass = None, std_fragment = None, std_mobility = None, std_charge = None):
     """Normalizes MS1 pixels to TIC or to an internal standard.
     The if images are of varying size, the standard image is reshaped to the size of the image to be normalized."""      
 
     normalize = get_normalize_value(normalize, ['None', 'TIC', 'intl_std'])
 
@@ -135,75 +135,36 @@
         pixels_normed = normalize_pixels(pixels, 0)
 
     else:
         pixels_normed = pixels
 
     return pixels_normed
 
-def save_images(pixels_normed, metadata, aspect = None, scale = .999, \
-                MSI_data_output = None, cmap = 'viridis', titles = None, \
-                threshold = None, title_fontsize = 10):
-    
-    # Get the titles for all figures:
-    mass_list = metadata["final_mass_list"]
-    
-    if titles == None:
-        titles = determine_titles(mass_list)
-
-    # make sure save directory exists
-    if MSI_data_output == None:
-        MSI_data_output = os.getcwd()
-    img_output_folder = os.path.join(MSI_data_output,'images')
-    if not os.path.exists(img_output_folder):
-        os.makedirs(img_output_folder)
-
-    # plot each image
-    img_height, img_width = metadata['image_dimensions']
-    # use manually given aspect ratio
-    a = aspect
-
-    if threshold:
-        thre = threshold
-
-    for i in range(len(pixels_normed)):
-        img = pixels_normed[i]
-        
-        if not threshold:
-            thre = np.quantile(img, scale)
-        if thre == 0: thre = 1
-
-        title = titles[i]
-        
-        # recalculate aspect ratio for each image
-        if aspect == None:
-            a = (img_height/img.shape[0])/(img_width/img.shape[1])
-
-        plt.figure(figsize=(6,6))
-        plt.imshow(img, cmap = cmap, aspect = a, vmax=thre, interpolation='none')
-        plt.title(title, fontsize = title_fontsize)
-        plt.xticks([])
-        plt.yticks([])
-        plt.colorbar()
-
-        plt.savefig(os.path.join(img_output_folder,title.replace(':','_').replace('\n',' ').replace('>','').replace('/','')+'.png') )
-        plt.close()
-
-
-
 def display_images(pixels_normed, metadata, aspect = None, scale = .999, how_many_images_to_display = 'all', \
-                    save_imgs = False, MSI_data_output = None, cmap = 'viridis', titles = None, threshold = None, title_fontsize = 10):
+                    save_imgs = False, MSI_data_output = None, cmap = 'viridis', titles = None, threshold = None, \
+                    title_fontsize = 10, image_savetype = "figure", axis_tick_marks = False):
 
     # parse args
-    if how_many_images_to_display == 'all': how_many_images_to_display = len(pixels_normed) 
+    if how_many_images_to_display == 'all':
+        how_many_images_to_display = len(pixels_normed)
+    if type(how_many_images_to_display) in [str, int, float]:
+        try:
+            how_many_images_to_display = list(range(int(how_many_images_to_display)))
+        except:
+            raise TypeError("how_many_images_to_display must be either 'all' or an integer")
+    if type(how_many_images_to_display) in [list, tuple]:
+        try:
+            how_many_images_to_display = [int(i) for i in how_many_images_to_display]
+        except:
+            raise TypeError("how_many_images_to_display must be 'all', an integer, or a list of integers")
 
     # Get the titles for all figures:
     mass_list = metadata["final_mass_list"]
     
-    if titles == None:
-        titles = determine_titles(mass_list)
+    default_titles = determine_titles(mass_list, idxs = how_many_images_to_display)
 
     # make sure save directory exists
     if save_imgs:
         if MSI_data_output == None:
             MSI_data_output = os.getcwd()
         img_output_folder = os.path.join(MSI_data_output,'images')
         if not os.path.exists(img_output_folder):
@@ -213,43 +174,35 @@
     img_height, img_width = metadata['image_dimensions']
     # use manually given aspect ratio
     a = aspect
 
     if threshold:
         thre = threshold
 
-    for i in range(len(pixels_normed)):
+    for i, img_idx in enumerate(how_many_images_to_display):
         # stop early if desired
-        if i>=how_many_images_to_display:
-            break
-
-        img = pixels_normed[i]
+        img = pixels_normed[img_idx]
         
         if not threshold:
             thre = np.quantile(img, scale)
         if thre == 0: thre = 1
 
-        title = titles[i]
+        if titles == None:
+            title = default_titles[i]
+        else:
+            title = titles[i]
+        default_title = default_titles[i]
         
         # recalculate aspect ratio for each image
         if aspect == None:
             a = (img_height/img.shape[0])/(img_width/img.shape[1])
 
-        plt.figure(figsize=(6,6))
-        plt.imshow(img, cmap = cmap, aspect = a, vmax=thre, interpolation='none')
-        plt.title(title, fontsize = title_fontsize)
-        plt.xticks([])
-        plt.yticks([])
-        plt.colorbar()
-        if save_imgs: 
-            plt.savefig(os.path.join(img_output_folder,title.replace(':','_').replace('\n',' ').replace('>','').replace('/','')+'.png') )
-        else:
-            plt.show()
-        plt.close()
-        plt.clf()
+        plot_image(img=img, img_output_folder=img_output_folder, title=title, default_title=default_title, title_fontsize=title_fontsize, \
+                cmap=cmap, aspect=a, save_imgs=save_imgs, thre=thre, log_scale = False, image_savetype=image_savetype, axis_tick_marks=axis_tick_marks)
+
 
 def determine_titles(mass_list, idxs = None, fract_abund = False, ratio_img=False):
     titles = []
     polarity_dict = { 1.0:'+',
                     0.0:'',
                     -1.0:'-'}
 
@@ -280,25 +233,24 @@
 
 
 # ===========================================================================================
 # fractional abuncance images
 # ===========================================================================================
 
 def fractional_abundance_images(pixels, metadata, idxs = [1,2], normalize = None,titles = None, \
-                        aspect = None, save_imgs = False, MSI_data_output = None, cmap = 'viridis', title_fontsize = 10):
+                        aspect = None, save_imgs = False, MSI_data_output = None, cmap = 'viridis', \
+                        title_fontsize = 10, image_savetype = 'figure', scale = 1.0, threshold=None):
     
-    fract_imgs, potential_titles = get_fractional_abundance_imgs(pixels, metadata, idxs, normalize)
-    if not titles: titles == potential_titles
-    display_fractional_images(fract_imgs, metadata, titles, aspect, save_imgs, MSI_data_output, cmap, title_fontsize)
+    fract_imgs = get_fractional_abundance_imgs(pixels, metadata, idxs, normalize)
+    display_fractional_images(fract_imgs, metadata, titles, aspect, save_imgs, MSI_data_output, cmap, \
+                              title_fontsize, idxs, image_savetype=image_savetype, scale=scale, threshold=threshold)
 
 def get_fractional_abundance_imgs(pixels, metadata, idxs = [1,2], normalize = None):
     normalize = get_normalize_value(normalize, ['None', 'base_peak'])
 
-    mass_list = metadata["final_mass_list"]
-
     imgs = [pixels[i] for i in idxs]
 
     # Ensure images are all the same size
     shapes = [img.shape for img in imgs]
     idxs_to_reshape = np.any(~np.equal(shapes[0],shapes), axis = 1)
     for idx, i in enumerate(idxs_to_reshape):
         if i: imgs[idx] = resize(imgs[idx], shapes[0], order=0)
@@ -308,87 +260,89 @@
 
     img_sum = np.sum(imgs, axis = 0)
 
     fract_imgs = []
     for i in imgs:
         fract_imgs.append(np.divide(i, img_sum, out=np.zeros_like(i), where=img_sum!=0))
 
-    titles = determine_titles(mass_list, idxs = idxs, fract_abund=True)
-
-    return fract_imgs, titles
+    return fract_imgs
 
 def display_fractional_images(fract_imgs, metadata, titles = None, aspect = None,\
                             save_imgs = False, MSI_data_output = None, cmap = 'viridis', \
-                            title_fontsize = 10):    
-    if titles == None:
-        titles = ['']*len(fract_imgs)
+                            title_fontsize = 10, idxs = [1,2], image_savetype='figure', \
+                            scale = 1.0, threshold = None):    
+
+    mass_list = metadata["final_mass_list"]
+    default_titles = determine_titles(mass_list, idxs = idxs, fract_abund=True)
 
     # make sure save directory exists
     if save_imgs:
         if MSI_data_output == None:
             MSI_data_output = os.getcwd()
         img_output_folder = os.path.join(MSI_data_output,'images')
         if not os.path.exists(img_output_folder):
             os.makedirs(img_output_folder)
 
+    if threshold:
+        thre = threshold
+
     # plot each image
     img_height, img_width = metadata['image_dimensions']
     # use manually given aspect ratio
     a = aspect
 
     for i in range(len(fract_imgs)):
+        
         img = fract_imgs[i]
-        title = titles[i]
+
+        if not threshold:
+            thre = np.quantile(img, scale)
+        if thre == 0: thre = 1
+
+        if titles == None:
+            title = default_titles[i]
+        else:
+            title = titles[i]
+        default_title = default_titles[i]
         
         # recalculate aspect ratio for each image in case image sizes are different
         if aspect == None:
             a = (img_height/img.shape[0])/(img_width/img.shape[1])
 
-        plt.figure(figsize=(6,6))
-        plt.imshow(img, cmap = cmap, aspect = a, vmin = 0, vmax=1, interpolation='none')
-        plt.title(title, fontsize = title_fontsize)
-        plt.xticks([])
-        plt.yticks([])
-        plt.colorbar()
-        if save_imgs: 
-            plt.savefig(os.path.join(img_output_folder,title.replace(':','_').replace('\n',' ').replace('>','').replace('/','')+'.png'))
-        else:
-            plt.show()
-        plt.close()
-        plt.clf()
+        plot_image(img=img, img_output_folder=img_output_folder, title=title, default_title=default_title, title_fontsize=title_fontsize, \
+                   cmap=cmap, aspect=a, save_imgs=save_imgs, thre=thre, log_scale = False, image_savetype=image_savetype)
 
 
 # ===========================================================================================
 # ratio images
 # ===========================================================================================
 
 def ratio_images(pixels, metadata, idxs = [1,2], normalize = None, handle_infinity = 'maximum', titles = None, \
                 aspect = None, scale = .999,save_imgs = False, MSI_data_output = None, cmap = 'viridis', \
-                log_scale = False, threshold = None, title_fontsize = 10):
+                log_scale = False, threshold = None, title_fontsize = 10, image_savetype = 'figure'):
     
-    ratio_imgs, titles = get_ratio_imgs(pixels, metadata, idxs, normalize, handle_infinity, titles)
-    display_ratio_images(ratio_imgs, metadata, titles, aspect, scale, save_imgs, MSI_data_output, cmap, log_scale, threshold, title_fontsize)
+    ratio_imgs = get_ratio_imgs(pixels, metadata, idxs, normalize, handle_infinity, titles)
+    display_ratio_images(ratio_imgs, metadata, titles, aspect, scale, save_imgs, MSI_data_output, cmap, log_scale, \
+                         threshold, title_fontsize, idxs, image_savetype=image_savetype)
 
 def get_ratio_imgs(pixels, metadata, idxs = [1,2], normalize = None, handle_infinity = 'maximum', titles = None):
     assert handle_infinity.lower() in ['maximum', 'infinity', 'zero'], "handle_infinity must be in ['maximum', 'infinity', 'zero']"
 
     idxs = idxs[:2]
     normalize = get_normalize_value(normalize, ['None', 'base_peak'])
 
-    mass_list = metadata["final_mass_list"]
-
     imgs = [pixels[i] for i in idxs]
 
     # Ensure images are all the same size
     shapes = [img.shape for img in imgs]
     idxs_to_reshape = np.any(~np.equal(shapes[0],shapes), axis = 1)
     for idx, i in enumerate(idxs_to_reshape):
         if i: imgs[idx] = resize(imgs[idx], shapes[0], order=0)
 
-    if normalize == 'base_peak':
+    if normalize == "base_peak":
         imgs = base_peak_normalize_pixels(imgs)
 
     ratio_imgs = []
 
     # Get default values for where the images are both 0
     img_background = np.zeros(imgs[0].shape)
     img_background[np.where((imgs[0] == 0) & (imgs[1] == 0))] = 1
@@ -406,23 +360,22 @@
     ratio_imgs.append(np.divide(imgs[1], imgs[0], out=img2_background, where=imgs[0]!=0))
 
     if handle_infinity == 'maximum':
         # set locations where you divided a non-zero value by zero to the maximum
         ratio_imgs[0][np.isinf(ratio_imgs[0])] = ratio_imgs[0][~np.isinf(ratio_imgs[0])].max()
         ratio_imgs[1][np.isinf(ratio_imgs[0])] = ratio_imgs[1][~np.isinf(ratio_imgs[1])].max()
 
-    if not titles:
-        titles = determine_titles(mass_list, idxs = idxs, ratio_img = True)
-
-    return ratio_imgs, titles
+    return ratio_imgs
 
 def display_ratio_images(ratio_imgs, metadata, titles = None, aspect = None, scale = .999,save_imgs = False, \
-                         MSI_data_output = None, cmap = 'viridis', log_scale = False, threshold = None, title_fontsize = 10):    
-    if titles == None:
-        titles = ['']*len(ratio_imgs)
+                         MSI_data_output = None, cmap = 'viridis', log_scale = False, threshold = None, \
+                         title_fontsize = 10, idxs = [1,2], image_savetype = 'figure'):    
+
+    mass_list = metadata["final_mass_list"]
+    default_titles = determine_titles(mass_list, idxs = idxs, ratio_img = True)
 
     # make sure save directory exists
     if save_imgs:
         if MSI_data_output == None:
             MSI_data_output = os.getcwd()
         img_output_folder = os.path.join(MSI_data_output,'images')
         if not os.path.exists(img_output_folder):
@@ -434,35 +387,109 @@
     a = aspect
 
     if threshold:
         thre = threshold
 
     for i in range(len(ratio_imgs)):
         img = ratio_imgs[i]
-        title = titles[i]
+
+        if titles == None:
+            title = default_titles[i]
+        else:
+            title = titles[i]
+        default_title = default_titles[i]
 
         if scale and (not threshold):
             thre = np.quantile(img, scale)
         elif not threshold: 
             thre = img.max()
 
         # recalculate aspect ratio for each image in case image sizes are different
         if aspect == None:
             a = (img_height/img.shape[0])/(img_width/img.shape[1])
 
+        plot_image(img=img, img_output_folder=img_output_folder, title=title, default_title=default_title, title_fontsize=title_fontsize, \
+                   cmap=cmap, aspect=a, save_imgs=save_imgs, thre=thre, log_scale = log_scale, image_savetype=image_savetype)
+
+def plot_image(img, img_output_folder, title, default_title, title_fontsize, cmap, aspect, save_imgs, thre, \
+    log_scale = False, image_savetype='figure', axis_tick_marks = False):
+
+    # Save images as publication-style figure, including a colorbar and title
+    if image_savetype == 'figure':
         plt.figure(figsize=(6,6))
         if log_scale:
-            plt.imshow(img, cmap = cmap, aspect = a, norm = colors.LogNorm(), interpolation='none')
+            # Prevent -inf values from taking log of zero
+            min_thre = np.min(img[np.nonzero(img)])/10
+            min_thre_img = np.where(img==0, min_thre, img)
+            plt.imshow(min_thre_img, cmap = cmap, aspect = aspect, norm = colors.LogNorm(), interpolation='none')
         else:
-            plt.imshow(img, cmap = cmap, aspect = a, vmin = 0, vmax=thre, interpolation='none')
+            plt.imshow(img, cmap = cmap, aspect = aspect, vmin = 0, vmax=thre, interpolation='none')
 
         plt.title(title, fontsize = title_fontsize)
-        plt.xticks([])
-        plt.yticks([])
+        
+        if not axis_tick_marks:
+            plt.xticks([])
+            plt.yticks([])
+
         plt.colorbar()
+
         if save_imgs: 
-            plt.savefig(os.path.join(img_output_folder,title.replace(':','_').replace('\n',' ').replace('>','').replace('/','')+'.png') )
+            try:
+                plt.savefig(os.path.join(img_output_folder,title.replace(':','_').replace('\n',' ').replace('>','').replace('/','')+'.png') )
+            except:
+                plt.savefig(os.path.join(img_output_folder,default_title.replace(':','_').replace('\n',' ').replace('>','').replace('/','')+'.png') )
         else:
             plt.show()
         plt.close()
         plt.clf()
-        
+
+    # Save as an image without any colorbar or title
+    elif image_savetype == 'image':
+        cm = plt.get_cmap(cmap)
+
+        if log_scale:
+            # Prevent -inf values from taking log of zero
+            min_thre = np.min(img[np.nonzero(img)])/10
+            min_thre_img = np.where(img==0, min_thre, img)
+            img = np.log10(min_thre_img)
+            thre = np.log10(thre)
+
+        img = np.where(img>thre, thre, img)
+        normed_img = (img-img.min())/(img.max()-img.min())
+        colored_img = cm(normed_img)
+        colored_img = (colored_img[:,:,:3]*255).astype(np.uint8)
+        
+        # get dimensions for resizing
+        h, w = colored_img.shape[:2]
+        
+        if save_imgs:
+            pil_img = Image.fromarray(colored_img)
+            if aspect >=1:
+                pil_img = pil_img.resize((round(h*aspect), w), resample=0)
+            else:
+                pil_img = pil_img.resize((h, w//aspect), resample=0)
+
+            try:
+                pil_img.save(os.path.join(img_output_folder,title.replace(':','_').replace('\n',' ').replace('>','').replace('/','')+"_threshold-"+str(thre)+'.png') )
+            except:
+                pil_img.save(os.path.join(img_output_folder,default_title.replace(':','_').replace('\n',' ').replace('>','').replace('/','')+"_threshold-"+str(thre)+'.png') )
+        else:
+            fig, ax = plt.subplots()
+            ax.axis('off')
+            ax.imshow(pil_img)
+            plt.show()
+            plt.clf()
+
+    # Save as an array in csv format
+    elif image_savetype == 'array':
+        if log_scale:
+            # Prevent -inf values from taking log of zero
+            min_thre = np.min(img[np.nonzero(img)])/10
+            min_thre_img = np.where(img==0, min_thre, img)
+            img = np.log10(min_thre_img)
+            thre = np.log10(thre)
+        img = np.where(img>thre, thre, img)
+        try:
+            np.savetxt(os.path.join(img_output_folder,title.replace(':','_').replace('\n',' ').replace('>','').replace('/','')+"_threshold-"+str(thre)+'.csv'), img, delimiter=",")
+        except:
+            np.savetxt(os.path.join(img_output_folder,default_title.replace(':','_').replace('\n',' ').replace('>','').replace('/','')+"_threshold-"+str(thre)+'.csv'), img, delimiter=",")
+
```

### Comparing `msigen-0.1.0/pyproject.toml` & `msigen-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "msigen"
-version = "0.1.0"
+version = "0.2.1"
 description = "A package for converting spectrometry imaging line scan data files to a visualizable format"
 authors = ["Emerson Hernly <elhernly@gmail.com>"]
 license = "MIT"
 readme = "README.md"
-repository = "https://github.com/EmersonHernly/MSIGen"
-homepage = "https://github.com/EmersonHernly/MSIGen"
+repository = "https://github.com/LabLaskin/MSIGen"
+homepage = "https://github.com/LabLaskin/MSIGen"
 
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: Microsoft :: Windows",
-  "Development Status :: 3 - Alpha",
+  "Development Status :: 4 - Beta",
   "Natural Language :: English",
   "Intended Audience :: Science/Research",
   "Topic :: Scientific/Engineering",
 ]
 
 include=['GUI shortcuts', 'tests']
```

### Comparing `msigen-0.1.0/README.md` & `msigen-0.2.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,47 @@
-# MSIGen
-MSIGen is designed for converting mass spectrometry imaging (MSI) data from the raw line-scan data to a visualizable format and is designed with nano-DESI MSI in mind. It has premade files for converting to images using a GUI, jupyter notebook, or from the command line.
-
-## Installation on Windows
-Using Anaconda (https://www.anaconda.com/download), create a new environment titled "MSIGen" with python >=3.8 and activate it. Then, MSIGen can be installed using the pip package manager.
-
-Run the following in anaconda prompt:
-```
-conda create --name MSIGen python=3.9
-conda activate MSIGen
-pip install MSIGen
-```
-### For GUI tool:
-Download "make GUI shortcut.py" from the tests folder in the Github repository. Run this code from Anaconda prompt.
-```
-conda activate MSIGen
-python "C:/path/to/make GUI shortcut.py"
-```
-After running with the actual location of "make GUI shortcut.py", there should be a shortcut called "MSIGen GUI" on your desktop. This runs the GUI for MSIGen.
-
-### For Jupyter Notebook Tool:
-Download "MSIGen_jupyter.ipynb" from the tests folder in the Github repository. Open Anaconda and run Jupyter Notebook in the MSIGen environment. Open "MSIGen_jupyter.ipynb" from Jupyter Notebook.
-
-### For Command Line Interface Tool:
-Download "MSIGen_CLI.py" from the tests folder in the Github repository. Create a configuration file for your experiment. An example can be found in the tests folder. Run the following in Anaconda Prompt:
-```
-conda activate MSIGen
-python "C:/Path/to/MSIGen_CLI.py" "C:/path/to/config_file1.json" "C:/path/to/config_file2.json"
-```
-Supply one configuration file for each dataset to be processed.
-
-
+# MSIGen
+MSIGen is designed for converting mass spectrometry imaging (MSI) data from the raw line-scan data to a visualizable format and is designed with nano-DESI MSI in mind. It has premade files for converting to images using a GUI, jupyter notebook, or from the command line.
+
+## Installation on Windows
+Using Anaconda (https://www.anaconda.com/download), create a new environment titled "MSIGen" with python >=3.9 and <3.12 and activate it. Then, MSIGen can be installed using the pip package manager.
+
+Run the following in Anaconda Prompt one line at a time:
+```
+conda create --name MSIGen python=3.11 -y
+conda activate MSIGen
+pip install MSIGen
+```
+### For GUI tool:
+Download "make GUI shortcut.py" from the tests folder in the Github repository. Run this code from Anaconda Prompt.
+```
+conda activate MSIGen
+python "C:/path/to/make GUI shortcut.py"
+```
+After running with the actual location of "make GUI shortcut.py", there should be a shortcut called "MSIGen GUI" on your desktop. This runs the GUI for MSIGen.
+
+### For Jupyter Notebook Tool:
+Download "MSIGen_jupyter.ipynb" from the tests folder in the Github repository. Open Anaconda Navigator and run Jupyter Notebook in the MSIGen environment. Open "MSIGen_jupyter.ipynb" from Jupyter Notebook. <br><br>Alternatively, Jupyter Notebook can be run from Anaconda Prompt. For the first time opening MSIGen:
+
+```
+conda activate MSIGen
+pip install notebook
+jupyter notebook
+```
+After the first run:
+```
+conda activate MSIGen
+jupyter notebook
+```
+
+### For Command Line Interface Tool:
+Download "MSIGen_CLI.py" from the tests folder in the Github repository. Create a configuration file for your experiment. An example can be found in the tests folder. Run the following in Anaconda Prompt:
+```
+conda activate MSIGen
+python "C:/Path/to/MSIGen_CLI.py" "C:/path/to/config_file1.json" "C:/path/to/config_file2.json"
+```
+Supply one configuration file for each dataset to be processed.
+
+# Referencing
+If MSIGen was used in your project, please reference it using the following:<br>
+[1.] Hernly E, Hu H, Laskin J. MSIGen: An Open-Source Python Package for Processing and Visualizing Mass Spectrometry Imaging Data. ChemRxiv. 2024; doi:10.26434/chemrxiv-2024-brc8d This content is a preprint and has not been peer-reviewed.
+
+
```

### Comparing `msigen-0.1.0/PKG-INFO` & `msigen-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: msigen
-Version: 0.1.0
+Version: 0.2.1
 Summary: A package for converting spectrometry imaging line scan data files to a visualizable format
-Home-page: https://github.com/EmersonHernly/MSIGen
+Home-page: https://github.com/LabLaskin/MSIGen
 License: MIT
 Author: Emerson Hernly
 Author-email: elhernly@gmail.com
 Requires-Python: >=3.9.0,<3.12
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -25,44 +25,60 @@
 Requires-Dist: opentimspy (==1.0.15)
 Requires-Dist: pandas (>=2.0.0)
 Requires-Dist: pymzml (>=2.5.2,<2.5.7)
 Requires-Dist: pywin32 (==306)
 Requires-Dist: scikit-image (>=0.19.0)
 Requires-Dist: scipy (>=1.10.1)
 Requires-Dist: tqdm (>=4.65.0)
+Project-URL: Homepage, https://github.com/EmersonHernly/MSIGen
 Project-URL: Issues, https://github.com/EmersonHernly/MSIGen/issues
-Project-URL: Repository, https://github.com/EmersonHernly/MSIGen
+Project-URL: Repository, https://github.com/LabLaskin/MSIGen
 Description-Content-Type: text/markdown
 
 # MSIGen
 MSIGen is designed for converting mass spectrometry imaging (MSI) data from the raw line-scan data to a visualizable format and is designed with nano-DESI MSI in mind. It has premade files for converting to images using a GUI, jupyter notebook, or from the command line.
 
 ## Installation on Windows
-Using Anaconda (https://www.anaconda.com/download), create a new environment titled "MSIGen" with python >=3.8 and activate it. Then, MSIGen can be installed using the pip package manager.
+Using Anaconda (https://www.anaconda.com/download), create a new environment titled "MSIGen" with python >=3.9 and <3.12 and activate it. Then, MSIGen can be installed using the pip package manager.
 
-Run the following in anaconda prompt:
+Run the following in Anaconda Prompt one line at a time:
 ```
-conda create --name MSIGen python=3.9
+conda create --name MSIGen python=3.11 -y
 conda activate MSIGen
 pip install MSIGen
 ```
 ### For GUI tool:
-Download "make GUI shortcut.py" from the tests folder in the Github repository. Run this code from Anaconda prompt.
+Download "make GUI shortcut.py" from the tests folder in the Github repository. Run this code from Anaconda Prompt.
 ```
 conda activate MSIGen
 python "C:/path/to/make GUI shortcut.py"
 ```
 After running with the actual location of "make GUI shortcut.py", there should be a shortcut called "MSIGen GUI" on your desktop. This runs the GUI for MSIGen.
 
 ### For Jupyter Notebook Tool:
-Download "MSIGen_jupyter.ipynb" from the tests folder in the Github repository. Open Anaconda and run Jupyter Notebook in the MSIGen environment. Open "MSIGen_jupyter.ipynb" from Jupyter Notebook.
+Download "MSIGen_jupyter.ipynb" from the tests folder in the Github repository. Open Anaconda Navigator and run Jupyter Notebook in the MSIGen environment. Open "MSIGen_jupyter.ipynb" from Jupyter Notebook. <br><br>Alternatively, Jupyter Notebook can be run from Anaconda Prompt. For the first time opening MSIGen:
+
+```
+conda activate MSIGen
+pip install notebook
+jupyter notebook
+```
+After the first run:
+```
+conda activate MSIGen
+jupyter notebook
+```
 
 ### For Command Line Interface Tool:
 Download "MSIGen_CLI.py" from the tests folder in the Github repository. Create a configuration file for your experiment. An example can be found in the tests folder. Run the following in Anaconda Prompt:
 ```
 conda activate MSIGen
 python "C:/Path/to/MSIGen_CLI.py" "C:/path/to/config_file1.json" "C:/path/to/config_file2.json"
 ```
 Supply one configuration file for each dataset to be processed.
 
+# Referencing
+If MSIGen was used in your project, please reference it using the following:<br>
+[1.] Hernly E, Hu H, Laskin J. MSIGen: An Open-Source Python Package for Processing and Visualizing Mass Spectrometry Imaging Data. ChemRxiv. 2024; doi:10.26434/chemrxiv-2024-brc8d This content is a preprint and has not been peer-reviewed.
+
```

