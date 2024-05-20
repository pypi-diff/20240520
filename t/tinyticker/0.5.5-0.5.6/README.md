# Comparing `tmp/tinyticker-0.5.5.tar.gz` & `tmp/tinyticker-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyticker-0.5.5.tar", max compression
+gzip compressed data, was "tinyticker-0.5.6.tar", max compression
```

## Comparing `tinyticker-0.5.5.tar` & `tinyticker-0.5.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1068 2024-05-06 18:57:54.410125 tinyticker-0.5.5/LICENSE
--rw-r--r--   0        0        0     3863 2024-05-06 18:57:54.410125 tinyticker-0.5.5/README.md
--rw-r--r--   0        0        0      919 2024-05-06 18:57:54.410125 tinyticker-0.5.5/pyproject.toml
--rw-r--r--   0        0        0      207 2024-05-06 18:57:54.410125 tinyticker-0.5.5/tinyticker/__init__.py
--rw-r--r--   0        0        0     6196 2024-05-06 18:57:54.410125 tinyticker-0.5.5/tinyticker/__main__.py
--rw-r--r--   0        0        0     1773 2024-05-06 18:57:54.410125 tinyticker-0.5.5/tinyticker/config.py
--rw-r--r--   0        0        0     8880 2024-05-06 18:57:54.410125 tinyticker-0.5.5/tinyticker/display.py
--rw-r--r--   0        0        0      345 2024-05-06 18:57:54.410125 tinyticker-0.5.5/tinyticker/paths.py
--rw-r--r--   0        0        0    15609 2024-05-06 18:57:54.410125 tinyticker-0.5.5/tinyticker/ticker.py
--rw-r--r--   0        0        0     2476 2024-05-06 18:57:54.410125 tinyticker-0.5.5/tinyticker/utils.py
--rw-r--r--   0        0        0      318 2024-05-06 18:57:54.410125 tinyticker-0.5.5/tinyticker/waveshare_lib/__init__.py
--rw-r--r--   0        0        0     1259 2024-05-06 18:57:54.410125 tinyticker-0.5.5/tinyticker/waveshare_lib/_base.py
--rw-r--r--   0        0        0     8376 2024-05-06 18:57:54.410125 tinyticker-0.5.5/tinyticker/waveshare_lib/epd2in13.py
--rw-r--r--   0        0        0    11895 2024-05-06 18:57:54.410125 tinyticker-0.5.5/tinyticker/waveshare_lib/epd2in13_V2.py
--rw-r--r--   0        0        0    14581 2024-05-06 18:57:54.414125 tinyticker-0.5.5/tinyticker/waveshare_lib/epd2in13_V3.py
--rw-r--r--   0        0        0    10457 2024-05-06 18:57:54.414125 tinyticker-0.5.5/tinyticker/waveshare_lib/epd2in13_V4.py
--rw-r--r--   0        0        0     5835 2024-05-06 18:57:54.414125 tinyticker-0.5.5/tinyticker/waveshare_lib/epd2in13b_V3.py
--rw-r--r--   0        0        0     6627 2024-05-06 18:57:54.414125 tinyticker-0.5.5/tinyticker/waveshare_lib/epd2in13b_V4.py
--rw-r--r--   0        0        0     5690 2024-05-06 18:57:54.414125 tinyticker-0.5.5/tinyticker/waveshare_lib/epd2in13bc.py
--rw-r--r--   0        0        0     3148 2024-05-06 18:57:54.414125 tinyticker-0.5.5/tinyticker/waveshare_lib/epdconfig.py
--rw-r--r--   0        0        0     1283 2024-05-06 18:57:54.414125 tinyticker-0.5.5/tinyticker/waveshare_lib/models.py
--rw-r--r--   0        0        0       95 2024-05-06 18:57:54.414125 tinyticker-0.5.5/tinyticker/web/__init__.py
--rw-r--r--   0        0        0     2608 2024-05-06 18:57:54.414125 tinyticker-0.5.5/tinyticker/web/__main__.py
--rw-r--r--   0        0        0     6610 2024-05-06 18:57:54.414125 tinyticker-0.5.5/tinyticker/web/app.py
--rw-r--r--   0        0        0     2909 2024-05-06 18:57:54.414125 tinyticker-0.5.5/tinyticker/web/command.py
--rw-r--r--   0        0        0   274777 2024-05-06 18:57:54.414125 tinyticker-0.5.5/tinyticker/web/templates/css/uikit.min.css
--rw-r--r--   0        0        0    12844 2024-05-06 18:57:54.414125 tinyticker-0.5.5/tinyticker/web/templates/images/apple-touch-icon.png
--rw-r--r--   0        0        0      742 2024-05-06 18:57:54.414125 tinyticker-0.5.5/tinyticker/web/templates/images/favicon-16x16.png
--rw-r--r--   0        0        0     1645 2024-05-06 18:57:54.414125 tinyticker-0.5.5/tinyticker/web/templates/images/favicon-32x32.png
--rw-r--r--   0        0        0    15476 2024-05-06 18:57:54.414125 tinyticker-0.5.5/tinyticker/web/templates/index.html
--rw-r--r--   0        0        0      787 2024-05-06 18:57:54.414125 tinyticker-0.5.5/tinyticker/web/templates/js/index.js
--rw-r--r--   0        0        0    65291 2024-05-06 18:57:54.414125 tinyticker-0.5.5/tinyticker/web/templates/js/uikit-icons.min.js
--rw-r--r--   0        0        0   136629 2024-05-06 18:57:54.414125 tinyticker-0.5.5/tinyticker/web/templates/js/uikit.min.js
--rw-r--r--   0        0        0     1369 2024-05-06 18:57:54.414125 tinyticker-0.5.5/tinyticker/web/templates/logfiles.html
--rw-r--r--   0        0        0     5152 1970-01-01 00:00:00.000000 tinyticker-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-20 00:08:45.326101 tinyticker-0.5.6/LICENSE
+-rw-r--r--   0        0        0     3858 2024-05-20 00:08:45.326101 tinyticker-0.5.6/README.md
+-rw-r--r--   0        0        0      917 2024-05-20 00:08:45.326101 tinyticker-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/__init__.py
+-rw-r--r--   0        0        0     6196 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/__main__.py
+-rw-r--r--   0        0        0     1773 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/config.py
+-rw-r--r--   0        0        0     8759 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/display.py
+-rw-r--r--   0        0        0      345 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/paths.py
+-rw-r--r--   0        0        0    15609 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/ticker.py
+-rw-r--r--   0        0        0     2391 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/utils.py
+-rw-r--r--   0        0        0      278 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/waveshare_lib/__init__.py
+-rw-r--r--   0        0        0     1297 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/waveshare_lib/_base.py
+-rw-r--r--   0        0        0     4104 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/waveshare_lib/device.py
+-rw-r--r--   0        0        0     8593 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13.py
+-rw-r--r--   0        0        0    12127 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13_V2.py
+-rw-r--r--   0        0        0    14828 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13_V3.py
+-rw-r--r--   0        0        0    10709 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13_V4.py
+-rw-r--r--   0        0        0     6057 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13b_V3.py
+-rw-r--r--   0        0        0     6860 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13b_V4.py
+-rw-r--r--   0        0        0     5907 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13bc.py
+-rw-r--r--   0        0        0     1283 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/waveshare_lib/models.py
+-rw-r--r--   0        0        0       95 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/web/__init__.py
+-rw-r--r--   0        0        0     2608 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/web/__main__.py
+-rw-r--r--   0        0        0     6610 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/web/app.py
+-rw-r--r--   0        0        0     2909 2024-05-20 00:08:45.330101 tinyticker-0.5.6/tinyticker/web/command.py
+-rw-r--r--   0        0        0   274777 2024-05-20 00:08:45.334101 tinyticker-0.5.6/tinyticker/web/templates/css/uikit.min.css
+-rw-r--r--   0        0        0    12844 2024-05-20 00:08:45.334101 tinyticker-0.5.6/tinyticker/web/templates/images/apple-touch-icon.png
+-rw-r--r--   0        0        0      742 2024-05-20 00:08:45.334101 tinyticker-0.5.6/tinyticker/web/templates/images/favicon-16x16.png
+-rw-r--r--   0        0        0     1645 2024-05-20 00:08:45.334101 tinyticker-0.5.6/tinyticker/web/templates/images/favicon-32x32.png
+-rw-r--r--   0        0        0    14553 2024-05-20 00:08:45.334101 tinyticker-0.5.6/tinyticker/web/templates/index.html
+-rw-r--r--   0        0        0     1573 2024-05-20 00:08:45.334101 tinyticker-0.5.6/tinyticker/web/templates/js/index.js
+-rw-r--r--   0        0        0    65291 2024-05-20 00:08:45.334101 tinyticker-0.5.6/tinyticker/web/templates/js/uikit-icons.min.js
+-rw-r--r--   0        0        0   136629 2024-05-20 00:08:45.334101 tinyticker-0.5.6/tinyticker/web/templates/js/uikit.min.js
+-rw-r--r--   0        0        0     1369 2024-05-20 00:08:45.334101 tinyticker-0.5.6/tinyticker/web/templates/logfiles.html
+-rw-r--r--   0        0        0     5147 1970-01-01 00:00:00.000000 tinyticker-0.5.6/PKG-INFO
```

### Comparing `tinyticker-0.5.5/LICENSE` & `tinyticker-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.5/README.md` & `tinyticker-0.5.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,21 +34,20 @@
 Flash the [tinyticker image](https://drive.google.com/drive/folders/1U-PGzkOtSynN6FGDq2MsXF9kXGdkzd0D) onto a SD card and you should be good to go.
 
 > [!NOTE]
 > To build your own image, see the [`pi-gen`](https://github.com/loiccoyle/pi-gen) repo.
 
 ### Manual setup
 
-  > [!NOTE]
-  > This is much more involved than the recommended setup and will most likely require some debugging.
+> [!NOTE]
+> This is much more involved than the recommended setup and will most likely require some debugging.
 
  <details>
   <summary>Expand</summary>
 
-
 I highly recommend using [comitup](https://github.com/davesteele/comitup) to setup the networking on your RPi.
 
 - Write the `comitup` [image](https://davesteele.github.io/comitup/latest/comitup-lite-img-latest.html) to your sd card
 - Boot up the RPi and setup the networking
 - ssh into your RPi, you'll probably want to change the password while you're at it
 - Enable the [SPI interface](https://www.raspberrypi-spy.co.uk/2014/08/enabling-the-spi-interface-on-the-raspberry-pi/)
 - (Optional) rename the hostname of your RPi by editing the `/etc/hostname` and `/etc/hosts` file
```

### Comparing `tinyticker-0.5.5/pyproject.toml` & `tinyticker-0.5.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "tinyticker"
-version = "0.5.5"
+version = "0.5.6"
 description = "A tiny Raspberry Pi powered ePaper ticker."
 authors = ["Loic Coyle <loic.coyle@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/loiccoyle/tinyticker"
 keywords = ["raspberry-pi", "ticker", "stock", "crypto", "epaper", "finance"]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
-"RPi.GPIO" = "^0.7.0"
 spidev = "^3.5"
 Pillow = "^10.0.1"
 cryptocompare = "^0.7.5"
 pandas = "^1.3.5"
 matplotlib = "^3.5.1"
 mplfinance = "^0.12.7-alpha.17"
 Flask = "^2.0.2"
 yfinance = "^0.2.0"
 qrcode = "^7.3.1"
 packaging = "^23.0"
 numpy = "^1.26"
 watchdog = "^4.0.0"
 waitress = "^3.0.0"
+gpiozero = "^2.0.1"
 
 [tool.poetry.scripts]
 tinyticker = 'tinyticker.__main__:main'
 tinyticker-web = 'tinyticker.web.__main__:main'
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
```

### Comparing `tinyticker-0.5.5/tinyticker/__main__.py` & `tinyticker-0.5.6/tinyticker/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.5/tinyticker/config.py` & `tinyticker-0.5.6/tinyticker/config.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.5/tinyticker/display.py` & `tinyticker-0.5.6/tinyticker/display.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import matplotlib.pyplot as plt
 import mplfinance as mpf
 import numpy as np
 import pandas as pd
 from PIL import Image
 
 from .config import TinytickerConfig
-from .waveshare_lib import CONFIG, MODELS
+from .waveshare_lib import MODELS
 from .waveshare_lib._base import EPDHighlight
 
 MARKETCOLORS = mpf.make_marketcolors(
     up="white",
     down="black",
     edge="black",
     wick="black",
@@ -259,13 +259,7 @@
                 bbox=TEXT_BBOX,
             )
 
         fig.tight_layout(pad=0)
         if show:
             self.show_fig(fig)
         return fig, ax
-
-    def __del__(self):
-        try:
-            CONFIG.module_exit()
-        except Exception:
-            pass
```

### Comparing `tinyticker-0.5.5/tinyticker/ticker.py` & `tinyticker-0.5.6/tinyticker/ticker.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.5/tinyticker/utils.py` & `tinyticker-0.5.6/tinyticker/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import argparse
-import json
 import logging
 import socket
-from urllib.request import urlopen
 
 import pandas as pd
 import qrcode
-from packaging.version import Version
 from PIL import Image, ImageChops
 
 
 def dashboard_qrcode(epd_width: int, epd_height: int, port: int = 8000) -> Image.Image:
     """Generate a qrcode pointing to the dashboard url.
 
     Args:
```

### Comparing `tinyticker-0.5.5/tinyticker/waveshare_lib/_base.py` & `tinyticker-0.5.6/tinyticker/waveshare_lib/_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,49 @@
 from abc import abstractmethod
-from typing import Literal, Optional
+from typing import Literal, Optional, Type
 
 from PIL import Image
 
+from .device import RaspberryPi
+
 
 class EPDBase:
     width: int
     height: int
 
     @abstractmethod
-    def __init__(self) -> None:
-        ...
+    def __init__(self, device: Type[RaspberryPi] = RaspberryPi) -> None: ...
 
     @abstractmethod
-    def init(self) -> Literal[0, -1]:
-        ...
+    def init(self) -> Literal[0, -1]: ...
 
     @abstractmethod
-    def getbuffer(self, image: Image.Image) -> bytearray:
-        ...
+    def getbuffer(self, image: Image.Image) -> bytearray: ...
 
     @abstractmethod
-    def Clear(self) -> None:
-        ...
+    def Clear(self) -> None: ...
 
     @abstractmethod
-    def sleep(self) -> None:
-        ...
+    def sleep(self) -> None: ...
 
 
 class EPDMonochrome(EPDBase):
     """EPD with only black and white color"""
 
     @abstractmethod
-    def display(self, image: bytearray) -> None:
-        ...
+    def display(self, image: bytearray) -> None: ...
 
 
 class EPDHighlight(EPDBase):
     """EPD with black and white color, and an extra color"""
 
     @abstractmethod
-    def display(self, imageblack: bytearray, highlights: Optional[bytearray]) -> None:
-        ...
+    def display(
+        self, imageblack: bytearray, highlights: Optional[bytearray]
+    ) -> None: ...
 
 
 # Could be used later to utilize the partial refresh feature of some of the EPDs
 # class EPDPartial(EPDBase):
 #     @abstractmethod
 #     def display(self, image: bytearray) -> None:
 #         ...
```

### Comparing `tinyticker-0.5.5/tinyticker/waveshare_lib/epd2in13.py` & `tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,33 +23,34 @@
 # FITNESS OR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
-
 import logging
+from typing import Type
 
 from ._base import EPDMonochrome
-from .epdconfig import CONFIG
+from .device import RaspberryPi
 
 # Display resolution
 EPD_WIDTH = 122
 EPD_HEIGHT = 250
 
 logger = logging.getLogger(__name__)
 
 
 class EPD(EPDMonochrome):
-    def __init__(self):
-        self.reset_pin = CONFIG.RST_PIN
-        self.dc_pin = CONFIG.DC_PIN
-        self.busy_pin = CONFIG.BUSY_PIN
-        self.cs_pin = CONFIG.CS_PIN
+    def __init__(self, device: Type[RaspberryPi] = RaspberryPi):
+        self.device = device()
+        self.reset_pin = self.device.RST_PIN
+        self.dc_pin = self.device.DC_PIN
+        self.busy_pin = self.device.BUSY_PIN
+        self.cs_pin = self.device.CS_PIN
         self.width = EPD_WIDTH
         self.height = EPD_HEIGHT
 
     lut_full_update = [
         0x22,
         0x55,
         0xAA,
@@ -113,49 +114,49 @@
         0x00,
         0x00,
         0x00,
     ]
 
     # Hardware reset
     def reset(self):
-        CONFIG.digital_write(self.reset_pin, 1)
-        CONFIG.delay_ms(200)
-        CONFIG.digital_write(self.reset_pin, 0)
-        CONFIG.delay_ms(5)
-        CONFIG.digital_write(self.reset_pin, 1)
-        CONFIG.delay_ms(200)
+        self.device.digital_write(self.reset_pin, 1)
+        self.device.delay_ms(200)
+        self.device.digital_write(self.reset_pin, 0)
+        self.device.delay_ms(5)
+        self.device.digital_write(self.reset_pin, 1)
+        self.device.delay_ms(200)
 
     def send_command(self, command):
-        CONFIG.digital_write(self.dc_pin, 0)
-        CONFIG.digital_write(self.cs_pin, 0)
-        CONFIG.spi_writebyte([command])
-        CONFIG.digital_write(self.cs_pin, 1)
+        self.device.digital_write(self.dc_pin, 0)
+        self.device.digital_write(self.cs_pin, 0)
+        self.device.spi_writebyte([command])
+        self.device.digital_write(self.cs_pin, 1)
 
     def send_data(self, data):
-        CONFIG.digital_write(self.dc_pin, 1)
-        CONFIG.digital_write(self.cs_pin, 0)
-        CONFIG.spi_writebyte([data])
-        CONFIG.digital_write(self.cs_pin, 1)
+        self.device.digital_write(self.dc_pin, 1)
+        self.device.digital_write(self.cs_pin, 0)
+        self.device.spi_writebyte([data])
+        self.device.digital_write(self.cs_pin, 1)
 
     def ReadBusy(self):
-        while CONFIG.digital_read(self.busy_pin) == 1:  # 0: idle, 1: busy
-            CONFIG.delay_ms(100)
+        while self.device.digital_read(self.busy_pin) == 1:  # 0: idle, 1: busy
+            self.device.delay_ms(100)
 
     def TurnOnDisplay(self):
         self.send_command(0x22)  # DISPLAY_UPDATE_CONTROL_2
         self.send_data(0xC4)
         self.send_command(0x20)  # MASTER_ACTIVATION
         self.send_command(0xFF)  # TERMINATE_FRAME_READ_WRITE
 
         logger.debug("e-Paper busy")
         self.ReadBusy()
         logger.debug("e-Paper busy release")
 
     def init(self):
-        if CONFIG.module_init() != 0:
+        if self.device.module_init() != 0:
             return -1
         # EPD hardware init start
         self.reset()
         self.send_command(0x01)  # DRIVER_OUTPUT_CONTROL
         self.send_data((EPD_HEIGHT - 1) & 0xFF)
         self.send_data(((EPD_HEIGHT - 1) >> 8) & 0xFF)
         self.send_data(0x00)  # GD = 0 SM = 0 TB = 0
@@ -267,11 +268,11 @@
             for _ in range(0, linewidth):
                 self.send_data(color)
         self.TurnOnDisplay()
 
     def sleep(self):
         self.send_command(0x10)  # enter deep sleep
         self.send_data(0x01)
-        CONFIG.delay_ms(100)
+        self.device.delay_ms(100)
 
-        CONFIG.delay_ms(2000)
-        CONFIG.module_exit()
+        self.device.delay_ms(2000)
+        self.device.module_exit()
```

### Comparing `tinyticker-0.5.5/tinyticker/waveshare_lib/epd2in13_V2.py` & `tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13_V2.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,33 +23,34 @@
 # FITNESS OR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
-
 import logging
+from typing import Type
 
 from ._base import EPDMonochrome
-from .epdconfig import CONFIG
+from .device import RaspberryPi
 
 # Display resolution
 EPD_WIDTH = 122
 EPD_HEIGHT = 250
 
 logger = logging.getLogger(__name__)
 
 
 class EPD(EPDMonochrome):
-    def __init__(self):
-        self.reset_pin = CONFIG.RST_PIN
-        self.dc_pin = CONFIG.DC_PIN
-        self.busy_pin = CONFIG.BUSY_PIN
-        self.cs_pin = CONFIG.CS_PIN
+    def __init__(self, device: Type[RaspberryPi] = RaspberryPi):
+        self.device = device()
+        self.reset_pin = self.device.RST_PIN
+        self.dc_pin = self.device.DC_PIN
+        self.busy_pin = self.device.BUSY_PIN
+        self.cs_pin = self.device.CS_PIN
         self.width = EPD_WIDTH
         self.height = EPD_HEIGHT
 
     FULL_UPDATE = 0
     PART_UPDATE = 1
     lut_full_update = [
         0x80,
@@ -207,58 +208,58 @@
         0x32,
         0x30,
         0x0A,
     ]
 
     # Hardware reset
     def reset(self):
-        CONFIG.digital_write(self.reset_pin, 1)
-        CONFIG.delay_ms(200)
-        CONFIG.digital_write(self.reset_pin, 0)
-        CONFIG.delay_ms(5)
-        CONFIG.digital_write(self.reset_pin, 1)
-        CONFIG.delay_ms(200)
+        self.device.digital_write(self.reset_pin, 1)
+        self.device.delay_ms(200)
+        self.device.digital_write(self.reset_pin, 0)
+        self.device.delay_ms(5)
+        self.device.digital_write(self.reset_pin, 1)
+        self.device.delay_ms(200)
 
     def send_command(self, command):
-        CONFIG.digital_write(self.dc_pin, 0)
-        CONFIG.digital_write(self.cs_pin, 0)
-        CONFIG.spi_writebyte([command])
-        CONFIG.digital_write(self.cs_pin, 1)
+        self.device.digital_write(self.dc_pin, 0)
+        self.device.digital_write(self.cs_pin, 0)
+        self.device.spi_writebyte([command])
+        self.device.digital_write(self.cs_pin, 1)
 
     def send_data(self, data):
-        CONFIG.digital_write(self.dc_pin, 1)
-        CONFIG.digital_write(self.cs_pin, 0)
-        CONFIG.spi_writebyte([data])
-        CONFIG.digital_write(self.cs_pin, 1)
+        self.device.digital_write(self.dc_pin, 1)
+        self.device.digital_write(self.cs_pin, 0)
+        self.device.spi_writebyte([data])
+        self.device.digital_write(self.cs_pin, 1)
 
     # send a lot of data
     def send_data2(self, data):
-        CONFIG.digital_write(self.dc_pin, 1)
-        CONFIG.digital_write(self.cs_pin, 0)
-        CONFIG.spi_writebyte2(data)
-        CONFIG.digital_write(self.cs_pin, 1)
+        self.device.digital_write(self.dc_pin, 1)
+        self.device.digital_write(self.cs_pin, 0)
+        self.device.spi_writebyte2(data)
+        self.device.digital_write(self.cs_pin, 1)
 
     def ReadBusy(self):
-        while CONFIG.digital_read(self.busy_pin) == 1:  # 0: idle, 1: busy
-            CONFIG.delay_ms(100)
+        while self.device.digital_read(self.busy_pin) == 1:  # 0: idle, 1: busy
+            self.device.delay_ms(100)
 
     def TurnOnDisplay(self):
         self.send_command(0x22)
         self.send_data(0xC7)
         self.send_command(0x20)
         self.ReadBusy()
 
     def TurnOnDisplayPart(self):
         self.send_command(0x22)
         self.send_data(0x0C)
         self.send_command(0x20)
         self.ReadBusy()
 
     def init(self, update=0):
-        if CONFIG.module_init() != 0:
+        if self.device.module_init() != 0:
             return -1
         # EPD hardware init start
         self.reset()
         if update == self.FULL_UPDATE:
             self.ReadBusy()
             self.send_command(0x12)  # soft reset
             self.ReadBusy()
@@ -428,9 +429,9 @@
     def sleep(self):
         # self.send_command(0x22) #POWER OFF
         # self.send_data(0xC3)
         # self.send_command(0x20)
 
         self.send_command(0x10)  # enter deep sleep
         self.send_data(0x03)
-        CONFIG.delay_ms(2000)
-        CONFIG.module_exit()
+        self.device.delay_ms(2000)
+        self.device.module_exit()
```

### Comparing `tinyticker-0.5.5/tinyticker/waveshare_lib/epd2in13_V3.py` & `tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13_V3.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,33 +23,34 @@
 # FITNESS OR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
-
 import logging
+from typing import Type
 
 from ._base import EPDMonochrome
-from .epdconfig import CONFIG
+from .device import RaspberryPi
 
 # Display resolution
 EPD_WIDTH = 122
 EPD_HEIGHT = 250
 
 logger = logging.getLogger(__name__)
 
 
 class EPD(EPDMonochrome):
-    def __init__(self):
-        self.reset_pin = CONFIG.RST_PIN
-        self.dc_pin = CONFIG.DC_PIN
-        self.busy_pin = CONFIG.BUSY_PIN
-        self.cs_pin = CONFIG.CS_PIN
+    def __init__(self, device: Type[RaspberryPi] = RaspberryPi):
+        self.device = device()
+        self.reset_pin = self.device.RST_PIN
+        self.dc_pin = self.device.DC_PIN
+        self.busy_pin = self.device.BUSY_PIN
+        self.cs_pin = self.device.CS_PIN
         self.width = EPD_WIDTH
         self.height = EPD_HEIGHT
 
     lut_partial_update = [
         0x0,
         0x40,
         0x0,
@@ -375,61 +376,61 @@
 
     """
     function :Hardware reset
     parameter:
     """
 
     def reset(self):
-        CONFIG.digital_write(self.reset_pin, 1)
-        CONFIG.delay_ms(20)
-        CONFIG.digital_write(self.reset_pin, 0)
-        CONFIG.delay_ms(2)
-        CONFIG.digital_write(self.reset_pin, 1)
-        CONFIG.delay_ms(20)
+        self.device.digital_write(self.reset_pin, 1)
+        self.device.delay_ms(20)
+        self.device.digital_write(self.reset_pin, 0)
+        self.device.delay_ms(2)
+        self.device.digital_write(self.reset_pin, 1)
+        self.device.delay_ms(20)
 
     """
     function :send command
     parameter:
      command : Command register
     """
 
     def send_command(self, command):
-        CONFIG.digital_write(self.dc_pin, 0)
-        CONFIG.digital_write(self.cs_pin, 0)
-        CONFIG.spi_writebyte([command])
-        CONFIG.digital_write(self.cs_pin, 1)
+        self.device.digital_write(self.dc_pin, 0)
+        self.device.digital_write(self.cs_pin, 0)
+        self.device.spi_writebyte([command])
+        self.device.digital_write(self.cs_pin, 1)
 
     """
     function :send data
     parameter:
      data : Write data
     """
 
     def send_data(self, data):
-        CONFIG.digital_write(self.dc_pin, 1)
-        CONFIG.digital_write(self.cs_pin, 0)
-        CONFIG.spi_writebyte([data])
-        CONFIG.digital_write(self.cs_pin, 1)
+        self.device.digital_write(self.dc_pin, 1)
+        self.device.digital_write(self.cs_pin, 0)
+        self.device.spi_writebyte([data])
+        self.device.digital_write(self.cs_pin, 1)
 
     # send a lot of data
     def send_data2(self, data):
-        CONFIG.digital_write(self.dc_pin, 1)
-        CONFIG.digital_write(self.cs_pin, 0)
-        CONFIG.spi_writebyte2(data)
-        CONFIG.digital_write(self.cs_pin, 1)
+        self.device.digital_write(self.dc_pin, 1)
+        self.device.digital_write(self.cs_pin, 0)
+        self.device.spi_writebyte2(data)
+        self.device.digital_write(self.cs_pin, 1)
 
     """
     function :Wait until the busy_pin goes LOW
     parameter:
     """
 
     def ReadBusy(self):
         logger.debug("e-Paper busy")
-        while CONFIG.digital_read(self.busy_pin) == 1:  # 0: idle, 1: busy
-            CONFIG.delay_ms(10)
+        while self.device.digital_read(self.busy_pin) == 1:  # 0: idle, 1: busy
+            self.device.delay_ms(10)
         logger.debug("e-Paper busy release")
 
     """
     function : Turn On Display
     parameter:
     """
 
@@ -520,15 +521,15 @@
 
     """
     function : Initialize the e-Paper register
     parameter:
     """
 
     def init(self):
-        if CONFIG.module_init() != 0:
+        if self.device.module_init() != 0:
             return -1
         # EPD hardware init start
         self.reset()
 
         self.ReadBusy()
         self.send_command(0x12)  # SWRESET
         self.ReadBusy()
@@ -607,17 +608,17 @@
     """
     function : Sends the image buffer in RAM to e-Paper and partial refresh
     parameter:
         image : Image data
     """
 
     def displayPartial(self, image):
-        CONFIG.digital_write(self.reset_pin, 0)
-        CONFIG.delay_ms(1)
-        CONFIG.digital_write(self.reset_pin, 1)
+        self.device.digital_write(self.reset_pin, 0)
+        self.device.delay_ms(1)
+        self.device.digital_write(self.reset_pin, 1)
 
         self.SetLut(self.lut_partial_update)
         self.send_command(0x37)
         self.send_data(0x00)
         self.send_data(0x00)
         self.send_data(0x00)
         self.send_data(0x00)
@@ -681,9 +682,9 @@
     parameter:
     """
 
     def sleep(self):
         self.send_command(0x10)  # enter deep sleep
         self.send_data(0x01)
 
-        CONFIG.delay_ms(2000)
-        CONFIG.module_exit()
+        self.device.delay_ms(2000)
+        self.device.module_exit()
```

### Comparing `tinyticker-0.5.5/tinyticker/waveshare_lib/epd2in13b_V4.py` & `tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13b_V4.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,69 +24,71 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
 import logging
+from typing import Type
 
 from ._base import EPDHighlight
-from .epdconfig import CONFIG
+from .device import RaspberryPi
 
 # Display resolution
 EPD_WIDTH = 122
 EPD_HEIGHT = 250
 
 logger = logging.getLogger(__name__)
 
 
 class EPD(EPDHighlight):
-    def __init__(self):
-        self.reset_pin = CONFIG.RST_PIN
-        self.dc_pin = CONFIG.DC_PIN
-        self.busy_pin = CONFIG.BUSY_PIN
-        self.cs_pin = CONFIG.CS_PIN
+    def __init__(self, device: Type[RaspberryPi] = RaspberryPi):
+        self.device = device()
+        self.reset_pin = self.device.RST_PIN
+        self.dc_pin = self.device.DC_PIN
+        self.busy_pin = self.device.BUSY_PIN
+        self.cs_pin = self.device.CS_PIN
         self.width = EPD_WIDTH
         self.height = EPD_HEIGHT
 
     # hardware reset
     def reset(self):
-        CONFIG.digital_write(self.reset_pin, 1)
-        CONFIG.delay_ms(20)
-        CONFIG.digital_write(self.reset_pin, 0)
-        CONFIG.delay_ms(2)
-        CONFIG.digital_write(self.reset_pin, 1)
-        CONFIG.delay_ms(20)
+        self.device.digital_write(self.reset_pin, 1)
+        self.device.delay_ms(20)
+        self.device.digital_write(self.reset_pin, 0)
+        self.device.delay_ms(2)
+        self.device.digital_write(self.reset_pin, 1)
+        self.device.delay_ms(20)
 
     # send 1 byte command
     def send_command(self, command):
-        CONFIG.digital_write(self.dc_pin, 0)
-        CONFIG.digital_write(self.cs_pin, 0)
-        CONFIG.spi_writebyte([command])
-        CONFIG.digital_write(self.cs_pin, 1)
+        self.device.digital_write(self.dc_pin, 0)
+        self.device.digital_write(self.cs_pin, 0)
+        self.device.spi_writebyte([command])
+        self.device.digital_write(self.cs_pin, 1)
 
     # send 1 byte data
     def send_data(self, data):
-        CONFIG.digital_write(self.dc_pin, 1)
-        CONFIG.digital_write(self.cs_pin, 0)
-        CONFIG.spi_writebyte([data])
-        CONFIG.digital_write(self.cs_pin, 1)
+        self.device.digital_write(self.dc_pin, 1)
+        self.device.digital_write(self.cs_pin, 0)
+        self.device.spi_writebyte([data])
+        self.device.digital_write(self.cs_pin, 1)
 
     # send a lot of data
     def send_data2(self, data):
-        CONFIG.digital_write(self.dc_pin, 1)
-        CONFIG.digital_write(self.cs_pin, 0)
-        CONFIG.spi_writebyte2(data)
-        CONFIG.digital_write(self.cs_pin, 1)
+        self.device.digital_write(self.dc_pin, 1)
+        self.device.digital_write(self.cs_pin, 0)
+        self.device.spi_writebyte2(data)
+        self.device.digital_write(self.cs_pin, 1)
 
     # judge e-Paper whether is ReadBusy
     def ReadBusy(self):
         logger.debug("e-Paper busy")
-        while CONFIG.digital_read(self.busy_pin) != 0:
-            CONFIG.delay_ms(10)
+        while self.device.digital_read(self.busy_pin) != 0:
+            self.device.delay_ms(10)
         logger.debug("e-Paper busy release")
 
     # set the display window
     def set_windows(self, xstart, ystart, xend, yend):
         self.send_command(0x44)  # SET_RAM_X_ADDRESS_START_END_POSITION
         self.send_data((xstart >> 3) & 0xFF)
         self.send_data((xend >> 3) & 0xFF)
@@ -104,15 +106,15 @@
 
         self.send_command(0x4F)  # SET_RAM_Y_ADDRESS_COUNTER
         self.send_data(ystart & 0xFF)
         self.send_data((ystart >> 8) & 0xFF)
 
     # initialize
     def init(self):
-        if CONFIG.module_init() != 0:
+        if self.device.module_init() != 0:
             return -1
 
         self.reset()
 
         self.ReadBusy()
         self.send_command(0x12)  # SWRESET
         self.ReadBusy()
@@ -202,9 +204,9 @@
         self.clear()
 
     # sleep
     def sleep(self):
         self.send_command(0x10)  # DEEP_SLEEP
         self.send_data(0x01)  # check code
 
-        CONFIG.delay_ms(2000)
-        CONFIG.module_exit()
+        self.device.delay_ms(2000)
+        self.device.module_exit()
```

### Comparing `tinyticker-0.5.5/tinyticker/waveshare_lib/epd2in13bc.py` & `tinyticker-0.5.6/tinyticker/waveshare_lib/epd2in13bc.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,63 +24,65 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
 import logging
+from typing import Type
 
 from ._base import EPDHighlight
-from .epdconfig import CONFIG
+from .device import RaspberryPi
 
 # Display resolution
 EPD_WIDTH = 104
 EPD_HEIGHT = 212
 
 logger = logging.getLogger(__name__)
 
 
 class EPD(EPDHighlight):
-    def __init__(self):
-        self.reset_pin = CONFIG.RST_PIN
-        self.dc_pin = CONFIG.DC_PIN
-        self.busy_pin = CONFIG.BUSY_PIN
-        self.cs_pin = CONFIG.CS_PIN
+    def __init__(self, device: Type[RaspberryPi] = RaspberryPi):
+        self.device = device()
+        self.reset_pin = self.device.RST_PIN
+        self.dc_pin = self.device.DC_PIN
+        self.busy_pin = self.device.BUSY_PIN
+        self.cs_pin = self.device.CS_PIN
         self.width = EPD_WIDTH
         self.height = EPD_HEIGHT
 
     # Hardware reset
     def reset(self):
-        CONFIG.digital_write(self.reset_pin, 1)
-        CONFIG.delay_ms(200)
-        CONFIG.digital_write(self.reset_pin, 0)
-        CONFIG.delay_ms(5)
-        CONFIG.digital_write(self.reset_pin, 1)
-        CONFIG.delay_ms(200)
+        self.device.digital_write(self.reset_pin, 1)
+        self.device.delay_ms(200)
+        self.device.digital_write(self.reset_pin, 0)
+        self.device.delay_ms(5)
+        self.device.digital_write(self.reset_pin, 1)
+        self.device.delay_ms(200)
 
     def send_command(self, command):
-        CONFIG.digital_write(self.dc_pin, 0)
-        CONFIG.digital_write(self.cs_pin, 0)
-        CONFIG.spi_writebyte([command])
-        CONFIG.digital_write(self.cs_pin, 1)
+        self.device.digital_write(self.dc_pin, 0)
+        self.device.digital_write(self.cs_pin, 0)
+        self.device.spi_writebyte([command])
+        self.device.digital_write(self.cs_pin, 1)
 
     def send_data(self, data):
-        CONFIG.digital_write(self.dc_pin, 1)
-        CONFIG.digital_write(self.cs_pin, 0)
-        CONFIG.spi_writebyte([data])
-        CONFIG.digital_write(self.cs_pin, 1)
+        self.device.digital_write(self.dc_pin, 1)
+        self.device.digital_write(self.cs_pin, 0)
+        self.device.spi_writebyte([data])
+        self.device.digital_write(self.cs_pin, 1)
 
     def ReadBusy(self):
         logger.debug("e-Paper busy")
-        while CONFIG.digital_read(self.busy_pin) == 0:  # 0: idle, 1: busy
-            CONFIG.delay_ms(100)
+        while self.device.digital_read(self.busy_pin) == 0:  # 0: idle, 1: busy
+            self.device.delay_ms(100)
         logger.debug("e-Paper busy release")
 
     def init(self):
-        if CONFIG.module_init() != 0:
+        if self.device.module_init() != 0:
             return -1
 
         self.reset()
 
         self.send_command(0x06)  # BOOSTER_SOFT_START
         self.send_data(0x17)
         self.send_data(0x17)
@@ -138,25 +140,25 @@
         self.send_command(0x12)  # REFRESH
         self.ReadBusy()
 
     def Clear(self):
         self.send_command(0x10)
         for _ in range(0, int(self.width * self.height / 8)):
             self.send_data(0xFF)
-        self.send_command(0x92)
+        # self.send_command(0x92)
 
         self.send_command(0x13)
         for _ in range(0, int(self.width * self.height / 8)):
             self.send_data(0xFF)
-        self.send_command(0x92)
+        # self.send_command(0x92)
 
         self.send_command(0x12)  # REFRESH
         self.ReadBusy()
 
     def sleep(self):
         self.send_command(0x02)  # POWER_OFF
         self.ReadBusy()
         self.send_command(0x07)  # DEEP_SLEEP
         self.send_data(0xA5)  # check code
 
-        CONFIG.delay_ms(2000)
-        CONFIG.module_exit()
+        self.device.delay_ms(2000)
+        self.device.module_exit()
```

### Comparing `tinyticker-0.5.5/tinyticker/waveshare_lib/models.py` & `tinyticker-0.5.6/tinyticker/waveshare_lib/models.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.5/tinyticker/web/__main__.py` & `tinyticker-0.5.6/tinyticker/web/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.5/tinyticker/web/app.py` & `tinyticker-0.5.6/tinyticker/web/app.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.5/tinyticker/web/command.py` & `tinyticker-0.5.6/tinyticker/web/command.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.5/tinyticker/web/templates/css/uikit.min.css` & `tinyticker-0.5.6/tinyticker/web/templates/css/uikit.min.css`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.5/tinyticker/web/templates/images/apple-touch-icon.png` & `tinyticker-0.5.6/tinyticker/web/templates/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.5/tinyticker/web/templates/images/favicon-16x16.png` & `tinyticker-0.5.6/tinyticker/web/templates/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.5/tinyticker/web/templates/images/favicon-32x32.png` & `tinyticker-0.5.6/tinyticker/web/templates/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.5/tinyticker/web/templates/index.html` & `tinyticker-0.5.6/tinyticker/web/templates/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -22,40 +22,16 @@
       href="img/favicon-16x16.png"
     />
     <!-- CSS FILES -->
     <link rel="stylesheet" type="text/css" href="css/uikit.min.css" />
     <!-- JS FILES -->
     <script src="js/uikit.min.js"></script>
     <script src="js/uikit-icons.min.js"></script>
+    <script src="js/index.js"></script>
     <script>
-      /**
-       * Compares two semver strings.
-       *
-       * @param {string} v1 - The first version.
-       * @param {string} v2 - The second version.
-       * @returns {boolean} - Returns true if v1 is greater than v2, otherwise returns false.
-       */
-      function isGreater(v1, v2) {
-        let [v1major, v1minor, v1patch] = v1.split(".").map(Number);
-        let [v2major, v2minor, v2patch] = v2.split(".").map(Number);
-        return (
-          v1major > v2major ||
-          (v1major == v2major &&
-            (v1minor > v2minor || (v1minor == v2minor && v1patch > v2patch)))
-        );
-      }
-
-      async function checkForUpdate(currentVersion) {
-        const url = "https://pypi.org/pypi/tinyticker/json";
-        const response = await fetch(url);
-        const data = await response.json();
-        const pypiVersion = data.info.version;
-        return isGreater(pypiVersion, currentVersion);
-      }
-
       checkForUpdate("{{version}}").then((isUpdateAvailable) => {
         document.getElementById("updateDiv").style.display = isUpdateAvailable
           ? "block"
           : "none";
       });
     </script>
   </head>
@@ -365,9 +341,8 @@
           title="issues"
           target="_blank"
           >Report an issue</a
         >
       </span>
     </div>
   </body>
-  <script src="js/index.js"></script>
 </html>
```

### Comparing `tinyticker-0.5.5/tinyticker/web/templates/js/uikit-icons.min.js` & `tinyticker-0.5.6/tinyticker/web/templates/js/uikit-icons.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.5/tinyticker/web/templates/js/uikit.min.js` & `tinyticker-0.5.6/tinyticker/web/templates/js/uikit.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.5/tinyticker/web/templates/logfiles.html` & `tinyticker-0.5.6/tinyticker/web/templates/logfiles.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.5/PKG-INFO` & `tinyticker-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyticker
-Version: 0.5.5
+Version: 0.5.6
 Summary: A tiny Raspberry Pi powered ePaper ticker.
 Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT
 Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance
 Author: Loic Coyle
 Author-email: loic.coyle@hotmail.fr
 Requires-Python: >=3.9
@@ -12,16 +12,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Flask (>=2.0.2,<3.0.0)
 Requires-Dist: Pillow (>=10.0.1,<11.0.0)
-Requires-Dist: RPi.GPIO (>=0.7.0,<0.8.0)
 Requires-Dist: cryptocompare (>=0.7.5,<0.8.0)
+Requires-Dist: gpiozero (>=2.0.1,<3.0.0)
 Requires-Dist: matplotlib (>=3.5.1,<4.0.0)
 Requires-Dist: mplfinance (>=0.12.7-alpha.17,<0.13.0)
 Requires-Dist: numpy (>=1.26,<2.0)
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: pandas (>=1.3.5,<2.0.0)
 Requires-Dist: qrcode (>=7.3.1,<8.0.0)
 Requires-Dist: spidev (>=3.5,<4.0)
@@ -67,21 +67,20 @@
 Flash the [tinyticker image](https://drive.google.com/drive/folders/1U-PGzkOtSynN6FGDq2MsXF9kXGdkzd0D) onto a SD card and you should be good to go.
 
 > [!NOTE]
 > To build your own image, see the [`pi-gen`](https://github.com/loiccoyle/pi-gen) repo.
 
 ### Manual setup
 
-  > [!NOTE]
-  > This is much more involved than the recommended setup and will most likely require some debugging.
+> [!NOTE]
+> This is much more involved than the recommended setup and will most likely require some debugging.
 
  <details>
   <summary>Expand</summary>
 
-
 I highly recommend using [comitup](https://github.com/davesteele/comitup) to setup the networking on your RPi.
 
 - Write the `comitup` [image](https://davesteele.github.io/comitup/latest/comitup-lite-img-latest.html) to your sd card
 - Boot up the RPi and setup the networking
 - ssh into your RPi, you'll probably want to change the password while you're at it
 - Enable the [SPI interface](https://www.raspberrypi-spy.co.uk/2014/08/enabling-the-spi-interface-on-the-raspberry-pi/)
 - (Optional) rename the hostname of your RPi by editing the `/etc/hostname` and `/etc/hosts` file
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: tinyticker Version: 0.5.5 Summary: A tiny Raspberry
+Metadata-Version: 2.1 Name: tinyticker Version: 0.5.6 Summary: A tiny Raspberry
 Pi powered ePaper ticker. Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance Author:
 Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Flask (>=2.0.2,<3.0.0) Requires-Dist: Pillow (>=10.0.1,<11.0.0)
-Requires-Dist: RPi.GPIO (>=0.7.0,<0.8.0) Requires-Dist: cryptocompare
-(>=0.7.5,<0.8.0) Requires-Dist: matplotlib (>=3.5.1,<4.0.0) Requires-Dist:
+Requires-Dist: cryptocompare (>=0.7.5,<0.8.0) Requires-Dist: gpiozero
+(>=2.0.1,<3.0.0) Requires-Dist: matplotlib (>=3.5.1,<4.0.0) Requires-Dist:
 mplfinance (>=0.12.7-alpha.17,<0.13.0) Requires-Dist: numpy (>=1.26,<2.0)
 Requires-Dist: packaging (>=23.0,<24.0) Requires-Dist: pandas (>=1.3.5,<2.0.0)
 Requires-Dist: qrcode (>=7.3.1,<8.0.0) Requires-Dist: spidev (>=3.5,<4.0)
 Requires-Dist: waitress (>=3.0.0,<4.0.0) Requires-Dist: watchdog
 (>=4.0.0,<5.0.0) Requires-Dist: yfinance (>=0.2.0,<0.3.0) Project-URL:
 Repository, https://github.com/loiccoyle/tinyticker Description-Content-Type:
 text/markdown
```

