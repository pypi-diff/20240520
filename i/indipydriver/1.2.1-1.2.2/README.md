# Comparing `tmp/indipydriver-1.2.1.tar.gz` & `tmp/indipydriver-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipydriver-1.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "indipydriver-1.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `indipydriver-1.2.1.tar` & `indipydriver-1.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-07-31 15:52:08.000000 indipydriver-1.2.1/LICENSE
--rw-r--r--   0        0        0     2469 2024-04-18 11:52:22.000000 indipydriver-1.2.1/README.md
--rw-r--r--   0        0        0      573 2024-05-18 22:07:32.000000 indipydriver-1.2.1/indipydriver/__init__.py
--rw-r--r--   0        0        0    21484 2024-05-18 21:58:43.000000 indipydriver-1.2.1/indipydriver/comms.py
--rw-r--r--   0        0        0    24981 2024-05-16 20:54:58.000000 indipydriver-1.2.1/indipydriver/events.py
--rw-r--r--   0        0        0    21236 2024-05-16 20:30:24.000000 indipydriver-1.2.1/indipydriver/ipydriver.py
--rw-r--r--   0        0        0    11494 2024-05-18 21:50:05.000000 indipydriver-1.2.1/indipydriver/ipyserver.py
--rw-r--r--   0        0        0    12256 2024-05-16 20:34:45.000000 indipydriver-1.2.1/indipydriver/propertymembers.py
--rw-r--r--   0        0        0    43286 2024-04-25 22:33:51.000000 indipydriver-1.2.1/indipydriver/propertyvectors.py
--rw-r--r--   0        0        0      814 2024-05-18 22:07:10.000000 indipydriver-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 indipydriver-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-31 15:52:08.000000 indipydriver-1.2.2/LICENSE
+-rw-r--r--   0        0        0     2469 2024-04-18 11:52:22.000000 indipydriver-1.2.2/README.md
+-rw-r--r--   0        0        0      658 2024-05-20 09:54:27.000000 indipydriver-1.2.2/indipydriver/__init__.py
+-rw-r--r--   0        0        0    18853 2024-05-19 21:11:41.000000 indipydriver-1.2.2/indipydriver/comms.py
+-rw-r--r--   0        0        0    24981 2024-05-16 20:54:58.000000 indipydriver-1.2.2/indipydriver/events.py
+-rw-r--r--   0        0        0    22537 2024-05-19 21:52:18.000000 indipydriver-1.2.2/indipydriver/ipydriver.py
+-rw-r--r--   0        0        0    11485 2024-05-19 21:17:11.000000 indipydriver-1.2.2/indipydriver/ipyserver.py
+-rw-r--r--   0        0        0    12256 2024-05-16 20:34:45.000000 indipydriver-1.2.2/indipydriver/propertymembers.py
+-rw-r--r--   0        0        0    43660 2024-05-19 21:32:10.000000 indipydriver-1.2.2/indipydriver/propertyvectors.py
+-rw-r--r--   0        0        0      814 2024-05-20 09:54:15.000000 indipydriver-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 indipydriver-1.2.2/PKG-INFO
```

### Comparing `indipydriver-1.2.1/LICENSE` & `indipydriver-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `indipydriver-1.2.1/README.md` & `indipydriver-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `indipydriver-1.2.1/indipydriver/__init__.py` & `indipydriver-1.2.2/indipydriver/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 
 
+
+import logging
+logging.getLogger('indipydriver').addHandler(logging.NullHandler())
+
 from .ipydriver import IPyDriver, Device
 from .propertyvectors import SwitchVector, LightVector, TextVector, BLOBVector, NumberVector
 from .propertymembers import SwitchMember, LightMember, TextMember, BLOBMember, NumberMember
 from .events import getProperties, enableBLOB, newSwitchVector, newTextVector, newNumberVector, newBLOBVector, Message, delProperty, defSwitchVector, defTextVector, defNumberVector, defLightVector, defBLOBVector, setSwitchVector, setTextVector, setNumberVector, setLightVector, setBLOBVector
 from .ipyserver import IPyServer
 
