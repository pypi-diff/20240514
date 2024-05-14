# Comparing `tmp/mapieng-0.1.0.tar.gz` & `tmp/mapieng-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapieng-0.1.0.tar", last modified: Thu Apr 18 07:38:18 2024, max compression
+gzip compressed data, was "mapieng-0.1.1.tar", last modified: Tue May 14 08:45:05 2024, max compression
```

## Comparing `mapieng-0.1.0.tar` & `mapieng-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 07:38:18.144052 mapieng-0.1.0/
--rw-rw-rw-   0        0        0       79 2024-04-18 07:33:03.000000 mapieng-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      326 2024-04-18 07:38:18.143050 mapieng-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-04-04 07:56:20.000000 mapieng-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 07:38:18.123183 mapieng-0.1.0/base/
--rw-rw-rw-   0        0        0     3680 2024-04-11 11:11:21.000000 mapieng-0.1.0/base/ReportUtil.py
--rw-rw-rw-   0        0        0       17 2024-04-18 06:48:05.000000 mapieng-0.1.0/base/__init__.py
--rw-rw-rw-   0        0        0     7980 2024-04-05 06:25:39.000000 mapieng-0.1.0/base/baseformidasapi.py
--rw-rw-rw-   0        0        0    18179 2024-04-15 07:11:37.000000 mapieng-0.1.0/base/calculator_asd.py
--rw-rw-rw-   0        0        0       38 2024-04-05 06:25:39.000000 mapieng-0.1.0/base/engineers.py
--rw-rw-rw-   0        0        0     7065 2024-04-04 07:56:20.000000 mapieng-0.1.0/base/engineers_server.py
--rw-rw-rw-   0        0        0     9894 2024-04-04 07:56:20.000000 mapieng-0.1.0/base/engineers_web.py
--rw-rw-rw-   0        0        0     8194 2024-04-04 07:56:20.000000 mapieng-0.1.0/base/geometry.py
--rw-rw-rw-   0        0        0    13475 2024-04-04 07:56:20.000000 mapieng-0.1.0/base/hello.html
--rw-rw-rw-   0        0        0      961 2024-04-15 02:58:29.000000 mapieng-0.1.0/base/meshutil.py
--rw-rw-rw-   0        0        0     5919 2024-04-09 08:44:07.000000 mapieng-0.1.0/base/midasapi.py
--rw-rw-rw-   0        0        0     3412 2024-04-09 08:44:07.000000 mapieng-0.1.0/base/midasutil.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:38:18.127145 mapieng-0.1.0/base/steel/
--rw-rw-rw-   0        0        0     1141 2024-04-05 06:25:39.000000 mapieng-0.1.0/base/steel/KS18.json
--rw-rw-rw-   0        0        0       17 2024-04-18 06:48:05.000000 mapieng-0.1.0/base/steel/__init__.py
--rw-rw-rw-   0        0        0     2575 2024-04-09 08:44:07.000000 mapieng-0.1.0/base/steel/steelutil.py
--rw-rw-rw-   0        0        0     1100 2024-04-05 06:25:39.000000 mapieng-0.1.0/base/symbol.py
--rw-rw-rw-   0        0        0      126 2024-04-04 07:56:20.000000 mapieng-0.1.0/base/test.py
--rw-rw-rw-   0        0        0      502 2024-04-15 01:54:35.000000 mapieng-0.1.0/base/testmesh.py
--rw-rw-rw-   0        0        0    35253 2024-04-15 07:11:36.000000 mapieng-0.1.0/base/unit_converter.py
--rw-rw-rw-   0        0        0    19024 2024-04-04 07:56:20.000000 mapieng-0.1.0/base/vector.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:38:18.141054 mapieng-0.1.0/mapieng.egg-info/
--rw-rw-rw-   0        0        0      326 2024-04-18 07:38:17.000000 mapieng-0.1.0/mapieng.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      802 2024-04-18 07:38:18.000000 mapieng-0.1.0/mapieng.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 07:38:17.000000 mapieng-0.1.0/mapieng.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-18 07:38:17.000000 mapieng-0.1.0/mapieng.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-18 07:38:17.000000 mapieng-0.1.0/mapieng.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-18 07:38:18.134363 mapieng-0.1.0/project/
--rw-rw-rw-   0        0        0        0 2024-04-18 07:32:24.000000 mapieng-0.1.0/project/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:38:18.137689 mapieng-0.1.0/project/baseplate_KDS41_30_2022/
--rw-rw-rw-   0        0        0      638 2024-04-16 04:59:23.000000 mapieng-0.1.0/project/baseplate_KDS41_30_2022/Test.py
--rw-rw-rw-   0        0        0       73 2024-04-18 07:27:21.000000 mapieng-0.1.0/project/baseplate_KDS41_30_2022/__init__.py
--rw-rw-rw-   0        0        0     5747 2024-04-15 07:11:37.000000 mapieng-0.1.0/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py
--rw-rw-rw-   0        0        0     7275 2024-04-11 11:16:20.000000 mapieng-0.1.0/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py
--rw-rw-rw-   0        0        0       42 2024-04-18 07:38:18.144052 mapieng-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      547 2024-04-18 07:38:11.000000 mapieng-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:45:05.238845 mapieng-0.1.1/
+-rw-rw-rw-   0        0        0       79 2024-05-14 08:44:17.000000 mapieng-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      326 2024-05-14 08:45:05.237845 mapieng-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-05-14 08:44:17.000000 mapieng-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 08:45:05.213331 mapieng-0.1.1/base/
+-rw-rw-rw-   0        0        0     2988 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/ReportUtil.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/__init__.py
+-rw-rw-rw-   0        0        0     7980 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/baseformidasapi.py
+-rw-rw-rw-   0        0        0    18374 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/calculator_asd.py
+-rw-rw-rw-   0        0        0       38 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/engineers.py
+-rw-rw-rw-   0        0        0     7065 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/engineers_server.py
+-rw-rw-rw-   0        0        0     9894 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/engineers_web.py
+-rw-rw-rw-   0        0        0     8194 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/geometry.py
+-rw-rw-rw-   0        0        0    13475 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/hello.html
+-rw-rw-rw-   0        0        0     7301 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/midasapi.py
+-rw-rw-rw-   0        0        0     3412 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/midasutil.py
+-rw-rw-rw-   0        0        0      449 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/section_property.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:45:05.217337 mapieng-0.1.1/base/steel/
+-rw-rw-rw-   0        0        0     1141 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/steel/KS18.json
+-rw-rw-rw-   0        0        0        0 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/steel/__init__.py
+-rw-rw-rw-   0        0        0     2527 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/steel/steelutil.py
+-rw-rw-rw-   0        0        0     1100 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/symbol.py
+-rw-rw-rw-   0        0        0      126 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/test.py
+-rw-rw-rw-   0        0        0    35253 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/unit_converter.py
+-rw-rw-rw-   0        0        0    19024 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/vector.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:45:05.235845 mapieng-0.1.1/mapieng.egg-info/
+-rw-rw-rw-   0        0        0      326 2024-05-14 08:45:04.000000 mapieng-0.1.1/mapieng.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2024-05-14 08:45:05.000000 mapieng-0.1.1/mapieng.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 08:45:04.000000 mapieng-0.1.1/mapieng.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-14 08:45:04.000000 mapieng-0.1.1/mapieng.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-14 08:45:04.000000 mapieng-0.1.1/mapieng.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 08:45:05.226336 mapieng-0.1.1/project/
+-rw-rw-rw-   0        0        0        0 2024-05-14 08:44:18.000000 mapieng-0.1.1/project/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:45:05.230845 mapieng-0.1.1/project/baseplate_KDS41_30_2022/
+-rw-rw-rw-   0        0        0        0 2024-05-14 08:44:18.000000 mapieng-0.1.1/project/baseplate_KDS41_30_2022/__init__.py
+-rw-rw-rw-   0        0        0     5747 2024-05-14 08:44:18.000000 mapieng-0.1.1/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py
+-rw-rw-rw-   0        0        0     7275 2024-05-14 08:44:18.000000 mapieng-0.1.1/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py
+-rw-rw-rw-   0        0        0       42 2024-05-14 08:45:05.239846 mapieng-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      547 2024-05-14 08:44:53.000000 mapieng-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:45:05.233845 mapieng-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-14 08:44:18.000000 mapieng-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      808 2024-05-14 08:44:18.000000 mapieng-0.1.1/tests/test_baseplate_kds.py
```

### Comparing `mapieng-0.1.0/base/ReportUtil.py` & `mapieng-0.1.1/base/ReportUtil.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     VOLUME = 8
 
 class CReportUtil(MdUtils):
     def __init__(self, file_name, title=""):
         super().__init__(file_name=file_name, title=title)
         self.__header_count = 0
         self.__paragraph_count = 0
