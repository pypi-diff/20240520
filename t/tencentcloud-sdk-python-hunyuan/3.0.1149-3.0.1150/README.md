# Comparing `tmp/tencentcloud-sdk-python-hunyuan-3.0.1149.tar.gz` & `tmp/tencentcloud-sdk-python-hunyuan-3.0.1150.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-hunyuan-3.0.1149.tar", last modified: Thu May 16 20:42:14 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-hunyuan-3.0.1150.tar", last modified: Sun May 19 21:05:06 2024, max compression
```

## Comparing `tencentcloud-sdk-python-hunyuan-3.0.1149.tar` & `tencentcloud-sdk-python-hunyuan-3.0.1150.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:42:14.000000 tencentcloud-sdk-python-hunyuan-3.0.1149/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:42:14.000000 tencentcloud-sdk-python-hunyuan-3.0.1149/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      631 2024-05-16 20:42:14.000000 tencentcloud-sdk-python-hunyuan-3.0.1149/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:42:14.000000 tencentcloud-sdk-python-hunyuan-3.0.1149/tencentcloud/hunyuan/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:42:14.000000 tencentcloud-sdk-python-hunyuan-3.0.1149/tencentcloud/hunyuan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:42:14.000000 tencentcloud-sdk-python-hunyuan-3.0.1149/tencentcloud/hunyuan/v20230901/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:42:14.000000 tencentcloud-sdk-python-hunyuan-3.0.1149/tencentcloud/hunyuan/v20230901/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2032 2024-05-16 20:42:14.000000 tencentcloud-sdk-python-hunyuan-3.0.1149/tencentcloud/hunyuan/v20230901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    48610 2024-05-16 20:42:14.000000 tencentcloud-sdk-python-hunyuan-3.0.1149/tencentcloud/hunyuan/v20230901/models.py
--rw-r--r--   0 root         (0) root         (0)    10489 2024-05-16 20:42:14.000000 tencentcloud-sdk-python-hunyuan-3.0.1149/tencentcloud/hunyuan/v20230901/hunyuan_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:42:14.000000 tencentcloud-sdk-python-hunyuan-3.0.1149/tencentcloud_sdk_python_hunyuan.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 20:42:14.000000 tencentcloud-sdk-python-hunyuan-3.0.1149/tencentcloud_sdk_python_hunyuan.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-16 20:42:14.000000 tencentcloud-sdk-python-hunyuan-3.0.1149/tencentcloud_sdk_python_hunyuan.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-16 20:42:14.000000 tencentcloud-sdk-python-hunyuan-3.0.1149/tencentcloud_sdk_python_hunyuan.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      539 2024-05-16 20:42:14.000000 tencentcloud-sdk-python-hunyuan-3.0.1149/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1680 2024-05-16 20:42:14.000000 tencentcloud-sdk-python-hunyuan-3.0.1149/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2024-05-16 20:42:14.000000 tencentcloud-sdk-python-hunyuan-3.0.1149/README.rst
--rw-r--r--   0 root         (0) root         (0)     1081 2024-05-16 20:42:14.000000 tencentcloud-sdk-python-hunyuan-3.0.1149/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-05-16 20:42:14.000000 tencentcloud-sdk-python-hunyuan-3.0.1149/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1680 2024-05-16 20:42:14.000000 tencentcloud-sdk-python-hunyuan-3.0.1149/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:05:06.000000 tencentcloud-sdk-python-hunyuan-3.0.1150/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:05:06.000000 tencentcloud-sdk-python-hunyuan-3.0.1150/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      631 2024-05-19 21:05:06.000000 tencentcloud-sdk-python-hunyuan-3.0.1150/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:05:06.000000 tencentcloud-sdk-python-hunyuan-3.0.1150/tencentcloud/hunyuan/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 21:05:06.000000 tencentcloud-sdk-python-hunyuan-3.0.1150/tencentcloud/hunyuan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:05:06.000000 tencentcloud-sdk-python-hunyuan-3.0.1150/tencentcloud/hunyuan/v20230901/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 21:05:06.000000 tencentcloud-sdk-python-hunyuan-3.0.1150/tencentcloud/hunyuan/v20230901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2024-05-19 21:05:06.000000 tencentcloud-sdk-python-hunyuan-3.0.1150/tencentcloud/hunyuan/v20230901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    49419 2024-05-19 21:05:06.000000 tencentcloud-sdk-python-hunyuan-3.0.1150/tencentcloud/hunyuan/v20230901/models.py
+-rw-r--r--   0 root         (0) root         (0)    10489 2024-05-19 21:05:06.000000 tencentcloud-sdk-python-hunyuan-3.0.1150/tencentcloud/hunyuan/v20230901/hunyuan_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:05:06.000000 tencentcloud-sdk-python-hunyuan-3.0.1150/tencentcloud_sdk_python_hunyuan.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-19 21:05:06.000000 tencentcloud-sdk-python-hunyuan-3.0.1150/tencentcloud_sdk_python_hunyuan.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-19 21:05:06.000000 tencentcloud-sdk-python-hunyuan-3.0.1150/tencentcloud_sdk_python_hunyuan.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-19 21:05:06.000000 tencentcloud-sdk-python-hunyuan-3.0.1150/tencentcloud_sdk_python_hunyuan.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      539 2024-05-19 21:05:06.000000 tencentcloud-sdk-python-hunyuan-3.0.1150/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-05-19 21:05:06.000000 tencentcloud-sdk-python-hunyuan-3.0.1150/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2024-05-19 21:05:06.000000 tencentcloud-sdk-python-hunyuan-3.0.1150/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-05-19 21:05:06.000000 tencentcloud-sdk-python-hunyuan-3.0.1150/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-19 21:05:06.000000 tencentcloud-sdk-python-hunyuan-3.0.1150/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-05-19 21:05:06.000000 tencentcloud-sdk-python-hunyuan-3.0.1150/PKG-INFO
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1149/tencentcloud/__init__.py` & `tencentcloud-sdk-python-hunyuan-3.0.1150/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.1149'
+__version__ = '3.0.1150'
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1149/tencentcloud/hunyuan/v20230901/errorcodes.py` & `tencentcloud-sdk-python-hunyuan-3.0.1150/tencentcloud/hunyuan/v20230901/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1149/tencentcloud/hunyuan/v20230901/models.py` & `tencentcloud-sdk-python-hunyuan-3.0.1150/tencentcloud/hunyuan/v20230901/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,21 +66,29 @@
 3. 非必要不建议使用，不合理的取值会影响效果。
         :type TopP: float
         :param _Temperature: 说明：
 1. 较高的数值会使输出更加随机，而较低的数值会使其更加集中和确定。
 2. 默认 1.0，取值区间为 [0.0, 2.0]。
 3. 非必要不建议使用，不合理的取值会影响效果。
         :type Temperature: float
