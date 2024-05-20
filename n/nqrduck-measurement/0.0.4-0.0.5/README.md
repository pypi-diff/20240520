# Comparing `tmp/nqrduck_measurement-0.0.4.tar.gz` & `tmp/nqrduck_measurement-0.0.5.tar.gz`

## Comparing `nqrduck_measurement-0.0.4.tar` & `nqrduck_measurement-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0  5520293 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/docs/img/measurement_ui_labeled_v2.png
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/src/nqrduck_measurement/__init__.py
--rw-r--r--   0        0        0     9959 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/src/nqrduck_measurement/controller.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/src/nqrduck_measurement/measurement.py
--rw-r--r--   0        0        0     5893 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/src/nqrduck_measurement/model.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/src/nqrduck_measurement/signalprocessing_options.py
--rw-r--r--   0        0        0    14533 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/src/nqrduck_measurement/view.py
--rw-r--r--   0        0        0     9123 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/src/nqrduck_measurement/widget.py
--rw-r--r--   0        0        0     8047 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/src/nqrduck_measurement/resources/measurement_widget.ui
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/src/nqrduck_measurement/resources/mesurement.ini
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/LICENSE
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/README.md
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0  5520293 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/docs/img/measurement_ui_labeled_v2.png
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/src/nqrduck_measurement/__init__.py
+-rw-r--r--   0        0        0    10837 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/src/nqrduck_measurement/controller.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/src/nqrduck_measurement/measurement.py
+-rw-r--r--   0        0        0     5893 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/src/nqrduck_measurement/model.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/src/nqrduck_measurement/signalprocessing_options.py
+-rw-r--r--   0        0        0    18209 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/src/nqrduck_measurement/view.py
+-rw-r--r--   0        0        0     9123 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/src/nqrduck_measurement/widget.py
+-rw-r--r--   0        0        0     8047 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/src/nqrduck_measurement/resources/measurement_widget.ui
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/src/nqrduck_measurement/resources/mesurement.ini
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/README.md
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.5/PKG-INFO
```

### Comparing `nqrduck_measurement-0.0.4/.github/workflows/python-publish.yml` & `nqrduck_measurement-0.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.4/docs/img/measurement_ui_labeled_v2.png` & `nqrduck_measurement-0.0.5/docs/img/measurement_ui_labeled_v2.png`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.4/src/nqrduck_measurement/controller.py` & `nqrduck_measurement-0.0.5/src/nqrduck_measurement/controller.py`

 * *Files 14% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 
         logger.debug("View mode changed to: " + self.module.model.view_mode)
 
     def start_measurement(self) -> None:
         """Emit the start measurement signal."""
         logger.debug("Start measurement clicked")
         self.module.view.measurement_dialog.show()
+        QApplication.processEvents()
 
         # Set the measurement parameters again in case the user switches spectrometer
         self.module.nqrduck_signal.emit(
             "set_frequency", str(self.module.model.measurement_frequency)
         )
         self.module.nqrduck_signal.emit("set_averages", str(self.module.model.averages))
         QApplication.processEvents()
@@ -229,16 +230,21 @@
         dialog.deleteLater()
 
         self.module.model.displayed_measurement = apodized_measurement
         self.module.model.add_measurement(apodized_measurement)
 
     @pyqtSlot()
     def change_displayed_measurement(self, measurement=None) -> None:
-        """Change the displayed measurement."""
+        """Change the displayed measurement.
+
+        If no measurement is provided, the displayed measurement is changed to the selected measurement in the selection box.
 
+        Args:
+            measurement (Measurement, optional): The measurement to display. Defaults to None.
+        """
         if not self.module.model.measurements:
             logger.debug("No measurements to display.")
             return
 
         if not measurement:
             index = self.module.view._ui_form.selectionBox.value()
             self.module.model.displayed_measurement = self.module.model.measurements[
@@ -266,7 +272,24 @@
         if measurement == self.module.model.displayed_measurement:
             if self.module.model.measurements:
                 self.module.model.displayed_measurement = (
                     self.module.model.measurements[-1]
                 )
             else:
                 self.module.model.displayed_measurement = None
+
+    def edit_measurement(
+        self, old_measurement: Measurement, new_measurement: Measurement
+    ) -> None:
+        """Edit a measurement.
+
+        Args:
+            old_measurement (Measurement): The measurement to edit.
+            new_measurement (Measurement): The new measurement.
+        """
+        logger.debug("Editing measurement.")
+        # Delete the old measurement
+        self.delete_measurement(old_measurement)
+
+        # Add the new measurement
+        self.module.model.add_measurement(new_measurement)
+        self.module.model.displayed_measurement = new_measurement
```

### Comparing `nqrduck_measurement-0.0.4/src/nqrduck_measurement/model.py` & `nqrduck_measurement-0.0.5/src/nqrduck_measurement/model.py`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.4/src/nqrduck_measurement/signalprocessing_options.py` & `nqrduck_measurement-0.0.5/src/nqrduck_measurement/signalprocessing_options.py`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.4/src/nqrduck_measurement/view.py` & `nqrduck_measurement-0.0.5/src/nqrduck_measurement/view.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     QLabel,
     QVBoxLayout,
     QHBoxLayout,
     QPushButton,
     QListWidgetItem,
     QSizePolicy,
     QApplication,
+    QLineEdit,
 )
 from PyQt6.QtGui import QFontMetrics
 from PyQt6.QtCore import pyqtSlot, Qt
 from nqrduck.module.module_view import ModuleView
 from nqrduck.assets.icons import Logos
 from nqrduck.assets.animations import DuckAnimations
 from .widget import Ui_Form
@@ -50,15 +51,15 @@
         # Initialize plotter
         self.init_plotter()
         logger.debug(
             f"Facecolor {str(self._ui_form.plotter.canvas.ax.get_facecolor())}"
         )
 
         # Measurement dialog
-        self.measurement_dialog = self.MeasurementDialog()
+        self.measurement_dialog = self.MeasurementDialog(self)
 
         # Connect signals
         self.module.model.displayed_measurement_changed.connect(
             self.update_displayed_measurement
         )
         self.module.model.view_mode_changed.connect(self.update_displayed_measurement)
 
@@ -131,14 +132,19 @@
         plotter.canvas.ax.set_xlim(0, 100)
         plotter.canvas.ax.set_ylim(0, 1)
         plotter.canvas.ax.set_xlabel("Time (µs)")
         plotter.canvas.ax.set_ylabel("Amplitude (a.u.)")
         plotter.canvas.ax.set_title("Measurement data - Time domain")
         plotter.canvas.ax.grid()
 
+    @pyqtSlot()
+    def on_settings_changed(self) -> None:
+        """Redraw the plots in case the according settings have changed."""
+        self.update_displayed_measurement()
+
     def change_to_time_view(self) -> None:
         """Change plotter to time domain view."""
         plotter = self._ui_form.plotter
         self._ui_form.fftButton.setText("FFT")
         plotter.canvas.ax.clear()
         plotter.canvas.ax.set_xlabel("Time (µs)")
         plotter.canvas.ax.set_ylabel("Amplitude (a.u.)")
@@ -160,24 +166,24 @@
         """Update displayed measurement data."""
         logger.debug("Updating displayed measurement view.")
         plotter = self._ui_form.plotter
         plotter.canvas.ax.clear()
         try:
             if self.module.model.displayed_measurement is None:
                 logger.debug("No measurement data to display. Clearing plotter.")
-                
+
                 if self.module.model.view_mode == self.module.model.FFT_VIEW:
                     self.change_to_fft_view()
                 else:
                     self.change_to_time_view()
 
                 self._ui_form.plotter.canvas.draw()
 
                 return
