# Comparing `tmp/py_ocsf_models-0.1.0.tar.gz` & `tmp/py_ocsf_models-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ocsf_models-0.1.0.tar", max compression
+gzip compressed data, was "py_ocsf_models-0.1.1.tar", max compression
```

## Comparing `py_ocsf_models-0.1.0.tar` & `py_ocsf_models-0.1.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    11345 2024-04-10 06:53:46.385317 py_ocsf_models-0.1.0/LICENSE
--rw-r--r--   0        0        0     2332 2024-04-10 06:53:46.385515 py_ocsf_models-0.1.0/README.md
--rw-r--r--   0        0        0       23 2024-04-24 14:18:36.627863 py_ocsf_models-0.1.0/py_ocsf_models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 06:53:46.386592 py_ocsf_models-0.1.0/py_ocsf_models/events/__init__.py
--rw-r--r--   0        0        0     4003 2024-04-24 14:18:36.628064 py_ocsf_models-0.1.0/py_ocsf_models/events/base_event.py
--rw-r--r--   0        0        0        0 2024-04-10 06:53:46.386832 py_ocsf_models-0.1.0/py_ocsf_models/events/findings/__init__.py
--rw-r--r--   0        0        0     7853 2024-04-24 14:18:36.628249 py_ocsf_models-0.1.0/py_ocsf_models/events/findings/detection_finding.py
--rw-r--r--   0        0        0     8441 2024-04-10 06:53:46.387180 py_ocsf_models-0.1.0/py_ocsf_models/events/findings/finding.py
--rw-r--r--   0        0        0        0 2024-04-10 06:53:46.387272 py_ocsf_models-0.1.0/py_ocsf_models/objects/__init__.py
--rw-r--r--   0        0        0     1211 2024-04-24 14:18:36.628443 py_ocsf_models-0.1.0/py_ocsf_models/objects/account.py
--rw-r--r--   0        0        0     1314 2024-04-10 06:53:46.387506 py_ocsf_models-0.1.0/py_ocsf_models/objects/api.py
--rw-r--r--   0        0        0     1151 2024-04-10 06:53:46.387609 py_ocsf_models-0.1.0/py_ocsf_models/objects/cloud.py
--rw-r--r--   0        0        0     1274 2024-04-10 06:53:46.387716 py_ocsf_models-0.1.0/py_ocsf_models/objects/container.py
--rw-r--r--   0        0        0     6676 2024-04-10 06:53:46.387841 py_ocsf_models-0.1.0/py_ocsf_models/objects/device.py
--rw-r--r--   0        0        0     3533 2024-04-10 06:53:46.387952 py_ocsf_models-0.1.0/py_ocsf_models/objects/device_hardware_info.py
--rw-r--r--   0        0        0     2078 2024-04-10 06:53:46.388069 py_ocsf_models-0.1.0/py_ocsf_models/objects/dns_query.py
--rw-r--r--   0        0        0      879 2024-04-10 06:53:46.388184 py_ocsf_models-0.1.0/py_ocsf_models/objects/enrichment.py
--rw-r--r--   0        0        0     1985 2024-04-10 06:53:46.388295 py_ocsf_models-0.1.0/py_ocsf_models/objects/evidence_artifacts.py
--rw-r--r--   0        0        0        0 2024-04-10 06:53:46.388337 py_ocsf_models-0.1.0/py_ocsf_models/objects/finding_info.py
--rw-r--r--   0        0        0     1883 2024-04-10 06:53:46.388481 py_ocsf_models-0.1.0/py_ocsf_models/objects/fingerprint.py
--rw-r--r--   0        0        0     1540 2024-04-10 06:53:46.388598 py_ocsf_models-0.1.0/py_ocsf_models/objects/geolocation.py
--rw-r--r--   0        0        0     1064 2024-04-10 06:53:46.388718 py_ocsf_models-0.1.0/py_ocsf_models/objects/group.py
--rw-r--r--   0        0        0      832 2024-04-10 06:53:46.388824 py_ocsf_models-0.1.0/py_ocsf_models/objects/image.py
--rw-r--r--   0        0        0     1431 2024-04-10 06:53:46.388928 py_ocsf_models-0.1.0/py_ocsf_models/objects/kb_article.py
--rw-r--r--   0        0        0     2735 2024-04-10 06:53:46.389041 py_ocsf_models-0.1.0/py_ocsf_models/objects/ldap_person.py
--rw-r--r--   0        0        0     5100 2024-04-10 06:53:46.389161 py_ocsf_models-0.1.0/py_ocsf_models/objects/metadata.py
--rw-r--r--   0        0        0     2996 2024-04-10 06:53:46.389267 py_ocsf_models-0.1.0/py_ocsf_models/objects/mitre_attack.py
--rw-r--r--   0        0        0     1847 2024-04-10 06:53:46.389378 py_ocsf_models-0.1.0/py_ocsf_models/objects/network_interface.py
--rw-r--r--   0        0        0     6923 2024-04-10 06:53:46.389531 py_ocsf_models-0.1.0/py_ocsf_models/objects/observable.py
--rw-r--r--   0        0        0     2320 2024-04-10 06:53:46.389663 py_ocsf_models-0.1.0/py_ocsf_models/objects/operating_system.py
--rw-r--r--   0        0        0      799 2024-04-10 06:53:46.389783 py_ocsf_models-0.1.0/py_ocsf_models/objects/organization.py
--rw-r--r--   0        0        0     1882 2024-04-10 06:53:46.389892 py_ocsf_models-0.1.0/py_ocsf_models/objects/product.py
--rw-r--r--   0        0        0     1688 2024-04-10 06:53:46.390005 py_ocsf_models-0.1.0/py_ocsf_models/objects/related_event.py
--rw-r--r--   0        0        0      822 2024-04-10 06:53:46.390107 py_ocsf_models-0.1.0/py_ocsf_models/objects/remediation.py
--rw-r--r--   0        0        0      892 2024-04-10 06:53:46.390226 py_ocsf_models-0.1.0/py_ocsf_models/objects/request_elements.py
--rw-r--r--   0        0        0     1786 2024-04-10 06:53:46.390327 py_ocsf_models-0.1.0/py_ocsf_models/objects/resource_details.py
--rw-r--r--   0        0        0     1582 2024-04-10 06:53:46.390432 py_ocsf_models-0.1.0/py_ocsf_models/objects/response_elements.py
--rw-r--r--   0        0        0      931 2024-04-10 06:53:46.390540 py_ocsf_models-0.1.0/py_ocsf_models/objects/service.py
--rw-r--r--   0        0        0     2096 2024-04-10 06:53:46.390657 py_ocsf_models-0.1.0/py_ocsf_models/objects/user.py
--rw-r--r--   0        0        0     2951 2024-04-10 06:53:46.390772 py_ocsf_models-0.1.0/py_ocsf_models/objects/vulnerability_details.py
--rw-r--r--   0        0        0     1476 2024-04-24 14:19:02.409406 py_ocsf_models-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3442 1970-01-01 00:00:00.000000 py_ocsf_models-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-03-06 15:31:21.265125 py_ocsf_models-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2332 2024-03-11 12:09:10.837734 py_ocsf_models-0.1.1/README.md
+-rw-r--r--   0        0        0       23 2024-05-17 07:25:14.303134 py_ocsf_models-0.1.1/py_ocsf_models/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-06 15:31:21.266538 py_ocsf_models-0.1.1/py_ocsf_models/events/__init__.py
+-rw-r--r--   0        0        0     4003 2024-05-17 07:25:14.303816 py_ocsf_models-0.1.1/py_ocsf_models/events/base_event.py
+-rw-r--r--   0        0        0        0 2024-03-06 15:31:21.267031 py_ocsf_models-0.1.1/py_ocsf_models/events/findings/__init__.py
+-rw-r--r--   0        0        0     7853 2024-05-17 07:25:14.304460 py_ocsf_models-0.1.1/py_ocsf_models/events/findings/detection_finding.py
+-rw-r--r--   0        0        0     8441 2024-03-11 12:09:10.840439 py_ocsf_models-0.1.1/py_ocsf_models/events/findings/finding.py
+-rw-r--r--   0        0        0        0 2024-03-06 15:31:21.267967 py_ocsf_models-0.1.1/py_ocsf_models/objects/__init__.py
+-rw-r--r--   0        0        0     1211 2024-05-17 07:25:14.304786 py_ocsf_models-0.1.1/py_ocsf_models/objects/account.py
+-rw-r--r--   0        0        0     1314 2024-03-06 15:31:21.268346 py_ocsf_models-0.1.1/py_ocsf_models/objects/api.py
+-rw-r--r--   0        0        0     1151 2024-03-06 15:31:21.268692 py_ocsf_models-0.1.1/py_ocsf_models/objects/cloud.py
+-rw-r--r--   0        0        0     1274 2024-03-06 15:31:21.268963 py_ocsf_models-0.1.1/py_ocsf_models/objects/container.py
+-rw-r--r--   0        0        0     6676 2024-03-11 12:09:10.841141 py_ocsf_models-0.1.1/py_ocsf_models/objects/device.py
+-rw-r--r--   0        0        0     3533 2024-03-06 15:31:21.269601 py_ocsf_models-0.1.1/py_ocsf_models/objects/device_hardware_info.py
+-rw-r--r--   0        0        0     2078 2024-03-11 12:09:10.841513 py_ocsf_models-0.1.1/py_ocsf_models/objects/dns_query.py
+-rw-r--r--   0        0        0      879 2024-03-11 12:09:10.841860 py_ocsf_models-0.1.1/py_ocsf_models/objects/enrichment.py
+-rw-r--r--   0        0        0     1985 2024-03-11 12:09:10.842241 py_ocsf_models-0.1.1/py_ocsf_models/objects/evidence_artifacts.py
+-rw-r--r--   0        0        0        0 2024-03-06 15:31:21.270134 py_ocsf_models-0.1.1/py_ocsf_models/objects/finding_info.py
+-rw-r--r--   0        0        0     1883 2024-03-11 12:09:10.842541 py_ocsf_models-0.1.1/py_ocsf_models/objects/fingerprint.py
+-rw-r--r--   0        0        0     1540 2024-03-06 15:31:21.270417 py_ocsf_models-0.1.1/py_ocsf_models/objects/geolocation.py
+-rw-r--r--   0        0        0     1064 2024-03-11 12:09:10.842863 py_ocsf_models-0.1.1/py_ocsf_models/objects/group.py
+-rw-r--r--   0        0        0      832 2024-03-06 15:31:21.270778 py_ocsf_models-0.1.1/py_ocsf_models/objects/image.py
+-rw-r--r--   0        0        0     1431 2024-03-06 15:31:21.271013 py_ocsf_models-0.1.1/py_ocsf_models/objects/kb_article.py
+-rw-r--r--   0        0        0     2735 2024-03-06 15:31:21.271448 py_ocsf_models-0.1.1/py_ocsf_models/objects/ldap_person.py
+-rw-r--r--   0        0        0     5100 2024-03-11 12:09:10.843189 py_ocsf_models-0.1.1/py_ocsf_models/objects/metadata.py
+-rw-r--r--   0        0        0     2996 2024-03-06 15:31:21.271939 py_ocsf_models-0.1.1/py_ocsf_models/objects/mitre_attack.py
+-rw-r--r--   0        0        0     1847 2024-03-11 12:09:10.843473 py_ocsf_models-0.1.1/py_ocsf_models/objects/network_interface.py
+-rw-r--r--   0        0        0     6923 2024-03-11 12:09:10.843766 py_ocsf_models-0.1.1/py_ocsf_models/objects/observable.py
+-rw-r--r--   0        0        0     2320 2024-03-11 12:09:10.844124 py_ocsf_models-0.1.1/py_ocsf_models/objects/operating_system.py
+-rw-r--r--   0        0        0      799 2024-03-11 12:09:10.844545 py_ocsf_models-0.1.1/py_ocsf_models/objects/organization.py
+-rw-r--r--   0        0        0     1882 2024-03-11 12:09:10.844874 py_ocsf_models-0.1.1/py_ocsf_models/objects/product.py
+-rw-r--r--   0        0        0     1688 2024-03-10 09:15:43.853081 py_ocsf_models-0.1.1/py_ocsf_models/objects/related_event.py
+-rw-r--r--   0        0        0      822 2024-03-06 15:31:21.273171 py_ocsf_models-0.1.1/py_ocsf_models/objects/remediation.py
+-rw-r--r--   0        0        0      892 2024-03-11 12:09:10.845163 py_ocsf_models-0.1.1/py_ocsf_models/objects/request_elements.py
+-rw-r--r--   0        0        0     1786 2024-03-11 12:09:10.845495 py_ocsf_models-0.1.1/py_ocsf_models/objects/resource_details.py
+-rw-r--r--   0        0        0     1582 2024-03-11 12:09:10.845781 py_ocsf_models-0.1.1/py_ocsf_models/objects/response_elements.py
+-rw-r--r--   0        0        0      931 2024-03-06 15:31:21.273846 py_ocsf_models-0.1.1/py_ocsf_models/objects/service.py
+-rw-r--r--   0        0        0     2096 2024-03-06 15:31:21.274093 py_ocsf_models-0.1.1/py_ocsf_models/objects/user.py
+-rw-r--r--   0        0        0     2951 2024-03-06 15:31:21.274373 py_ocsf_models-0.1.1/py_ocsf_models/objects/vulnerability_details.py
+-rw-r--r--   0        0        0     1477 2024-05-20 08:48:55.265979 py_ocsf_models-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3442 1970-01-01 00:00:00.000000 py_ocsf_models-0.1.1/PKG-INFO
```

### Comparing `py_ocsf_models-0.1.0/LICENSE` & `py_ocsf_models-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/README.md` & `py_ocsf_models-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/events/base_event.py` & `py_ocsf_models-0.1.1/py_ocsf_models/events/base_event.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/events/findings/detection_finding.py` & `py_ocsf_models-0.1.1/py_ocsf_models/events/findings/detection_finding.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/events/findings/finding.py` & `py_ocsf_models-0.1.1/py_ocsf_models/events/findings/finding.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/account.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/account.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/api.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/api.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/cloud.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/cloud.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/container.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/container.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/device.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/device.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/device_hardware_info.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/device_hardware_info.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/dns_query.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/dns_query.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/enrichment.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/enrichment.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/evidence_artifacts.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/evidence_artifacts.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/fingerprint.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/fingerprint.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/geolocation.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/geolocation.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/group.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/group.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/image.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/image.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/kb_article.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/kb_article.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/ldap_person.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/ldap_person.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/metadata.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/metadata.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/mitre_attack.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/mitre_attack.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/network_interface.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/network_interface.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/observable.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/observable.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/operating_system.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/operating_system.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/organization.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/organization.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/product.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/product.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/related_event.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/related_event.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/remediation.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/remediation.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/request_elements.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/request_elements.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/resource_details.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/resource_details.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/response_elements.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/response_elements.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/service.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/service.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/user.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/user.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/py_ocsf_models/objects/vulnerability_details.py` & `py_ocsf_models-0.1.1/py_ocsf_models/objects/vulnerability_details.py`

 * *Files identical despite different names*

### Comparing `py_ocsf_models-0.1.0/pyproject.toml` & `py_ocsf_models-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -21,34 +21,34 @@
   "Pepe Fagoaga <pepe@prowler.com>"
 ]
 name = "py-ocsf-models"
 packages = [
   {include = "py_ocsf_models"}
 ]
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 
 [tool.poetry.dependencies]
 email-validator = "2.1.1"
 pydantic = "1.10.15"
 python = ">=3.9,<3.13"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "1.7.8"
