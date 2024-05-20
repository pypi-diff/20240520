# Comparing `tmp/nqrduck_spectrometer-0.0.8.tar.gz` & `tmp/nqrduck_spectrometer-0.0.9.tar.gz`

## Comparing `nqrduck_spectrometer-0.0.8.tar` & `nqrduck_spectrometer-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/CHANGELOG.md
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/__init__.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/base_spectrometer.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/base_spectrometer_controller.py
--rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/base_spectrometer_model.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/base_spectrometer_view.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/base_spectrometer_widget.py
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/controller.py
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/measurement.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/model.py
--rw-r--r--   0        0        0    21069 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/pulseparameters.py
--rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/pulsesequence.py
--rw-r--r--   0        0        0    12162 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/settings.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/spectrometer.py
--rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/view.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/widget.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/resources/base_spectrometer_widget.ui
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/resources/spectrometer.ini
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/resources/spectrometer_widget.ui
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/LICENSE
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/README.md
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/CHANGELOG.md
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/__init__.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/base_spectrometer.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/base_spectrometer_controller.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/base_spectrometer_model.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/base_spectrometer_view.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/base_spectrometer_widget.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/controller.py
+-rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/measurement.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/model.py
+-rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/pulseparameters.py
+-rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/pulsesequence.py
+-rw-r--r--   0        0        0    12356 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/settings.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/spectrometer.py
+-rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/view.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/widget.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/resources/base_spectrometer_widget.ui
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/resources/spectrometer.ini
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/resources/spectrometer_widget.ui
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/README.md
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 nqrduck_spectrometer-0.0.9/PKG-INFO
```

### Comparing `nqrduck_spectrometer-0.0.8/.github/workflows/python-publish.yml` & `nqrduck_spectrometer-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/base_spectrometer.py` & `nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/base_spectrometer.py`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/base_spectrometer_controller.py` & `nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/base_spectrometer_controller.py`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/base_spectrometer_model.py` & `nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/base_spectrometer_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
             Raises:
                 ValueError : If no option with the specified name is found
             """
             for option in self.options:
                 if option.name == name:
                     return option
-            raise ValueError("Option with name %s not found" % name)
+            raise ValueError(f"Option with name {name} not found")
 
     def __init__(self, module):
         """Initializes the spectrometer model.
 
         Args:
             module (Module) : The module that the spectrometer is connected to
         """
@@ -123,15 +123,15 @@
         Raises:
             ValueError : If no setting with the specified name is found
         """
         for category in self.settings.keys():
             for setting in self.settings[category]:
                 if setting.name == name:
                     return setting
-        raise ValueError("Setting with name %s not found" % name)
+        raise ValueError(f"Setting with name {name} not found")
 
     def add_pulse_parameter_option(
         self, name: str, pulse_parameter_class: PulseParameter
     ) -> None:
         """Adds a pulse parameter option to the spectrometer.
 
         Args:
```

### Comparing `nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/base_spectrometer_view.py` & `nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/base_spectrometer_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,24 +34,24 @@
         self._ui_form = Ui_Form()
         self.widget = widget
         self._ui_form.setupUi(self)
 
         grid = self._ui_form.gridLayout
         self._ui_form.verticalLayout.removeItem(self._ui_form.gridLayout)
         # Add name of the spectrometer to the view
-        label = QLabel("%s Settings:" % self.module.model.toolbar_name)
+        label = QLabel(f"{self.module.model.toolbar_name} Settings:")
         label.setStyleSheet("font-weight: bold;")
         self._ui_form.verticalLayout.setSpacing(5)
         self._ui_form.verticalLayout.addWidget(label)
         self._ui_form.verticalLayout.addLayout(grid)
 
         for category_count, category in enumerate(self.module.model.settings.keys()):
             logger.debug("Adding settings for category: %s", category)
             category_layout = QVBoxLayout()
-            category_label = QLabel("%s:" % category)
+            category_label = QLabel(f"{category}:")
             category_label.setStyleSheet("font-weight: bold;")
             row = category_count // 2
             column = category_count % 2
 
             category_layout.addWidget(category_label)
             for setting in self.module.model.settings[category]:
                 logger.debug("Adding setting to settings view: %s", setting.name)
```

### Comparing `nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/base_spectrometer_widget.py` & `nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/base_spectrometer_widget.py`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/controller.py` & `nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/controller.py`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/measurement.py` & `nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/measurement.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Class for handling measurement data."""
 
 import logging
 import numpy as np
 from nqrduck.helpers.signalprocessing import SignalProcessing as sp
+from nqrduck.helpers.functions import Function
 
 logger = logging.getLogger(__name__)
 
 
 class Measurement:
     """This class defines how measurement data should look.
 
@@ -35,20 +36,51 @@
         tdx,
         tdy,
         target_frequency,
         frequency_shift: float = 0,
         IF_frequency: float = 0,
     ) -> None:
         """Initializes the measurement."""
+        # Convert to decimal 
         self.tdx = tdx
         self.tdy = tdy
         self.target_frequency = target_frequency
         self.fdx, self.fdy = sp.fft(tdx, tdy, frequency_shift)
         self.IF_frequency = IF_frequency
 
+    def apodization(self, function : Function):
+        """Applies apodization to the measurement data.
+
+        Args:
+            function (Function): Apodization function.
+
+        returns:
+            Measurement : The apodized measurement.
+        """
+        # Get the y data weights from the function
+        duration = (self.tdx[-1] - self.tdx[0]) * 1e-6
+
+        resolution = duration / len(self.tdx)
+
+        logger.debug("Resolution: %s", resolution)
+
+        y_weight = function.get_pulse_amplitude(duration, resolution)
+
+        tdy_measurement = self.tdy * y_weight
+
+        apodized_measurement = Measurement(
+            self.tdx,
+            tdy_measurement,
+            target_frequency=self.target_frequency,
+            IF_frequency=self.IF_frequency,
+        )
+
+        return apodized_measurement
+
+
     # Data saving and loading
 
     def to_json(self):
         """Converts the measurement to a json-compatible format.
 
         Returns:
             dict : The measurement in json-compatible format.
