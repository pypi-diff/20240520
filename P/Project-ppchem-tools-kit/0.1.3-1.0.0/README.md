# Comparing `tmp/project_ppchem_tools_kit-0.1.3.tar.gz` & `tmp/project_ppchem_tools_kit-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project_ppchem_tools_kit-0.1.3.tar", max compression
+gzip compressed data, was "project_ppchem_tools_kit-1.0.0.tar", max compression
```

## Comparing `project_ppchem_tools_kit-0.1.3.tar` & `project_ppchem_tools_kit-1.0.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1096 2024-05-17 13:18:42.194501 project_ppchem_tools_kit-0.1.3/LICENSE
--rw-r--r--   0        0        0     8430 2024-05-19 10:20:46.232370 project_ppchem_tools_kit-0.1.3/README.md
--rw-r--r--   0        0        0      669 2024-05-19 10:23:18.372980 project_ppchem_tools_kit-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-16 20:44:57.565187 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/__init__.py
--rw-r--r--   0        0        0      566 2024-05-18 16:20:56.501812 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/add_data_point.py
--rw-r--r--   0        0        0      376 2024-05-19 09:11:37.994019 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/bind_enter.py
--rw-r--r--   0        0        0      672 2024-05-18 17:45:23.130803 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/browse_excel_file.py
--rw-r--r--   0        0        0      164 2024-05-18 17:45:23.131373 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/clear_input.py
--rw-r--r--   0        0        0      504 2024-05-19 07:44:17.259322 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/copy_text.py
--rw-r--r--   0        0        0      979 2024-05-19 09:11:37.994184 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/create_radio_button.py
--rw-r--r--   0        0        0     2704 2024-05-19 09:11:37.993513 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/display_graph.py
--rw-r--r--   0        0        0     2147 2024-05-18 16:20:56.504673 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/display_max_point_and_coords.py
--rw-r--r--   0        0        0     1574 2024-05-17 12:06:36.279430 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/display_molecule.py
--rw-r--r--   0        0        0      581 2024-05-18 16:20:56.505034 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/display_result.py
--rw-r--r--   0        0        0     6226 2024-05-19 07:58:29.644129 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/error_calculation_interface.py
--rw-r--r--   0        0        0     9287 2024-05-18 13:16:11.687288 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/graph_function.py
--rw-r--r--   0        0        0     1646 2024-05-19 09:11:38.148414 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/linear_regression.py
--rw-r--r--   0        0        0     1064 2024-05-19 09:11:38.148314 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/make_graph.py
--rw-r--r--   0        0        0      371 2024-05-16 10:14:47.990043 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/name_to_smiles.py
--rw-r--r--   0        0        0      226 2024-05-18 17:45:23.132897 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/on_closing.py
--rw-r--r--   0        0        0      358 2024-05-19 09:11:37.994342 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/on_radio_select.py
--rw-r--r--   0        0        0     1784 2024-05-19 09:11:37.993793 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/open_graph_settings_window.py
--rw-r--r--   0        0        0     2504 2024-05-19 09:11:37.993466 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/process_input.py
--rw-r--r--   0        0        0      212 2024-05-19 08:19:40.701466 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/relative_to_assets.py
--rw-r--r--   0        0        0      147 2024-05-18 16:20:56.506233 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/select_all.py
--rw-r--r--   0        0        0      391 2024-05-18 16:20:56.506577 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/set_axes_color.py
--rw-r--r--   0        0        0      526 2024-05-18 16:20:56.506862 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/set_background_color.py
--rw-r--r--   0        0        0      619 2024-05-18 16:20:56.507221 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/set_custom_labels_and_title.py
--rw-r--r--   0        0        0      184 2024-05-18 16:20:56.507696 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/set_grid_color.py
--rw-r--r--   0        0        0      270 2024-05-18 16:20:56.508228 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/set_label_color.py
--rw-r--r--   0        0        0      432 2024-05-18 16:20:56.508577 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/set_line_color.py
--rw-r--r--   0        0        0      492 2024-05-18 16:20:56.508962 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/set_scale.py
--rw-r--r--   0        0        0      231 2024-05-16 10:14:47.987920 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/smiles_to_molar_mass.py
--rw-r--r--   0        0        0      124 2024-05-18 16:20:56.509235 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/toggle_grid.py
--rw-r--r--   0        0        0      573 2024-05-18 17:45:23.133845 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/update_clock.py
--rw-r--r--   0        0        0      908 2024-05-19 08:54:54.692946 project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/welcome_message.py
--rw-r--r--   0        0        0     9403 1970-01-01 00:00:00.000000 project_ppchem_tools_kit-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-05-17 13:18:42.194501 project_ppchem_tools_kit-1.0.0/LICENSE
+-rw-r--r--   0        0        0     9620 2024-05-20 14:19:51.999970 project_ppchem_tools_kit-1.0.0/README.md
+-rw-r--r--   0        0        0     1119 2024-05-20 15:24:49.364904 project_ppchem_tools_kit-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-16 20:44:57.565187 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/__init__.py
+-rw-r--r--   0        0        0      537 2024-05-20 14:52:11.199976 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/add_data_point.py
+-rw-r--r--   0        0        0      439 2024-05-20 14:52:11.201062 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/bind_enter.py
+-rw-r--r--   0        0        0      672 2024-05-20 12:02:51.196051 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/browse_excel_file.py
+-rw-r--r--   0        0        0      164 2024-05-18 17:45:23.131373 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/clear_input.py
+-rw-r--r--   0        0        0      528 2024-05-20 14:52:11.201388 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/copy_text.py
+-rw-r--r--   0        0        0      979 2024-05-20 12:23:16.912190 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/create_radio_button.py
+-rw-r--r--   0        0        0     3300 2024-05-20 14:52:11.202010 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/display_graph.py
+-rw-r--r--   0        0        0     2646 2024-05-20 14:52:11.202368 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/display_max_point_and_coords.py
+-rw-r--r--   0        0        0     1229 2024-05-20 14:52:11.203373 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/display_molecule.py
+-rw-r--r--   0        0        0      581 2024-05-18 16:20:56.505034 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/display_result.py
+-rw-r--r--   0        0        0     8474 2024-05-20 14:52:11.203706 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/error_calculation_interface.py
+-rw-r--r--   0        0        0    11926 2024-05-20 14:52:11.204368 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/graph_function.py
+-rw-r--r--   0        0        0     2251 2024-05-20 14:52:11.205130 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/linear_regression.py
+-rw-r--r--   0        0        0     1555 2024-05-20 14:52:11.206095 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/make_graph.py
+-rw-r--r--   0        0        0      710 2024-05-20 14:52:11.206377 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/name_to_smiles.py
+-rw-r--r--   0        0        0      568 2024-05-20 14:52:11.207080 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/on_closing.py
+-rw-r--r--   0        0        0      358 2024-05-19 09:11:37.994342 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/on_radio_select.py
+-rw-r--r--   0        0        0     1893 2024-05-20 14:52:11.207375 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/open_graph_settings_window.py
+-rw-r--r--   0        0        0     2291 2024-05-20 14:52:11.207905 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/process_input.py
+-rw-r--r--   0        0        0      462 2024-05-20 14:52:11.208858 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/relative_to_assets.py
+-rw-r--r--   0        0        0      364 2024-05-20 14:52:11.209157 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/select_all.py
+-rw-r--r--   0        0        0      564 2024-05-20 14:52:11.209435 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/set_axes_color.py
+-rw-r--r--   0        0        0      701 2024-05-20 14:52:11.209690 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/set_background_color.py
+-rw-r--r--   0        0        0      840 2024-05-20 14:52:11.210035 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/set_custom_labels_and_title.py
+-rw-r--r--   0        0        0      401 2024-05-20 14:52:11.210482 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/set_grid_color.py
+-rw-r--r--   0        0        0      493 2024-05-20 14:52:11.211071 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/set_label_color.py
+-rw-r--r--   0        0        0      590 2024-05-20 14:52:11.211500 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/set_line_color.py
+-rw-r--r--   0        0        0      706 2024-05-20 14:52:11.211802 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/set_scale.py
+-rw-r--r--   0        0        0      515 2024-05-20 14:52:11.212405 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/smiles_to_molar_mass.py
+-rw-r--r--   0        0        0      308 2024-05-20 14:52:11.212717 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/toggle_grid.py
+-rw-r--r--   0        0        0      654 2024-05-20 14:52:11.213814 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/update_clock.py
+-rw-r--r--   0        0        0      987 2024-05-20 14:52:11.214223 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/welcome_message.py
+-rw-r--r--   0        0        0    10969 1970-01-01 00:00:00.000000 project_ppchem_tools_kit-1.0.0/PKG-INFO
```

### Comparing `project_ppchem_tools_kit-0.1.3/LICENSE` & `project_ppchem_tools_kit-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.3/README.md` & `project_ppchem_tools_kit-1.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 
 <p align="center">
    <img width="1245" alt="logo_project" src="https://github.com/sgrunber/Project-ppchem-tools-kit/raw/main/docs/source/_static/images/logo_project.png">
