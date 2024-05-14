# Comparing `tmp/ofdcomparer-1.5.42.tar.gz` & `tmp/ofdcomparer-1.5.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofdcomparer-1.5.42.tar", last modified: Fri Apr 26 16:04:32 2024, max compression
+gzip compressed data, was "ofdcomparer-1.5.43.tar", last modified: Tue May 14 05:55:24 2024, max compression
```

## Comparing `ofdcomparer-1.5.42.tar` & `ofdcomparer-1.5.43.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:04:32.066263 ofdcomparer-1.5.42/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-19 22:27:07.000000 ofdcomparer-1.5.42/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1567 2024-04-26 16:04:32.066263 ofdcomparer-1.5.42/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      975 2023-11-15 14:23:23.000000 ofdcomparer-1.5.42/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:04:32.065263 ofdcomparer-1.5.42/ofdcomparer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-19 22:27:07.000000 ofdcomparer-1.5.42/ofdcomparer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2024-01-20 12:23:39.000000 ofdcomparer-1.5.42/ofdcomparer/allure_helper.py
--rw-rw-rw-   0 root         (0) root         (0)    21525 2024-04-04 19:15:02.000000 ofdcomparer-1.5.42/ofdcomparer/compare_ffd.py
--rw-rw-rw-   0 root         (0) root         (0)      145 2024-04-26 16:04:11.000000 ofdcomparer-1.5.42/ofdcomparer/configs.py
--rw-rw-rw-   0 root         (0) root         (0)    13995 2024-04-26 16:04:11.000000 ofdcomparer-1.5.42/ofdcomparer/convert.py
--rw-rw-rw-   0 root         (0) root         (0)    39684 2024-04-26 16:04:11.000000 ofdcomparer-1.5.42/ofdcomparer/dto10.py
--rw-rw-rw-   0 root         (0) root         (0)    38192 2024-04-26 16:04:11.000000 ofdcomparer-1.5.42/ofdcomparer/dto_error_descriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8301 2024-03-06 23:14:00.000000 ofdcomparer-1.5.42/ofdcomparer/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1562 2024-04-26 16:04:11.000000 ofdcomparer-1.5.42/ofdcomparer/ofd_cri_atol.py
--rw-rw-rw-   0 root         (0) root         (0)     2183 2024-01-20 12:23:39.000000 ofdcomparer-1.5.42/ofdcomparer/ofd_taxcom.py
--rw-rw-rw-   0 root         (0) root         (0)    40745 2024-04-26 16:04:11.000000 ofdcomparer-1.5.42/ofdcomparer/tags_fn.py
--rw-rw-rw-   0 root         (0) root         (0)    10168 2024-04-04 19:15:02.000000 ofdcomparer-1.5.42/ofdcomparer/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:04:32.066263 ofdcomparer-1.5.42/ofdcomparer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1567 2024-04-26 16:04:32.000000 ofdcomparer-1.5.42/ofdcomparer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      516 2024-04-26 16:04:32.000000 ofdcomparer-1.5.42/ofdcomparer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 16:04:32.000000 ofdcomparer-1.5.42/ofdcomparer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-26 16:04:32.000000 ofdcomparer-1.5.42/ofdcomparer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-26 16:04:32.000000 ofdcomparer-1.5.42/ofdcomparer.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-26 16:04:32.067263 ofdcomparer-1.5.42/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-26 16:04:11.000000 ofdcomparer-1.5.42/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 05:55:24.976123 ofdcomparer-1.5.43/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-20 08:16:51.000000 ofdcomparer-1.5.43/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1567 2024-05-14 05:55:24.976123 ofdcomparer-1.5.43/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      975 2023-11-06 21:06:45.000000 ofdcomparer-1.5.43/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 05:55:24.974123 ofdcomparer-1.5.43/ofdcomparer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-20 08:16:51.000000 ofdcomparer-1.5.43/ofdcomparer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2024-01-12 07:39:03.000000 ofdcomparer-1.5.43/ofdcomparer/allure_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)    21905 2024-05-14 05:55:09.000000 ofdcomparer-1.5.43/ofdcomparer/compare_ffd.py
+-rw-rw-rw-   0 root         (0) root         (0)      145 2024-04-11 05:15:32.000000 ofdcomparer-1.5.43/ofdcomparer/configs.py
+-rw-rw-rw-   0 root         (0) root         (0)    13995 2024-04-11 05:15:32.000000 ofdcomparer-1.5.43/ofdcomparer/convert.py
+-rw-rw-rw-   0 root         (0) root         (0)    39683 2024-05-14 05:55:09.000000 ofdcomparer-1.5.43/ofdcomparer/dto10.py
+-rw-rw-rw-   0 root         (0) root         (0)    38192 2024-04-11 05:15:32.000000 ofdcomparer-1.5.43/ofdcomparer/dto_error_descriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8301 2024-01-25 10:39:56.000000 ofdcomparer-1.5.43/ofdcomparer/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1562 2024-04-11 15:37:51.000000 ofdcomparer-1.5.43/ofdcomparer/ofd_cri_atol.py
+-rw-rw-rw-   0 root         (0) root         (0)     2183 2024-01-12 14:13:15.000000 ofdcomparer-1.5.43/ofdcomparer/ofd_taxcom.py
+-rw-rw-rw-   0 root         (0) root         (0)    40745 2024-05-14 05:55:09.000000 ofdcomparer-1.5.43/ofdcomparer/tags_fn.py
+-rw-rw-rw-   0 root         (0) root         (0)    10168 2024-04-11 05:15:32.000000 ofdcomparer-1.5.43/ofdcomparer/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 05:55:24.976123 ofdcomparer-1.5.43/ofdcomparer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1567 2024-05-14 05:55:24.000000 ofdcomparer-1.5.43/ofdcomparer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      516 2024-05-14 05:55:24.000000 ofdcomparer-1.5.43/ofdcomparer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 05:55:24.000000 ofdcomparer-1.5.43/ofdcomparer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-14 05:55:24.000000 ofdcomparer-1.5.43/ofdcomparer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-14 05:55:24.000000 ofdcomparer-1.5.43/ofdcomparer.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-14 05:55:24.977123 ofdcomparer-1.5.43/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-14 05:55:09.000000 ofdcomparer-1.5.43/setup.py
```

### Comparing `ofdcomparer-1.5.42/PKG-INFO` & `ofdcomparer-1.5.43/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofdcomparer
-Version: 1.5.42
+Version: 1.5.43
 Summary: Библиотека для сравнивания ФД из ФН и ОФД
 Home-page: UNKNOWN
 Author-email: k.kabisova@atol.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ofdcomparer-1.5.42/README.md` & `ofdcomparer-1.5.43/README.md`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.42/ofdcomparer/compare_ffd.py` & `ofdcomparer-1.5.43/ofdcomparer/compare_ffd.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 
 from ofdcomparer import ofd_cri_atol
 from ofdcomparer.allure_helper import attach_compare_results
 from ofdcomparer.tags_fn import tags
 from ofdcomparer.utils import Utils, DictModifier
 
 
+class GetFdFnError(Exception):
+    def __init__(self, message='Ошибка получения документа из ФН'):
+        super().__init__(message)
+        self.message = message
+
+
 class ComparerOfd:
     def __init__(self, dto10):
         # Конечный результат обработки
         self.result = {}
         self.DTO10 = dto10
         self.utils = Utils(self.DTO10)
         self.dict_modifier = DictModifier()
@@ -90,14 +96,16 @@
         Метод сравнивает эталон с последним ФД в ФН.
         """
         logging.debug(f"{inspect.currentframe().f_code.co_name} < {etalon=} {changes=} {rnm} {fn} {fd}")
         logging.info("Сравнение ФД, ЭТАЛОН : ФН : ОФД")
         if bool(changes):
             etalon = self.dict_modifier.change_values_in_dict(etalon, changes)
         comparable = self.DTO10.get_fd_from_fn(self.DTO10.get_last_fd_number())
+        if comparable is None:
+            raise GetFdFnError
         logging.info("Сравнение ФД, ЭТАЛОН : ФН")
         self.compare(etalon=etalon,
                      comparable=comparable)
         self.output_result_to_log()
         attach_compare_results(result=self.result, name="Результат сравнения ФД. ЭТАЛОН - ФН")
         if self.is_have_failed():
             return False
@@ -110,14 +118,16 @@
         Метод сравнивает эталон с последним ФД в ФН, затем последний ФД в ФН с ФД в ОФД.
         """
         logging.debug(f"{inspect.currentframe().f_code.co_name} < {etalon=} {changes=} {rnm} {fn} {fd}")
         logging.info("Сравнение ФД, ЭТАЛОН : ФН : ОФД")
         if bool(changes):
             etalon = self.dict_modifier.change_values_in_dict(etalon, changes)
         comparable = self.DTO10.get_fd_from_fn(self.DTO10.get_last_fd_number())
+        if comparable is None:
+            raise GetFdFnError
         logging.info("Сравнение ФД, ЭТАЛОН : ФН")
         self.compare(etalon=etalon,
                      comparable=comparable)
         self.output_result_to_log()
         attach_compare_results(result=self.result, name="Результат сравнения ФД. ЭТАЛОН - ФН")
         if self.is_have_failed():
             return False
@@ -142,14 +152,16 @@
         logging.info("Сравнение ФД, ФН : ОФД")
         if rnm is None:
             rnm = self.DTO10.registrationNumber
         if fn is None:
             fn = self.DTO10.fnSerial
         if fd is None:
             fd = self.DTO10.get_fd_from_fn(self.DTO10.get_last_fd_number())
+            if fd is None:
+                raise GetFdFnError
         if bool(changes):
             fd = self.dict_modifier.change_values_in_dict(fd, changes)
         self.DTO10.wait_for_sent_all_fd()
         self.compare_tags(rnm=rnm, fn=fn, fd=fd)
         self.output_result_to_log()
         if self.is_have_failed():
             return False
```

