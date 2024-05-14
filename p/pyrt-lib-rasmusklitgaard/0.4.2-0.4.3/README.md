# Comparing `tmp/pyrt_lib_rasmusklitgaard-0.4.2.tar.gz` & `tmp/pyrt_lib_rasmusklitgaard-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrt_lib_rasmusklitgaard-0.4.2.tar", last modified: Tue May  7 12:46:00 2024, max compression
+gzip compressed data, was "pyrt_lib_rasmusklitgaard-0.4.3.tar", last modified: Tue May 14 12:55:50 2024, max compression
```

## Comparing `pyrt_lib_rasmusklitgaard-0.4.2.tar` & `pyrt_lib_rasmusklitgaard-0.4.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-07 12:46:00.282420 pyrt_lib_rasmusklitgaard-0.4.2/
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    35076 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.2/LICENSE
--rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1776 2024-05-07 12:46:00.278420 pyrt_lib_rasmusklitgaard-0.4.2/PKG-INFO
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      967 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.2/README.md
--rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)     1060 2024-05-07 12:45:54.000000 pyrt_lib_rasmusklitgaard-0.4.2/pyproject.toml
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-07 12:46:00.278420 pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard/
--rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      150 2024-05-01 13:21:00.000000 pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard/__init__.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4113 2024-05-07 12:45:58.000000 pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard/cohort.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    11066 2024-05-07 12:45:58.000000 pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard/helpers.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      793 2024-04-09 08:44:14.000000 pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard/image_looper.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    14910 2024-05-07 12:45:58.000000 pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     8758 2024-05-07 12:45:58.000000 pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard/parameter_parser.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    32603 2024-05-07 12:45:58.000000 pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard/patient.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    12317 2024-05-07 12:45:58.000000 pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard/pyrt_database.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4724 2024-05-07 12:45:58.000000 pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard/resample.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     1242 2024-05-07 12:45:58.000000 pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard/select_structures.py
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-07 12:46:00.278420 pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard.egg-info/
--rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1776 2024-05-07 12:46:00.000000 pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      714 2024-05-07 12:46:00.000000 pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)        1 2024-05-07 12:46:00.000000 pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard.egg-info/dependency_links.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      134 2024-05-07 12:46:00.000000 pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard.egg-info/entry_points.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      140 2024-05-07 12:46:00.000000 pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard.egg-info/requires.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       25 2024-05-07 12:46:00.000000 pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard.egg-info/top_level.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       38 2024-05-07 12:46:00.282420 pyrt_lib_rasmusklitgaard-0.4.2/setup.cfg
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-14 12:55:50.128553 pyrt_lib_rasmusklitgaard-0.4.3/
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    35076 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.3/LICENSE
+-rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1777 2024-05-14 12:55:50.128553 pyrt_lib_rasmusklitgaard-0.4.3/PKG-INFO
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      967 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.3/README.md
+-rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)     1061 2024-05-14 12:55:45.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyproject.toml
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-14 12:55:50.124553 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/
+-rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      150 2024-05-01 13:21:00.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/__init__.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4113 2024-05-14 12:55:47.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/cohort.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    11578 2024-05-14 12:55:47.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/helpers.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      793 2024-04-09 08:44:14.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/image_looper.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    14910 2024-05-14 12:55:47.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     8758 2024-05-14 12:55:47.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/parameter_parser.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    32694 2024-05-14 12:55:47.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/patient.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    12316 2024-05-14 12:55:47.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/pyrt_database.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4724 2024-05-14 12:55:47.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/resample.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     1242 2024-05-14 12:55:47.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/select_structures.py
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-14 12:55:50.124553 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard.egg-info/
+-rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1777 2024-05-14 12:55:50.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      714 2024-05-14 12:55:50.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)        1 2024-05-14 12:55:50.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard.egg-info/dependency_links.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      134 2024-05-14 12:55:50.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard.egg-info/entry_points.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      141 2024-05-14 12:55:50.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard.egg-info/requires.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       25 2024-05-14 12:55:50.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard.egg-info/top_level.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       38 2024-05-14 12:55:50.128553 pyrt_lib_rasmusklitgaard-0.4.3/setup.cfg
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.2/LICENSE` & `pyrt_lib_rasmusklitgaard-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.2/PKG-INFO` & `pyrt_lib_rasmusklitgaard-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyrt_lib_rasmusklitgaard
-Version: 0.4.2
+Version: 0.4.3
 Summary: PYthon RadioTherapy library
 Author-email: Rasmus Klitgaard <rasmusklitgaard97@gmail.com>
 Project-URL: Homepage, https://gitlab.com/dcpt-research/pyrt-lib
 Project-URL: Issues, https://gitlab.com/dcpt-research/pyrt-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.26.3
 Requires-Dist: matplotlib>=3.5.1
 Requires-Dist: openpyxl>=3.1.2
 Requires-Dist: pymedphys>=0.39.3
