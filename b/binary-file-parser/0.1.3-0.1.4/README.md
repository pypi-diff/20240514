# Comparing `tmp/binary-file-parser-0.1.3.tar.gz` & `tmp/binary_file_parser-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binary-file-parser-0.1.3.tar", last modified: Fri Feb 23 10:57:33 2024, max compression
+gzip compressed data, was "binary_file_parser-0.1.4.tar", last modified: Tue May 14 12:27:38 2024, max compression
```

## Comparing `binary-file-parser-0.1.3.tar` & `binary_file_parser-0.1.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-02-23 10:57:33.482445 binary-file-parser-0.1.3/
--rw-rw-rw-   0        0        0     1084 2022-12-14 12:48:09.000000 binary-file-parser-0.1.3/LICENSE
--rw-rw-rw-   0        0        0        0 2022-12-15 05:10:52.000000 binary-file-parser-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6028 2024-02-23 10:57:33.480443 binary-file-parser-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3865 2023-08-26 05:31:53.000000 binary-file-parser-0.1.3/README.md
--rw-rw-rw-   0        0        0      908 2024-02-23 10:55:24.000000 binary-file-parser-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-23 10:57:33.483443 binary-file-parser-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-23 10:57:33.393443 binary-file-parser-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2024-02-23 10:57:33.408444 binary-file-parser-0.1.3/src/binary_file_parser/
--rw-rw-rw-   0        0        0      290 2023-05-02 04:00:31.000000 binary-file-parser-0.1.3/src/binary_file_parser/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 10:57:33.432444 binary-file-parser-0.1.3/src/binary_file_parser/errors/
--rw-rw-rw-   0        0        0      118 2022-12-15 18:24:53.000000 binary-file-parser-0.1.3/src/binary_file_parser/errors/CompressionError.py
--rw-rw-rw-   0        0        0      119 2023-08-30 11:43:12.000000 binary-file-parser-0.1.3/src/binary_file_parser/errors/DefaultValueError.py
--rw-rw-rw-   0        0        0       42 2022-12-15 07:13:59.000000 binary-file-parser-0.1.3/src/binary_file_parser/errors/ParsingError.py
--rw-rw-rw-   0        0        0      114 2022-12-15 18:24:20.000000 binary-file-parser-0.1.3/src/binary_file_parser/errors/VersionError.py
--rw-rw-rw-   0        0        0      178 2023-08-30 11:43:12.000000 binary-file-parser-0.1.3/src/binary_file_parser/errors/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 10:57:33.448445 binary-file-parser-0.1.3/src/binary_file_parser/retrievers/
--rw-rw-rw-   0        0        0     2647 2023-02-18 09:06:26.000000 binary-file-parser-0.1.3/src/binary_file_parser/retrievers/MapValidate.py
--rw-rw-rw-   0        0        0     2272 2023-04-24 11:23:48.000000 binary-file-parser-0.1.3/src/binary_file_parser/retrievers/RetreiverCombiner.py
--rw-rw-rw-   0        0        0     1518 2023-04-24 11:16:38.000000 binary-file-parser-0.1.3/src/binary_file_parser/retrievers/RetreiverRef.py
--rw-rw-rw-   0        0        0    12583 2024-02-23 10:54:26.000000 binary-file-parser-0.1.3/src/binary_file_parser/retrievers/Retriever.py
--rw-rw-rw-   0        0        0      199 2023-04-21 01:37:15.000000 binary-file-parser-0.1.3/src/binary_file_parser/retrievers/__init__.py
--rw-rw-rw-   0        0        0    16316 2024-02-23 10:54:26.000000 binary-file-parser-0.1.3/src/binary_file_parser/retrievers/base_struct.py
-drwxrwxrwx   0        0        0        0 2024-02-23 10:57:33.477443 binary-file-parser-0.1.3/src/binary_file_parser/types/
--rw-rw-rw-   0        0        0     6438 2023-04-21 03:06:40.000000 binary-file-parser-0.1.3/src/binary_file_parser/types/Array.py
--rw-rw-rw-   0        0        0      928 2023-04-18 12:21:20.000000 binary-file-parser-0.1.3/src/binary_file_parser/types/Bool.py
--rw-rw-rw-   0        0        0     2796 2022-11-29 16:43:10.000000 binary-file-parser-0.1.3/src/binary_file_parser/types/ByteStream.py
--rw-rw-rw-   0        0        0      855 2023-04-18 12:21:20.000000 binary-file-parser-0.1.3/src/binary_file_parser/types/Bytes.py
--rw-rw-rw-   0        0        0      867 2023-04-18 12:21:20.000000 binary-file-parser-0.1.3/src/binary_file_parser/types/Float.py
--rw-rw-rw-   0        0        0      987 2023-04-18 12:21:20.000000 binary-file-parser-0.1.3/src/binary_file_parser/types/Int.py
--rw-rw-rw-   0        0        0     1345 2023-04-21 02:01:03.000000 binary-file-parser-0.1.3/src/binary_file_parser/types/Parseable.py
--rw-rw-rw-   0        0        0     3272 2024-02-23 10:54:26.000000 binary-file-parser-0.1.3/src/binary_file_parser/types/RefList.py
--rw-rw-rw-   0        0        0     3037 2023-04-18 12:21:20.000000 binary-file-parser-0.1.3/src/binary_file_parser/types/Str.py
--rw-rw-rw-   0        0        0      564 2023-09-09 10:18:09.000000 binary-file-parser-0.1.3/src/binary_file_parser/types/__init__.py
--rw-rw-rw-   0        0        0      894 2023-09-09 09:57:11.000000 binary-file-parser-0.1.3/src/binary_file_parser/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-23 10:57:33.479443 binary-file-parser-0.1.3/src/binary_file_parser.egg-info/
--rw-rw-rw-   0        0        0     6028 2024-02-23 10:57:33.000000 binary-file-parser-0.1.3/src/binary_file_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1260 2024-02-23 10:57:33.000000 binary-file-parser-0.1.3/src/binary_file_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-23 10:57:33.000000 binary-file-parser-0.1.3/src/binary_file_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2024-02-23 10:57:33.000000 binary-file-parser-0.1.3/src/binary_file_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-02-23 10:57:33.000000 binary-file-parser-0.1.3/src/binary_file_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 12:27:38.032729 binary_file_parser-0.1.4/
+-rw-rw-rw-   0        0        0     1084 2022-12-14 12:48:09.000000 binary_file_parser-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0        0 2022-12-15 05:10:52.000000 binary_file_parser-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6028 2024-05-14 12:27:38.029729 binary_file_parser-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3865 2023-08-26 05:31:53.000000 binary_file_parser-0.1.4/README.md
+-rw-rw-rw-   0        0        0      908 2024-05-14 12:15:10.000000 binary_file_parser-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-14 12:27:38.032729 binary_file_parser-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-14 12:27:37.922728 binary_file_parser-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 12:27:37.937742 binary_file_parser-0.1.4/src/binary_file_parser/
+-rw-rw-rw-   0        0        0      290 2023-05-02 04:00:31.000000 binary_file_parser-0.1.4/src/binary_file_parser/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:27:37.963729 binary_file_parser-0.1.4/src/binary_file_parser/errors/
+-rw-rw-rw-   0        0        0      118 2022-12-15 18:24:53.000000 binary_file_parser-0.1.4/src/binary_file_parser/errors/CompressionError.py
+-rw-rw-rw-   0        0        0      119 2023-08-30 11:43:12.000000 binary_file_parser-0.1.4/src/binary_file_parser/errors/DefaultValueError.py
+-rw-rw-rw-   0        0        0       42 2022-12-15 07:13:59.000000 binary_file_parser-0.1.4/src/binary_file_parser/errors/ParsingError.py
+-rw-rw-rw-   0        0        0      114 2022-12-15 18:24:20.000000 binary_file_parser-0.1.4/src/binary_file_parser/errors/VersionError.py
+-rw-rw-rw-   0        0        0      178 2023-08-30 11:43:12.000000 binary_file_parser-0.1.4/src/binary_file_parser/errors/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:27:37.981724 binary_file_parser-0.1.4/src/binary_file_parser/retrievers/
+-rw-rw-rw-   0        0        0     2647 2024-05-08 01:30:59.000000 binary_file_parser-0.1.4/src/binary_file_parser/retrievers/MapValidate.py
+-rw-rw-rw-   0        0        0     2272 2023-04-24 11:23:48.000000 binary_file_parser-0.1.4/src/binary_file_parser/retrievers/RetreiverCombiner.py
+-rw-rw-rw-   0        0        0     1518 2023-04-24 11:16:38.000000 binary_file_parser-0.1.4/src/binary_file_parser/retrievers/RetreiverRef.py
+-rw-rw-rw-   0        0        0    12480 2024-05-14 12:10:26.000000 binary_file_parser-0.1.4/src/binary_file_parser/retrievers/Retriever.py
+-rw-rw-rw-   0        0        0      199 2023-04-21 01:37:15.000000 binary_file_parser-0.1.4/src/binary_file_parser/retrievers/__init__.py
+-rw-rw-rw-   0        0        0    16362 2024-05-13 08:16:58.000000 binary_file_parser-0.1.4/src/binary_file_parser/retrievers/base_struct.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:27:38.020727 binary_file_parser-0.1.4/src/binary_file_parser/types/
+-rw-rw-rw-   0        0        0     6438 2023-04-21 03:06:40.000000 binary_file_parser-0.1.4/src/binary_file_parser/types/Array.py
+-rw-rw-rw-   0        0        0      928 2023-04-18 12:21:20.000000 binary_file_parser-0.1.4/src/binary_file_parser/types/Bool.py
+-rw-rw-rw-   0        0        0     2796 2022-11-29 16:43:10.000000 binary_file_parser-0.1.4/src/binary_file_parser/types/ByteStream.py
+-rw-rw-rw-   0        0        0      855 2023-04-18 12:21:20.000000 binary_file_parser-0.1.4/src/binary_file_parser/types/Bytes.py
+-rw-rw-rw-   0        0        0      867 2023-04-18 12:21:20.000000 binary_file_parser-0.1.4/src/binary_file_parser/types/Float.py
+-rw-rw-rw-   0        0        0      987 2023-04-18 12:21:20.000000 binary_file_parser-0.1.4/src/binary_file_parser/types/Int.py
+-rw-rw-rw-   0        0        0     1345 2023-04-21 02:01:03.000000 binary_file_parser-0.1.4/src/binary_file_parser/types/Parseable.py
+-rw-rw-rw-   0        0        0     3274 2024-05-14 11:58:19.000000 binary_file_parser-0.1.4/src/binary_file_parser/types/RefList.py
+-rw-rw-rw-   0        0        0     3037 2023-04-18 12:21:20.000000 binary_file_parser-0.1.4/src/binary_file_parser/types/Str.py
+-rw-rw-rw-   0        0        0      564 2023-09-09 10:18:09.000000 binary_file_parser-0.1.4/src/binary_file_parser/types/__init__.py
+-rw-rw-rw-   0        0        0      894 2024-05-09 12:18:33.000000 binary_file_parser-0.1.4/src/binary_file_parser/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:27:38.024726 binary_file_parser-0.1.4/src/binary_file_parser.egg-info/
+-rw-rw-rw-   0        0        0     6028 2024-05-14 12:27:37.000000 binary_file_parser-0.1.4/src/binary_file_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1260 2024-05-14 12:27:37.000000 binary_file_parser-0.1.4/src/binary_file_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 12:27:37.000000 binary_file_parser-0.1.4/src/binary_file_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2024-05-14 12:27:37.000000 binary_file_parser-0.1.4/src/binary_file_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-14 12:27:37.000000 binary_file_parser-0.1.4/src/binary_file_parser.egg-info/top_level.txt
```

### Comparing `binary-file-parser-0.1.3/LICENSE` & `binary_file_parser-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.3/PKG-INFO` & `binary_file_parser-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binary-file-parser
-Version: 0.1.3
+Version: 0.1.4
 Summary: Read/Write binary files after describing their specifications in code (similar to an ORM table schema)
 Author-email: Divy1211 <divy1211.dc@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Alian713
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `binary-file-parser-0.1.3/README.md` & `binary_file_parser-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.3/pyproject.toml` & `binary_file_parser-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=57.4.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "binary-file-parser"
-version = "0.1.3"
+version = "0.1.4"
 description = "Read/Write binary files after describing their specifications in code (similar to an ORM table schema)"
 readme = "README.md"
 authors = [{ name = "Divy1211", email = "divy1211.dc@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `binary-file-parser-0.1.3/src/binary_file_parser/retrievers/MapValidate.py` & `binary_file_parser-0.1.4/src/binary_file_parser/retrievers/MapValidate.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.3/src/binary_file_parser/retrievers/RetreiverCombiner.py` & `binary_file_parser-0.1.4/src/binary_file_parser/retrievers/RetreiverCombiner.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.3/src/binary_file_parser/retrievers/RetreiverRef.py` & `binary_file_parser-0.1.4/src/binary_file_parser/retrievers/RetreiverRef.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.3/src/binary_file_parser/retrievers/Retriever.py` & `binary_file_parser-0.1.4/src/binary_file_parser/retrievers/Retriever.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,22 +136,19 @@
 
     def __set__(self, instance: BaseStruct, value: T) -> None:
         if not self.supported(instance.struct_ver):
             raise VersionError(
                 f"{self.p_name!r} is not supported in your scenario version {instance.struct_ver}"
             )
 
