# Comparing `tmp/sferriol_scb-0.1.1-py3-none-any.whl.zip` & `tmp/sferriol_scb-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8075 bytes, number of entries: 10
--rw-r--r--  2.0 unx      143 b- defN 24-Mar-27 06:42 sferriol/scb/__init__.py
--rw-r--r--  2.0 unx     1204 b- defN 24-Mar-27 06:42 sferriol/scb/asyncio_shared_circular_buffer.py
--rw-r--r--  2.0 unx     1293 b- defN 24-Mar-27 06:42 sferriol/scb/file_lock.py
--rw-r--r--  2.0 unx     9891 b- defN 24-Mar-27 06:42 sferriol/scb/shared_circular_buffer.py
--rw-r--r--  2.0 unx     3442 b- defN 24-Mar-27 06:42 sferriol/scb/shared_memory.py
--rw-rw-rw-  2.0 unx     1211 b- defN 24-Mar-27 08:41 sferriol_scb-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1185 b- defN 24-Mar-27 08:41 sferriol_scb-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-27 08:41 sferriol_scb-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Mar-27 08:41 sferriol_scb-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      856 b- defN 24-Mar-27 08:41 sferriol_scb-0.1.1.dist-info/RECORD
-10 files, 19326 bytes uncompressed, 6601 bytes compressed:  65.8%
+Zip file size: 8155 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      116 b- defN 24-May-14 12:21 sferriol/scb/__init__.py
+-rw-r--r--  2.0 unx     1339 b- defN 24-May-14 12:21 sferriol/scb/asyncio_shared_circular_buffer.py
+-rw-r--r--  2.0 unx     1293 b- defN 24-May-14 12:21 sferriol/scb/file_lock.py
+-rw-r--r--  2.0 unx     9948 b- defN 24-May-14 12:21 sferriol/scb/shared_circular_buffer.py
+-rw-r--r--  2.0 unx     3442 b- defN 24-May-14 12:21 sferriol/scb/shared_memory.py
+-rw-rw-rw-  2.0 unx     1211 b- defN 24-May-14 12:21 sferriol_scb-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1185 b- defN 24-May-14 12:21 sferriol_scb-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 12:21 sferriol_scb-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-May-14 12:21 sferriol_scb-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      856 b- defN 24-May-14 12:21 sferriol_scb-0.2.0.dist-info/RECORD
+10 files, 19491 bytes uncompressed, 6681 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: sferriol/scb/shared_circular_buffer.py
 Comment: 
 
 Filename: sferriol/scb/shared_memory.py
 Comment: 
 
-Filename: sferriol_scb-0.1.1.dist-info/LICENSE
+Filename: sferriol_scb-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: sferriol_scb-0.1.1.dist-info/METADATA
+Filename: sferriol_scb-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: sferriol_scb-0.1.1.dist-info/WHEEL
+Filename: sferriol_scb-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: sferriol_scb-0.1.1.dist-info/top_level.txt
+Filename: sferriol_scb-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sferriol_scb-0.1.1.dist-info/RECORD
+Filename: sferriol_scb-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sferriol/scb/__init__.py

```diff
@@ -1,3 +1,2 @@
-from .shared_circular_buffer import Reader
-from .shared_circular_buffer import Writer
+from .shared_circular_buffer import Reader, Writer, exists
 from .asyncio_shared_circular_buffer import Async_Reader
```

## sferriol/scb/asyncio_shared_circular_buffer.py

```diff
@@ -8,31 +8,34 @@
 class Async_Reader(Reader):
     """Asynchronous reader
 
     Parameters
     ----------
     name -- name of circular buffer
     timeout -- limit amount of time waiting notify event from writer
+    counter -- begin with counter value. If None, writer's counter is taken
 
     """
 
-    def __init__(self, name: str, timeout: float | None = None):
-        ret = Reader.__init__(self, name)
+    def __init__(
+        self, name: str, timeout: float | None = None, counter: int | None = None
+    ):
+        ret = Reader.__init__(self, name, counter)
         self.timeout = timeout
         self._inotify = Inotify()
         fpath = f"/dev/shm/{self._shm.name}"
         self._inotify.add_watch(fpath, Mask.ATTRIB)
         return ret
 
     async def get(self):
         """
         Return a copy of an array from the buffer or None if no array available.
         """
         put_counter = self.put_counter
-        if put_counter == self.get_counter:
+        while self.put_counter == self.get_counter:
             async with asyncio.timeout(self.timeout):
                 await self._inotify.get()
 
         self._check_next_put_counter()
         array = self._get()
         self._check_next_put_counter()
```

## sferriol/scb/shared_circular_buffer.py

```diff
@@ -104,26 +104,26 @@
 
     @property
     def shm_name(self):
         return _NAME_PREFIX + self.name
 
 
 class Reader(_Common):
-    def __init__(self, name: str):
+    def __init__(self, name: str, counter: int = None):
         self.name = name
 
         # test if it exists
         if not self._exists():
             raise OSError(f"Circular buffer ({name}): not found")
 
         self._shm = self._build_shm()
         self._init_from_shm()
         self.shm_np = self._build_shm_np()
 
-        self.get_counter = self.put_counter
+        self.get_counter = counter if counter is not None else self.put_counter
 
     def _build_shm(self):
         return SharedMemory(name=_NAME_PREFIX + self.name, create=False, read_only=True)
 
     def _check_next_put_counter(self):
         # read next_put_counter only once (like a snapshot)
         next_put_counter = self.next_put_counter
```

## Comparing `sferriol_scb-0.1.1.dist-info/LICENSE` & `sferriol_scb-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sferriol_scb-0.1.1.dist-info/METADATA` & `sferriol_scb-0.2.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sferriol-scb
-Version: 0.1.1
+Version: 0.2.0
 Summary: Circular buffer storing numpy arrays that can be shared between one writer and several readers
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: asyncinotify
 Requires-Dist: numpy
 Requires-Dist: posix-ipc
```