-version = "1.2.1"
+version = "1.2.2"
```

### Comparing `indipydriver-1.2.1/indipydriver/comms.py` & `indipydriver-1.2.2/indipydriver/comms.py`

 * *Files 20% similar despite different names*

```diff
@@ -78,73 +78,46 @@
 
 
 class STDOUT_TX:
     "An object that transmits data on stdout, used by STDINOUT as one half of the communications path"
 
     async def run_tx(self, writerque):
         """Gets data from writerque, and transmits it out on stdout"""
-        if logger.isEnabledFor(logging.DEBUG):
-            logenabled = True
-        else:
-            logenabled = False
         while True:
             await asyncio.sleep(0)
             # get block of data from writerque and transmit down stdout
             txdata = await writerque.get()
             writerque.task_done()
             if (txdata.tag == "setBLOBVector") and len(txdata):
                 # txdata is a setBLOBVector containing blobs
                 # the generator blob_xml_bytes yields bytes
                 for binarydata in blob_xml_bytes(txdata):
                     # transmit the data
                     sys.stdout.buffer.write(binarydata)
                     sys.stdout.buffer.flush()
                     await asyncio.sleep(0)
-                if logenabled:
-                    copytx = copy.deepcopy(txdata)
-                    for element in copytx:
-                        element.text = "NOT LOGGED"
-                    binarydata = ET.tostring(copytx)
-                    logger.debug(f"TX:{binarydata.decode('utf-8')}")
             else:
                 # its straight xml, send it out on stdout
                 binarydata = ET.tostring(txdata)
                 binarydata += b"\n"
                 sys.stdout.buffer.write(binarydata)
                 sys.stdout.buffer.flush()
-                if logenabled:
-                    logger.debug(f"TX:{binarydata.decode('utf-8')}")
 
 
 class STDIN_RX:
     """An object that receives data, parses it to ElementTree elements
        and passes it to the driver by appending it to the driver's readerque"""
 
     async def run_rx(self, readerque):
         "pass data to readerque"
         source = self.datasource()
-        if logger.isEnabledFor(logging.DEBUG):
-            logenabled = True
-        else:
-            logenabled = False
         async for rxdata in source:
             # get block of xml.etree.ElementTree data
             # from source and append it to  readerque
             await readerque.put(rxdata)
-            if logenabled:
-                if (rxdata.tag == "setBLOBVector" or rxdata.tag == "newBLOBVector") and len(rxdata):
-                    # rxdata contains blobs
-                    copyrx = copy.deepcopy(rxdata)
-                    for element in copyrx:
-                        element.text = "NOT LOGGED"
-                    binarydata = ET.tostring(copyrx)
-                    logger.debug(f"RX:{binarydata.decode('utf-8')}")
-                else:
-                    binarydata = ET.tostring(rxdata)
-                    logger.debug(f"RX:{binarydata.decode('utf-8')}")
 
 
     async def datasource(self):
         # get received data, parse it, and yield it as xml.etree.ElementTree object
         data_in = self.datainput()
         message = b''
         messagetagnumber = None
@@ -231,32 +204,28 @@
         # Set stdin to non-blocking mode
         flags = fcntl.fcntl(sys.stdin.fileno(), fcntl.F_GETFL)
         fcntl.fcntl(sys.stdin.fileno(), fcntl.F_SETFL, flags | os.O_NONBLOCK)
 
         rx = STDIN_RX()
         tx = STDOUT_TX()
 
-        logger.warning("Listening on STDIN")
+        logger.info("Listening on STDIN")
 
         await asyncio.gather(rx.run_rx(readerque),
                              tx.run_tx(writerque)
                              )
 
 class Port_TX():
     "An object that transmits data on a port, used by Portcomms as one half of the communications path"
 
     def __init__(self, blobstatus, writer, timer):
         self.blobstatus = blobstatus
         self.writer = writer
         self.timer = timer
-        self.addr = writer.get_extra_info('peername')
-        if logger.isEnabledFor(logging.DEBUG):
-            self.logenabled = True
-        else:
-            self.logenabled = False
+
 
     async def run_tx(self, writerque):
         """Gets data from writerque, and transmits it out on the port writer"""
         while True:
             await asyncio.sleep(0)
             # get block of data from writerque and transmit
             txdata = await writerque.get()
