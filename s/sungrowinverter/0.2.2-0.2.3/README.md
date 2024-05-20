# Comparing `tmp/sungrowinverter-0.2.2.tar.gz` & `tmp/sungrowinverter-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sungrowinverter-0.2.2.tar", max compression
+gzip compressed data, was "sungrowinverter-0.2.3.tar", max compression
```

## Comparing `sungrowinverter-0.2.2.tar` & `sungrowinverter-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      765 2022-12-12 08:25:28.519078 sungrowinverter-0.2.2/LICENSE
--rw-r--r--   0        0        0      971 2024-05-13 15:20:00.102039 sungrowinverter-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     6141 2024-05-13 15:11:12.460601 sungrowinverter-0.2.2/README.md
--rw-r--r--   0        0        0      126 2022-12-12 08:16:15.915983 sungrowinverter-0.2.2/sungrowinverter/__init__.py
--rw-r--r--   0        0        0       44 2022-12-12 08:16:24.896755 sungrowinverter-0.2.2/sungrowinverter/configs/__init.__.py
--rw-r--r--   0        0        0     3026 2022-12-12 08:17:18.584574 sungrowinverter-0.2.2/sungrowinverter/configs/common.py
--rw-r--r--   0        0        0     8230 2024-05-13 15:11:12.460601 sungrowinverter-0.2.2/sungrowinverter/configs/hybrid.py
--rw-r--r--   0        0        0     5850 2024-05-13 15:11:12.461602 sungrowinverter-0.2.2/sungrowinverter/configs/inverter.py
--rw-r--r--   0        0        0    10232 2022-12-12 08:26:34.207482 sungrowinverter-0.2.2/sungrowinverter/configs/string.py
--rw-r--r--   0        0        0    15963 2024-05-13 15:11:12.460601 sungrowinverter-0.2.2/sungrowinverter/SungrowInverter.py
--rw-r--r--   0        0        0     3950 2022-12-12 07:49:36.609548 sungrowinverter-0.2.2/sungrowinverter/SungrowModbusTCPClient.py
--rw-r--r--   0        0        0     7228 1970-01-01 00:00:00.000000 sungrowinverter-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      765 2022-12-12 08:25:28.519078 sungrowinverter-0.2.3/LICENSE
+-rw-r--r--   0        0        0      971 2024-05-20 12:57:28.094488 sungrowinverter-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6323 2024-05-20 12:52:16.869535 sungrowinverter-0.2.3/README.md
+-rw-r--r--   0        0        0      126 2022-12-12 08:16:15.915983 sungrowinverter-0.2.3/sungrowinverter/__init__.py
+-rw-r--r--   0        0        0       44 2022-12-12 08:16:24.896755 sungrowinverter-0.2.3/sungrowinverter/configs/__init.__.py
+-rw-r--r--   0        0        0     3026 2022-12-12 08:17:18.584574 sungrowinverter-0.2.3/sungrowinverter/configs/common.py
+-rw-r--r--   0        0        0     8230 2024-05-13 15:11:12.460601 sungrowinverter-0.2.3/sungrowinverter/configs/hybrid.py
+-rw-r--r--   0        0        0     5850 2024-05-13 15:11:12.461602 sungrowinverter-0.2.3/sungrowinverter/configs/inverter.py
+-rw-r--r--   0        0        0    10273 2024-05-20 12:50:43.638842 sungrowinverter-0.2.3/sungrowinverter/configs/string.py
+-rw-r--r--   0        0        0    15963 2024-05-20 12:57:25.718526 sungrowinverter-0.2.3/sungrowinverter/SungrowInverter.py
+-rw-r--r--   0        0        0     3950 2022-12-12 07:49:36.609548 sungrowinverter-0.2.3/sungrowinverter/SungrowModbusTCPClient.py
+-rw-r--r--   0        0        0     7410 1970-01-01 00:00:00.000000 sungrowinverter-0.2.3/PKG-INFO
```

### Comparing `sungrowinverter-0.2.2/LICENSE` & `sungrowinverter-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sungrowinverter-0.2.2/pyproject.toml` & `sungrowinverter-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sungrowinverter"
-version = "0.2.2"
+version = "0.2.3"
 description = "Query Sungrow residential hybrid or string inverters for current state and statistics using ModBus TCP client"
 authors = ["Mark Vandersteen <mark@vandersteen.me>"]
 license = "GNU General Public License"
 readme = "README.md"
 repository = "https://github.com/mvandersteen/SungrowInverter"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `sungrowinverter-0.2.2/README.md` & `sungrowinverter-0.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -65,21 +65,21 @@
 client.async_update()
 
 #Get a list data returned from the inverter.
 print(client.model)
 print(client.data)
 ```
 
-** of course change 192.168.1.127 to your inverter's ip address.
+** of course change 192.168.1.27 to your inverter's ip address.
 
 ## Methods and Variables
 
 ### Contructor
 
