# Comparing `tmp/qtmodel-0.3.4.tar.gz` & `tmp/qtmodel-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtmodel-0.3.4.tar", last modified: Fri May 17 07:11:14 2024, max compression
+gzip compressed data, was "qtmodel-0.3.5.tar", last modified: Mon May 20 02:54:00 2024, max compression
```

## Comparing `qtmodel-0.3.4.tar` & `qtmodel-0.3.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 07:11:14.711145 qtmodel-0.3.4/
--rw-rw-rw-   0        0        0    37701 2024-05-17 07:11:14.711145 qtmodel-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0    37273 2024-05-13 05:54:03.000000 qtmodel-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 07:11:14.702908 qtmodel-0.3.4/qtmodel/
--rw-rw-rw-   0        0        0       91 2024-05-17 07:08:34.000000 qtmodel-0.3.4/qtmodel/__init__.py
--rw-rw-rw-   0        0        0    83827 2024-05-16 02:19:25.000000 qtmodel-0.3.4/qtmodel/qt_mdb.py
--rw-rw-rw-   0        0        0     8492 2024-05-17 07:07:31.000000 qtmodel-0.3.4/qtmodel/qt_odb.py
--rw-rw-rw-   0        0        0     1029 2024-05-17 05:05:06.000000 qtmodel-0.3.4/qtmodel/qt_operate.py
--rw-rw-rw-   0        0        0     9890 2024-05-17 07:07:30.000000 qtmodel-0.3.4/qtmodel/res_db.py
-drwxrwxrwx   0        0        0        0 2024-05-17 07:11:14.708909 qtmodel-0.3.4/qtmodel.egg-info/
--rw-rw-rw-   0        0        0    37701 2024-05-17 07:11:14.000000 qtmodel-0.3.4/qtmodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-17 07:11:14.000000 qtmodel-0.3.4/qtmodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 07:11:14.000000 qtmodel-0.3.4/qtmodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-17 07:11:14.000000 qtmodel-0.3.4/qtmodel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 07:11:14.711145 qtmodel-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      758 2024-05-17 07:11:08.000000 qtmodel-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:54:00.705455 qtmodel-0.3.5/
+-rw-rw-rw-   0        0        0    37701 2024-05-20 02:54:00.704149 qtmodel-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0    37273 2024-05-13 05:54:03.000000 qtmodel-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 02:54:00.697132 qtmodel-0.3.5/qtmodel/
+-rw-rw-rw-   0        0        0       91 2024-05-17 07:08:34.000000 qtmodel-0.3.5/qtmodel/__init__.py
+-rw-rw-rw-   0        0        0      443 2024-05-20 02:17:18.000000 qtmodel-0.3.5/qtmodel/qt_db.py
+-rw-rw-rw-   0        0        0     2386 2024-05-20 02:22:27.000000 qtmodel-0.3.5/qtmodel/qt_helper.py
+-rw-rw-rw-   0        0        0    83069 2024-05-20 02:31:09.000000 qtmodel-0.3.5/qtmodel/qt_mdb.py
+-rw-rw-rw-   0        0        0     8827 2024-05-17 07:53:59.000000 qtmodel-0.3.5/qtmodel/qt_odb.py
+-rw-rw-rw-   0        0        0    14370 2024-05-20 02:45:48.000000 qtmodel-0.3.5/qtmodel/res_db.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:54:00.702770 qtmodel-0.3.5/qtmodel.egg-info/
+-rw-rw-rw-   0        0        0    37701 2024-05-20 02:54:00.000000 qtmodel-0.3.5/qtmodel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-20 02:54:00.000000 qtmodel-0.3.5/qtmodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 02:54:00.000000 qtmodel-0.3.5/qtmodel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-20 02:54:00.000000 qtmodel-0.3.5/qtmodel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 02:54:00.705455 qtmodel-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      758 2024-05-20 02:53:48.000000 qtmodel-0.3.5/setup.py
```

### Comparing `qtmodel-0.3.4/PKG-INFO` & `qtmodel-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmodel
-Version: 0.3.4
+Version: 0.3.5
 Summary: python modeling for qt  24/05/06 
 Home-page: https://github.com/Inface0443/pyqt
 Author: dqy-zhj
 Author-email: 1105417715@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qtmodel-0.3.4/README.md` & `qtmodel-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `qtmodel-0.3.4/qtmodel/qt_mdb.py` & `qtmodel-0.3.5/qtmodel/qt_mdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,33 @@
     """
     Mdb类负责建模相关操作
     """
 
     def __int__(self):
         self.initial()
 
+    # region 获取模型信息
+    @staticmethod
+    def get_app_stage():
+        return qt_model.GetApplicationStage()
+
+    # endregion
+
     # region 项目管理
     @staticmethod
+    def initial():
+        """
+        初始化模型,新建模型
+        example:
+                mdb.initial()
+        Returns: 无
+        """
+        qt_model.Initial()
+
+    @staticmethod
     def open_file(file_path: str):
         """
             打开bfmd文件
             example:
                     mdb.open_file("a.bfmd")
             Returns: 无
         """
@@ -87,27 +104,14 @@
                     mdb.do_solve()
             Returns: 无
         """
         qt_model.DoSolve()
 
     # endregion
 
-    # region 初始化模型
-    @staticmethod
-    def initial():
-        """
-        初始化模型
-        example:
-                mdb.initial()
-        Returns: 无
-        """
-        qt_model.Initial()
-
-    # endregion
-
     # region 节点单元操作
     @staticmethod
     def add_structure_group(name: str = "", index: int = -1):
         """
         添加结构组
         Args:
             name: 结构组名
@@ -418,14 +422,16 @@
         example:
             mdb.add_parameter_section(name="截面1",sec_type="矩形",sec_info=[2,4],bias_type="中心")
             mdb.add_parameter_section(name="截面2",sec_type="混凝土箱梁",box_height=2,box_number=3,
                 sec_info=[0.02,0,12,3,1,2,1,5,6,0.2,0.4,0.1,0.13,0.28,0.3,0.5,0.5,0.5,0.2],
                 charm_info=["1*0.2,0.1*0.2","0.5*0.15,0.3*0.2","0.4*0.2","0.5*0.2"])
         Returns: 无
         """
+        if qt_model.GetApplicationStage() == "首页":
+            raise Exception("起始页面下无法建模，请切换至前处理")
         sec_type_list = ["矩形", "圆形", "圆管", "箱型", "实腹八边形",
                          "空腹八边形", "内八角形", "实腹圆端型", "T形", "倒T形",
                          "I字形", "马蹄T形", "I字形混凝土", "混凝土箱梁", "带肋钢箱",
                          "带肋H截面", "钢桁箱梁1", "钢桁箱梁2", "钢桁箱梁3", "钢工字型带肋",
                          "钢管砼", "钢箱砼"]
         if sec_type not in sec_type_list:
             raise Exception(f"操作失败，参数截面仅支持以下截面类型{sec_type_list}")
@@ -997,14 +1003,15 @@
         Returns: 无
         """
         qt_model.RemoveLiveLoadCase(name=name)
 
     @staticmethod
     def update_model():
         qt_model.UpdateModel()
+
     # endregion
 
     # region 钢束操作
     @staticmethod
     def add_tendon_group(name: str = "", index: int = -1):
         """
         按照名称添加钢束组，添加时可指定钢束组id
@@ -1307,34 +1314,38 @@
             mdb.remove_nodal_displacement(case_name="荷载工况1",node_id=1)
         Returns: 无
         """
         qt_model.RemoveNodalDisplacement(caseName=case_name, nodeId=-node_id)
 
     @staticmethod
     def add_beam_load(beam_id: int = 1, case_name: str = "", load_type: int = 1, coord_system: int = 3, list_x: list[float, float] = None,
-                      list_load: list[float, float] = None, group_name="默认荷载组"):
+                      list_load: list[float, float] = None, group_name="默认荷载组", load_bias: tuple[bool, int, int, float] = None,
+                      projected: bool = False):
         """
         添加梁单元荷载
         Args:
             beam_id:单元编号
             case_name:荷载工况名
             load_type:荷载类型
                _ 1-集中荷载 2-集中弯矩 3-分布弯矩 4-分布弯矩
             coord_system:坐标系
                 _1-整体坐标X  2-整体坐标Y 3-整体坐标Z  4-局部坐标X  5-局部坐标Y  6-局部坐标Z_
             list_x:荷载位置信息 ,荷载距离单元I端的相对距离
             list_load:荷载数值信息
             group_name:荷载组名
+            load_bias:偏心荷载 (是否偏心,0-中心 1-偏心,偏心坐标系-int,偏心距离)
+            projected:是否投影
         example:
             mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=1,list_x=[0.1,0.5,0.8],list_load=[100,100,100])
             mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=3,list_x=[0.4,0.8],list_load=[100,200])
         Returns: 无
         """
         qt_model.AddBeamLoad(caseName=case_name, beamId=beam_id, loadType=load_type,
-                             coordinateSystem=coord_system, listX=list_x, listLoad=list_load, groupName=group_name)
+                             coordinateSystem=coord_system, listX=list_x, listLoad=list_load, groupName=group_name,
+                             biasInfo = load_bias, isProject = projected)
 
     @staticmethod
     def remove_beam_load(element_id: int = 1, case_name: str = "", load_type: int = 1, group_name: str = "默认荷载组"):
         """
         删除梁单元荷载
         Args:
             element_id:单元号
@@ -1828,46 +1839,7 @@
         """
         if name != "":
             qt_model.DeleteLoadCombine(name=name)
         else:
             qt_model.DeleteAllLoadCombine()
 
     # endregion
-
-    # region 辅助转换
-    @staticmethod
-    def parse_number_string(input_string):
-        """
-        将类似”1to5by2 11 13to18“的字符串转为list<int>型变量
-        Args:
-            input_string:传入字符串，字符串各部分用空格分开
-        Returns:
-            list[int]
-        """
-        if not input_string.strip():
-            return None
-
-        if input_string == 'nan':
-            return None
-
-        string_list = input_string.split(" ")
-        ids = []
-        for str_ids in string_list:
-            if "to" in str_ids:
-                range_parts = str_ids.split("to")
-                if "by" in range_parts[1]:
-                    range_parts = range_parts[1].split("by")
-
-                start = end = step = 0
-                if range_parts[0].isdigit() and range_parts[1].isdigit():
-                    start = int(range_parts[0])
-                    end = int(range_parts[1])
-                if len(range_parts) > 2 and range_parts[2].isdigit():
-                    step = int(range_parts[2])
-                else:
-                    step = 1
-                ids += [start + n * step for n in range((end - start) // step + 1)]
-            else:
-                ids.append(int(str_ids))
-        return ids
-    # endregion
-
```