@@ -271,67 +240,45 @@
                 # txdata is a setBLOBVector containing blobs
                 # the generator blob_xml_bytes yields bytes
                 for binarydata in blob_xml_bytes(txdata):
                     # Send to the port
                     self.timer.update()
                     self.writer.write(binarydata)
                     await self.writer.drain()
-                if self.logenabled:
-                    copytx = copy.deepcopy(txdata)
-                    for element in copytx:
-                        element.text = "NOT LOGGED"
-                    binarydata = ET.tostring(copytx)
-                    logger.debug(f"TX:{self.addr}:{binarydata.decode('utf-8')}")
             else:
                 # its straight xml, send it out on the port
                 binarydata = ET.tostring(txdata)
-                if self.logenabled:
-                    logger.debug(f"TX:{self.addr}:{binarydata.decode('utf-8')}")
                 # Send to the port
                 self.timer.update()
                 self.writer.write(binarydata)
                 await self.writer.drain()
 
 
 class Port_RX(STDIN_RX):
     """Produces xml.etree.ElementTree data from data received on the port,
        this is used by Portcomms as one half of the communications path.
        This overwrites methods of the STDIN_RX parent class."""
 
-    def __init__(self, blobstatus, reader, addr):
+    def __init__(self, blobstatus, reader):
         self.blobstatus = blobstatus
         self.reader = reader
-        self.addr = addr
-        if logger.isEnabledFor(logging.DEBUG):
-            self.logenabled = True
-        else:
-            self.logenabled = False
+
 
     async def run_rx(self, readerque):
         "pass data to readerque"
         source = self.datasource()
         async for rxdata in source:
             # get block of xml.etree.ElementTree data
             # from source and append it to  readerque
             if rxdata.tag == "enableBLOB":
                 # set permission flags in the blobstatus object
                 self.blobstatus.setpermissions(rxdata)
             # and place rxdata into readerque
             await readerque.put(rxdata)
-            if self.logenabled:
-                if (rxdata.tag == "setBLOBVector" or rxdata.tag == "newBLOBVector") and len(rxdata):
-                    # rxdata contains blobs
-                    copyrx = copy.deepcopy(rxdata)
-                    for element in copyrx:
-                        element.text = "NOT LOGGED"
-                    binarydata = ET.tostring(copyrx)
-                    logger.debug(f"RX:{self.addr}:{binarydata.decode('utf-8')}")
-                else:
-                    binarydata = ET.tostring(rxdata)
-                    logger.debug(f"RX:{self.addr}:{binarydata.decode('utf-8')}")
+
 
 
     async def datainput(self):
         "Generator producing binary string of data from the port"
         binarydata = b""
         while True:
             await asyncio.sleep(0)
@@ -390,15 +337,15 @@
         # the connection
         self.timer = TXTimer(timeout = 15)
 
     async def __call__(self, readerque, writerque):
         "Called from indipydriver.asyncrun() to run the communications"
         self.readerque = readerque
         self.writerque = writerque