-        
+
     def get_md_text(self):
         file = super().create_md_file()
         return super().read_md_file(file.file_name)
 
     def add_chapter(self, text):
         self.__header_count += 1
         self.__paragraph_count = 0
@@ -33,25 +33,25 @@
         self.__paragraph_count += 1
         self.new_paragraph(f"({self.__paragraph_count}) {text}")
 
     def add_image(self, path, image_text=""):
         self.new_line(self.new_inline_image(text=image_text, path=path))
 
     def add_line_svu(self, str, value, unit):
-            self.new_line(f"{str} {value} {self.get_str_unit(unit)}")
+        self.new_line(f"{str} {value} {self.get_str_unit(unit)}")
 
     def add_line_fvu(self, formula, value, unit):
         self.new_line(f"{self.add_formula(formula)} = {value} {self.get_str_unit(unit)}")
 
     def add_line(self, text):
         self.new_line(text)
 
     def add_formula(self, text):
         return f"${text}$"
-        
+
     def get_str_unit(self, unit):
         if unit == enUnit.LENGTH:
             return "mm"
         elif unit == enUnit.MEMBERLENGTH:
             return "m"
         elif unit == enUnit.AREA:
             return "$mm^2$"
@@ -87,26 +87,7 @@
     elif isinstance(data, (list, tuple)):
         for item in data:
             result = find_data(item, key_to_find)
             if result is not None:
                 return result
     # 찾는 키가 없을 경우 None 반환
     return None