### Comparing `qtmodel-0.3.4/qtmodel/qt_odb.py` & `qtmodel-0.3.5/qtmodel/qt_odb.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
             element_id: 单元编号
             stage_id: 施工极端号
             result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载
             increment_type: 1-全量    2-增量
             operation: 是否为运营阶段
             case_name: 运营阶段所需荷载工况名
         Returns:
-            list[ElementStress]
+            list[ElementStress] or ElementStress
         """
         if type(element_id) != int and type(element_id) != list:
             raise TypeError("类型错误,element_id仅支持 int和 list[int]")
-        bf_list = qt_model.GetBeamForce(element_id, stage_id, result_kind, increment_type, operation, case_name)
+        bf_list = qt_model.GetElementStress(element_id, stage_id, result_kind, increment_type, operation, case_name)
         list_res = []
         for item in bf_list:
             if item.ElementType == "BEAM":
                 stress_i = [item.StressI[0], item.StressI[1], item.StressI[2], item.StressI[3], item.StressI[4], item.StressI[5],
                             item.StressI[6], item.StressI[7], item.StressI[8]]
                 stress_j = [item.StressJ[0], item.StressJ[1], item.StressJ[2], item.StressJ[3], item.StressJ[4], item.StressJ[5],
                             item.StressJ[6], item.StressJ[7], item.StressJ[8]]
@@ -47,33 +47,35 @@
                 stress_i = [item.StressI[0], item.StressI[1], item.StressI[2], item.StressI[3], item.StressI[4], item.StressI[5],
                             item.StressI[6], item.StressI[7], item.StressI[8]]
                 stress_j = [item.StressJ[0], item.StressJ[1], item.StressJ[2], item.StressJ[3], item.StressJ[4], item.StressJ[5],
                             item.StressJ[6], item.StressJ[7], item.StressJ[8]]
                 list_res.append(TrussElementStress(item.ElementId, stress_i, stress_j))
             else:
                 raise TypeError(f"操作错误，不存在{item.ElementType}类型")
+        if len(list_res) == 1:
+            return list_res[0]
         return list_res
 
     @staticmethod
     def get_element_force(element_id, stage_id: int = 1, result_kind: int = 1, increment_type: int = 1, operation: bool = False, case_name=""):
         """
         获取单元内力,支持单个单元和单元列表
         Args:
             element_id: 单元编号
             stage_id: 施工极端号
             result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载
             increment_type: 1-全量    2-增量
             operation: 是否为运营阶段
             case_name: 运营阶段所需荷载工况名
         Returns:
-            list[ElementForce]
+            list[ElementForce] or ElementForce
         """
         if type(element_id) != int and type(element_id) != list:
             raise TypeError("类型错误,element_id仅支持 int和 list[int]")
-        bf_list = qt_model.GetBeamForce(element_id, stage_id, result_kind, increment_type, operation, case_name)
+        bf_list = qt_model.GetElementForce(element_id, stage_id, result_kind, increment_type, operation, case_name)
         list_res = []
         for item in bf_list:
             if item.ElementType == "BEAM":
                 force_i = [item.ForceI.Fx, item.ForceI.Fy, item.ForceI.Fz, item.ForceI.Mx, item.ForceI.My, item.ForceI.Mz]
                 force_j = [item.ForceJ.Fx, item.ForceJ.Fy, item.ForceJ.Fz, item.ForceJ.Mx, item.ForceJ.My, item.ForceJ.Mz]
                 list_res.append(BeamElementForce(item.ElementId, force_i, force_j))
             elif item.ElementType == "SHELL":
@@ -84,55 +86,61 @@
                 list_res.append(ShellElementForce(item.ElementId, force_i, force_j, force_k, force_l))
             elif item.ElementType == "TRUSS":
                 force_i = [item.ForceI.Fx, item.ForceI.Fy, item.ForceI.Fz, item.ForceI.Mx, item.ForceI.My, item.ForceI.Mz]
                 force_j = [item.ForceJ.Fx, item.ForceJ.Fy, item.ForceJ.Fz, item.ForceJ.Mx, item.ForceJ.My, item.ForceJ.Mz]
                 list_res.append(TrussElementForce(item.ElementId, force_i, force_j))
             else:
                 raise TypeError(f"操作错误，不存在{item.ElementType}类型")
+        if len(list_res) == 1:
+            return list_res[0]
         return list_res
 
     @staticmethod
     def get_reaction(node_id, stage_id: int = 1, result_kind: int = 1, increment_type: int = 1, operation: bool = False, case_name=""):
         """
         获取节点,支持单个节点和节点列表
         Args:
             node_id: 节点编号
             stage_id: 施工极端号
             result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载
             increment_type: 1-全量    2-增量
             operation: 是否为运营阶段
             case_name: 运营阶段所需荷载工况名
         Returns:
-            list[SupportReaction]
+            list[SupportReaction] or SupportReaction
         """
         if type(node_id) != int and type(node_id) != list:
             raise TypeError("类型错误,beam_id int和 list[int]")
         bs_list = qt_model.GetSupportReaction(node_id, stage_id, result_kind, increment_type, operation, case_name)
         list_res = []
         for item in bs_list:
             force = [item.Force.Fx, item.Force.Fy, item.Force.Fz, item.Force.Mx, item.Force.My, item.Force.Mz]
             list_res.append(SupportReaction(item.NodeId, force))
+        if len(list_res) == 1:
+            return list_res[0]
         return list_res
 
     @staticmethod
     def get_node_displacement(node_id, stage_id: int = 1, result_kind: int = 1, increment_type: int = 1, operation: bool = False, case_name=""):
         """
         获取节点,支持单个节点和节点列表
         Args:
             node_id: 节点号
             stage_id: 施工极端号
             result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载
             increment_type: 1-全量    2-增量
             operation: 是否为运营阶段
             case_name: 运营阶段所需荷载工况名
         Returns:
-            list[NodeDisplacement]
+            list[NodeDisplacement] or NodeDisplacement
         """
         if type(node_id) != int and type(node_id) != list:
             raise TypeError("类型错误,node_id仅支持 int和 list[int]")
         bf_list = qt_model.GetNodeDisplacement(node_id, stage_id, result_kind, increment_type, operation, case_name)
         list_res = []
         for item in bf_list:
             displacements = [item.Displacement.Dx, item.Displacement.Dy, item.Displacement.Dz,
                              item.Displacement.Rx, item.Displacement.Ry, item.Displacement.Rz]
             list_res.append(NodeDisplacement(item.NodeId, displacements))
+        if len(list_res) == 1:
+            return list_res[0]
         return list_res
```

### Comparing `qtmodel-0.3.4/qtmodel/res_db.py` & `qtmodel-0.3.5/qtmodel/res_db.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,54 @@
 import math
+import json
 
 
 class NodeDisplacement:
     """
     节点位移
     """
+
     def __init__(self, node_id, displacements: list[float]):
         if len(displacements) == 6:
             self.id = node_id
             self.dx = displacements[0]
             self.dy = displacements[1]
             self.dz = displacements[2]
             self.rx = displacements[3]
-            self.rx = displacements[4]
+            self.ry = displacements[4]
             self.rz = displacements[5]
         else:
             raise ValueError("操作错误:  'displacements' 列表有误")
 
     def __str__(self):
         attrs = vars(self)
         dict_str = '{' + ', '.join(f"'{k}': {v}" for k, v in attrs.items()) + '}'
         return dict_str
 
+    def to_json(self):
+        """
+        将对象转换为 JSON 格式的字符串
+        """
+        obj_dict = {
+            'id': self.id,
+            'dx': self.dx,
+            'dy': self.dy,
+            'dz': self.dz,
+            'rx': self.rx,
+            'ry': self.ry,
+            'rz': self.rz
+        }
+        return json.dumps(obj_dict)
+
 
 class SupportReaction:
     """
     支座反力
     """
+
     def __init__(self, support_id: int, force: list[float]):
         self.support_id = support_id
         if len(force) == 6:
             self.fx = force[0]
             self.fy = force[1]
             self.fz = force[2]
             self.mx = force[3]
@@ -40,19 +58,35 @@
             raise ValueError("操作错误:  'force' 列表有误")
 
     def __str__(self):
         attrs = vars(self)
         dict_str = '{' + ', '.join(f"'{k}': {v}" for k, v in attrs.items()) + '}'
         return dict_str
 
+    def to_json(self):
+        """
+        将对象转换为 JSON 格式的字符串
+        """
+        obj_dict = {
+            'support_id': self.support_id,
+            'fx': self.fx,
+            'fy': self.fy,
+            'fz': self.fz,
+            'mx': self.mx,
+            'my': self.my,
+            'mz': self.mz
+        }
+        return json.dumps(obj_dict)
+
 
 class BeamElementForce:
     """
     梁单元内力
     """
+
     def __init__(self, element_id: int, force_i: list[float], force_j: list[float]):
         """
         单元内力构造器
         Args:
             element_id: 单元id
             force_i: I端单元内力 [Fx,Fy,Fz,Mx,My,Mz]
             force_j: J端单元内力 [Fx,Fy,Fz,Mx,My,Mz]