-black = "24.4.0"
+black = "24.4.2"
 flake8 = "7.0.0"
-mypy = "1.9.0"
-pylint = "3.1.0"
-pytest = "8.1.1"
+mypy = "1.10.0"
+pylint = "3.2.2"
+pytest = "8.2.0"
 pytest-cov = "5.0.0"
 pytest-env = "1.1.3"
 pytest-randomly = "3.15.0"
-pytest-xdist = "3.5.0"
-ruff = "0.4.1"
-safety = "3.1.0"
+pytest-xdist = "3.6.1"
+ruff = "0.4.4"
+safety = "3.2.0"
 vulture = "2.11"
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/prowler-cloud/py-ocsf-models/releases"
 "Documentation" = "https://docs.prowler.cloud"
 "Homepage" = "https://github.com/prowler-cloud/py-ocsf-models"
 "Issue tracker" = "https://github.com/prowler-cloud/py-ocsf-models/issues"
```

### Comparing `py_ocsf_models-0.1.0/PKG-INFO` & `py_ocsf_models-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ocsf-models
-Version: 0.1.0
+Version: 0.1.1
 Summary: This is a Python implementation of the OCSF models. The models are used to represent the data of the OCSF Schema defined in https://schema.ocsf.io/.
 License: Apache-2.0
 Author: Prowler Team
 Author-email: engineering@prowler.com
 Maintainer: Sergio Garcia
 Maintainer-email: sergio@prowler.com
 Requires-Python: >=3.9,<3.13
```