-        logger.warning(f"Listening on {self.host} : {self.port}")
+        logger.info(f"Listening on {self.host} : {self.port}")
         server = await asyncio.start_server(self.handle_data, self.host, self.port)
         await server.serve_forever()
 
 
     async def _monitor_connection(self):
         """If connected and not transmitting, send def vectors every self.timeout seconds
            This ensures that if the connection has failed, due to the client disconnecting, the write
@@ -422,15 +369,15 @@
         if self.connected:
             # already connected, can only handle one connection
             writer.close()
             await writer.wait_closed()
             return
         self.connected = True
         addr = writer.get_extra_info('peername')
-        rx = Port_RX(self.blobstatus, reader, addr)
+        rx = Port_RX(self.blobstatus, reader)
         tx = Port_TX(self.blobstatus, writer, self.timer)
         logger.info(f"Connection received from {addr}")
         try:
             txtask = asyncio.create_task(tx.run_tx(self.writerque))
             rxtask = asyncio.create_task(rx.run_rx(self.readerque))
             montask = asyncio.create_task(self._monitor_connection())
             await asyncio.gather(txtask, rxtask, montask)
```

### Comparing `indipydriver-1.2.1/indipydriver/events.py` & `indipydriver-1.2.2/indipydriver/events.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.2.1/indipydriver/ipydriver.py` & `indipydriver-1.2.2/indipydriver/ipydriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,17 @@
         # These set the remote traffic which this driver is snooping
         # initially the driver is not snooping anything, until it sends
         # a getProperties
         self.snoopall = False           # gets set to True if it is snooping everything
         self.snoopdevices = set()       # gets set to a set of device names
         self.snoopvectors = set()       # gets set to a set of (devicename,vectorname) tuples
 
+        # If True, xmldata will be logged at DEBUG level
+        self.debug_enable = True
+
 
     def listen(self, host="localhost", port=7624):
         """If called, listens on the given host and port. Only one connection is accepted,
            further connection attempts while a client is already connected will be refused.
            This method also checks for enableBLOB instructions, and implements them.
            In general, using IPyServer is preferred."""
         if not self.comms is None:
@@ -128,27 +131,49 @@
         self.comms = Portcomms(self.devices, host, port)
 
 
     async def send(self, xmldata):
         "Transmits xmldata, this is an internal method, not normally called by a user."
         if self.comms.connected:
             await self.writerque.put(xmldata)
+            if logger.isEnabledFor(logging.DEBUG) and self.debug_enable:
+                if (xmldata.tag == "setBLOBVector") and len(xmldata):
+                    data = copy.deepcopy(xmldata)
+                    for element in data:
+                        element.text = "NOT LOGGED"
+                    binarydata = ET.tostring(data)
+                    logger.debug(f"TX:: {binarydata.decode('utf-8')}")
+                else:
+                    binarydata = ET.tostring(xmldata)
+                    logger.debug(f"TX:: {binarydata.decode('utf-8')}")
+
 
     def __setitem__(self, devicename):
         raise KeyError
 
     async def _read_readerque(self):
         client_tags = ("enableBLOB", "newSwitchVector", "newNumberVector", "newTextVector", "newBLOBVector")
         snoop_tags = ("message", 'delProperty', 'defSwitchVector', 'setSwitchVector', 'defLightVector',
                       'setLightVector', 'defTextVector', 'setTextVector', 'defNumberVector', 'setNumberVector',
                       'defBLOBVector', 'setBLOBVector')
         while True:
             await asyncio.sleep(0)
             # reads readerque, and sends xml data to the device via its dataque
             root = await self.readerque.get()
+            # log the received data
+            if logger.isEnabledFor(logging.DEBUG) and self.debug_enable:
+                if ((root.tag == "setBLOBVector") or (root.tag == "newBLOBVector")) and len(root):
+                    data = copy.deepcopy(root)
+                    for element in data:
+                        element.text = "NOT LOGGED"
+                    binarydata = ET.tostring(data)
+                    logger.debug(f"RX:: {binarydata.decode('utf-8')}")
+                else:
+                    binarydata = ET.tostring(root)
+                    logger.debug(f"RX:: {binarydata.decode('utf-8')}")
             if root.tag == "getProperties":
                 version = root.get("version")
                 if version != "1.7":
                     self.readerque.task_done()
                     continue
                 # getProperties received with correct version
                 devicename = root.get("device")
@@ -240,15 +265,15 @@
                 elif root.tag == "setBLOBVector":
                     # create event
                     event = events.setBLOBVector(root)
                     await self.snoopevent(event)
             except events.EventException as ex:
                 # if an EventException is raised, it is because received data is malformed
                 # so log it
-                logger.error(str(ex))
+                logger.exception("An exception occurred creating a snoop event")
             self.snoopque.task_done()
 
     async def send_message(self, message="", timestamp=None):
         "Send system wide message - without device name"
         tstring = timestamp_string(timestamp)
         if not tstring:
             logger.error("The timestamp given in send_message must be a datetime.datetime UTC object")
@@ -311,15 +336,15 @@
            any necessary actions.
            event is an object with attributes according to the data received."""
         pass
 
     async def asyncrun(self):
         """Gathers tasks to be run simultaneously"""
 
-        logger.warning(f"Driver {self.__class__.__name__} started")
+        logger.info(f"Driver {self.__class__.__name__} started")
 
         # set an object for communicating, as default this is stdin and stdout
         if self.comms is None:
             self.comms = STDINOUT()
 
         # get all tasks into a list
         self._tasks.append( self.comms(self.readerque, self.writerque) )    # run communications