+   
+
 
  </p>
 
 
 
 
  <h1 align="center">🧰 Tools Kit</h1>
@@ -45,15 +47,15 @@
 
 ```bash
 git clone https://github.com/sgrunber/Project-ppchem-tools-kit.git
 ```
 
 ### 3. ⬇️ Install with pip
 
-  <a href="https://pypi.org/project/Project-ppchem-tools-kit/"><img src="https://img.shields.io/badge/PyPI-v1.0.0-blue.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="PyPI"></a>
+  <a href="https://pypi.org/project/Project-ppchem-tools-kit/"><img src="https://img.shields.io/badge/PyPI-v0.1.3-blue.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="PyPI"></a>
 
 You can also install Tools Kit using pip:
 
 ```bash
 pip install Project_ppchem-tools-kit
 ```
 
@@ -178,23 +180,49 @@
 ```
 
 ### Chicago Style
 
 <a href="https://www.chicagomanualofstyle.org/home.html"><img src="https://img.shields.io/badge/Chicago%20Style-17th%20Ed.-5579A1.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="Chicago Style"></a>
 
 ```bash
-Enzinger, Méloé, and Sébastien Grunberg. 2024. Project-ppchem-tools-kit. Computer software. GitHub. https://github.com/username/Project-ppchem-tools-kit.` 
+Méloé Enzinger and Sébastien Grunberg. 2024. Project-ppchem-tools-kit. Computer software. GitHub. https://github.com/username/Project-ppchem-tools-kit.` 
 ```
 ## 📜 License
 
 <a href="https://github.com/sgrunber/Project-ppchem-tools-kit/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="License"></a>
 
 <a id="license"></a>
 
 This project is licensed under the MIT License. See the LICENSE file for details.
 
 ## 📸 Screenshots
 <a id="screenshots"></a>
-<img width="1002" alt="Capture d’écran 2024-05-18 à 16 44 09" src="https://github.com/sgrunber/Project-ppchem-tools-kit/raw/main/docs/source/_static/images/screen.png">
 
+**Note**: Graphs have much better quality when saved to your computer.
+
+## Interface
+<p align="center">
+<img width="700" alt="Capture d’écran 2024-05-18 à 16 44 09" src="https://github.com/sgrunber/Project-ppchem-tools-kit/raw/main/docs/source/_static/images/screen.png">
+   </p>
+   
+## Graph
+<p align="center">
+<img width="700" alt="graph" src="https://github.com/sgrunber/Project-ppchem-tools-kit/assets/160881864/8d1f8352-3815-4d5d-9545-0a7138f132a5">
+    </p>
+    
+## Linear Regression
+<p align="center">
+<img width="700" alt="linear_reg" src="https://github.com/sgrunber/Project-ppchem-tools-kit/assets/160881864/eb1a56fb-d801-457b-9a1d-56fc258a6478">
+ </p>
 
+## Graph & Linear Regression Settings
+<p align="center">
+<img width="220" alt="scale" src="https://github.com/sgrunber/Project-ppchem-tools-kit/assets/160881864/8bf14d9a-a573-43fd-bfce-721dccda3415">
+<img width="178" alt="graph_option" src="https://github.com/sgrunber/Project-ppchem-tools-kit/assets/160881864/2d08b793-6903-418b-a83d-ae3d24d36171">
+<img width="220" alt="Label" src="https://github.com/sgrunber/Project-ppchem-tools-kit/assets/160881864/ad9da31f-5d76-495b-8f81-b3324c2944a6">
+ </p>
+
+## Show Molecule
+<p align="center">
+<img width="398" alt="show_molecule" src="https://github.com/sgrunber/Project-ppchem-tools-kit/assets/160881864/691fda4c-1f1d-4aa3-90ef-88cf759a4f70">
+ </p>
```

#### html2text {}