-Requires-Dist: scipy>=1.8.0
+Requires-Dist: scipy>=1.13.0
 Requires-Dist: pydicom>=1.4.1
 Requires-Dist: numba>=0.58.1
 Requires-Dist: SimpleITK>=2.3.1
 Requires-Dist: shapely>=1.8.0
 
 # pyrt-lib
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.2/README.md` & `pyrt_lib_rasmusklitgaard-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.2/pyproject.toml` & `pyrt_lib_rasmusklitgaard-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pyrt_lib_rasmusklitgaard"
-version = "0.4.2"
+version = "0.4.3"
 authors = [
   { name="Rasmus Klitgaard", email="rasmusklitgaard97@gmail.com" },
 ]
 description = "PYthon RadioTherapy library"
 readme = "README.md"
 dependencies = [
 "numpy>=1.26.3",
 "matplotlib>=3.5.1",
 "openpyxl>=3.1.2",
 "pymedphys>=0.39.3",
-"scipy>=1.8.0",
+"scipy>=1.13.0",
 "pydicom>=1.4.1",
 "numba>=0.58.1",
 "SimpleITK>=2.3.1",
 "shapely>=1.8.0",
 ]
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard/cohort.py` & `pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/cohort.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard/helpers.py` & `pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 	code.InteractiveConsole(vars).interact()	
 
 def printStructures(structure):
 	print("There are the following structures available in your RTSTRUCT:")
 	for i, name in enumerate([a.ROIName for a in structure.StructureSetROISequence]):
 		print("{0:2}: {1}".format(i,name))
 