### Comparing `ofdcomparer-1.5.42/ofdcomparer/convert.py` & `ofdcomparer-1.5.43/ofdcomparer/convert.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.42/ofdcomparer/dto10.py` & `ofdcomparer-1.5.43/ofdcomparer/dto10.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,14 @@
         Извлечение ФД из ФН
         """
         logging.debug(f"get_fd_from_fn() < {fd}")
         if fd is None:
             logging.debug(f"get_fd_from_fn() > None")
             return None
         # JSON задание для чтения документа из ФН
-
         json_task = {
             "type": "getFnDocument",
             "fiscalDocumentNumber": int(fd),
             "withRawData": False,
         }
         fd_fn = self.execute_json(json_task)
         if fd_fn is None:
```

### Comparing `ofdcomparer-1.5.42/ofdcomparer/dto_error_descriptions.py` & `ofdcomparer-1.5.43/ofdcomparer/dto_error_descriptions.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.42/ofdcomparer/helpers.py` & `ofdcomparer-1.5.43/ofdcomparer/helpers.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.42/ofdcomparer/ofd_cri_atol.py` & `ofdcomparer-1.5.43/ofdcomparer/ofd_cri_atol.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.42/ofdcomparer/ofd_taxcom.py` & `ofdcomparer-1.5.43/ofdcomparer/ofd_taxcom.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.42/ofdcomparer/tags_fn.py` & `ofdcomparer-1.5.43/ofdcomparer/tags_fn.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.42/ofdcomparer/utils.py` & `ofdcomparer-1.5.43/ofdcomparer/utils.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.42/ofdcomparer.egg-info/PKG-INFO` & `ofdcomparer-1.5.43/ofdcomparer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofdcomparer
-Version: 1.5.42
+Version: 1.5.43
 Summary: Библиотека для сравнивания ФД из ФН и ОФД
 Home-page: UNKNOWN
 Author-email: k.kabisova@atol.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ofdcomparer-1.5.42/ofdcomparer.egg-info/SOURCES.txt` & `ofdcomparer-1.5.43/ofdcomparer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.42/setup.py` & `ofdcomparer-1.5.43/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="ofdcomparer",
-    version="1.5.42",
+    version="1.5.43",
     long_description=long_description,
     description="Библиотека для сравнивания ФД из ФН и ОФД",
     packages=["ofdcomparer"],
     author_email="k.kabisova@atol.ru",
     install_requires=[
         "requests==2.31.0",
         "requests-toolbelt==1.0.0",
```