-        # def set_parent(obj):
-        #     if isinstance(obj, BaseStruct):
-        #         obj.parent = instance
-        #     elif isinstance(obj, list):
-        #         for sub_obj in obj:
-        #             set_parent(sub_obj)
-        #
-        # set_parent(value)
+        if not isinstance(value, list):
+            super().__set__(instance, value)
+            return
+
+        value = self.atype(value, instance.struct_ver, instance.parent)
         super().__set__(instance, value)
 
     def __get__(self, instance: BaseStruct, owner: Type[BaseStruct]) -> Retriever | T:
         if instance is None:
             return self
 
         if not self.supported(instance.struct_ver):
```

### Comparing `binary-file-parser-0.1.3/src/binary_file_parser/retrievers/base_struct.py` & `binary_file_parser-0.1.4/src/binary_file_parser/retrievers/base_struct.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,23 +61,26 @@
             Use this to provide initial values to retrievers
         """
         self._struct_ver = struct_ver
         self._parent = parent
         self.idx = idx
 
         size = 0
+        if not initialise_defaults:
+            super().__init__(size)
+            return
+
         for retriever in self._retrievers:
             if not retriever.supported(struct_ver):
                 continue
 
-            if initialise_defaults:
-                init = retriever_inits.get(retriever.p_name, None)
-                if init is None:
-                    init = retriever.from_default(self)
-                setattr(self, retriever.p_name, init)
+            init = retriever_inits.get(retriever.p_name, None)
+            if init is None:
+                init = retriever.from_default(self)
+            setattr(self, retriever.p_name, init)
 
             # size += retriever.default.size if retriever.dtype.is_struct else retriever.dtype.size
         super().__init__(size)
 
     def __init_subclass__(cls, **kwargs):
         """
         Note: subclasses of BaseStruct which intend to act as ABCs need to override this