```diff
@@ -66,12 +66,22 @@
 for your contribution! Your efforts help improve the project for everyone. ##
 ð Cite Us If you use Tools Kit in your research work or academic projects,
 we would appreciate it if you could cite us. You can use the following BibTeX
 entry: _[_B_i_b_T_e_X_]```bibtex @misc{project-ppchem-tools-kit, title = {Project-
 ppchem-tools-kit}, author = {{MÃ©loÃ© Enzinger & SÃ©bastien Grunberg}}, year =
 {2024}, publisher = {GitHub}, journal = {GitHub Repository}, howpublished =
 {\url{https://github.com/username/Project-ppchem-tools-kit}} } ``` ### Chicago
-Style _[_C_h_i_c_a_g_o_ _S_t_y_l_e_]```bash Enzinger, MÃ©loÃ©, and SÃ©bastien Grunberg. 2024.
+Style _[_C_h_i_c_a_g_o_ _S_t_y_l_e_]```bash MÃ©loÃ© Enzinger and SÃ©bastien Grunberg. 2024.
 Project-ppchem-tools-kit. Computer software. GitHub. https://github.com/
 username/Project-ppchem-tools-kit.` ``` ## ð License _[_L_i_c_e_n_s_e_]This project
 is licensed under the MIT License. See the LICENSE file for details. ## ð¸
-Screenshots[Capture dâÃ©cran 2024-05-18 Ã  16 44 09]
+Screenshots **Note**: Graphs have much better quality when saved to your
+computer. ## Interface
+                  [Capture dâÃ©cran 2024-05-18 Ã  16 44 09]
+## Graph
+                                    [graph]
+## Linear Regression
+                                 [linear_reg]
+## Graph & Linear Regression Settings
+                         [scale][graph_option][Label]
+## Show Molecule
+                                [show_molecule]
```

### Comparing `project_ppchem_tools_kit-0.1.3/pyproject.toml` & `project_ppchem_tools_kit-1.0.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 [tool.poetry]
 name = "Project-ppchem-tools-kit"
-version = "0.1.3"
+version = "1.0.0"
 description = "Basic Chemistry Toolkit"
 authors = ["Méloé Enzinger <meloe.enzinger@epfl.ch> and Sébastien Grunberg <sebastien.grunberg@epfl.ch>"]
 license = "MIT"
 readme = "README.md"
+keywords = [
+    "Chemistry",
+    "Tools kit",
+    "Graph maker",
+    "Linear regression",
+    "Molecular structure",
+    "Molecular mass",
+    "Uncertainty propagation",
+    "standard deviation",
+    "tkinter interface",
+    "LaTeX",
+    "SMILES"
+    ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 scikit-learn = "1.3.0"
 numpy5 = "^0.1"
 numpy = "^1.26.4"
 pillow = "10.2.0"
@@ -23,7 +36,12 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.urls]
+Homepage = "https://github.com/sgrunber/Project-ppchem-tools-kit"
+Github_Sebastien_Grunberg = "https://github.com/sgrunber"
+Github_Meloe_Enzinger = "https://github.com/melozgr"
```

### Comparing `project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/browse_excel_file.py` & `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/browse_excel_file.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/create_radio_button.py` & `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/create_radio_button.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/display_graph.py` & `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/display_graph.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 from project_ppchem_tools_kit.toggle_grid import toggle_grid
 from project_ppchem_tools_kit.display_max_point_and_coords import display_max_point_and_coords
 from project_ppchem_tools_kit.open_graph_settings_window import open_graph_settings_window
 
 graph_window = None
 
 def display_graph(fig):
+    """Displays the graph in a new window with options to customize it.
+
+    Args:
+        fig (matplotlib.figure.Figure): The Figure object containing the plot.
+    """
     global graph_window
     if graph_window:
         graph_window.destroy()
 
     graph_window = tk.Toplevel()
     graph_window.title("Graph")
     graph_window.geometry("1000x600")
@@ -52,14 +57,27 @@
     display_max_button.pack(side=tk.LEFT, padx=5)
 
     graph_settings_button = tk.Button(graph_window, text="Graph Settings", command=lambda: open_graph_settings_window(fig, plot_canvas))
     graph_settings_button.pack(side=tk.LEFT, padx=5, pady=5)
     
     
     def on_closing_graph():
+        """Handle the closing event for the graph window.
+
+        This function is triggered when the user attempts to close the graph window.
+        It prompts the user with a confirmation dialog to ensure they want to quit.
+        If the user confirms (clicks 'OK'), the graph window is hidden and the 
+        main event loop is terminated.
+
+        Args:
+            None
+
+        Returns:
+            None
+        """
         if messagebox.askokcancel("Quit", "Are you sure you want to quit?"):
             graph_window.withdraw()  # Hide the window
             graph_window.quit()  # Quit the main loop
 
             
     graph_window.protocol("WM_DELETE_WINDOW", on_closing_graph)
     graph_window.mainloop()
```

### Comparing `project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/display_max_point_and_coords.py` & `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/display_max_point_and_coords.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,77 @@
 import numpy as np
 from tkinter import messagebox, colorchooser
 
 
 def display_max_point_and_coords(ax, plot_canvas):
+    """Performs a linear regression from an Excel file and plots the graph and R^2 value.
+
+    Args:
+        file_path (str): Path to the Excel file containing the data.
+        x_label (str): x-axis label.
+        y_label (str): y-axis label.
+        title (str): Title of the graph.
+        grid (bool): Whether to display grid lines on the plot. Defaults to True.
+        save_as (str, optional): File path to save the graph. Defaults to None, in which case it is not saved.
+        line_style (str, optional): Style of the line plot. Defaults to '-'.
+        line_color (str, optional): Color of the plot line. Defaults to 'k' (black).
+
+    Raises:
+        FileNotFoundError: If the specified file_path does not exist.
+    """
     def display_max_point(color):
-        # Trouver l'indice du maximum de la courbe
+        """Displays the maximum point on the plot with its coordinates.
+
+        Args:
+            color (str): Color of the marker and text.
+
+        Raises:
+            None
+        """
         max_index = np.argmax(ax.lines[0].get_ydata())
         
-        # Récupérer les coordonnées du maximum
         max_x = ax.lines[0].get_xdata()[max_index]
         max_y = ax.lines[0].get_ydata()[max_index]
 
-        # Déterminer la position relative du maximum par rapport aux axes
+
         x_lim = ax.get_xlim()
         y_lim = ax.get_ylim()
         
         if x_lim[0] < max_x < x_lim[1] and y_lim[0] < max_y < y_lim[1]:
-            # Déterminer la position relative du point sur les axes
             x_rel = (max_x - x_lim[0]) / (x_lim[1] - x_lim[0])
             y_rel = (max_y - y_lim[0]) / (y_lim[1] - y_lim[0])
             
-            # Calculer les décalages en fonction de la position relative
             dx = 0.03 * (x_lim[1] - x_lim[0])
             dy = 0.03 * (y_lim[1] - y_lim[0])
             
-            # Si le point est proche du bord droit, décaler à gauche
             if x_rel > 0.95:
                 ha = 'right'
                 dx = -dx
             else:
                 ha = 'left'
                 
-            # Si le point est proche du bord supérieur, décaler vers le bas
             if y_rel > 0.95:
                 va = 'top'
                 dy = -dy
             else:
                 va = 'bottom'
                 
-            # Afficher les coordonnées dans le graphique avec une seule décimale
             ax.scatter(max_x, max_y, color=color, zorder=10)
             ax.text(max_x + dx, max_y + dy, f'({max_x:.1f}, {max_y:.1f})', fontsize=14, fontweight='bold', ha=ha, va=va, color=color, bbox=dict(facecolor='white', edgecolor=color, boxstyle='round,pad=0.3'))
             plot_canvas.draw_idle()
         else:
             messagebox.showwarning("Warning", "Max point coordinates are out of range.")
 
     def choose_color():
-        color = colorchooser.askcolor(color='red')[1]  # Choisissez la couleur par défaut ici
+        """Opens a color chooser dialog and calls display_max_point with the chosen color.
+
+        Args:
+            None
+
+        Raises:
+            None
+        """
+        color = colorchooser.askcolor(color='red')[1]  
         if color:
             display_max_point(color)
 
     choose_color()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/display_molecule.py` & `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/display_molecule.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,40 +3,39 @@
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg, NavigationToolbar2Tk
 import tkinter as tk
 
 
 
 def display_molecule(entry_input):
-    
-    smiles = entry_input.get().strip()  # Obtenir la chaîne SMILES à partir de l'entrée utilisateur
-    mol = Chem.MolFromSmiles(smiles)  # Générer la structure moléculaire à partir de la chaîne SMILES
+    """Displays the 2D structure of a molecule from a given SMILES string.
+
+    Args:
+        entry_input (tk.Entry): The entry widget containing the SMILES string.
+    """
+    smiles = entry_input.get().strip()  
+    mol = Chem.MolFromSmiles(smiles)  
 
     if mol is not None:
-        # Fonction pour afficher la molécule en 2D
         def show_molecule_2d():
             img = Draw.MolToImage(mol)
 
-            # Créer une nouvelle fenêtre Tkinter pour afficher la structure moléculaire en 2D
             mol_window = tk.Toplevel()
             mol_window.title("Molecular Structure")
 
-            # Convertir l'image en format Tkinter PhotoImage
             pimg = FigureCanvasTkAgg(plt.Figure(figsize=(4, 3)), master=mol_window)
             ax = pimg.figure.add_subplot(111)
             ax.imshow(img, interpolation='bilinear')
             ax.axis('off')
 
-            # Créer un canevas Tkinter pour afficher l'image
             canvas = pimg.get_tk_widget()
             canvas.pack()
 
-            # Ajouter la barre d'outils de navigation
-            toolbar = NavigationToolbar2Tk(pimg, mol_window)  # Passer la figure à la barre d'outils
+            toolbar = NavigationToolbar2Tk(pimg, mol_window)  
             toolbar.update()
             toolbar.pack()
 
             mol_window.mainloop()
 
         show_molecule_2d()
     else:
-        print("Erreur : Impossible de générer une structure moléculaire à partir du SMILES fourni.")
+        print("Error : Can not generate a molecular structure from the input SMILES.")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/display_result.py` & `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/display_result.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/error_calculation_interface.py` & `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/error_calculation_interface.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,83 @@
-# Chem_pack/error_calculation.py
 import tkinter as tk
 import pyperclip
 
 def calculate_error_propagation(derivatives, uncertainties):
+    """
+    Calculate the propagation of error using given derivatives and uncertainties.
+
+    This function computes the standard deviation and the average value based on
+    the derivatives and uncertainties provided. It follows the formula for error
+    propagation in a system where each variable contributes to the overall uncertainty.
+
+    Args:
+        derivatives (list of float): The derivatives with respect to each variable.
+        uncertainties (list of float): The uncertainties associated with each variable.
+
+    Returns:
+        tuple: A tuple containing the standard deviation (float) and the average value (float).
+    """
     average_values = sum(derivatives) / len(derivatives)
     error = sum((unc / deriv) ** 2 for deriv, unc in zip(derivatives, uncertainties))
     standard_dev = (error ** 0.5) * average_values
     return standard_dev, average_values
 
 def error_calculation_interface():
+    """
+    Provide a graphical interface for error calculation and LaTeX code generation.
+
+    This function sets up a Tkinter window where users can input variable names,
+    values, and uncertainties. It calculates the propagation of uncertainty and 
+    displays the result. It also generates LaTeX code for the calculated values, 
+    which can be copied to the clipboard.
+
+    The interface includes:
+        - Adding and removing variable entries.
+        - Calculating and displaying the propagation of uncertainty.
+        - Generating and copying LaTeX code for the results.
+
+    Inner Functions:
+        copy_latex_code(latex_code): Copy generated LaTeX code to the clipboard.
+        calculate_and_display(): Calculate propagation of uncertainty and display results.
+        add_variable_entry(): Add a new row of input fields for a variable.
+        remove_variable_entry(row): Remove a specific row of input fields.
+    """
     def copy_latex_code(latex_code):
+        """
+        Copy the generated LaTeX code to the clipboard.
+
+        Args:
+            latex_code (str): The LaTeX code to be copied.
+        """
         pyperclip.copy(latex_code)
         result_window.clipboard_clear()
         result_window.clipboard_append(latex_code)
         result_window.update()
 
     def calculate_and_display():
+        """
+        Calculate the propagation of uncertainty and display the results.
+
+        This function retrieves data from the input fields, calculates the error 
+        propagation and average value, and displays the results in a new window. 
+        It also generates the corresponding LaTeX code for the calculations.
+        """
         data = []
         values = []
         uncertainties = []
         for i in range(len(entries)):
             var_name = entry_vars[i].get()
             var_value = float(entry_values[i].get())
             var_uncertainty = float(entry_uncertainties[i].get())
             data.append((var_name, var_value, var_uncertainty))
             values.append(var_value)
             uncertainties.append(var_uncertainty)
 
-        # Calculate the propagation of uncertainty
         error, average = calculate_error_propagation(values, uncertainties)
 
-        # Display the result with calculation details
         result_text = f"Propagation of Uncertainty (∆z): {error:.6f}\n"
         result_text += f"Average Value: {average:.6f}\n\n"
         result_text += "Calculation Details:\n"
         for var_name, var_value, var_uncertainty in data:
             result_text += f"{var_name}: Value: {var_value}, Uncertainty: {var_uncertainty}\n"
 
         latex_code = r"""
@@ -84,15 +127,20 @@
         result_textbox.grid(row=0, column=0, padx=5, pady=5)
 
         # Button to copy LaTeX code to clipboard
         copy_button = tk.Button(result_window, text="Copy LaTeX Code", command=lambda: copy_latex_code(latex_code))
         copy_button.grid(row=1, column=0, padx=5, pady=5)
 
     def add_variable_entry():
-        # Ajouter des champs d'entrée pour une nouvelle variable
+        """
+        Add a new row of input fields for a variable.
+
+        This function dynamically adds input fields for a new variable's name, 
+        value, and uncertainty to the interface.
+        """
         row = len(entries) + 1
 
         var_name_label = tk.Label(error_calc_window, text="Variable Name", bg="#1B262C", fg="white")
         var_name_label.grid(row=row, column=0, padx=5, pady=5)
         var_name_entry = tk.Entry(error_calc_window)
         var_name_entry.grid(row=row, column=1, padx=5, pady=5)
         entry_vars.append(var_name_entry)
@@ -116,36 +164,43 @@
 
         remove_variable_button = tk.Button(error_calc_window, text="Remove", command=lambda r=row: remove_variable_entry(r),
                                             bg="#FF0000", fg="#1B262C")
         remove_variable_button.grid(row=row, column=6, padx=5, pady=5)
         remove_buttons.append(remove_variable_button)
 
     def remove_variable_entry(row):
+        """
+        Remove a specific row of input fields.
+
+        This function removes the input fields for a variable specified by the row number.
+
+        Args:
+            row (int): The row number of the variable to be removed.
+        """
         entry = entries.pop(row - 1)
         for widget in entry:
             widget.destroy()
         for label in labels[(row - 1) * 3:(row - 1) * 3 + 3]:
             label.destroy()
         remove_buttons.pop(row - 1).destroy()
 
     error_calc_window = tk.Tk()
-    error_calc_window.title("Calcul d'erreur")
+    error_calc_window.title("Error calculation")
     error_calc_window.configure(bg="#1B262C")
 
-    add_variable_button = tk.Button(error_calc_window, text="Ajouter une variable", command=add_variable_entry, height=2,
+    add_variable_button = tk.Button(error_calc_window, text="Add a variable", command=add_variable_entry, height=2,
                                     bg="#0000FF", fg="#1B262C", font=("Times New Roman", 15))
     add_variable_button.grid(row=0, column=2, columnspan=3, padx=5, pady=5, sticky="")
 
-    # Pour le bouton "Calculer la propagation d'erreur"
-    calculate_error_button = tk.Button(error_calc_window, text="Calculer la propagation d'erreur",
+    calculate_error_button = tk.Button(error_calc_window, text="Calcule the error propagation",
                                         command=calculate_and_display, height=2, bg="#008000", fg="#1B262C",
                                         font=("Times New Roman", 15))
     calculate_error_button.grid(row=20, column=2, columnspan=3, padx=5, pady=5, sticky="")
 
-    # Listes pour stocker les widgets d'entrée
+    # List to stock input widgets
     entries = []
     entry_vars = []
     entry_values = []
     entry_uncertainties = []
     remove_buttons = []
     labels = []
```

### Comparing `project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/graph_function.py` & `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/graph_function.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,140 +1,209 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import tkinter as tk
 from tkinter import messagebox
 from tkinter import simpledialog, colorchooser
-from matplotlib.backends.backend_agg import FigureCanvasAgg as FigureCanvas
-from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg, NavigationToolbar2Tk, FigureCanvasTk
-from matplotlib.figure import Figure
+from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg, NavigationToolbar2Tk
 
+#NOTE : In order for the code to run, graph_function.py englobes the following functions :
+#   display_max_point_and_coords, 
+#   add_data_point, 
+#   set_line_color, 
+#   set_axes_color, 
+#   set_grud_color, 
+#   set_label_color, 
+#   set_background_color, 
+#   open_graph_settings_window, 
+#   toggle_grid, 
+#   set_scale, 
+#   set_custom_labels_and_title, 
+#   display_graph, 
+#   on_closing_graph
+# as well as the nested functions. However, in order to test each of the functions listed hereabove, separate _.py files were created for each main function.
 
 graph_window = None 
 
 def display_max_point_and_coords(ax, plot_canvas):
+    """Performs a linear regression from an Excel file and plots the graph and R^2 value.
+
+    Args:
+        file_path (str): Path to the Excel file containing the data.
+        x_label (str): x-axis label.
+        y_label (str): y-axis label.
+        title (str): Title of the graph.
+        grid (bool): Whether to display grid lines on the plot. Defaults to True.
+        save_as (str, optional): File path to save the graph. Defaults to None, in which case it is not saved.
+        line_style (str, optional): Style of the line plot. Defaults to '-'.
+        line_color (str, optional): Color of the plot line. Defaults to 'k' (black).
+
+    Raises:
+        FileNotFoundError: If the specified file_path does not exist.
+    """
     def display_max_point(color):
-        # Trouver l'indice du maximum de la courbe
+        """Displays the maximum point on the plot with its coordinates.
+
+        Args:
+            color (str): Color of the marker and text.
+
+        Raises:
+            None
+        """
         max_index = np.argmax(ax.lines[0].get_ydata())
         
-        # Récupérer les coordonnées du maximum
         max_x = ax.lines[0].get_xdata()[max_index]
         max_y = ax.lines[0].get_ydata()[max_index]
 
-        # Déterminer la position relative du maximum par rapport aux axes
         x_lim = ax.get_xlim()
         y_lim = ax.get_ylim()
         
         if x_lim[0] < max_x < x_lim[1] and y_lim[0] < max_y < y_lim[1]:
-            # Déterminer la position relative du point sur les axes
             x_rel = (max_x - x_lim[0]) / (x_lim[1] - x_lim[0])
             y_rel = (max_y - y_lim[0]) / (y_lim[1] - y_lim[0])
             
-            # Calculer les décalages en fonction de la position relative
             dx = 0.01 * (x_lim[1] - x_lim[0])
             dy = 0.05 * (y_lim[1] - y_lim[0])
             
-            # Si le point est proche du bord droit, décaler à gauche
             if x_rel > 0.95:
                 ha = 'right'
                 dx = -dx
             else:
                 ha = 'left'
                 
-            # Si le point est proche du bord supérieur, décaler vers le bas
             if y_rel > 0.95:
                 va = 'top'
                 dy = -dy
             else:
                 va = 'bottom'
                 
-            # Afficher les coordonnées dans le graphique avec une seule décimale
             ax.scatter(max_x, max_y, color=color, zorder=10)
             ax.text(max_x + dx, max_y + dy, f'({max_x:.1f}, {max_y:.1f})', fontsize=14, fontweight='bold', ha=ha, va=va, color=color, bbox=dict(facecolor='white', edgecolor=color, boxstyle='round,pad=0.3'))
             plot_canvas.draw_idle()
         else:
             messagebox.showwarning("Warning", "Max point coordinates are out of range.")
 
     def choose_color():
-        color = colorchooser.askcolor(color='red')[1]  # Choisissez la couleur par défaut ici
+        """Opens a color chooser dialog and calls display_max_point with the chosen color.
+
+        Args:
+            None
+
+        Raises:
+            None
+        """
+        color = colorchooser.askcolor(color='red')[1] 
         if color:
             display_max_point(color)
 
     choose_color()
     
 def add_data_point(ax, plot_canvas):
-    # Demander à l'utilisateur de choisir une couleur
+    """Adds data points to the graph with a chosen color.
+
+    Args:
+        ax (matplotlib.axes.Axes): The Axes object containing the plot.
+        plot_canvas (FigureCanvasTkAgg): The canvas on which the plot is drawn.
+    """
     color = colorchooser.askcolor()[1]
     if color:
-        # Récupérer les données x et y du graphique
         x_data = ax.lines[0].get_xdata()
         y_data = ax.lines[0].get_ydata()
 
-        # Ajouter les points avec la couleur spécifiée à l'aide de ax.scatter
         
         ax.scatter(x_data, y_data, color=color, zorder=10) 
 
-        # Mettre à jour le canvas pour afficher les modifications
         plot_canvas.draw_idle()
 
 def set_line_color(ax, plot_canvas):
+    """Sets the line color and style for the plot.
+
+    Args:
+        ax (matplotlib.axes.Axes): The Axes object containing the plot.
+        plot_canvas (FigureCanvasTkAgg): The canvas on which the plot is drawn.
+    """    
     color = colorchooser.askcolor()[1]
     line_style = simpledialog.askstring("Line Style", "Enter line style ('-', '--', ':', '-.'):")
     if color and line_style:
-        ax.lines[0].set_color(color)  # Change seulement la couleur de la première ligne (la courbe)
+        ax.lines[0].set_color(color)
         ax.lines[0].set_linestyle(line_style)  
         plot_canvas.draw_idle()
 
 def set_axes_color(ax, plot_canvas):
+    """Sets the color of the axes and their tick marks.
+
+    Args:
+        ax (matplotlib.axes.Axes): The Axes object containing the plot.
+        plot_canvas (FigureCanvasTkAgg): The canvas on which the plot is drawn.
+    """
     color = colorchooser.askcolor()[1]
     if color:
         for spine in ax.spines.values():
             spine.set_color(color)
         
-        # Changer la couleur des valeurs sur les axes
         ax.tick_params(axis='x', colors=color)
         ax.tick_params(axis='y', colors=color)
 
         plot_canvas.draw_idle()
 
 
 def set_grid_color(ax, plot_canvas):
+    """Sets the grid line color for the plot.
+
+    Args:
+        ax (matplotlib.axes.Axes): The Axes object containing the plot.
+        plot_canvas (FigureCanvasTkAgg): The canvas on which the plot is drawn.
+    """    
     color = colorchooser.askcolor()[1]
     if color:
         ax.grid(color=color)
         plot_canvas.draw_idle()
 
 def set_label_color(ax, plot_canvas):
+    """Sets the color of the axis labels and title.
+
+    Args:
+        ax (matplotlib.axes.Axes): The Axes object containing the plot.
+        plot_canvas (FigureCanvasTkAgg): The canvas on which the plot is drawn.
+    """
     color = colorchooser.askcolor()[1]
     if color:
         ax.xaxis.label.set_color(color)
         ax.yaxis.label.set_color(color)
         ax.title.set_color(color)
         plot_canvas.draw_idle()
 
 def set_background_color(ax, plot_canvas):
+    """Sets the background color of the plot and canvas.
+
+    Args:
+        ax (matplotlib.axes.Axes): The Axes object containing the plot.
+        plot_canvas (FigureCanvasTkAgg): The canvas on which the plot is drawn.
+    """
     color = colorchooser.askcolor()[1]
     if color:
-        # Set the background color of the entire plot
         fig = ax.figure
         fig.set_facecolor(color)
 
-        # Set the background color of the canvas containing the plot
         plot_canvas.get_tk_widget().configure(bg=color)
         
-        # Set the background color of each axis
         for ax in fig.get_axes():
             ax.set_facecolor(color)
 
         plot_canvas.draw_idle()
     
 def open_graph_settings_window(fig, plot_canvas):
+    """Opens a new window with options to customize the graph settings.
+
+    Args:
+        fig (matplotlib.figure.Figure): The Figure object containing the plot.
+        plot_canvas (FigureCanvasTkAgg): The canvas on which the plot is drawn.
+    """
     graph_settings_window = tk.Toplevel()
     graph_settings_window.title("Graph Settings")
 
-    # Boutons pour les paramètres du graphique
     set_line_color_button = tk.Button(graph_settings_window, text="Set Line Color", command=lambda: set_line_color(fig.axes[0], plot_canvas))
     set_line_color_button.pack(side=tk.TOP, padx=5, pady=5)
 
     set_axes_color_button = tk.Button(graph_settings_window, text="Set Axis Color", command=lambda: set_axes_color(fig.axes[0], plot_canvas))
     set_axes_color_button.pack(side=tk.TOP, padx=5, pady=5)
 
     set_grid_color_button = tk.Button(graph_settings_window, text="Set grid", command=lambda: set_grid_color(fig.axes[0], plot_canvas))
@@ -142,47 +211,68 @@
 
     set_label_color_button = tk.Button(graph_settings_window, text="Set Label Color", command=lambda: set_label_color(fig.axes[0], plot_canvas))
     set_label_color_button.pack(side=tk.TOP, padx=5, pady=5)
 
     set_background_color_button = tk.Button(graph_settings_window, text="Set Background Color", command=lambda: set_background_color(fig.axes[0], plot_canvas))
     set_background_color_button.pack(side=tk.TOP, padx=5, pady=5)
 
-    # Bouton pour fermer la fenêtre des paramètres du graphique
     close_button = tk.Button(graph_settings_window, text="Close", command=graph_settings_window.destroy)
     close_button.pack(side=tk.BOTTOM, padx=5, pady=5)
 
 
 def toggle_grid(ax, plot_canvas):
-    # Set the grid lines visibility to True
+    """Toggles the visibility of grid lines on the plot.
+
+    Args:
+        ax (matplotlib.axes.Axes): The Axes object containing the plot.
+        plot_canvas (FigureCanvasTkAgg): The canvas on which the plot is drawn.
+    """
     ax.grid(True)
     plot_canvas.draw_idle()
 
 def set_scale(ax, plot_canvas):
+    """Sets the scale of the x and y axes.
+
+    Args:
+        ax (matplotlib.axes.Axes): The Axes object containing the plot.
+        plot_canvas (FigureCanvasTkAgg): The canvas on which the plot is drawn.
+    """
     x_spacing = simpledialog.askfloat("X Spacing", "Enter spacing between x ticks:")
     y_spacing = simpledialog.askfloat("Y Spacing", "Enter spacing between y ticks:")
     if x_spacing and y_spacing:
         ax.xaxis.set_major_locator(plt.MultipleLocator(x_spacing))
         ax.yaxis.set_major_locator(plt.MultipleLocator(y_spacing))
         plt.tight_layout()
         plot_canvas.draw_idle()
 
 def set_custom_labels_and_title(ax, plot_canvas):
+    """Sets custom labels and title for the plot.
+
+    Args:
+        ax (matplotlib.axes.Axes): The Axes object containing the plot.
+        plot_canvas (FigureCanvasTkAgg): The canvas on which the plot is drawn.
+    """
     x_label = simpledialog.askstring("Custom Labels and Title", "Enter X-axis Label:")
     y_label = simpledialog.askstring("Custom Labels and Title", "Enter Y-axis Label:")
     title = simpledialog.askstring("Custom Labels and Title", "Enter Graph Title:")
     if x_label and y_label and title:
         ax.set_xlabel(x_label, fontsize=20)
         ax.set_ylabel(y_label, fontsize=20)
         ax.set_title(title, fontsize=25, fontweight='bold')
         plt.tight_layout() 
         plot_canvas.draw_idle()
 
 
 
 def display_graph(fig):
+    """Displays the graph in a new window with options to customize it.
+
+    Args:
+        fig (matplotlib.figure.Figure): The Figure object containing the plot.
+    """
     global graph_window
     if graph_window:
         graph_window.destroy()
 
     graph_window = tk.Toplevel()
     graph_window.title("Graph")
     graph_window.geometry("1000x600")
@@ -196,15 +286,15 @@
     toolbar.update()
 
     
     for ax in fig.get_axes():
         ax.set_autoscale_on(False)
         ax.set_xlim(auto=True)
         ax.set_ylim(auto=True)
-        ax.lines[0].set_linewidth(1)  # Reset line width
+        ax.lines[0].set_linewidth(1) 
 
 
     custom_button = tk.Button(graph_window, text="Custom Labels and Title", command=lambda: set_custom_labels_and_title(fig.axes[0], plot_canvas))
     custom_button.pack(side=tk.LEFT, padx=5)
 
     add_data_point_button = tk.Button(graph_window, text="Add Data Point", command=lambda: add_data_point(fig.axes[0], plot_canvas))
     add_data_point_button.pack(side=tk.LEFT, padx=5)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/linear_regression.py` & `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/linear_regression.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,17 +4,31 @@
 from project_ppchem_tools_kit.graph_function import display_graph
 from sklearn.linear_model import LinearRegression
 from sklearn.metrics import r2_score
 import numpy as np
 
 
 def linear_regression(entry_input, x_label, y_label, title, grid=True, save_as=None, line_style='-', line_color='k'):
+    """Performs a linear regression from an Excel file and plots the graph and R^2 value.
+
+    Args:
+        file_path (str): Path to the Excel file containing the data.
+        x_label (str): x-axis label.
+        y_label (str): y-axis label.
+        title (str): Title of the graph.
+        grid (bool): Whether to display grid lines on the plot. Defaults to True.
+        save_as (str, optional): File path to save the graph. Defaults to None, in which case it is not saved.
+        line_style (str, optional): Style of the line plot. Defaults to '-'.
+        line_color (str, optional): Color of the plot line. Defaults to 'k' (black).
+
+    Raises:
+        FileNotFoundError: If the specified file_path does not exist.
+    """    
     try:
-        # Récupérez les données du fichier Excel ou d'une autre source
-        df = pd.read_excel(entry_input.get().strip())  # Utilisez entry_input pour obtenir le chemin du fichier
+        df = pd.read_excel(entry_input.get().strip())  
         data_list = df.values.tolist()
         x_values = np.array([row[0] for row in data_list]).reshape(-1, 1)
         y_values = [row[1] for row in data_list]
 
         model = LinearRegression()
         model.fit(x_values, y_values)
```

### Comparing `project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/open_graph_settings_window.py` & `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/open_graph_settings_window.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import tkinter as tk
-from tkinter import Button
 from project_ppchem_tools_kit.set_axes_color import set_axes_color
 from project_ppchem_tools_kit.set_grid_color import set_grid_color
 from project_ppchem_tools_kit.set_label_color import set_label_color
 from project_ppchem_tools_kit.set_background_color import set_background_color
 
 def open_graph_settings_window(fig, plot_canvas):
+    """Opens a new window with options to customize the graph settings.
+
+    Args:
+        fig (matplotlib.figure.Figure): The Figure object containing the plot.
+        plot_canvas (FigureCanvasTkAgg): The canvas on which the plot is drawn.
+    """
     graph_settings_window = tk.Toplevel()
     graph_settings_window.title("Graph Settings")
 
-    # Boutons pour les paramètres du graphique
     set_line_color_button = tk.Button(graph_settings_window, text="Set Line Color", command=lambda: set_axes_color(fig.axes[0], plot_canvas))
     set_line_color_button.pack(side=tk.TOP, padx=5, pady=5)
 
     set_axes_color_button = tk.Button(graph_settings_window, text="Set Axis Color", command=lambda: set_axes_color(fig.axes[0], plot_canvas))
     set_axes_color_button.pack(side=tk.TOP, padx=5, pady=5)
 
     set_grid_color_button = tk.Button(graph_settings_window, text="Set grid", command=lambda: set_grid_color(fig.axes[0], plot_canvas))
@@ -21,10 +25,9 @@
 
     set_label_color_button = tk.Button(graph_settings_window, text="Set Label Color", command=lambda: set_label_color(fig.axes[0], plot_canvas))
     set_label_color_button.pack(side=tk.TOP, padx=5, pady=5)
 
     set_background_color_button = tk.Button(graph_settings_window, text="Set Background Color", command=lambda: set_background_color(fig.axes[0], plot_canvas))
     set_background_color_button.pack(side=tk.TOP, padx=5, pady=5)
 
-    # Bouton pour fermer la fenêtre des paramètres du graphique
     close_button = tk.Button(graph_settings_window, text="Close", command=graph_settings_window.destroy)
     close_button.pack(side=tk.BOTTOM, padx=5, pady=5)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/process_input.py` & `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/process_input.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,18 +31,18 @@
         else:
             result_text = "Invalid SMILES or molecule not found."
     elif selected_radio.get() in ["3", "4"]:
         if selected_radio.get() == "3":
             make_graph(entry_input, x_label, y_label, title)
         else:
             linear_regression(entry_input, x_label, y_label, title)
-        return  # Return to prevent displaying the result window
-    elif selected_radio.get() == "5":  # Ajouter cette condition pour le bouton radio "5"
-        display_molecule(entry_input)  # Appeler la fonction pour afficher la structure moléculaire
-        return  # Return to prevent displaying the result window
+        return
+    elif selected_radio.get() == "5": 
+        display_molecule(entry_input)
+        return 
 
     elif selected_radio.get() == "6":
         error_calculation_interface()
     else:
         result_text = "Please select an input type."
 
     display_result(result_text)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/set_background_color.py` & `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/set_background_color.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 from tkinter import colorchooser
 
 def set_background_color(ax, plot_canvas):
+    """Sets the background color of the plot and canvas.
+
+    Args:
+        ax (matplotlib.axes.Axes): The Axes object containing the plot.
+        plot_canvas (FigureCanvasTkAgg): The canvas on which the plot is drawn.
+    """
     color = colorchooser.askcolor()[1]
     if color:
-        # Set the background color of the entire plot
+
         fig = ax.figure
         fig.set_facecolor(color)
 
         # Set the background color of the canvas containing the plot
         plot_canvas.get_tk_widget().configure(bg=color)
         
         # Set the background color of each axis
```

### Comparing `project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/set_custom_labels_and_title.py` & `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/set_custom_labels_and_title.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 from tkinter import simpledialog
 import matplotlib.pyplot as plt
 
 def set_custom_labels_and_title(ax, plot_canvas):
+    """Sets custom labels and title for the plot.
+
+    Args:
+        ax (matplotlib.axes.Axes): The Axes object containing the plot.
+        plot_canvas (FigureCanvasTkAgg): The canvas on which the plot is drawn.
+    """
     x_label = simpledialog.askstring("Custom Labels and Title", "Enter X-axis Label:")
     y_label = simpledialog.askstring("Custom Labels and Title", "Enter Y-axis Label:")
     title = simpledialog.askstring("Custom Labels and Title", "Enter Graph Title:")
     if x_label and y_label and title:
         ax.set_xlabel(x_label, fontsize=20)
         ax.set_ylabel(y_label, fontsize=20)
         ax.set_title(title, fontsize=25, fontweight='bold')
```

### Comparing `project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/update_clock.py` & `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/update_clock.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 window = None
 import tkinter as tk
 from datetime import datetime
 
+
+
 def update_clock():
+    """Updates the clock label with the current time and date every second."""
     current_time = datetime.now().strftime('%H:%M:%S')
     current_date = datetime.now().strftime('%Y-%m-%d')
     clock_label.config(text=current_time)
     date_label.config(text=current_date)
     window.after(1000, update_clock)
 
 date_label = tk.Label(window, text="", font=("Times New Roman", 20), bg="#1B262C", fg="#FFFFFF")
```

### Comparing `project_ppchem_tools_kit-0.1.3/src/project_ppchem_tools_kit/welcome_message.py` & `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/welcome_message.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import tkinter as tk
 window = None
 
 def welcome_message():
+    """Displays a welcome message with project information in a new window."""
     global entry_input
     welcome_window = tk.Toplevel(window)
     welcome_window.title("Welcome Message")
 
     welcome_text = (
         "✨ Welcome to Our Project! ✨\n\n"
         "We are excited to share our project with you.\n\n"
```

### Comparing `project_ppchem_tools_kit-0.1.3/PKG-INFO` & `project_ppchem_tools_kit-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: Project-ppchem-tools-kit
-Version: 0.1.3
+Version: 1.0.0
 Summary: Basic Chemistry Toolkit
 License: MIT
+Keywords: Chemistry,Tools kit,Graph maker,Linear regression,Molecular structure,Molecular mass,Uncertainty propagation,standard deviation,tkinter interface,LaTeX,SMILES
 Author: Méloé Enzinger
 Author-email: meloe.enzinger@epfl.ch> and Sébastien Grunberg <sebastien.grunberg@epfl.ch
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -19,19 +20,24 @@
 Requires-Dist: pillow (==10.2.0)
 Requires-Dist: pubchempy (==1.0.4)
 Requires-Dist: pyperclip (==1.8.2)
 Requires-Dist: rdkit (==2023.9.6)
 Requires-Dist: reportlab (==4.2.0)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: scikit-learn (==1.3.0)
+Project-URL: Github_Sebastien_Grunberg, https://github.com/sgrunber
+Project-URL: Github_Meloe_Enzinger, https://github.com/melozgr
+Project-URL: Homepage, https://github.com/sgrunber/Project-ppchem-tools-kit
 Description-Content-Type: text/markdown
 
 
 <p align="center">
    <img width="1245" alt="logo_project" src="https://github.com/sgrunber/Project-ppchem-tools-kit/raw/main/docs/source/_static/images/logo_project.png">
+   
+
 
  </p>
 
 
 
 
  <h1 align="center">🧰 Tools Kit</h1>
@@ -72,15 +78,15 @@
 
 ```bash
 git clone https://github.com/sgrunber/Project-ppchem-tools-kit.git
 ```
 
 ### 3. ⬇️ Install with pip
 
-  <a href="https://pypi.org/project/Project-ppchem-tools-kit/"><img src="https://img.shields.io/badge/PyPI-v1.0.0-blue.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="PyPI"></a>
+  <a href="https://pypi.org/project/Project-ppchem-tools-kit/"><img src="https://img.shields.io/badge/PyPI-v0.1.3-blue.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="PyPI"></a>
 
 You can also install Tools Kit using pip:
 
 ```bash
 pip install Project_ppchem-tools-kit
 ```
 
@@ -205,24 +211,50 @@
 ```
 
 ### Chicago Style
 
 <a href="https://www.chicagomanualofstyle.org/home.html"><img src="https://img.shields.io/badge/Chicago%20Style-17th%20Ed.-5579A1.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="Chicago Style"></a>
 
 ```bash
-Enzinger, Méloé, and Sébastien Grunberg. 2024. Project-ppchem-tools-kit. Computer software. GitHub. https://github.com/username/Project-ppchem-tools-kit.` 
+Méloé Enzinger and Sébastien Grunberg. 2024. Project-ppchem-tools-kit. Computer software. GitHub. https://github.com/username/Project-ppchem-tools-kit.` 
 ```
 ## 📜 License
 
 <a href="https://github.com/sgrunber/Project-ppchem-tools-kit/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="License"></a>
 
 <a id="license"></a>
 
 This project is licensed under the MIT License. See the LICENSE file for details.
 
 ## 📸 Screenshots
 <a id="screenshots"></a>
-<img width="1002" alt="Capture d’écran 2024-05-18 à 16 44 09" src="https://github.com/sgrunber/Project-ppchem-tools-kit/raw/main/docs/source/_static/images/screen.png">
 
+**Note**: Graphs have much better quality when saved to your computer.
+
+## Interface
+<p align="center">
+<img width="700" alt="Capture d’écran 2024-05-18 à 16 44 09" src="https://github.com/sgrunber/Project-ppchem-tools-kit/raw/main/docs/source/_static/images/screen.png">
+   </p>
+   
+## Graph
+<p align="center">
+<img width="700" alt="graph" src="https://github.com/sgrunber/Project-ppchem-tools-kit/assets/160881864/8d1f8352-3815-4d5d-9545-0a7138f132a5">
+    </p>
+    
+## Linear Regression
+<p align="center">
+<img width="700" alt="linear_reg" src="https://github.com/sgrunber/Project-ppchem-tools-kit/assets/160881864/eb1a56fb-d801-457b-9a1d-56fc258a6478">
+ </p>
 
+## Graph & Linear Regression Settings
+<p align="center">
+<img width="220" alt="scale" src="https://github.com/sgrunber/Project-ppchem-tools-kit/assets/160881864/8bf14d9a-a573-43fd-bfce-721dccda3415">
+<img width="178" alt="graph_option" src="https://github.com/sgrunber/Project-ppchem-tools-kit/assets/160881864/2d08b793-6903-418b-a83d-ae3d24d36171">
+<img width="220" alt="Label" src="https://github.com/sgrunber/Project-ppchem-tools-kit/assets/160881864/ad9da31f-5d76-495b-8f81-b3324c2944a6">
+ </p>
+
+## Show Molecule
+<p align="center">
+<img width="398" alt="show_molecule" src="https://github.com/sgrunber/Project-ppchem-tools-kit/assets/160881864/691fda4c-1f1d-4aa3-90ef-88cf759a4f70">
+ </p>
```

#### html2text {}

```diff
@@ -1,20 +1,25 @@
-Metadata-Version: 2.1 Name: Project-ppchem-tools-kit Version: 0.1.3 Summary:
-Basic Chemistry Toolkit License: MIT Author: MÃ©loÃ© Enzinger Author-email:
-meloe.enzinger@epfl.ch> and SÃ©bastien Grunberg
+Metadata-Version: 2.1 Name: Project-ppchem-tools-kit Version: 1.0.0 Summary:
+Basic Chemistry Toolkit License: MIT Keywords: Chemistry,Tools kit,Graph
+maker,Linear regression,Molecular structure,Molecular mass,Uncertainty
+propagation,standard deviation,tkinter interface,LaTeX,SMILES Author: MÃ©loÃ©
+Enzinger Author-email: meloe.enzinger@epfl.ch> and SÃ©bastien Grunberg
 epfl.ch Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: matplotlib
 (==3.7.2) Requires-Dist: numpy (>=1.26.4,<2.0.0) Requires-Dist: numpy5
 (>=0.1,<0.2) Requires-Dist: openpyxl (==3.1.2) Requires-Dist: pandas (==2.0.3)
 Requires-Dist: pillow (==10.2.0) Requires-Dist: pubchempy (==1.0.4) Requires-
 Dist: pyperclip (==1.8.2) Requires-Dist: rdkit (==2023.9.6) Requires-Dist:
 reportlab (==4.2.0) Requires-Dist: requests (==2.31.0) Requires-Dist: scikit-
-learn (==1.3.0) Description-Content-Type: text/markdown
+learn (==1.3.0) Project-URL: Github_Sebastien_Grunberg, https://github.com/
+sgrunber Project-URL: Github_Meloe_Enzinger, https://github.com/melozgr
+Project-URL: Homepage, https://github.com/sgrunber/Project-ppchem-tools-kit
+Description-Content-Type: text/markdown
                                 [logo_project]
                          ************ ?ð??§?° TToooollss KKiitt ************
                        _[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_]_[_L_i_c_e_n_s_e_]
 ## ð Description The **Tools Kit** package allows chemistry students to find
 basic information on molecules and provides easy access to some graphs and
 calculations required in experimental laboratories. **ð Note**: For an
 aesthetically pleasing experience, it is recommended to use the dark mode
@@ -79,12 +84,22 @@
 for your contribution! Your efforts help improve the project for everyone. ##
 ð Cite Us If you use Tools Kit in your research work or academic projects,
 we would appreciate it if you could cite us. You can use the following BibTeX
 entry: _[_B_i_b_T_e_X_]```bibtex @misc{project-ppchem-tools-kit, title = {Project-
 ppchem-tools-kit}, author = {{MÃ©loÃ© Enzinger & SÃ©bastien Grunberg}}, year =
 {2024}, publisher = {GitHub}, journal = {GitHub Repository}, howpublished =
 {\url{https://github.com/username/Project-ppchem-tools-kit}} } ``` ### Chicago
-Style _[_C_h_i_c_a_g_o_ _S_t_y_l_e_]```bash Enzinger, MÃ©loÃ©, and SÃ©bastien Grunberg. 2024.
+Style _[_C_h_i_c_a_g_o_ _S_t_y_l_e_]```bash MÃ©loÃ© Enzinger and SÃ©bastien Grunberg. 2024.
 Project-ppchem-tools-kit. Computer software. GitHub. https://github.com/
 username/Project-ppchem-tools-kit.` ``` ## ð License _[_L_i_c_e_n_s_e_]This project
 is licensed under the MIT License. See the LICENSE file for details. ## ð¸
-Screenshots[Capture dâÃ©cran 2024-05-18 Ã  16 44 09]
+Screenshots **Note**: Graphs have much better quality when saved to your
+computer. ## Interface
+                  [Capture dâÃ©cran 2024-05-18 Ã  16 44 09]
+## Graph
+                                    [graph]
+## Linear Regression
+                                 [linear_reg]
+## Graph & Linear Regression Settings
+                         [scale][graph_option][Label]
+## Show Molecule
+                                [show_molecule]
```