-def selectStructures(structure, selections):
+def selectStructures(structure, selections, ctvfallback=None):
 	"""
 		This function takes an RTSTRUCT and a list of wanted structure names
 		It then tries to find them automagically based on their names,
 		but if unable it will prompt the user for help.
 		If one is not available the user can enter this
 		and the function will return with the ones found.
 		The function returns a list of strings corresponding to the structurenames.
@@ -158,26 +158,36 @@
 			break
 	if not iii == -1:
 		del selections[iii]
 
 	return_list = ["NOT_FOUND_YET"] * len(selections)
 	# first we try to find the correct structures. Then only ask for what we need.
 	listOfStructures = [a.ROIName for a in structure.StructureSetROISequence]
-	for j,sel in enumerate(selections):
+	for j,sel in enumerate(selections):			
 		if sel.lower() in [l.lower() for l in listOfStructures] \
 		or sel.lower() in [l.lower().replace("_"," ") for l in listOfStructures] \
 		or sel.lower().replace("_"," ") in [l.lower() for l in listOfStructures]:
-
 			sel_indx = -1
 			for i, name in enumerate(listOfStructures):
 				if sel.lower() == name.lower() or sel.lower().replace("_"," ") == name.lower():
 					sel_indx = j
 					break
 			if sel_indx != -1:
 				return_list[sel_indx] = name
+		elif ctvfallback.lower() in [l.lower() for l in listOfStructures] \
+		or ctvfallback.lower() in [l.lower().replace("_"," ") for l in listOfStructures] \
+		or ctvfallback.lower().replace("_"," ") in [l.lower() for l in listOfStructures]:
+			sel_indx = -1
+			for i, name in enumerate(listOfStructures):
+				if ctvfallback.lower() == name.lower() or ctvfallback.lower().replace("_"," ") == name.lower():
+					sel_indx = j
+					break
+			if sel_indx != -1:
+				return_list[sel_indx] = name
+				
 	if "NOT_FOUND_YET" not in return_list:
 		return return_list
 	
 	missing_indices = []
 	for i, struct in enumerate(return_list):
 		if struct == "NOT_FOUND_YET":
 			missing_indices.append(i)
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard/image_looper.py` & `pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/image_looper.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard/lkb_ntcp.py` & `pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/lkb_ntcp.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard/parameter_parser.py` & `pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/parameter_parser.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard/patient.py` & `pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/patient.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 import copy
 
 class Patient():
 	# class to hold all info on a patient.
 	def __init__(self, 
 				patient_folder_path: str,
 				wanted_structures: list = "default",
-				xlsx_workbook: openpyxl.workbook.workbook.Workbook = None) -> None:
+				xlsx_workbook: openpyxl.workbook.workbook.Workbook = None,
+				*args, **kwargs) -> None:
 		t0=time.time()
 		self.rtdose_letd = None
 		self.rtdose_dose = None
 		self.rtstruct	 = None
 		t1=time.time()
 		self.path_to_rtdose_letd = None
 		self.path_to_rtdose_dose = None
@@ -47,15 +48,15 @@
 		t5=time.time()
 		self.set_default_rtdoses()
 		t6=time.time()
 
 		try:
 			if self.wanted_structures == "default":
 				self.wanted_structures = ["ctv", "bladder", "bladder wall", "rectum", "rectal wall", "Bladder Wall", "Rectal Wall", "Rectum", "Bladder", "CTV", "Rectal_Wall", "Bladder_Wall"]
-			self.actual_structure_names = self.get_actual_structure_names(self.wanted_structures)
+			self.actual_structure_names = self.get_actual_structure_names(self.wanted_structures , *args, **kwargs)
 		except AttributeError as e:
 			print("THERE HAS BEEN AN ATTRIBUTE ERROR")
 			print(str(e))
 			code_interact(globals(),locals())
 		t7=time.time()
 
 		self.set_structure_indices()
@@ -318,15 +319,15 @@
 		patient_metadata = {}
 		for column_id, column_header in column_headers.items():
 			this_value = patient_data_sheet["{0}{1}".format(column_id, this_patient_row)].value
 			patient_metadata[column_header] = this_value
 
 		return patient_metadata
 
-	def get_actual_structure_names(self, wanted_structures: list):
+	def get_actual_structure_names(self, wanted_structures: list , *args, **kwargs):
 		if not wanted_structures:
 			return None
 		if self.rtstruct == None or self.rtdose_dose == None or self.rtdose_letd == None:
 			self.set_default_rtdoses()
 
 		actual_structurenames_found = False
 		actual_structurenames_file = ""
@@ -340,25 +341,25 @@
 			with open(actual_structurenames_file, "r") as f:
 				for line in f:
 					key = line.split(":")[0]
 					val = line.split(":")[-1].replace("\n","")
 					actual_structurenames_dict[key] = val
 			for wanted_struct in wanted_structures: 
 				if wanted_struct not in list(actual_structurenames_dict.keys()):
-					act_struct = selectStructures(self.rtstruct, [wanted_struct])[0]
+					act_struct = selectStructures(self.rtstruct, [wanted_struct], *args, **kwargs)[0]
 					actual_structurenames_dict[wanted_struct] = act_struct
 					with open(actual_structurenames_file, "a") as f:
 						f.write("{}:{}\n".format(wanted_struct, act_struct))
 			add_these = list(actual_structurenames_dict.values())
 			for value in add_these:
 				actual_structurenames_dict[value] = value
 			return actual_structurenames_dict
 
 
-		actual_structures = selectStructures(self.rtstruct, wanted_structures)
+		actual_structures = selectStructures(self.rtstruct, wanted_structures, *args, **kwargs)
 		writepath = ""
 		writepath = writepath + self.patient_folder_path
 		if not self.patient_folder_path[-1] == "/":
 			writepath = writepath + "/"
 		writepath = writepath + "actual_structure_names.txt"
 		with open(writepath, "w") as f:
 			for key, value in zip(wanted_structures, actual_structures):
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard/pyrt_database.py` & `pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/pyrt_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 
 def load_patient(patient_path):
     return Patient(patient_path, wanted_structures="default")
 
 def get_database_path(database_name):
     # Returns a list of dictionaries, each list element relating to a patient.
 
-
     database_path = ""
     with open(str(config_file_path), 'r') as f:
         for line in f:
             this_database_path = line.split(":")[0].strip()
             this_database_name = str(Path(this_database_path).name).strip()
             if this_database_name == database_name:
                 database_path = this_database_path
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard/resample.py` & `pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/resample.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard/select_structures.py` & `pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/select_structures.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO` & `pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyrt_lib_rasmusklitgaard
-Version: 0.4.2
+Version: 0.4.3
 Summary: PYthon RadioTherapy library
 Author-email: Rasmus Klitgaard <rasmusklitgaard97@gmail.com>
 Project-URL: Homepage, https://gitlab.com/dcpt-research/pyrt-lib
 Project-URL: Issues, https://gitlab.com/dcpt-research/pyrt-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.26.3
 Requires-Dist: matplotlib>=3.5.1
 Requires-Dist: openpyxl>=3.1.2
 Requires-Dist: pymedphys>=0.39.3
-Requires-Dist: scipy>=1.8.0
+Requires-Dist: scipy>=1.13.0
 Requires-Dist: pydicom>=1.4.1
 Requires-Dist: numba>=0.58.1
 Requires-Dist: SimpleITK>=2.3.1
 Requires-Dist: shapely>=1.8.0
 
 # pyrt-lib
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.2/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt` & `pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