@@ -65,19 +99,31 @@
             raise ValueError("操作错误:  'force_i' and 'force_j' 列表有误")
 
     def __str__(self):
         attrs = vars(self)
         dict_str = '{' + ', '.join(f"'{k}': {v}" for k, v in attrs.items()) + '}'
         return dict_str
 
+    def to_json(self):
+        """
+        将 BeamElementForce 对象转换为 JSON 格式的字符串
+        """
+        obj_dict = {
+            'id': self.id,
+            'force_i': self.force_i.to_json(),
+            'force_j': self.force_j.to_json()
+        }
+        return json.dumps(obj_dict)
+
 
 class TrussElementForce:
     """
     桁架单元内力
     """
+
     def __init__(self, element_id: int, force_i: list[float], force_j: list[float]):
         """
         单元内力构造器
         Args:
             element_id: 单元id
             force_i: I端单元内力 [Fx,Fy,Fz,Mx,My,Mz]
             force_j: J端单元内力 [Fx,Fy,Fz,Mx,My,Mz]
@@ -96,19 +142,37 @@
             raise ValueError("操作错误:  'stress_i' and 'stress_j' 列表有误")
 
     def __str__(self):
         attrs = vars(self)
         dict_str = '{' + ', '.join(f"'{k}': {v}" for k, v in attrs.items()) + '}'
         return dict_str
 
+    def to_json(self):
+        """
+        将对象转换为 JSON 格式的字符串
+        """
+        obj_dict = {
+            'id': self.id,
+            'Ni': self.Ni,
+            'Fxi': self.Fxi,
+            'Fyi': self.Fyi,
+            'Fzi': self.Fzi,
+            'Nj': self.Nj,
+            'Fxj': self.Fxj,
+            'Fyj': self.Fyj,
+            'Fzj': self.Fzj
+        }
+        return json.dumps(obj_dict)
+
 
 class ShellElementForce:
     """
     板单元内力
     """
+
     def __init__(self, element_id: int, force_i: list[float], force_j: list[float], force_k: list[float], force_l: list[float]):
         """
         单元内力构造器
         Args:
             element_id: 单元id
             force_i: I端单元内力 [Fx,Fy,Fz,Mx,My,Mz]
             force_j: J端单元内力 [Fx,Fy,Fz,Mx,My,Mz]