@@ -191,30 +194,30 @@
 
         :param bytes_: The remaining (compressed) bytes of the compressed section of the struct
         :return: decompressed bytes
         :raises CompressionError: - When unimplemented
         """
         raise CompressionError(
             "Unable to read object from file. "
-            "A Structure with compressed section needs to implement 'decompress' classmethod."
+            "A Structure with a compressed section needs to implement 'decompress' classmethod."
         )
 
     @classmethod
     def compress(cls, bytes_: bytes) -> bytes:
         """
         If remaining_compressed is set to True in a Retriever, this method is used to compress the bytes before they are
         written to file from the struct object
 
         :param bytes_: The remaining (uncompressed) bytes of the compressed section of the struct
         :return: compressed bytes
         :raises CompressionError: - When unimplemented
         """
         raise CompressionError(
             "Unable to write object to file. "
-            "A Structure with compressed section needs to implement 'compress' classmethod."
+            "A Structure with a compressed section needs to implement 'compress' classmethod."
         )
 
     def map(self) -> BaseStruct:
         """
         This method is called after a struct is read from bytes to allow any modifications post reading
 
         :return: A BaseStruct instance
```

### Comparing `binary-file-parser-0.1.3/src/binary_file_parser/types/Array.py` & `binary_file_parser-0.1.4/src/binary_file_parser/types/Array.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.3/src/binary_file_parser/types/Bool.py` & `binary_file_parser-0.1.4/src/binary_file_parser/types/Bool.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.3/src/binary_file_parser/types/ByteStream.py` & `binary_file_parser-0.1.4/src/binary_file_parser/types/ByteStream.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.3/src/binary_file_parser/types/Bytes.py` & `binary_file_parser-0.1.4/src/binary_file_parser/types/Bytes.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.3/src/binary_file_parser/types/Float.py` & `binary_file_parser-0.1.4/src/binary_file_parser/types/Float.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.3/src/binary_file_parser/types/Int.py` & `binary_file_parser-0.1.4/src/binary_file_parser/types/Int.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.3/src/binary_file_parser/types/Parseable.py` & `binary_file_parser-0.1.4/src/binary_file_parser/types/Parseable.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.3/src/binary_file_parser/types/RefList.py` & `binary_file_parser-0.1.4/src/binary_file_parser/types/RefList.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 class RefList(list, Generic[T]):
     def __init__(self, iterable: Iterable[T], struct_ver = Version((0,)), parent: BaseStruct = None):
         # todo: set idxs on structs where relevant
         # todo: set own idx for nested lists
         # todo: stop recursive set struct vers and parents if same
         iterable = map(ref_listify(self.__class__, struct_ver, parent), iterable)
         super().__init__(iterable)