-`SungrowInverter(ip_address, port=502, slave=0x01, retries3, timeout=60)`
+`SungrowInverter(ip_address, port=502, slave=0x01, retries=3, timeout=60)`
 
 port: modbus TCP port defaults to 502 on sungrow inverters used here
 
 slave: defaulted to 0x01 as per specs your inverter may need to change this.
 
 retries: number of attempts to query the registers on the inverter before failing
 
@@ -130,10 +130,10 @@
   
 ## Python Version prior to 3.9
 
 Refer to https://github.com/mvandersteen/SungrowInverter/issues/2 if you are having issues, where @hallonstedt explains how to resolve for a prior version of python.
 
 
 ## Note
-2024-05-13: I don't have a sungrow invester to test changes on any longer as house is being rebuilt, will look to update again once new build is complete and solar re-added. For now apologies will not be muc help to anyone other than accepting merge every now and then, i don't get on here much any longer.
+2024-05-13: I don't have a sungrow invester to test changes on any longer as house is being rebuilt, will look to update again once new build is complete and solar re-added. For now apologies will not be of much help to anyone other than accepting merge every now and then.
 
-If you have an inverter not supported by this module BUT do get a response back from the sungrow inverter with a device ID, then you could follow what was done for this pull request https://github.com/mvandersteen/SungrowInverter/commit/9bef6dfcc4db7672edb1140b98bbdd34c672a987 by @ortogonal that is add an entry for your inverter in the inverter list and also if you have a 3 phase inverter (usually denoted by RT) add your inverter number into the list of support inverter for the relevant parameter data pulled from the inverter.
+If you have an inverter not supported by this module BUT do get a response back from the sungrow inverter with a device ID, then you could follow what was done for this pull request https://github.com/mvandersteen/SungrowInverter/commit/9bef6dfcc4db7672edb1140b98bbdd34c672a987 by @ortogonal; that is add an entry for your inverter in the inverter list with your deviceID defined. Then if you have a 3 phase inverter (eg. SHxxRT or SGxxRT) add your inverter deviceID returned in unsupported message into the list of valid_inverters in the registers config config sections (see hybrid.py or string.py config files), (eg. ModBusRegister(5020, "phase_b_voltage", "U16", 0.1, VOLTAGE, valid_inverters=[0xE00,0xE01,0xE02,0xE03,0xE0D,0xE0E,0xE0F,0xE13])
```

### Comparing `sungrowinverter-0.2.2/sungrowinverter/configs/common.py` & `sungrowinverter-0.2.3/sungrowinverter/configs/common.py`

 * *Files identical despite different names*

### Comparing `sungrowinverter-0.2.2/sungrowinverter/configs/hybrid.py` & `sungrowinverter-0.2.3/sungrowinverter/configs/hybrid.py`

 * *Files identical despite different names*

### Comparing `sungrowinverter-0.2.2/sungrowinverter/configs/inverter.py` & `sungrowinverter-0.2.3/sungrowinverter/configs/inverter.py`

 * *Files identical despite different names*

### Comparing `sungrowinverter-0.2.2/sungrowinverter/configs/string.py` & `sungrowinverter-0.2.3/sungrowinverter/configs/string.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,214 +1,215 @@
-"""
-#
-# Sungrow Grid Connect String Inverter Series
-#
-# Valid device types:
-#   SG3.0RT, SG4.0RT, SG5.0RT, SG6.0RT, SG7.0RT, SG8.0RT, SG10RT, SG12RT, SG15RT, SG17RT, SG20RT
-#   SG30KTL-M, SG30KTL-M-V31, SG33KTL-M, SG36KTL-M, SG33K3J, SG49K5J, SG34KJ, LP_P34KSG,
-#   SG50KTL-M-20, SG60KTL, G80KTL, SG80KTL-20, SG60KU-M
-#   SG5KTL-MT, SG6KTL-MT, SG8KTL-M, SG10KTL-M, SG10KTL-MT, SG12KTL-M, SG15KTL-M,
-#   SG17KTL-M, SG20KTL-M,
-#   SG80KTL-M, SG85BF, SG80HV, SG80BF, SG110HV-M, SG111HV, SG125HV, SG125HV-20
-#   SG25CX-SA, SG30CX, SG33CX, SG40CX, SG50CX, SG36CX-US, SG60CX-US, SG75CX, SG100CX
-#   SG100CX-JP, SG110CX, SG136TX, SG225HX, SG250HX
-#   SG250HX-IN, SG250HX-US
-#
-#   Discontinued (as @ 2021-07-12):
-#   SG30KTL, SG10KTL, SG12KTL, SG15KTL, SG20KTL, SG30KU, SG36KTL, SG36KU, SG40KTL,
-#   SG40KTL-M, SG50KTL-M, SG60KTL-M, SG60KU
-#
-# Sungrow string inverter register definitions
-"""
-
-from sungrowinverter.configs.common import (
-    ModBusRegister,
-    TEMP_CELSIUS,
-    KILO_WATT_HOUR,
-    WATT,
-    VOLTAGE,
-    AMPERE,
-    HERTZ,
-    OUTPUT_TYPE_CODES,
-    HOUR,
-    MINUTE,
-    VOLT_AMPS,
-)
-
-DEVICE_WORK_STATE_1_CODES = {
-    0x0:    "Run",
-    0x8000: "Stopped",
-    0x1300: "Key stop",
-    0x1500: "Emergency stop",
-    0x1400: "Standby",
-    0x1200: "Initial standby",
-    0x1600: "Starting",
-    0x9100: "Alarm run",
-    0x8100: "Derating run",
-    0x8200: "Dispatch run",
-    0x5500: "Fault",
-}
-
-DEVICE_WORK_STATE_2_CODES = {
-    0b0000000000000000001: "status_run",
-    0b0000000000000000010: "status_stop",
-    0b0000000000000000100: "status_key_stop",
-    0b0000000000000001000: "status_initial_standby",
-    0b0000000000000010000: "status_standby",
-    0b0000000000000100000: "status_emergency_stop",
-    0b0000000000001000000: "status_starting",
-    0b0000000001000000000: "status_fault",
-    0b0000000010000000000: "status_alarm_run",
-    0b0000000100000000000: "status_derating_run",
-    0b0000001000000000000: "status_dispatch_run",
-    0b0000010000000000000: "status_communicate_fault",
-    0b0100000000000000000: "status_grid_connected",
-    0b1000000000000000000: "status_fault_stop",
-}
-
-COUNTRY_CODES = {
-    61: "America",
-    98: "America(1741-SA)",
-    59: "America(Hawaii)",
-    97: "America(ISO-NE)",
-    27: "Arab Emirates",
-    6: "Australia",
-    20: "Australia (West)",
-    5: "Austria",
-    25: "Austria (Vorarlberg)",
-    8: "Belgium",
-    66: "Brazil",
-    60: "Canada",
-    65: "Chile",
-    14: "China",
-    67: "Chinese Taipei",
-    7: "Czech",
-    9: "Denmark",
-    76: "EN50549-1 Europe",
-    77: "EN50549-2 Europe",
-    40: "Finland",
-    2: "France",
-    1: "Germany",
-    0: "Great Britain",
-    11: "Greece (Island)",
-    10: "Greece (Land)",
-    29: "Hungary",
-    26: "IND India",
-    41: "Ireland",
-    28: "Israel",
-    3: "Italy",
-    69: "Japan",
-    63: "Korea",
-    30: "Malaysia",
-    170: "Mexico",
-    12: "Netherlands",
-    38: "Oman",
-    16: "Other 50Hz",
-    62: "Other 60Hz",
-    31: "Philippines",
-    32: "Poland",
-    34: "Poland",
-    13: "Portugal",
-    17: "Romania",
-    39: "Sandi Arabia",
-    64: "South Africa",
-    4: "Spain",
-    15: "Sweden",
-    18: "Thailand",
-    35: "Thailand-MEA",
-    19: "Turkey",
-    36: "Vietnam",
-}
-
-# the scan register start 1 less than the actual register recorded in specs.
-# reason being registers start at 0, document for modbus usually refers to register 1 as the start of registers.
-STRING_SCAN = {
-    "read": [
-        {"scan_start": 4999, "scan_range": 110},
-        {"scan_start": 5112, "scan_range": 50},
-    ],
-    "holding": [
-        {"scan_start": 4999, "scan_range": 6},
-    ],
-}
-
-STRING_READ_REGISTERS: tuple[ModBusRegister, ...] = (
-    ModBusRegister(5002, "output_type", "U16", table=OUTPUT_TYPE_CODES),
-    ModBusRegister(5003, "daily_energy_yield", "U16", 0.1, KILO_WATT_HOUR),
-    ModBusRegister(5004, "total_energy_yield", "U32", unit_of_measure=KILO_WATT_HOUR),
-    ModBusRegister(5005, "total_running_time", "U32", unit_of_measure=HOUR),
-    ModBusRegister(5008, "inside_temperature", "U16", 0.1, TEMP_CELSIUS, description="Internal inverter temperature"),
-    ModBusRegister(5009, "total_aparent_power", "U32", unit_of_measure=VOLT_AMPS),
-    ModBusRegister(5011, "mppt_1_voltage", "U16", 0.1, VOLTAGE),
-    ModBusRegister(5012, "mppt_1_current", "U16", 0.1, AMPERE),
-    ModBusRegister(5013, "mppt_2_voltage", "U16", 0.1, VOLTAGE),
-    ModBusRegister(5014, "mppt_2_current", "U16", 0.1, AMPERE),
-    ModBusRegister(5015, "mppt_3_voltage", "U16", 0.1, VOLTAGE),
-    ModBusRegister(5016, "mppt_3_current", "U16", 0.1, AMPERE),
-    ModBusRegister(5017, "total_dc_power", "U32", unit_of_measure=WATT, description="PV power that is usable (inverter after inefficiency)"),
-    ModBusRegister(5019, "grid_voltage", "U16", 0.1, VOLTAGE), # here for single phase only (not applicable for 3 phase)
-    ModBusRegister(5019, "phase_a_voltage", "U16", 0.1, VOLTAGE, description="Phase A (1-2) voltage is also the grid voltage on a single phase inverter"),
-    ModBusRegister(5020, "phase_b_voltage", "U16", 0.1, VOLTAGE),
-    ModBusRegister(5021, "phase_c_voltage", "U16", 0.1, VOLTAGE),
-    ModBusRegister(5022, "phase_a_current", "U16", 0.1, AMPERE),
-    ModBusRegister(5023, "phase_b_current", "U16", 0.1, AMPERE),
-    ModBusRegister(5024, "phase_c_current", "U16", 0.1, AMPERE),
-    ModBusRegister(5031, "total_active_power", "U32", unit_of_measure=WATT),
-    ModBusRegister(5033, "reactive_power", "S32", unit_of_measure="var"),
-    ModBusRegister(5035, "power_factor", "U16", 0.001),
-    ModBusRegister(5036, "grid_frequency", "U16", 0.1, HERTZ),
-    ModBusRegister(5038, "system_state", "U16", table=DEVICE_WORK_STATE_1_CODES),
-    ModBusRegister(5049, "nominal_reactive_power", "U16", 0.1, "kVar"),
-    ModBusRegister(5071, "array_insulation_resistance", "U16", unit_of_measure="kΩ"),
-    ModBusRegister(5038, "running_state", "U32", transform="BINARY", length=19, table=DEVICE_WORK_STATE_2_CODES, description='Tanslates into work states (refer appendix 2 of sungrow refernce)'),
-    ModBusRegister(5083, "meter_power", "S32", unit_of_measure=WATT, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
-    ModBusRegister(5085, "meter_a_phase_power", "S32", unit_of_measure=WATT, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
-    ModBusRegister(5087, "meter_b_phase_power", "S32", unit_of_measure=WATT, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
-    ModBusRegister(5089, "meter_c_phase_power", "S32", unit_of_measure=WATT, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
-    ModBusRegister(5091, "load_power", "S32", unit_of_measure=WATT, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
-    ModBusRegister(5093, "daily_export_from_pv", "U32", 0.1, KILO_WATT_HOUR, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
-    ModBusRegister(5093, "daily_export_energy", "U32", 0.1, KILO_WATT_HOUR, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
-    ModBusRegister(5095, "total_export_energy", "U32", 0.1, KILO_WATT_HOUR, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
-    ModBusRegister(5095, "total_export_from_pv", "U32", 0.1, KILO_WATT_HOUR, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
-    ModBusRegister(5097, "daily_import_energy", "U32", 0.1, KILO_WATT_HOUR, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
-    ModBusRegister(5099, "total_import_energy", "U32", 0.1, KILO_WATT_HOUR, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
-    ModBusRegister(5101, "daily_direct_energy_consumption", "U32", 0.1, KILO_WATT_HOUR, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
-    ModBusRegister(5103, "total_direct_energy_consumption", "U32", 0.1, KILO_WATT_HOUR, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
-    ModBusRegister(5113, "daily_running_time", "U16", unit_of_measure=MINUTE),
-    ModBusRegister(5114, "present_country", "U16", table=COUNTRY_CODES),
-    ModBusRegister(5115, "mppt_4_voltage", "U16", 0.1, VOLTAGE),
-    ModBusRegister(5116, "mppt_4_current", "U16", 0.1, AMPERE),
-    ModBusRegister(5117, "mppt_5_voltage", "U16", 0.1, VOLTAGE),
-    ModBusRegister(5118, "mppt_5_current", "U16", 0.1, AMPERE),
-    ModBusRegister(5119, "mppt_6_voltage", "U16", 0.1, VOLTAGE),
-    ModBusRegister(5120, "mppt_6_current", "U16", 0.1, AMPERE),
-    ModBusRegister(5121, "mppt_7_voltage", "U16", 0.1, VOLTAGE),
-    ModBusRegister(5122, "mppt_7_current", "U16", 0.1, AMPERE),
-    ModBusRegister(5123, "mppt_8_voltage", "U16", 0.1, VOLTAGE),
-    ModBusRegister(5124, "mppt_8_current", "U16", 0.1, AMPERE),
-
-    ModBusRegister(5128, "monthly_energy_yield", "U32", 0.1, KILO_WATT_HOUR),
-
-    ModBusRegister(5130, "mppt_9_voltage", "U16", 0.1, VOLTAGE),
-    ModBusRegister(5131, "mppt_9_current", "U16", 0.1, AMPERE),
-    ModBusRegister(5132, "mppt_10_voltage", "U16", 0.1, VOLTAGE),
-    ModBusRegister(5133, "mppt_10_current", "U16", 0.1, AMPERE),
-    ModBusRegister(5134, "mppt_11_voltage", "U16", 0.1, VOLTAGE),
-    ModBusRegister(5135, "mppt_11_current", "U16", 0.1, AMPERE),
-    ModBusRegister(5136, "mppt_12_voltage", "U16", 0.1, VOLTAGE),
-    ModBusRegister(5137, "mppt_12_current", "U16", 0.1, AMPERE),
-
-    ModBusRegister(5144, "total_power_yields", "U32", 0.1, KILO_WATT_HOUR,
-        valid_inverters=[0x139,0x13B,0x13C,0x13E,0x13F,0x142,0x143,0x147,0x148,0x149,
-                         0x14C,0x2430,0x2431,0x2432,0x2433,0x2434,0x2435,0x2436,0x2437,0x2437,
-                         0x243C,0x243D,0x243E,0x2C00,0x2C01,0x2C02,0x2C03,0x2C06,0x2C0A,0x2C0B,
-                         0x2C0C,0x2C0F,0x2C10,0x2C11,0x2C12,0x2C13,0x2C15,0x2C22]),
-)
-
-STRING_HOLDING_REGISTERS: tuple[ModBusRegister, ...] = (
-    ModBusRegister(5000, "year", "U16"),
-    ModBusRegister(5001, "month", "U16"),
-    ModBusRegister(5002, "day", "U16"),
-    ModBusRegister(5003, "hour", "U16"),
-    ModBusRegister(5004, "minute", "U16"),
-    ModBusRegister(5005, "second", "U16"),
+"""
+#
+# Sungrow Grid Connect String Inverter Series
+#
+# Valid device types:
+#   SG3.0RT, SG4.0RT, SG5.0RT, SG6.0RT, SG7.0RT, SG8.0RT, SG10RT, SG12RT, SG15RT, SG17RT, SG20RT
+#   SG30KTL-M, SG30KTL-M-V31, SG33KTL-M, SG36KTL-M, SG33K3J, SG49K5J, SG34KJ, LP_P34KSG,
+#   SG50KTL-M-20, SG60KTL, G80KTL, SG80KTL-20, SG60KU-M
+#   SG5KTL-MT, SG6KTL-MT, SG8KTL-M, SG10KTL-M, SG10KTL-MT, SG12KTL-M, SG15KTL-M,
+#   SG17KTL-M, SG20KTL-M,
+#   SG80KTL-M, SG85BF, SG80HV, SG80BF, SG110HV-M, SG111HV, SG125HV, SG125HV-20
+#   SG25CX-SA, SG30CX, SG33CX, SG40CX, SG50CX, SG36CX-US, SG60CX-US, SG75CX, SG100CX
+#   SG100CX-JP, SG110CX, SG136TX, SG225HX, SG250HX
+#   SG250HX-IN, SG250HX-US
+#
+#   Discontinued (as @ 2021-07-12):
+#   SG30KTL, SG10KTL, SG12KTL, SG15KTL, SG20KTL, SG30KU, SG36KTL, SG36KU, SG40KTL,
+#   SG40KTL-M, SG50KTL-M, SG60KTL-M, SG60KU
+#
+# Sungrow string inverter register definitions
+"""
+
+from sungrowinverter.configs.common import (
+    ModBusRegister,
+    TEMP_CELSIUS,
+    KILO_WATT_HOUR,
+    WATT,
+    VOLTAGE,
+    AMPERE,
+    HERTZ,
+    OUTPUT_TYPE_CODES,
+    HOUR,
+    MINUTE,
+    VOLT_AMPS,
+)
+
+DEVICE_WORK_STATE_1_CODES = {
+    0x0:    "Run",
+    0x8000: "Stopped",
+    0x1300: "Key stop",
+    0x1500: "Emergency stop",
+    0x1400: "Standby",
+    0x1200: "Initial standby",
+    0x1600: "Starting",
+    0x9100: "Alarm run",
+    0x8100: "Derating run",
+    0x8200: "Dispatch run",
+    0x5500: "Fault",
+}
+
+DEVICE_WORK_STATE_2_CODES = {
+    1 <<  0: "status_run",
+    1 <<  1: "status_stop",
+    1 <<  3: "status_key_stop",
+    1 <<  5: "status_emergency_stop",
+    1 <<  4: "status_standby",
+    1 <<  2: "status_initial_standby",
+    1 <<  6: "status_starting",
+    1 << 10: "status_alarm_run",
+    1 << 11: "status_derating_run",
+    1 << 12: "status_dispatch_run",
+    1 <<  9: "status_fault",
+    1 << 13: "status_communicate_fault",
+    1 << 17: "status_grid_connected",
+    1 << 18: "status_fault_stop",
+}
+
+COUNTRY_CODES = {
+    61: "America",
+    98: "America(1741-SA)",
+    59: "America(Hawaii)",
+    97: "America(ISO-NE)",
+    27: "Arab Emirates",
+    6: "Australia",
+    20: "Australia (West)",
+    5: "Austria",
+    25: "Austria (Vorarlberg)",
+    8: "Belgium",
+    66: "Brazil",
+    60: "Canada",
+    65: "Chile",
+    14: "China",
+    67: "Chinese Taipei",
+    7: "Czech",
+    9: "Denmark",
+    76: "EN50549-1 Europe",
+    77: "EN50549-2 Europe",
+    40: "Finland",
+    2: "France",
+    1: "Germany",
+    0: "Great Britain",
+    11: "Greece (Island)",
+    10: "Greece (Land)",
+    29: "Hungary",
+    26: "IND India",
+    41: "Ireland",
+    28: "Israel",
+    3: "Italy",
+    69: "Japan",
+    63: "Korea",
+    30: "Malaysia",
+    170: "Mexico",
+    12: "Netherlands",
+    99: "New Zealand",
+    38: "Oman",
+    16: "Other 50Hz",
+    62: "Other 60Hz",
+    31: "Philippines",
+    32: "Poland",
+    34: "Poland",
+    13: "Portugal",
+    17: "Romania",
+    39: "Sandi Arabia",
+    64: "South Africa",
+    4: "Spain",
+    15: "Sweden",
+    18: "Thailand",
+    35: "Thailand-MEA",
+    19: "Turkey",
+    36: "Vietnam",
+}
+
+# the scan register start 1 less than the actual register recorded in specs.
+# reason being registers start at 0, document for modbus usually refers to register 1 as the start of registers.
+STRING_SCAN = {
+    "read": [
+        {"scan_start": 4999, "scan_range": 110},
+        {"scan_start": 5112, "scan_range": 50},
+    ],
+    "holding": [
+        {"scan_start": 4999, "scan_range": 6},
+    ],
+}
+
+STRING_READ_REGISTERS: tuple[ModBusRegister, ...] = (
+    ModBusRegister(5002, "output_type", "U16", table=OUTPUT_TYPE_CODES),
+    ModBusRegister(5003, "daily_energy_yield", "U16", 0.1, KILO_WATT_HOUR),
+    ModBusRegister(5004, "total_energy_yield", "U32", unit_of_measure=KILO_WATT_HOUR),
+    ModBusRegister(5005, "total_running_time", "U32", unit_of_measure=HOUR),
+    ModBusRegister(5008, "inside_temperature", "U16", 0.1, TEMP_CELSIUS, description="Internal inverter temperature"),
+    ModBusRegister(5009, "total_aparent_power", "U32", unit_of_measure=VOLT_AMPS),
+    ModBusRegister(5011, "mppt_1_voltage", "U16", 0.1, VOLTAGE),
+    ModBusRegister(5012, "mppt_1_current", "U16", 0.1, AMPERE),
+    ModBusRegister(5013, "mppt_2_voltage", "U16", 0.1, VOLTAGE),
+    ModBusRegister(5014, "mppt_2_current", "U16", 0.1, AMPERE),
+    ModBusRegister(5015, "mppt_3_voltage", "U16", 0.1, VOLTAGE),
+    ModBusRegister(5016, "mppt_3_current", "U16", 0.1, AMPERE),
+    ModBusRegister(5017, "total_dc_power", "U32", unit_of_measure=WATT, description="PV power that is usable (inverter after inefficiency)"),
+    ModBusRegister(5019, "grid_voltage", "U16", 0.1, VOLTAGE), # here for single phase only (not applicable for 3 phase)
+    ModBusRegister(5019, "phase_a_voltage", "U16", 0.1, VOLTAGE, description="Phase A (1-2) voltage is also the grid voltage on a single phase inverter"),
+    ModBusRegister(5020, "phase_b_voltage", "U16", 0.1, VOLTAGE),
+    ModBusRegister(5021, "phase_c_voltage", "U16", 0.1, VOLTAGE),
+    ModBusRegister(5022, "phase_a_current", "U16", 0.1, AMPERE),
+    ModBusRegister(5023, "phase_b_current", "U16", 0.1, AMPERE),
+    ModBusRegister(5024, "phase_c_current", "U16", 0.1, AMPERE),
+    ModBusRegister(5031, "total_active_power", "U32", unit_of_measure=WATT),
+    ModBusRegister(5033, "reactive_power", "S32", unit_of_measure="var"),
+    ModBusRegister(5035, "power_factor", "U16", 0.001),
+    ModBusRegister(5036, "grid_frequency", "U16", 0.1, HERTZ),
+    ModBusRegister(5038, "system_state", "U16", table=DEVICE_WORK_STATE_1_CODES),
+    ModBusRegister(5049, "nominal_reactive_power", "U16", 0.1, "kVar"),
+    ModBusRegister(5071, "array_insulation_resistance", "U16", unit_of_measure="kΩ"),
+    ModBusRegister(5081, "running_state", "U32", transform="BINARY", length=19, table=DEVICE_WORK_STATE_2_CODES, description='Tanslates into work states (refer appendix 2 of sungrow refernce)'),
+    ModBusRegister(5083, "meter_power", "S32", unit_of_measure=WATT, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
+    ModBusRegister(5085, "meter_a_phase_power", "S32", unit_of_measure=WATT, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
+    ModBusRegister(5087, "meter_b_phase_power", "S32", unit_of_measure=WATT, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
+    ModBusRegister(5089, "meter_c_phase_power", "S32", unit_of_measure=WATT, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
+    ModBusRegister(5091, "load_power", "S32", unit_of_measure=WATT, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
+    ModBusRegister(5093, "daily_export_from_pv", "U32", 0.1, KILO_WATT_HOUR, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
+    ModBusRegister(5093, "daily_export_energy", "U32", 0.1, KILO_WATT_HOUR, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
+    ModBusRegister(5095, "total_export_energy", "U32", 0.1, KILO_WATT_HOUR, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
+    ModBusRegister(5095, "total_export_from_pv", "U32", 0.1, KILO_WATT_HOUR, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
+    ModBusRegister(5097, "daily_import_energy", "U32", 0.1, KILO_WATT_HOUR, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
+    ModBusRegister(5099, "total_import_energy", "U32", 0.1, KILO_WATT_HOUR, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
+    ModBusRegister(5101, "daily_direct_energy_consumption", "U32", 0.1, KILO_WATT_HOUR, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
+    ModBusRegister(5103, "total_direct_energy_consumption", "U32", 0.1, KILO_WATT_HOUR, valid_inverters=[0x013C,0x013E,0x013F,0x0142,0x0143,0x0147,0x0148,0x0149,0x2C0F]),
+    ModBusRegister(5113, "daily_running_time", "U16", unit_of_measure=MINUTE),
+    ModBusRegister(5114, "present_country", "U16", table=COUNTRY_CODES),
+    ModBusRegister(5115, "mppt_4_voltage", "U16", 0.1, VOLTAGE),
+    ModBusRegister(5116, "mppt_4_current", "U16", 0.1, AMPERE),
+    ModBusRegister(5117, "mppt_5_voltage", "U16", 0.1, VOLTAGE),
+    ModBusRegister(5118, "mppt_5_current", "U16", 0.1, AMPERE),
+    ModBusRegister(5119, "mppt_6_voltage", "U16", 0.1, VOLTAGE),
+    ModBusRegister(5120, "mppt_6_current", "U16", 0.1, AMPERE),
+    ModBusRegister(5121, "mppt_7_voltage", "U16", 0.1, VOLTAGE),
+    ModBusRegister(5122, "mppt_7_current", "U16", 0.1, AMPERE),
+    ModBusRegister(5123, "mppt_8_voltage", "U16", 0.1, VOLTAGE),
+    ModBusRegister(5124, "mppt_8_current", "U16", 0.1, AMPERE),
+
+    ModBusRegister(5128, "monthly_energy_yield", "U32", 0.1, KILO_WATT_HOUR),
+
+    ModBusRegister(5130, "mppt_9_voltage", "U16", 0.1, VOLTAGE),
+    ModBusRegister(5131, "mppt_9_current", "U16", 0.1, AMPERE),
+    ModBusRegister(5132, "mppt_10_voltage", "U16", 0.1, VOLTAGE),
+    ModBusRegister(5133, "mppt_10_current", "U16", 0.1, AMPERE),
+    ModBusRegister(5134, "mppt_11_voltage", "U16", 0.1, VOLTAGE),
+    ModBusRegister(5135, "mppt_11_current", "U16", 0.1, AMPERE),
+    ModBusRegister(5136, "mppt_12_voltage", "U16", 0.1, VOLTAGE),
+    ModBusRegister(5137, "mppt_12_current", "U16", 0.1, AMPERE),
+
+    ModBusRegister(5144, "total_power_yields", "U32", 0.1, KILO_WATT_HOUR,
+        valid_inverters=[0x139,0x13B,0x13C,0x13E,0x13F,0x142,0x143,0x147,0x148,0x149,
+                         0x14C,0x2430,0x2431,0x2432,0x2433,0x2434,0x2435,0x2436,0x2437,0x2437,
+                         0x243C,0x243D,0x243E,0x2C00,0x2C01,0x2C02,0x2C03,0x2C06,0x2C0A,0x2C0B,
+                         0x2C0C,0x2C0F,0x2C10,0x2C11,0x2C12,0x2C13,0x2C15,0x2C22]),
+)
+
+STRING_HOLDING_REGISTERS: tuple[ModBusRegister, ...] = (
+    ModBusRegister(5000, "year", "U16"),
+    ModBusRegister(5001, "month", "U16"),
+    ModBusRegister(5002, "day", "U16"),
+    ModBusRegister(5003, "hour", "U16"),
+    ModBusRegister(5004, "minute", "U16"),
+    ModBusRegister(5005, "second", "U16"),
 )
```

### Comparing `sungrowinverter-0.2.2/sungrowinverter/SungrowInverter.py` & `sungrowinverter-0.2.3/sungrowinverter/SungrowInverter.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Connect to a Sungrow modbus via TCP
 
 Supports Sungrow Hybrid & String inverters
 
 Refer configs/hybrid.py and configs/string.py for inverters that are supported.
 """
 
-__version__ = "0.2.1"
+__version__ = "0.2.3"
 
 from sungrowinverter.SungrowModbusTCPClient import SungrowModbusTcpClient
 from sungrowinverter.configs.inverter import (
     INVERTER_SCAN,
     INVERTER_READ_REGISTERS,
     INVERTER_HOLDING_REGISTERS,
     INVERTER_MODELS,
```

### Comparing `sungrowinverter-0.2.2/sungrowinverter/SungrowModbusTCPClient.py` & `sungrowinverter-0.2.3/sungrowinverter/SungrowModbusTCPClient.py`

 * *Files identical despite different names*

### Comparing `sungrowinverter-0.2.2/PKG-INFO` & `sungrowinverter-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sungrowinverter
-Version: 0.2.2
+Version: 0.2.3
 Summary: Query Sungrow residential hybrid or string inverters for current state and statistics using ModBus TCP client
 Home-page: https://github.com/mvandersteen/SungrowInverter
 License: GNU General Public License
 Author: Mark Vandersteen
 Author-email: mark@vandersteen.me
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -92,21 +92,21 @@
 client.async_update()
 
 #Get a list data returned from the inverter.
 print(client.model)
 print(client.data)
 ```
 
-** of course change 192.168.1.127 to your inverter's ip address.
+** of course change 192.168.1.27 to your inverter's ip address.
 
 ## Methods and Variables
 
 ### Contructor
 
-`SungrowInverter(ip_address, port=502, slave=0x01, retries3, timeout=60)`
+`SungrowInverter(ip_address, port=502, slave=0x01, retries=3, timeout=60)`
 
 port: modbus TCP port defaults to 502 on sungrow inverters used here
 
 slave: defaulted to 0x01 as per specs your inverter may need to change this.
 
 retries: number of attempts to query the registers on the inverter before failing
 
@@ -157,11 +157,11 @@
   
 ## Python Version prior to 3.9
 
 Refer to https://github.com/mvandersteen/SungrowInverter/issues/2 if you are having issues, where @hallonstedt explains how to resolve for a prior version of python.
 
 
 ## Note
-2024-05-13: I don't have a sungrow invester to test changes on any longer as house is being rebuilt, will look to update again once new build is complete and solar re-added. For now apologies will not be muc help to anyone other than accepting merge every now and then, i don't get on here much any longer.
+2024-05-13: I don't have a sungrow invester to test changes on any longer as house is being rebuilt, will look to update again once new build is complete and solar re-added. For now apologies will not be of much help to anyone other than accepting merge every now and then.
 
-If you have an inverter not supported by this module BUT do get a response back from the sungrow inverter with a device ID, then you could follow what was done for this pull request https://github.com/mvandersteen/SungrowInverter/commit/9bef6dfcc4db7672edb1140b98bbdd34c672a987 by @ortogonal that is add an entry for your inverter in the inverter list and also if you have a 3 phase inverter (usually denoted by RT) add your inverter number into the list of support inverter for the relevant parameter data pulled from the inverter.
+If you have an inverter not supported by this module BUT do get a response back from the sungrow inverter with a device ID, then you could follow what was done for this pull request https://github.com/mvandersteen/SungrowInverter/commit/9bef6dfcc4db7672edb1140b98bbdd34c672a987 by @ortogonal; that is add an entry for your inverter in the inverter list with your deviceID defined. Then if you have a 3 phase inverter (eg. SHxxRT or SGxxRT) add your inverter deviceID returned in unsupported message into the list of valid_inverters in the registers config config sections (see hybrid.py or string.py config files), (eg. ModBusRegister(5020, "phase_b_voltage", "U16", 0.1, VOLTAGE, valid_inverters=[0xE00,0xE01,0xE02,0xE03,0xE0D,0xE0E,0xE0F,0xE13])
```