@@ -126,19 +190,33 @@
             raise ValueError("操作错误:  内力列表有误")
 
     def __str__(self):
         attrs = vars(self)
         dict_str = '{' + ', '.join(f"'{k}': {v}" for k, v in attrs.items()) + '}'
         return dict_str
 
+    def to_json(self):
+        """
+        将 ShellElementForce 对象转换为 JSON 格式的字符串
+        """
+        obj_dict = {
+            'id': self.id,
+            'force_i': self.force_i.to_json(),
+            'force_j': self.force_j.to_json(),
+            'force_k': self.force_k.to_json(),
+            'force_l': self.force_l.to_json()
+        }
+        return json.dumps(obj_dict)
+
 
 class BeamElementStress:
     """
     梁单元应力
     """
+
     def __init__(self, element_id: int, stress_i: list[float], stress_j: list[float]):
         """
         单元内力构造器
         Args:
             element_id: 单元id
             stress_i: I端单元应力 [top_left, top_right, bot_left, bot_right, sfx, smz_left, smz_right, smy_top, smy_bot]
             stress_j: J端单元应力  [top_left, top_right, bot_left, bot_right, sfx, smz_left, smz_right, smy_top, smy_bot]
@@ -151,19 +229,31 @@
             raise ValueError("操作错误:  'stress_i' or 'stress_j' 列表有误")
 
     def __str__(self):
         attrs = vars(self)
         dict_str = '{' + ', '.join(f"'{k}': {v}" for k, v in attrs.items()) + '}'
         return dict_str
 
+    def to_json(self):
+        """
+        将 BeamElementStress 对象转换为 JSON 格式的字符串
+        """
+        obj_dict = {
+            'id': self.id,
+            'stress_i': self.stress_i.to_json(),
+            'stress_j': self.stress_j.to_json()
+        }
+        return json.dumps(obj_dict)
+
 
 class ShellElementStress:
     """
     板架单元应力
     """
+
     def __init__(self, frame_id: int, stress_i_top: list[float], stress_j_top: list[float], stress_k_top: list[float], stress_l_top: list[float]
                  , stress_i_bot: list[float], stress_j_bot: list[float], stress_k_bot: list[float], stress_l_bot: list[float]):
         """
         单元内力构造器
         Args:
             frame_id: 单元id
             stress_i_top: I端单元上部应力 [sx,sy,sxy,s1,s2]
@@ -192,19 +282,37 @@
             raise ValueError("操作错误:  'stress' 列表有误")
 
     def __str__(self):
         attrs = vars(self)
         dict_str = '{' + ', '.join(f"'{k}': {v}" for k, v in attrs.items()) + '}'
         return dict_str
 
+    def to_json(self):
+        """
+        将 ShellElementStress 对象转换为 JSON 格式的字符串
+        """
+        obj_dict = {
+            'id': self.id,
+            'stress_i_top': self.stress_i_top.to_json(),
+            'stress_j_top': self.stress_j_top.to_json(),
+            'stress_k_top': self.stress_k_top.to_json(),
+            'stress_l_top': self.stress_l_top.to_json(),
+            'stress_i_bot': self.stress_i_bot.to_json(),
+            'stress_j_bot': self.stress_j_bot.to_json(),
+            'stress_k_bot': self.stress_k_bot.to_json(),
+            'stress_l_bot': self.stress_l_bot.to_json()
+        }
+        return json.dumps(obj_dict)
+
 
 class TrussElementStress:
     """
     桁架单元应力
     """
