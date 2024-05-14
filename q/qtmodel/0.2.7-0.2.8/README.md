# Comparing `tmp/qtmodel-0.2.7.tar.gz` & `tmp/qtmodel-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtmodel-0.2.7.tar", last modified: Mon May  6 04:03:44 2024, max compression
+gzip compressed data, was "qtmodel-0.2.8.tar", last modified: Tue May 14 08:27:53 2024, max compression
```

## Comparing `qtmodel-0.2.7.tar` & `qtmodel-0.2.8.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 04:03:44.267276 qtmodel-0.2.7/
--rw-rw-rw-   0        0        0    37701 2024-05-06 04:03:44.266276 qtmodel-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0    37273 2024-04-25 08:56:24.000000 qtmodel-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 04:03:44.249027 qtmodel-0.2.7/qtmodel/
--rw-rw-rw-   0        0        0       93 2024-04-10 06:50:13.000000 qtmodel-0.2.7/qtmodel/__init__.py
--rw-rw-rw-   0        0        0    80502 2024-05-06 03:52:43.000000 qtmodel-0.2.7/qtmodel/qt_mdb.py
--rw-rw-rw-   0        0        0     3834 2024-04-10 06:52:58.000000 qtmodel-0.2.7/qtmodel/qt_odb.py
--rw-rw-rw-   0        0        0     3405 2024-04-17 03:39:04.000000 qtmodel-0.2.7/qtmodel/res_db.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:03:44.264743 qtmodel-0.2.7/qtmodel.egg-info/
--rw-rw-rw-   0        0        0    37701 2024-05-06 04:03:43.000000 qtmodel-0.2.7/qtmodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2024-05-06 04:03:44.000000 qtmodel-0.2.7/qtmodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 04:03:43.000000 qtmodel-0.2.7/qtmodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-06 04:03:44.000000 qtmodel-0.2.7/qtmodel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 04:03:44.267276 qtmodel-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      758 2024-05-06 04:03:38.000000 qtmodel-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:27:53.063749 qtmodel-0.2.8/
+-rw-rw-rw-   0        0        0    37701 2024-05-14 08:27:53.063749 qtmodel-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0    37273 2024-05-13 05:54:03.000000 qtmodel-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 08:27:53.051693 qtmodel-0.2.8/qtmodel/
+-rw-rw-rw-   0        0        0      117 2024-05-14 06:05:14.000000 qtmodel-0.2.8/qtmodel/__init__.py
+-rw-rw-rw-   0        0        0    82266 2024-05-14 08:25:47.000000 qtmodel-0.2.8/qtmodel/qt_mdb.py
+-rw-rw-rw-   0        0        0     3834 2024-05-13 05:54:03.000000 qtmodel-0.2.8/qtmodel/qt_odb.py
+-rw-rw-rw-   0        0        0      939 2024-05-14 06:03:36.000000 qtmodel-0.2.8/qtmodel/qt_post.py
+-rw-rw-rw-   0        0        0     3405 2024-04-17 03:39:04.000000 qtmodel-0.2.8/qtmodel/res_db.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:27:53.060340 qtmodel-0.2.8/qtmodel.egg-info/
+-rw-rw-rw-   0        0        0    37701 2024-05-14 08:27:52.000000 qtmodel-0.2.8/qtmodel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-05-14 08:27:52.000000 qtmodel-0.2.8/qtmodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 08:27:52.000000 qtmodel-0.2.8/qtmodel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-14 08:27:52.000000 qtmodel-0.2.8/qtmodel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-14 08:27:52.000000 qtmodel-0.2.8/qtmodel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 08:27:53.063749 qtmodel-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      860 2024-05-14 08:27:24.000000 qtmodel-0.2.8/setup.py
```

### Comparing `qtmodel-0.2.7/PKG-INFO` & `qtmodel-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmodel
-Version: 0.2.7
+Version: 0.2.8
 Summary: python modeling for qt  24/05/06 
 Home-page: https://github.com/Inface0443/pyqt
 Author: dqy-zhj
 Author-email: 1105417715@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qtmodel-0.2.7/README.md` & `qtmodel-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `qtmodel-0.2.7/qtmodel/qt_mdb.py` & `qtmodel-0.2.8/qtmodel/qt_mdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,84 @@
     """
     Mdb类负责建模相关操作
     """
 
     def __int__(self):
         self.initial()
 
+    # region 项目管理
+    @staticmethod
+    def open_file(file_path: str):
+        """
+            打开bfmd文件
+            example:
+                    mdb.open_file("a.bfmd")
+            Returns: 无
+        """
+        if not file_path.endswith(".bfmd"):
+            raise Exception("操作错误，仅支持bfmd文件")
+        qt_model.OpenFile(file_path)
+
+    @staticmethod
+    def save_file(file_path: str):
+        """
+            保存bfmd文件
+            example:
+                    mdb.save_file("a.bfmd")
+            Returns: 无
+        """
+        qt_model.OpenFile(file_path)
+
+    @staticmethod
+    def close_project():
+        """
+            关闭项目
+            example:
+                mdb.close_project()
+            Returns: 无
+        """
+        qt_model.CloseFile()
+
+    @staticmethod
+    def import_command(command: str, command_type: int = 1):
+        """
+            导入命令
+            Args:
+                command:命令字符
+                command_type:命令类型 1-桥通命令
+            example:
+                mdb.import_command("*SECTION")
+            Returns: 无
+        """
+        qt_model.ImportQtCommand(command)
+
+    @staticmethod
+    def export_file(file_path: str):
+        """
+            导入命令
+            Args:
+                file_path:导出文件(.mct/.qdat/.PGF/.3dx)
+            example:
+                qt_model.ExportFile("a.mct")
+            Returns: 无
+        """
+        qt_model.ExportFile(file_path)
+
+    @staticmethod
+    def do_solve():
+        """
+            运行分析
+            example:
+                    mdb.do_solve()
+            Returns: 无
+        """
+        qt_model.DoSolve()
+
+    # endregion
+
     # region 初始化模型
     @staticmethod
     def initial():
         """
         初始化模型
         example:
                 mdb.initial()
@@ -39,53 +109,53 @@
     def remove_structure_group(name: str = "", index: int = -1):
         """
         可根据结构与组名或结构组编号删除结构组，当组名和组编号均为默认则删除所有结构组
         Args:
             name:结构组名称
             index:结构组编号
         example:
-                mdb.remove_structure_group(name="新建结构组1")
-                mdb.remove_structure_group(index = 2)
+            mdb.remove_structure_group(name="新建结构组1")
+            mdb.remove_structure_group(index = 2)
         Returns: 无
         """
         if index != -1:
             qt_model.RemoveStructureGroup(id=index)
         elif name != "":
             qt_model.RemoveStructureGroup(name=name)
         else:
             qt_model.RemoveAllStructureGroup()
 
     @staticmethod
     def add_structure_to_group(name: str = "", node_ids: list[int] = None, element_ids: list[int] = None):
         """
         为结构组添加节点和/或单元
         Args:
-             name: 结构组名
-             node_ids: 节点编号列表(可选参数)
-             element_ids: 单元编号列表(可选参数)
+            name: 结构组名
+            node_ids: 节点编号列表(可选参数)
+            element_ids: 单元编号列表(可选参数)
         example:
-                mdb.add_structure_to_group(name="现有结构组1",node_ids=[1,2,3,4],element_ids=[1,2])
+            mdb.add_structure_to_group(name="现有结构组1",node_ids=[1,2,3,4],element_ids=[1,2])
         Returns: 无
         """
         if node_ids is None:
             node_ids = []
         if element_ids is None:
             element_ids = []
         qt_model.AddStructureToGroup(name=name, nodeIds=node_ids, elementIds=element_ids)
 
     @staticmethod
     def remove_structure_in_group(name: str = "", node_ids: list[int] = None, element_ids=None):
         """
         为结构组删除节点和/或单元
         Args:
-             name: 结构组名
-             node_ids: 节点编号列表(可选参数)
-             element_ids: 单元编号列表(可选参数)
+            name: 结构组名
+            node_ids: 节点编号列表(可选参数)
+            element_ids: 单元编号列表(可选参数)
         example:
-                mdb.add_structure_to_group(name="现有结构组1",node_ids=[1,2,3,4],element_ids=[1,2])
+            mdb.add_structure_to_group(name="现有结构组1",node_ids=[1,2,3,4],element_ids=[1,2])
         Returns: 无
         """
         if node_ids is None:
             node_ids = []
         if element_ids is None:
             element_ids = []
         qt_model.RemoveStructureOnGroup(name=name, nodeIds=node_ids, elementIds=element_ids)
@@ -456,14 +526,15 @@
             mdb.remove_section(1)
         Returns: 无
         """
         if index == -1:
             qt_model.RemoveAllSection()
         else:
             qt_model.RemoveSection(id=index)
+
     # endregion
 
     # region 板厚操作
     @staticmethod
     def add_thickness(index: int = -1, name: str = "", t: float = 0,
                       thick_type: int = 0, bias_info: tuple[int, float] = None,
                       rib_pos: int = 0, dist_v: float = 0, dist_l: float = 0, rib_v=None, rib_l=None):
@@ -1218,16 +1289,16 @@
         example:
             mdb.remove_nodal_displacement(case_name="荷载工况1",node_id=1)
         Returns: 无
         """
         qt_model.RemoveNodalDisplacement(caseName=case_name, nodeId=-node_id)
 
     @staticmethod
-    def add_beam_load(beam_id: int = 1, case_name: str = "", load_type: int = 1, coord_system: int = 3, list_x: list[tuple[float,float]] = None,
-                      list_load: list[tuple[float,float]] = None, group_name="默认荷载组"):
+    def add_beam_load(beam_id: int = 1, case_name: str = "", load_type: int = 1, coord_system: int = 3, list_x: list[tuple[float, float]] = None,
+                      list_load: list[tuple[float, float]] = None, group_name="默认荷载组"):
         """
         添加梁单元荷载
         Args:
             beam_id:单元编号
             case_name:荷载工况名
             load_type:荷载类型
                _ 1-集中荷载 2-集中弯矩 3-分布弯矩 4-分布弯矩
@@ -1238,15 +1309,15 @@
             group_name:荷载组名
         example:
             mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=1,list_x=[0.1,0.5,0.8],list_load=[100,100,100])
             mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=3,list_x=[0.4,0.8],list_load=[100,200])
         Returns: 无
         """
         qt_model.AddBeamLoad(caseName=case_name, beamId=beam_id, loadType=load_type,
-                             coordinateSystem=coord_system, listX=list_x, listLoad=list_load,  groupName=group_name)
+                             coordinateSystem=coord_system, listX=list_x, listLoad=list_load, groupName=group_name)
 
     @staticmethod
     def remove_beam_load(element_id: int = 1, case_name: str = "", load_type: int = 1, group_name: str = "默认荷载组"):
         """
         删除梁单元荷载
         Args:
             element_id:单元号
@@ -1710,14 +1781,15 @@
             mdb.remove_construction_stage(name="施工阶段1")
         Returns: 无
         """
         if name == "":
             qt_model.RemoveAllConstructionStage()
         else:
             qt_model.RemoveConstructionStage(name=name)
+
     # endregion
 
     # region 荷载组合
     @staticmethod
     def add_load_combine(name: str = "", combine_type: int = 1, describe: str = "", combine_info: list[tuple[str, str, float]] = None):
         """
         添加荷载组合
```

### Comparing `qtmodel-0.2.7/qtmodel/qt_odb.py` & `qtmodel-0.2.8/qtmodel/qt_odb.py`

 * *Files identical despite different names*

### Comparing `qtmodel-0.2.7/qtmodel/res_db.py` & `qtmodel-0.2.8/qtmodel/res_db.py`

 * *Files identical despite different names*

### Comparing `qtmodel-0.2.7/qtmodel.egg-info/PKG-INFO` & `qtmodel-0.2.8/qtmodel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmodel
-Version: 0.2.7
+Version: 0.2.8
 Summary: python modeling for qt  24/05/06 
 Home-page: https://github.com/Inface0443/pyqt
 Author: dqy-zhj
 Author-email: 1105417715@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