```

### Comparing `indipydriver-1.2.1/indipydriver/ipyserver.py` & `indipydriver-1.2.2/indipydriver/ipyserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
         self.drivers = drivers
         self.host = host
         self.port = port
 
     async def _runserver(self):
         "Runs the server on the given host and port"
-        logger.warning(f"{self.__class__.__name__} listening on {self.host} : {self.port}")
+        logger.info(f"{self.__class__.__name__} listening on {self.host} : {self.port}")
         server = await asyncio.start_server(self.handle_data, self.host, self.port)
         await server.serve_forever()
 
 
     async def handle_data(self, reader, writer):
         "Used by asyncio.start_server, called to handle a client connection"
 
@@ -247,15 +247,15 @@
 
 
     async def handle_data(self, reader, writer):
         "Used by asyncio.start_server, called to handle a client connection"
         self.connected = True
         blobstatus = BLOBSstatus(self.devices)
         addr = writer.get_extra_info('peername')
-        rx = Port_RX(blobstatus, reader, addr)
+        rx = Port_RX(blobstatus, reader)
         tx = Port_TX(blobstatus, writer, self.timer)
         logger.info(f"Connection received from {addr}")
         try:
             txtask = asyncio.create_task(tx.run_tx(self.txque))
             rxtask = asyncio.create_task(rx.run_rx(self.serverreaderque))
             montask = asyncio.create_task(self._monitor_connection())
             await asyncio.gather(txtask, rxtask, montask)
```

### Comparing `indipydriver-1.2.1/indipydriver/propertymembers.py` & `indipydriver-1.2.2/indipydriver/propertymembers.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.2.1/indipydriver/propertyvectors.py` & `indipydriver-1.2.2/indipydriver/propertyvectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,21 +131,21 @@
         return self._state
 
     @state.setter
     def state(self, value):
         try:
             self._state = self.checkvalue(value, ['Idle','Ok','Busy','Alert'])
         except ValueError as ex:
-            logger.error(str(ex))
+            logger.exception("Invalid state value")
 
     def __setitem__(self, membername, value):
         try:
             self.data[membername].membervalue = value
         except ValueError as ex:
-            logger.error(str(ex))
+            logger.exception("Unable to set value")
 
     def __getitem__(self, membername):
         return self.data[membername].membervalue
 
 
 class SwitchVector(PropertyVector):
 
@@ -175,26 +175,26 @@
         return self._perm
 
     @perm.setter
     def perm(self, value):
         try:
             self._perm = self.checkvalue(value, ['ro','wo','rw'])
         except ValueError as ex:
-            logger.error(str(ex))
+            logger.exception("Invalid permission value")
 
     @property
     def rule(self):
         return self._rule
 
     @rule.setter
     def rule(self, value):
         try:
             self._rule = self.checkvalue(value, ['OneOfMany','AtMostOne','AnyOfMany'])
         except ValueError as ex:
-            logger.error(str(ex))
+            logger.exception("Invalid rule value")
 
     async def _handler(self):
         """Check received data and take action"""
         while True:
             await asyncio.sleep(0)
             try:
                 root = await self.dataque.get()
@@ -204,15 +204,15 @@
                     await self.driver.clientevent(event)
                 elif root.tag == "newSwitchVector":
                     # create event
                     event = newSwitchVector(self.devicename, self.name, self, root)
                     await self.driver.clientevent(event)
             except EventException as ex:
                 # if an error is raised parsing the incoming data, just continue
-                logger.error(str(ex))
+                logger.exception("Unable to create event from received data")
             self.dataque.task_done()
 
 
     def _make_defVector(self, message='', timestamp=None):
         "Creates xml data object for vector definition"
         if not self.device.enable:
             return
@@ -392,15 +392,15 @@
                 root = await self.dataque.get()
                 if root.tag == "getProperties":
                     # create event
                     event = getProperties(self.devicename, self.name, self, root)
                     await self.driver.clientevent(event)
             except EventException as ex:
                 # if an error is raised parsing the incoming data, just continue