+
     def __init__(self, frame_id: int, stress_i: list[float], stress_j: list[float]):
         """
         单元内力构造器
         Args:
             frame_id: 单元id
             stress_i: I端单元应力
             stress_j: J端单元应力
@@ -217,14 +325,25 @@
             raise ValueError("操作错误:  'stress_i' and 'stress_j' 列表有误")
 
     def __str__(self):
         attrs = vars(self)
         dict_str = '{' + ', '.join(f"'{k}': {v}" for k, v in attrs.items()) + '}'
         return dict_str
 
+    def to_json(self):
+        """
+        将 TrussElementStress 对象转换为 JSON 格式的字符串
+        """
+        obj_dict = {
+            'id': self.id,
+            'Si': self.Si,
+            'Sj': self.Sj
+        }
+        return json.dumps(obj_dict)
+
 
 class Force:
     """
     用于梁单元内力和板单元内力
     """
 
     def __init__(self, fx, fy, fz, mx, my, mz):
@@ -238,14 +357,30 @@
         self.m_xyz = math.sqrt((self.mx * self.mx + self.my * self.my + self.mz * self.mz))
 
     def __str__(self):
         attrs = vars(self)
         dict_str = '{' + ', '.join(f"'{k}': {v:.3f}" for k, v in attrs.items()) + '}'
         return dict_str
 
+    def to_json(self):
+        """
+        将 Force 对象转换为 JSON 格式的字典
+        """
+        obj_dict = {
+            'fx': self.fx,
+            'fy': self.fy,
+            'fz': self.fz,
+            'mx': self.mx,
+            'my': self.my,
+            'mz': self.mz,
+            'f_xyz': self.f_xyz,
+            'm_xyz': self.m_xyz
+        }
+        return obj_dict
+
 
 class ShellStress:
     """
     用于板单元应力分量
     """
 
     def __init__(self, sx, sy, sxy, s1, s2):
@@ -256,14 +391,27 @@
         self.s2 = s2
 
     def __str__(self):
         attrs = vars(self)
         dict_str = '{' + ', '.join(f"'{k}': {v:.3f}" for k, v in attrs.items()) + '}'
         return dict_str
 
+    def to_json(self):
+        """
+        将 ShellStress 对象转换为 JSON 格式的字符串
+        """
+        obj_dict = {
+            'sx': self.sx,
+            'sy': self.sy,
+            'sxy': self.sxy,
+            's1': self.s1,
+            's2': self.s2
+        }
+        return json.dumps(obj_dict)
+
 
 class BeamStress:
     """
     用于梁单元应力分量
     """
 
     def __init__(self, top_left, top_right, bot_left, bot_right, sfx, smz_left, smz_right, smy_top, smy_bot):
@@ -277,7 +425,24 @@
         self.smy_top = smy_top  # My引起的+z轴应力
         self.smy_bot = smy_bot  # My引起的-z轴应力
 
     def __str__(self):
         attrs = vars(self)
         dict_str = '{' + ', '.join(f"'{k}': {v:.3f}" for k, v in attrs.items()) + '}'
         return dict_str
+
+    def to_json(self):
+        """
+        将 BeamStress 对象转换为 JSON 格式的字典
+        """
+        obj_dict = {
+            'top_left': self.top_left,
+            'top_right': self.top_right,
+            'bot_left': self.bot_left,
+            'bot_right': self.bot_right,
+            'sfx': self.sfx,
+            'smz_left': self.smz_left,
+            'smz_right': self.smz_right,
+            'smy_top': self.smy_top,
+            'smy_bot': self.smy_bot
+        }
+        return obj_dict
```

### Comparing `qtmodel-0.3.4/qtmodel.egg-info/PKG-INFO` & `qtmodel-0.3.5/qtmodel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmodel
-Version: 0.3.4
+Version: 0.3.5
 Summary: python modeling for qt  24/05/06 
 Home-page: https://github.com/Inface0443/pyqt
 Author: dqy-zhj
 Author-email: 1105417715@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qtmodel-0.3.4/setup.py` & `qtmodel-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # 读取文件内容
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="qtmodel",
-    version="0.3.4",
+    version="0.3.5",
     author="dqy-zhj",
     author_email="1105417715@qq.com",
     description="python modeling for qt  24/05/06 ",
     long_description=long_description,  # 使用读取的 README.md 文件内容
     long_description_content_type="text/markdown",  # 指明内容格式为markdown
     url="https://github.com/Inface0443/pyqt",
     packages=find_packages(),
```