-
-
-def find_value_by_keys_only(data, keys):
-    def find(data, keys, index):
-        if index == len(keys):  # 모든 키를 성공적으로 찾음
-            return data
-        key = keys[index]
-        if isinstance(data, dict):
-            if key in data:
-                return find(data[key], keys, index + 1)
-        elif isinstance(data, list):
-            # 리스트의 각 항목에서 키를 찾음
-            for item in data:
-                result = find(item, keys, index)
-                if result is not None:
-                    return result
-        return None  # 경로에 맞는 데이터가 없음
-
-    return find(data, keys, 0)
```

### Comparing `mapieng-0.1.0/base/baseformidasapi.py` & `mapieng-0.1.1/base/baseformidasapi.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.0/base/calculator_asd.py` & `mapieng-0.1.1/base/calculator_asd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-#내용은 아래 참고요..
-#https://midasitdev.atlassian.net/wiki/spaces/DGNDEV/pages/610730064/ASDEngine
-from math import *
+# 내용은 아래 참고요..
+# https://midasitdev.atlassian.net/wiki/spaces/DGNDEV/pages/610730064/ASDEngine
+import math
 
 class CalculatorASDEngine:
     def __init__(self):
         self._nIterationNo = 0
 
         self._Fck = self._Fy = 0.0
         self._Ec = self._Es = 0.0
@@ -185,50 +185,50 @@
         if not self.eq0(self._CentroidX):
             _my -= _p * self._CentroidX
             self._CentroidX = 0.0
         if not self.eq0(self._CentroidY):
             _mx -= _p * self._CentroidY
             self._CentroidY = 0.0
 
-        _mn = hypot(_mx, _my)
+        _mn = math.hypot(_mx, _my)
         if self.eq0(_mn, self.get_radian_tolerance()):
             return self.calc_axial_only(_p)
 
         _angle = self.calc_moment_angle(_mx, _my)
         _rotation = _angle
-        if fabs(_mn / _p) < 0.0001:
+        if math.fabs(_mn / _p) < 0.0001:
             self.rotate_section(_rotation)
             self.calc_strain_rebar(_p, _mx, _my)
             return True
 
         _angle_temp = 0.0
         _angle_max = self._PI
         _angle_min = -self._PI
         for i in range(self._nIterationNo):
             self.rotate_section(_rotation)
             self.calc_strain_rebar(_p, _mx, _my)
 
             if self._Pn == 0.0:
-                _angle_temp = atan(1.0)
+                _angle_temp = math.atan(1.0)
             else:
                 _angle_temp = self.calc_moment_angle(self._Mnx, self._Mny)
 
-            if fabs(_angle - _angle_temp) < 0.0001:
+            if math.fabs(_angle - _angle_temp) < 0.0001:
                 break
 
             if _angle < _angle_temp:
                 _angle_max = _rotation
             else:
                 _angle_min = _rotation
 
             _rotation = (_angle_max + _angle_min) / 2.0
 
-        if fabs(_angle - _angle_temp) > 0.1:
+        if math.fabs(_angle - _angle_temp) > 0.1:
             return False
-        if (fabs(_p / self._Pn) < 0.99) or (fabs(_p / self._Pn) > 1.01):
+        if (math.fabs(_p / self._Pn) < 0.99) or (math.fabs(_p / self._Pn) > 1.01):
             return False
         return True
 
     def calc_neutralaxis(self, _p, _xmin, _xmax):
         if _xmin < self._ASDEngineZero:
             _xmin = self._ASDEngineZero
         if _xmax < self._ASDEngineZero:
@@ -254,15 +254,15 @@
 
             if self._Pn > _p:
                 _xmax = self._Xc
             else:
                 _xmin = self._Xc
 
     def calc_strain_rebar(self, _p, _mx, _my):
-        _mn = sqrt(_mx**2 + _my**2)  # if _mn == 0.0, consider setting _mn to a small nonzero value
+        _mn = math.sqrt(_mx**2 + _my**2)  # if _mn == 0.0, consider setting _mn to a small nonzero value
 
         self._Eyc = self._Fck / self._Ec
         for i in range(self._nIterationNo):
             self.calc_neutralaxis(_p, 0, 0)  # Assuming dXmin and dXmax need to be passed or determined within calc_neutralaxis
             if _mn < self._Mnxy:
                 break
 
@@ -302,70 +302,70 @@
         elif _my == 0.0:
             if _mx < 0.0:
                 _angle = -self._PI
             else:
                 _angle = 0.0
         elif _mx < 0.0:
             if _my < 0.0:
-                _angle = -self._PI + atan(_my / _mx)
+                _angle = -self._PI + math.atan(_my / _mx)
             else:
-                _angle = self._PI + atan(_my / _mx)
+                _angle = self._PI + math.atan(_my / _mx)
         else:
-            _angle = atan(_my / _mx)
+            _angle = math.atan(_my / _mx)
         return _angle
 
     def rotate_section(self, _rotation):
         self._RotationAngle = _rotation
 
         _dist_x = _dist_y = _dist = 0.0
         _angle = _theta = _length_temp = _length_max = float('-inf')
 
         for asd_con in self._arCon:
             _dist_x = asd_con['dX']
             _dist_y = asd_con['dY']
-            _dist = sqrt(_dist_x**2 + _dist_y**2)
+            _dist = math.sqrt(_dist_x**2 + _dist_y**2)
 
-            _angle = pi / 2.0 if _dist_x == 0.0 else atan(_dist_y / _dist_x)
+            _angle = math.pi / 2.0 if _dist_x == 0.0 else math.atan(_dist_y / _dist_x)
 
-            _length_temp = _dist * sin(_angle + _rotation)
+            _length_temp = _dist * math.sin(_angle + _rotation)
 
             if _dist_x < 0.0:
                 _length_temp *= -1.0
 
             if _length_temp > _length_max:
                 _length_max = _length_temp
                 self._OriginX = asd_con['dX'] + asd_con['dWidth'] / 2.0 if asd_con['dX'] > 0.0 else asd_con['dX'] - asd_con['dWidth'] / 2.0
                 self._OriginY = asd_con['dY'] + asd_con['dHeight'] / 2.0 if asd_con['dY'] > 0.0 else asd_con['dY'] - asd_con['dHeight'] / 2.0
 
         _dist_x = self._OriginX - self._CentroidX
         _dist_y = self._OriginY - self._CentroidY