-        self.struct_ver = struct_ver
-        self.parent = parent
+        self._struct_ver = struct_ver
+        self._parent = parent
 
     def __deepcopy__(self, memo):
         cls = self.__class__
 
         cloned_list = copy.deepcopy(list(self), memo)
 
         reflist = cls(cloned_list, copy.deepcopy(self.struct_ver), None)
```

### Comparing `binary-file-parser-0.1.3/src/binary_file_parser/types/Str.py` & `binary_file_parser-0.1.4/src/binary_file_parser/types/Str.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.3/src/binary_file_parser/types/__init__.py` & `binary_file_parser-0.1.4/src/binary_file_parser/types/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.3/src/binary_file_parser/utils.py` & `binary_file_parser-0.1.4/src/binary_file_parser/utils.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.1.3/src/binary_file_parser.egg-info/PKG-INFO` & `binary_file_parser-0.1.4/src/binary_file_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binary-file-parser
-Version: 0.1.3
+Version: 0.1.4
 Summary: Read/Write binary files after describing their specifications in code (similar to an ORM table schema)
 Author-email: Divy1211 <divy1211.dc@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Alian713
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `binary-file-parser-0.1.3/src/binary_file_parser.egg-info/SOURCES.txt` & `binary_file_parser-0.1.4/src/binary_file_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