+        :param _EnableEnhancement: 功能增强（如搜索）开关。
+说明：
+1. 仅 hunyuan-pro 模型可用，其它版本不生效。
+2. 未传值时默认打开开关。
+3. 关闭时将直接由主模型生成回复内容，可以降低响应时延（对于流式输出时的首字时延尤为明显）。但在少数场景里，回复效果可能会下降。
+4. 安全审核能力不属于功能增强范围，不受此字段影响。
+        :type EnableEnhancement: bool
         """
         self._Model = None
         self._Messages = None
         self._Stream = None
         self._StreamModeration = None
         self._TopP = None
         self._Temperature = None
+        self._EnableEnhancement = None
 
     @property
     def Model(self):
         return self._Model
 
     @Model.setter
     def Model(self, Model):
@@ -122,27 +130,36 @@
     def Temperature(self):
         return self._Temperature
 
     @Temperature.setter
     def Temperature(self, Temperature):
         self._Temperature = Temperature
 
+    @property
+    def EnableEnhancement(self):
+        return self._EnableEnhancement
+
+    @EnableEnhancement.setter
+    def EnableEnhancement(self, EnableEnhancement):
+        self._EnableEnhancement = EnableEnhancement
+
 
     def _deserialize(self, params):
         self._Model = params.get("Model")
         if params.get("Messages") is not None:
             self._Messages = []
             for item in params.get("Messages"):
                 obj = Message()
                 obj._deserialize(item)
                 self._Messages.append(obj)
         self._Stream = params.get("Stream")
         self._StreamModeration = params.get("StreamModeration")
         self._TopP = params.get("TopP")
         self._Temperature = params.get("Temperature")
+        self._EnableEnhancement = params.get("EnableEnhancement")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1149/tencentcloud/hunyuan/v20230901/hunyuan_client.py` & `tencentcloud-sdk-python-hunyuan-3.0.1150/tencentcloud/hunyuan/v20230901/hunyuan_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1149/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-hunyuan-3.0.1150/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1149/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO` & `tencentcloud-sdk-python-hunyuan-3.0.1150/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hunyuan
-Version: 3.0.1149
+Version: 3.0.1150
 Summary: Tencent Cloud Hunyuan SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1149/README.rst` & `tencentcloud-sdk-python-hunyuan-3.0.1150/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1149/setup.py` & `tencentcloud-sdk-python-hunyuan-3.0.1150/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-hunyuan',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1149"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1150"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Hunyuan SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1149/PKG-INFO` & `tencentcloud-sdk-python-hunyuan-3.0.1150/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hunyuan
-Version: 3.0.1149
+Version: 3.0.1150
 Summary: Tencent Cloud Hunyuan SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