-            
+
             if self.module.model.view_mode == self.module.model.FFT_VIEW:
                 self.change_to_fft_view()
                 y = self.module.model.displayed_measurement.fdy
                 x = (
                     self.module.model.displayed_measurement.fdx
                     + float(
                         self.module.model.displayed_measurement.target_frequency
@@ -294,25 +300,33 @@
             delete_button = QPushButton()
             delete_button.setIcon(Logos.Garbage12x12())
             delete_button.setFixedWidth(delete_button.iconSize().width())
             delete_button.clicked.connect(
                 lambda: self.module.controller.delete_measurement(measurement)
             )
 
+            edit_button = QPushButton()
+            edit_button.setIcon(Logos.Pen12x12())
+            edit_button.setFixedWidth(edit_button.iconSize().width())
+            edit_button.clicked.connect(lambda: self.show_measurement_edit(measurement))
+
             name_button = QPushButton()
             name_button.clicked.connect(
-                partial(self.module.controller.change_displayed_measurement, measurement)
+                partial(
+                    self.module.controller.change_displayed_measurement, measurement
+                )
             )
 
             # Not sure if this is pretty
             name_button.setProperty("measurement", measurement)
             name_button.setSizePolicy(
                 QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Preferred
             )  # Set size policy
 
+            layout.addWidget(edit_button)
             layout.addWidget(name_button)
             layout.addWidget(delete_button)
             layout.addStretch()  # Add stretch after delete button to ensure name button takes up space
 
             item = QListWidgetItem()
             item.setSizeHint(measurement_widget.sizeHint())
 
@@ -337,47 +351,131 @@
             fontMetrics = QFontMetrics(name_button.font())
             elidedText = fontMetrics.elidedText(
                 measurement.name, Qt.TextElideMode.ElideRight, maxWidth
             )
             name_button.setText(elidedText)
             name_button.setToolTip(measurement.name)
 
+    def show_measurement_edit(self, measurement) -> None:
+        """Show the measurement dialog.
+
+        Args:
+            measurement (Measurement): The measurement to edit.
+        """
+        dialog = self.MeasurementEdit(measurement, parent=self)
+        result = dialog.exec()
+
+        if result == QDialog.DialogCode.Accepted:
+            logger.debug("Measurement edited.")
+            self.module.controller.edit_measurement(measurement, dialog.measurement)
+        else:
+            logger.debug("Measurement edit canceled.")
+
     class MeasurementDialog(QDialog):
         """This Dialog is shown when the measurement is started and therefore blocks the main window.
 
         It shows the duck animation and a message.
 
         Attributes:
             finished (bool): True if the spinner movie is finished.
         """
 
-        def __init__(self):
+        def __init__(self, parent=None):
             """Initialize the dialog."""
-            super().__init__()
-            self.finished = True
+            super().__init__(parent)
+            self.setParent(parent)
+            self.finished = False
             self.setModal(True)
             self.setWindowFlag(Qt.WindowType.FramelessWindowHint)
             self.setAttribute(Qt.WidgetAttribute.WA_TranslucentBackground)
+            self.setWindowFlag(Qt.WindowType.WindowStaysOnTopHint)  # Ensure the window stays on top
+
+            self.message_label = QLabel("Measuring...")
+            # Make label bold and text larger
+            font = self.message_label.font()
+            font.setPointSize(20)
+            font.setBold(True)
+            self.message_label.setFont(font)
 
-            self.message_label = "Measuring..."
             self.spinner_movie = DuckAnimations.DuckKick128x128()
             self.spinner_label = QLabel(self)
+            # Make spinner label 
             self.spinner_label.setMovie(self.spinner_movie)
 
             self.layout = QVBoxLayout(self)
-            self.layout.addWidget(QLabel(self.message_label))
+            self.layout.addWidget(self.message_label)
             self.layout.addWidget(self.spinner_label)
 
             self.spinner_movie.finished.connect(self.on_movie_finished)
 
-            self.spinner_movie.start()
+        def show(self) -> None:
+            """Show the dialog and ensure it is raised and activated."""
+            super().show()
+            self.raise_()  # Bring the dialog to the front
+            self.activateWindow()  # Give the dialog focus
+            self.spinner_movie.start()  # Ensure the movie starts playing
 
         def on_movie_finished(self) -> None:
             """Called when the spinner movie is finished."""
             self.finished = True
 
         def hide(self) -> None:
             """Hide the dialog and stop the spinner movie."""
-            while not self.finished:
-                continue
             self.spinner_movie.stop()
             super().hide()
+
+    class MeasurementEdit(QDialog):
+        """This dialog is displayed when the measurement edit button is clicked.
+
+        It allows the user to edit the measurement parameters (e.g. name, ...)
+        """
+
+        def __init__(self, measurement, parent=None) -> None:
+            """Initialize the dialog."""
+            super().__init__(parent)
+            self.setParent(parent)
+
+            self.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Expanding)
+
+            logger.debug("Edit measurement dialog started.")
+
+            self.measurement = measurement
+
+            self.setWindowTitle("Edit Measurement")
+            self.layout = QVBoxLayout(self)
+            self.setLayout(self.layout)
+
+            self.name_layout = QHBoxLayout()
+            self.name_label = QLabel("Name:")
+            self.name_edit = QLineEdit(measurement.name)
+            font_metrics = self.name_edit.fontMetrics()
+            self.name_edit.setFixedWidth(
+                font_metrics.horizontalAdvance(self.name_edit.text()) + 10
+            )
+            self.name_edit.adjustSize()
+
+            self.name_layout.addWidget(self.name_label)
+            self.name_layout.addWidget(self.name_edit)
+
+            self.ok_button = QPushButton("OK")
+            self.ok_button.clicked.connect(self.on_ok_button_clicked)
+
+            self.cancel_button = QPushButton("Cancel")
+            self.cancel_button.clicked.connect(self.close)
+
+            self.layout.addLayout(self.name_layout)
+
+            button_layout = QHBoxLayout()
+            button_layout.addWidget(self.cancel_button)
+            button_layout.addWidget(self.ok_button)
+
+            self.layout.addLayout(button_layout)
+
+            # Resize the dialog
+            self.adjustSize()
+
+        def on_ok_button_clicked(self) -> None:
+            """Slot for when the OK button is clicked."""
+            logger.debug("OK button clicked.")
+            self.measurement.name = self.name_edit.text()
+            self.accept()
+            self.close()
```

### Comparing `nqrduck_measurement-0.0.4/src/nqrduck_measurement/widget.py` & `nqrduck_measurement-0.0.5/src/nqrduck_measurement/widget.py`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.4/src/nqrduck_measurement/resources/measurement_widget.ui` & `nqrduck_measurement-0.0.5/src/nqrduck_measurement/resources/measurement_widget.ui`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.4/LICENSE` & `nqrduck_measurement-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.4/README.md` & `nqrduck_measurement-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.4/pyproject.toml` & `nqrduck_measurement-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "nqrduck-measurement"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="jupfi", email="support@nqrduck.cool" },
 ]
 
 description = "A module for the NQRduck program (a simple python script™) to perform single frequency measurements."
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `nqrduck_measurement-0.0.4/PKG-INFO` & `nqrduck_measurement-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nqrduck-measurement
-Version: 0.0.4
+Version: 0.0.5
 Summary: A module for the NQRduck program (a simple python script™) to perform single frequency measurements.
 Project-URL: Homepage, https://nqrduck.cool
 Project-URL: Bug Tracker, https://github.com/nqrduck/nqrduck-measurement/issues
 Project-URL: Source Code, https://github.com/nqrduck/nqrduck-measurement
 Author-email: jupfi <support@nqrduck.cool>
 License: MIT License
```