-                logger.error(str(ex))
+                logger.exception("Unable to create event from received data")
             self.dataque.task_done()
 
     @property
     def perm(self):
         return "ro"
 
     def _make_defVector(self, message='', timestamp=None):
@@ -539,15 +539,15 @@
         return self._perm
 
     @perm.setter
     def perm(self, value):
         try:
             self._perm = self.checkvalue(value, ['ro','wo','rw'])
         except ValueError as ex:
-            logger.error(str(ex))
+            logger.exception("Invalid permission value")
 
     async def _handler(self):
         """Check received data and take action"""
         while True:
             await asyncio.sleep(0)
             try:
                 root = await self.dataque.get()
@@ -557,15 +557,15 @@
                     await self.driver.clientevent(event)
                 elif root.tag == "newTextVector":
                     # create event
                     event = newTextVector(self.devicename, self.name, self, root)
                     await self.driver.clientevent(event)
             except EventException as ex:
                 # if an error is raised parsing the incoming data, just continue
-                logger.error(str(ex))
+                logger.exception("Unable to create event from received data")
             self.dataque.task_done()
 
     def _make_defVector(self, message='', timestamp=None):
         "Creates xml data object for vector definition"
         if not self.device.enable:
             return
         if not self.enable:
@@ -717,15 +717,15 @@
         return self._perm
 
     @perm.setter
     def perm(self, value):
         try:
             self._perm = self.checkvalue(value, ['ro','wo','rw'])
         except ValueError as ex:
-            logger.error(str(ex))
+            logger.exception("Invalid permission value")
 
     async def _handler(self):
         """Check received data and take action"""
         while True:
             await asyncio.sleep(0)
             try:
                 root = await self.dataque.get()
@@ -735,15 +735,15 @@
                     await self.driver.clientevent(event)
                 elif root.tag == "newNumberVector":
                     # create event
                     event = newNumberVector(self.devicename, self.name, self, root)
                     await self.driver.clientevent(event)
             except EventException as ex:
                 # if an error is raised parsing the incoming data, just continue
-                logger.error(str(ex))
+                logger.exception("Unable to create event from received data")
             self.dataque.task_done()
 
     def _make_defVector(self, message='', timestamp=None):
         "Creates xml data object for vector definition"
         if not self.device.enable:
             return
         if not self.enable:
@@ -910,15 +910,15 @@
         return self._perm
 
     @perm.setter
     def perm(self, value):
         try:
             self._perm = self.checkvalue(value, ['ro','wo','rw'])
         except ValueError as ex:
-            logger.error(str(ex))
+            logger.exception("Invalid permission value")
 
     async def _handler(self):
         """Check received data and take action"""
         while True:
             await asyncio.sleep(0)
             try:
                 root = await self.dataque.get()
@@ -932,15 +932,15 @@
                     await self.driver.clientevent(event)
                 elif root.tag == "newBLOBVector":
                     # create event
                     event = newBLOBVector(self.devicename, self.name, self, root)
                     await self.driver.clientevent(event)
             except EventException as ex:
                 # if an error is raised parsing the incoming data, just continue
-                logger.error(str(ex))
+                logger.exception("Unable to create event from received data")
             self.dataque.task_done()
 
     def _make_defVector(self, message='', timestamp=None):
         "Creates xml data object for vector definition"
         if not self.device.enable:
             return
         if not self.enable:
@@ -1009,9 +1009,9 @@
         if message:
             xmldata.set("message", message)
         for blob in self.data.values():
             if (blob.name in members) and (blob.membervalue is not None):
                 try:
                     xmldata.append(blob.oneblob())
                 except ValueError as ex:
-                    logger.error(str(ex))
+                    logger.exception("Unable to create setBLOBVector")
         await self.driver.send(xmldata)
```

### Comparing `indipydriver-1.2.1/pyproject.toml` & `indipydriver-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipydriver"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "1.2.1"
+version = "1.2.2"
 description="Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'driver', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipydriver.readthedocs.io"
```

### Comparing `indipydriver-1.2.1/PKG-INFO` & `indipydriver-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indipydriver
-Version: 1.2.1
+Version: 1.2.2
 Summary: Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver.
 Keywords: indi,driver,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