```

### Comparing `nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/model.py` & `nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/model.py`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/pulsesequence.py` & `nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/pulsesequence.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Contains the PulseSequence class that is used to store a pulse sequence and its events."""
 
 import logging
+import importlib.metadata
 from collections import OrderedDict
 from nqrduck.helpers.unitconverter import UnitConverter
 from nqrduck_spectrometer.pulseparameters import Option
 
 logger = logging.getLogger(__name__)
 
 
@@ -15,17 +16,22 @@
         name (str): The name of the pulse sequence
 
     Attributes:
         name (str): The name of the pulse sequence
         events (list): The events of the pulse sequence
     """
 
-    def __init__(self, name) -> None:
+    def __init__(self, name, version = None) -> None:
         """Initializes the pulse sequence."""
         self.name = name
+        # Saving version to check for compatability of saved sequence
+        if version is not None:
+            self.version = version
+        else:
+            self.version = importlib.metadata.version("nqrduck_spectrometer")
         self.events = list()
 
     def get_event_names(self) -> list:
         """Returns a list of the names of the events in the pulse sequence.
 
         Returns:
             list: The names of the events
@@ -107,29 +113,30 @@
             """The duration of the event."""
             return self._duration
 
         @duration.setter
         def duration(self, duration: str):
             # Duration needs to be a positive number
             try:
-                duration = UnitConverter.to_decimal(duration)
+                duration = UnitConverter.to_float(duration)
             except ValueError:
                 raise ValueError("Duration needs to be a number")
             if duration < 0:
                 raise ValueError("Duration needs to be a positive number")
 
             self._duration = duration
 
     def to_json(self):
         """Returns a dict with all the data in the pulse sequence.
 
         Returns:
             dict: The dict with the sequence data
         """
-        data = {"name": self.name, "events": []}
+        # Get the versions of this package
+        data = {"name": self.name, "version" : self.version, "events": []}
         for event in self.events:
             event_data = {
                 "name": event.name,
                 "duration": event.duration,
                 "parameters": [],
             }
             for parameter in event.parameters.keys():
@@ -152,15 +159,15 @@
 
         Returns:
             PulseSequence: The loaded pulse sequence
 
         Raises:
             KeyError: If the pulse parameter options are not the same as the ones in the pulse sequence
         """
-        obj = cls(sequence["name"])
+        obj = cls(sequence["name"], version = sequence["version"])
         for event_data in sequence["events"]:
             obj.events.append(cls.Event.load_event(event_data, pulse_parameter_options))
 
         return obj
 
     class Variable:
         """A variable is a parameter that can be used within a pulsesequence as a placeholder.
```

### Comparing `nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/settings.py` & `nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -152,22 +152,24 @@
 
         Args:
             state (bool): The state of the input (valid or not).
             text (str): The new value of the setting.
         """
         if state:
             self.value = text
+            self.settings_changed.emit()
 
     @property
     def value(self):
         """The value of the setting. In this case, a float."""
         return self._value
 
     @value.setter
     def value(self, value):
+        logger.debug(f"Setting {self.name} to {value}")
         self._value = float(value)
         self.settings_changed.emit()
 
 
 class IntSetting(NumericalSetting):
     """A setting that is an Integer.
 
@@ -206,22 +208,24 @@
 
         Args:
             state (bool): The state of the input (valid or not).
             text (str): The new value of the setting.
         """
         if state:
             self.value = text
+            self.settings_changed.emit()
 
     @property
     def value(self):
         """The value of the setting. In this case, an int."""
         return self._value
 
     @value.setter
     def value(self, value):
+        logger.debug(f"Setting {self.name} to {value}")
         value = int(float(value))
         self._value = value
         self.settings_changed.emit()
 
 
 
 class BooleanSetting(Setting):
```

### Comparing `nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/view.py` & `nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/view.py`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/widget.py` & `nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/widget.py`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/resources/base_spectrometer_widget.ui` & `nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/resources/base_spectrometer_widget.ui`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer-0.0.8/src/nqrduck_spectrometer/resources/spectrometer_widget.ui` & `nqrduck_spectrometer-0.0.9/src/nqrduck_spectrometer/resources/spectrometer_widget.ui`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer-0.0.8/LICENSE` & `nqrduck_spectrometer-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer-0.0.8/README.md` & `nqrduck_spectrometer-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer-0.0.8/pyproject.toml` & `nqrduck_spectrometer-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "nqrduck-spectrometer"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="jupfi", email="support@nqruck.cool" },
 ]
 
 description = "A module for the NQRduck program (a simple python script™) to control different NQR/NMR spectrometers."
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `nqrduck_spectrometer-0.0.8/PKG-INFO` & `nqrduck_spectrometer-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nqrduck-spectrometer
-Version: 0.0.8
+Version: 0.0.9
 Summary: A module for the NQRduck program (a simple python script™) to control different NQR/NMR spectrometers.
 Project-URL: Homepage, https://nqrduck.cool
 Project-URL: Bug Tracker, https://github.com/nqrduck/nqrduck-spectrometer/issues
 Project-URL: Source Code, https://github.com/nqrduck/nqrduck-spectrometer
 Author-email: jupfi <support@nqruck.cool>
 License: MIT License
```