-        _dist = sqrt(_dist_x**2 + _dist_y**2)
-        _angle = pi / 2.0 if fabs(_dist_x) < self._ASDEngineZero else atan(_dist_y / _dist_x)
+        _dist = math.sqrt(_dist_x**2 + _dist_y**2)
+        _angle = math.pi / 2.0 if math.fabs(_dist_x) < self._ASDEngineZero else math.atan(_dist_y / _dist_x)
         _theta = _rotation + _angle
-        _l_origin2centroid = fabs(_dist * sin(_theta))
+        _l_origin2centroid = math.fabs(_dist * math.sin(_theta))
 
         for asd_con in self._arCon:
             _dist_x = self._OriginX - asd_con['dX']
             _dist_y = self._OriginY - asd_con['dY']
-            _dist = sqrt(_dist_x**2 + _dist_y**2)
-            _angle = pi / 2.0 if fabs(_dist_x) < self._ASDEngineZero else atan(_dist_y / _dist_x)
+            _dist = math.sqrt(_dist_x**2 + _dist_y**2)
+            _angle = math.pi / 2.0 if math.fabs(_dist_x) < self._ASDEngineZero else math.atan(_dist_y / _dist_x)
             _theta = _rotation + _angle
 
-            asd_con['dDorigin'] = fabs(_dist * sin(_theta))
+            asd_con['dDorigin'] = math.fabs(_dist * math.sin(_theta))
             asd_con['dDcentroid'] = _l_origin2centroid - asd_con['dDorigin']
 
         _max_d = 0.0
         for asd_bar in self._arBar:
             _dist_x = self._OriginX - asd_bar['dX']
             _dist_y = self._OriginY - asd_bar['dY']
-            _dist = sqrt(_dist_x**2 + _dist_y**2)
-            _angle = pi / 2.0 if fabs(_dist_x) < self._ASDEngineZero else atan(_dist_y / _dist_x)
+            _dist = math.sqrt(_dist_x**2 + _dist_y**2)
+            _angle = math.pi / 2.0 if math.fabs(_dist_x) < self._ASDEngineZero else math.atan(_dist_y / _dist_x)
             _theta = _rotation + _angle
 
-            asd_bar['dDorigin'] = fabs(_dist * sin(_theta))
+            asd_bar['dDorigin'] = math.fabs(_dist * math.sin(_theta))
             asd_bar['dDcentroid'] = _l_origin2centroid - asd_bar['dDorigin']
 
             if asd_bar['dDorigin'] > _max_d:
                 _max_d = asd_bar['dDorigin']
 
         return _max_d
 
@@ -450,20 +450,20 @@
 
     def get_sigma2(self, _point_x, _point_y):
         if self._AxialOnly:
             return self.safe_div(self._Fx, self._Area)
 
         _dist_x = self._OriginX - _point_x
         _dist_y = self._OriginY - _point_y
-        _dist = sqrt(_dist_x**2 + _dist_y**2)
-        _angle = self._PI / 2.0 if fabs(_dist_x) < self._ASDEngineZero else atan(_dist_y / _dist_x)
+        _dist = math.sqrt(_dist_x**2 + _dist_y**2)
+        _angle = self._PI / 2.0 if math.fabs(_dist_x) < self._ASDEngineZero else math.atan(_dist_y / _dist_x)
         _theta = self._RotationAngle + _angle
 
-        _dorigin = fabs(_dist * sin(_theta))
-        _eyc = ((self._Xc - _dorigin) / self._Xc) * fabs(self._Eyc)
+        _dorigin = math.fabs(_dist * math.sin(_theta))
+        _eyc = ((self._Xc - _dorigin) / self._Xc) * math.fabs(self._Eyc)
         if self._Eyc < 0.0:
             _eyc += self._Eyc * 2.0
 
         _sigma = _eyc * self._Ec
         if _sigma < 0.0:
             _sigma = 0.0
 
@@ -500,12 +500,12 @@
         _sigma_my = self.safe_div(_mx, _zy)
         _sigma_mx_byp = self.safe_div(_p * _center_to_dcentroid_x * -1.0, _zx)
         _sigma_my_byp = self.safe_div(_p * _center_to_dcentroid_y * -1.0, _zy)
 
         return _sigma_p + _sigma_mx + _sigma_my + _sigma_mx_byp + _sigma_my_byp
 
     def eq0(self, value, tolerance=1.0e-7):
-        return fabs(value) < tolerance
+        return math.fabs(value) < tolerance
 
     def get_radian_tolerance(self):
         # Assuming a placeholder value for radian tolerance
         return 1.0e-4
```

### Comparing `mapieng-0.1.0/base/engineers_server.py` & `mapieng-0.1.1/base/engineers_server.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.0/base/engineers_web.py` & `mapieng-0.1.1/base/engineers_web.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.0/base/geometry.py` & `mapieng-0.1.1/base/geometry.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.0/base/hello.html` & `mapieng-0.1.1/base/hello.html`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.0/base/midasapi.py` & `mapieng-0.1.1/base/midasapi.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,35 +21,60 @@
     def db_create(item_name, items):
         url = f'{g_base_url}/db/{item_name}'
         return midas_util.post(url, headers=g_headers, json={'Assign': items})
 
     def db_create_item(item_name, item_id, item):
         url = f'{g_base_url}/db/{item_name}/{item_id}'
         return midas_util.post(url, headers=g_headers, json={'Assign': item})
-
-    def db_read(item_name):
+    
+    def db_read(item_name: str)-> dict:
+        """
+        Requst(using api) All items from the specified name collection
+        !!! don't use this function in the loop, it's too slow !!!
+        
+        Args:
+            item_name (str): The item name
+            
+        Returns:
+            dict: The item of the current document
+            e.g. db_read("NODE") -> {1: {'X': 0.0, 'Y': 0.0, 'Z': 0.0 }}
+            e.g. db_read("ELEM") -> {1: {'TYPE': 'BEAM', 'MATL': 1, 'SECT': 1, 'NODE': [1, 2, 0, 0, 0, 0, 0, 0], 'ANGLE': 0, 'STYPE': 0}}
+        """
         url = f'{g_base_url}/db/{item_name}'
         responseJson = midas_util.get(url, headers=g_headers)
         # check response.json()[item_name] is Exist
         if item_name not in responseJson:
-            # print(f"Error: Unable to find the registry key or value for {item_name}")
-            # return None
-            return midas_util.ERROR_DICT(message=f"Unable to find the registry key or value for {item_name}")
+            print(f"Error: Unable to find the registry key or value for {item_name}")
+            return None
+            # return midas_util.ERROR_DICT(message=f"Unable to find the registry key or value for {item_name}")
         keyVals = responseJson[item_name]
         return {int(k): v for k, v in keyVals.items()}
 
     def db_read_item(item_name, item_id):
+        """
+        Requst(using api) the item from the current document
+        !!! don't use this function in the loop, it's too slow !!!
+        
+        Args:
+            item_name (str): The item name
+            item_id (int): The item id
+            
+        Returns:
+            dict: The item of the current document
+            e.g. db_read_item("NODE", 1) -> {'X': 0.0, 'Y': 0.0, 'Z': 0.0 }
+            e.g. db_read_item("ELEM", 1) -> {'TYPE': 'BEAM', 'MATL': 1, 'SECT': 1, 'NODE': [1, 2, 0, 0, 0, 0, 0, 0], 'ANGLE': 0, 'STYPE': 0}
+        """
         item_id_str = str(item_id)
         url = f'{g_base_url}/db/{item_name}/{item_id_str}'
         responseJson = midas_util.get(url, headers=g_headers)
         # check response.json()[item_name] is Exist
         if item_name not in responseJson:
             print(f"Error: Unable to find the registry key or value for {item_name}")
-            # return None
-            return midas_util.ERROR_DICT(message=f"Unable to find the registry key or value for {item_name}")
+            return None
+            # return midas_util.ERROR_DICT(message=f"Unable to find the registry key or value for {item_name}")
         if item_id_str not in responseJson[item_name]:
             print(
                 f"Error: Unable to find the registry key or value for {item_id}")
             # return None
             return midas_util.ERROR_DICT(message=f"Unable to find the registry key or value for {item_id}")
         return responseJson[item_name][item_id_str]
 
@@ -82,14 +107,21 @@
         res_all = midas_util.db_read(item_name)
         if not res_all:
             return 1
         return min(map(int, res_all.keys()))
 
     ## view ############################################################################################################
     def view_select_get():
+        """
+        Get the selected NODE/ELEM of the current document view
+        
+        Returns:
+            dict: The selected NODE/ELEM of the current view
+            e.g. view_select_get() -> {'NODE_LIST': [1, 2], 'ELEM_LIST': [1]}        
+        """
         url = f'{g_base_url}/view/select'
         responseJson = midas_util.get(url, headers=g_headers)
         if 'error' in responseJson:
             return responseJson
         else:
             return responseJson['SELECT']
```

### Comparing `mapieng-0.1.0/base/midasutil.py` & `mapieng-0.1.1/base/midasutil.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.0/base/steel/KS18.json` & `mapieng-0.1.1/base/steel/KS18.json`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.0/base/steel/steelutil.py` & `mapieng-0.1.1/base/steel/steelutil.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 def get_fy(material_code, MatlName, thickness):
     materials = _read_materials_from_json(path)
     matl = "steel"
     if matl in materials:
         material = materials[matl]
         material = material[material_code]
         fy_data = material[0]['Fy']
-        fu_value = material[1]['Fu']
         fy_value = _get_fy_for_thickness(fy_data, thickness)
         return fy_value
     else:
         return None
 
 def get_fu(material_code, MatlName, thickness):
     materials = _read_materials_from_json(path)
@@ -43,40 +42,40 @@
     if matl in materials:
         material = materials[matl]
         material = material[material_code]
         fu_value = material[1]['Fu']
         return fu_value
     else:
         return None
-    
+
 def get_bolt_Fnt(material_code):
     materials = _read_materials_from_json(path)
     matl = "bolt"
     if matl in materials:
         material = materials[matl]
         material = material[material_code]
         Fnt_data = material['Fnt']
         return Fnt_data
     else:
         return None
-    
+
 def get_bolt_Fnv(material_code):
     materials = _read_materials_from_json(path)
     matl = "bolt"
     if matl in materials:
         material = materials[matl]
         material = material[material_code]
         Fnt_data = material['Fnv']
         return Fnt_data
     else:
         return None
-    
+
 def get_bolt_Fu(material_code):
     materials = _read_materials_from_json(path)
     matl = "bolt"
     if matl in materials:
         material = materials[matl]
         material = material[material_code]
         Fnt_data = material['Fu']
         return Fnt_data
     else:
-        return None
+        return None
```

### Comparing `mapieng-0.1.0/base/symbol.py` & `mapieng-0.1.1/base/symbol.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.0/base/unit_converter.py` & `mapieng-0.1.1/base/unit_converter.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.0/base/vector.py` & `mapieng-0.1.1/base/vector.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.0/mapieng.egg-info/SOURCES.txt` & `mapieng-0.1.1/mapieng.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 base/baseformidasapi.py
 base/calculator_asd.py
 base/engineers.py
 base/engineers_server.py
 base/engineers_web.py
 base/geometry.py
 base/hello.html
-base/meshutil.py
 base/midasapi.py
 base/midasutil.py
+base/section_property.py
 base/symbol.py
 base/test.py
-base/testmesh.py
 base/unit_converter.py
 base/vector.py
 base/steel/KS18.json
 base/steel/__init__.py
 base/steel/steelutil.py
 mapieng.egg-info/PKG-INFO
 mapieng.egg-info/SOURCES.txt
 mapieng.egg-info/dependency_links.txt
 mapieng.egg-info/requires.txt
 mapieng.egg-info/top_level.txt
 project/__init__.py
-project/baseplate_KDS41_30_2022/Test.py
 project/baseplate_KDS41_30_2022/__init__.py
 project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py
-project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py
+project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py
+tests/__init__.py
+tests/test_baseplate_kds.py
```

### Comparing `mapieng-0.1.0/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py` & `mapieng-0.1.1/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.0/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py` & `mapieng-0.1.1/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.0/setup.py` & `mapieng-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
+
 setup(
     name='mapieng',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     include_package_data=True,
     description='mapi engineers',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     license='MIT',
     author='bschoi',
     url='https://github.com/MIDASIT-Co-Ltd/engineers-api-python',
     install_requires=['mdutils', "numpy", "matplotlib",],
-    
-)
+    )
```

