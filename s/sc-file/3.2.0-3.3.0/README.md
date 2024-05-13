# Comparing `tmp/sc_file-3.2.0.tar.gz` & `tmp/sc_file-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc_file-3.2.0.tar", max compression
+gzip compressed data, was "sc_file-3.3.0.tar", max compression
```

## Comparing `sc_file-3.2.0.tar` & `sc_file-3.3.0.tar`

### file list

```diff
@@ -1,41 +1,46 @@
--rw-r--r--   0        0        0     1083 2023-01-22 13:34:34.609366 sc_file-3.2.0/LICENSE
--rw-r--r--   0        0        0      795 2024-04-30 01:54:55.746800 sc_file-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     5065 2024-04-14 14:09:27.400282 sc_file-3.2.0/README.md
--rw-r--r--   0        0        0      186 2024-04-14 13:44:35.652910 sc_file-3.2.0/scfile/__init__.py
--rw-r--r--   0        0        0     1485 2024-04-14 13:10:00.131909 sc_file-3.2.0/scfile/__main__.py
--rw-r--r--   0        0        0     1269 2024-04-30 03:15:55.753849 sc_file-3.2.0/scfile/consts.py
--rw-r--r--   0        0        0     1143 2024-04-14 13:45:32.018913 sc_file-3.2.0/scfile/enums.py
--rw-r--r--   0        0        0      427 2024-03-20 03:27:16.312140 sc_file-3.2.0/scfile/exceptions/__init__.py
--rw-r--r--   0        0        0       84 2024-03-20 03:27:16.312140 sc_file-3.2.0/scfile/exceptions/base.py
--rw-r--r--   0        0        0     1408 2024-03-20 03:27:16.313140 sc_file-3.2.0/scfile/exceptions/basic.py
--rw-r--r--   0        0        0      641 2024-03-20 03:27:16.313140 sc_file-3.2.0/scfile/exceptions/decode.py
--rw-r--r--   0        0        0     1409 2024-03-20 03:27:16.313140 sc_file-3.2.0/scfile/exceptions/mcsa.py
--rw-r--r--   0        0        0      866 2024-03-20 03:27:16.314140 sc_file-3.2.0/scfile/exceptions/ol.py
--rw-r--r--   0        0        0        2 2024-03-20 03:27:16.314140 sc_file-3.2.0/scfile/file/__init__.py
--rw-r--r--   0        0        0      780 2024-03-20 03:27:16.314140 sc_file-3.2.0/scfile/file/base.py
--rw-r--r--   0        0        0      394 2024-03-25 13:19:34.701976 sc_file-3.2.0/scfile/file/data.py
--rw-r--r--   0        0        0     2162 2024-03-20 03:27:16.315140 sc_file-3.2.0/scfile/file/dds/encoder.py
--rw-r--r--   0        0        0     1124 2024-03-20 03:27:16.315140 sc_file-3.2.0/scfile/file/dds/structure.py
--rw-r--r--   0        0        0     3185 2024-03-26 21:28:59.417991 sc_file-3.2.0/scfile/file/decoder.py
--rw-r--r--   0        0        0     1840 2024-03-26 21:28:59.418992 sc_file-3.2.0/scfile/file/encoder.py
--rw-r--r--   0        0        0     6784 2024-04-30 01:57:33.155844 sc_file-3.2.0/scfile/file/mcsa/decoder.py
--rw-r--r--   0        0        0      682 2024-03-26 21:28:59.419991 sc_file-3.2.0/scfile/file/mcsa/flags.py
--rw-r--r--   0        0        0      153 2024-03-20 03:27:16.317139 sc_file-3.2.0/scfile/file/mcsa/versions.py
--rw-r--r--   0        0        0      611 2024-03-20 03:27:16.317139 sc_file-3.2.0/scfile/file/mic/decoder.py
--rw-r--r--   0        0        0     2327 2024-04-30 03:00:13.820947 sc_file-3.2.0/scfile/file/obj/encoder.py
--rw-r--r--   0        0        0      694 2024-04-27 19:31:59.469317 sc_file-3.2.0/scfile/file/ol/converter/base.py
--rw-r--r--   0        0        0      189 2024-03-20 03:27:16.318139 sc_file-3.2.0/scfile/file/ol/converter/bgra8.py
--rw-r--r--   0        0        0      244 2024-03-20 03:27:16.318139 sc_file-3.2.0/scfile/file/ol/converter/rgba32f.py
--rw-r--r--   0        0        0     3864 2024-03-26 21:28:59.419991 sc_file-3.2.0/scfile/file/ol/decoder.py
--rw-r--r--   0        0        0      144 2024-03-20 03:27:16.319140 sc_file-3.2.0/scfile/file/ol/formats.py
--rw-r--r--   0        0        0      295 2024-03-20 03:27:16.319140 sc_file-3.2.0/scfile/file/png/encoder.py
--rw-r--r--   0        0        0        0 2024-03-20 03:27:16.319140 sc_file-3.2.0/scfile/io/__init__.py
--rw-r--r--   0        0        0     1578 2024-04-27 19:35:49.133419 sc_file-3.2.0/scfile/io/base.py
--rw-r--r--   0        0        0      261 2024-03-20 03:27:16.320140 sc_file-3.2.0/scfile/io/binary.py
--rw-r--r--   0        0        0     1980 2024-04-30 03:21:38.728106 sc_file-3.2.0/scfile/io/mcsa.py
--rw-r--r--   0        0        0      405 2024-03-20 03:27:16.321141 sc_file-3.2.0/scfile/io/ol.py
--rw-r--r--   0        0        0      122 2024-03-26 21:28:59.420991 sc_file-3.2.0/scfile/types.py
--rw-r--r--   0        0        0     3862 2024-04-14 13:46:22.120912 sc_file-3.2.0/scfile/utils/convert.py
--rw-r--r--   0        0        0     3157 2024-04-30 03:00:20.451006 sc_file-3.2.0/scfile/utils/model.py
--rw-r--r--   0        0        0     6116 1970-01-01 00:00:00.000000 sc_file-3.2.0/setup.py
--rw-r--r--   0        0        0     5579 1970-01-01 00:00:00.000000 sc_file-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-01-22 13:34:34.609366 sc_file-3.3.0/LICENSE
+-rw-r--r--   0        0        0      794 2024-05-13 23:22:43.357943 sc_file-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5271 2024-05-13 23:22:43.357943 sc_file-3.3.0/README.md
+-rw-r--r--   0        0        0      264 2024-05-13 23:22:43.358942 sc_file-3.3.0/scfile/__init__.py
+-rw-r--r--   0        0        0       77 2024-05-13 23:22:43.358942 sc_file-3.3.0/scfile/__main__.py
+-rw-r--r--   0        0        0       21 2024-05-13 23:22:43.369941 sc_file-3.3.0/scfile/cli/__init__.py
+-rw-r--r--   0        0        0     1059 2024-05-13 23:22:43.369941 sc_file-3.3.0/scfile/cli/default.py
+-rw-r--r--   0        0        0      584 2024-05-13 23:22:43.369941 sc_file-3.3.0/scfile/cli/utils.py
+-rw-r--r--   0        0        0     1306 2024-05-13 23:22:43.369941 sc_file-3.3.0/scfile/consts.py
+-rw-r--r--   0        0        0     1180 2024-05-13 23:22:43.370941 sc_file-3.3.0/scfile/enums.py
+-rw-r--r--   0        0        0      427 2024-03-20 03:27:16.312140 sc_file-3.3.0/scfile/exceptions/__init__.py
+-rw-r--r--   0        0        0       84 2024-03-20 03:27:16.312140 sc_file-3.3.0/scfile/exceptions/base.py
+-rw-r--r--   0        0        0     1408 2024-05-13 23:14:32.103578 sc_file-3.3.0/scfile/exceptions/basic.py
+-rw-r--r--   0        0        0      641 2024-05-13 23:14:29.277578 sc_file-3.3.0/scfile/exceptions/decode.py
+-rw-r--r--   0        0        0     1409 2024-05-13 23:14:25.216581 sc_file-3.3.0/scfile/exceptions/mcsa.py
+-rw-r--r--   0        0        0      866 2024-05-13 23:14:23.130279 sc_file-3.3.0/scfile/exceptions/ol.py
+-rw-r--r--   0        0        0        2 2024-03-20 03:27:16.314140 sc_file-3.3.0/scfile/file/__init__.py
+-rw-r--r--   0        0        0      780 2024-05-13 23:14:20.801280 sc_file-3.3.0/scfile/file/base.py
+-rw-r--r--   0        0        0      394 2024-05-13 23:14:18.500218 sc_file-3.3.0/scfile/file/data.py
+-rw-r--r--   0        0        0     2162 2024-05-13 23:14:13.719219 sc_file-3.3.0/scfile/file/dds/encoder.py
+-rw-r--r--   0        0        0     1124 2024-03-20 03:27:16.315140 sc_file-3.3.0/scfile/file/dds/structure.py
+-rw-r--r--   0        0        0     3185 2024-05-13 23:14:17.306217 sc_file-3.3.0/scfile/file/decoder.py
+-rw-r--r--   0        0        0     1830 2024-05-13 23:22:43.370941 sc_file-3.3.0/scfile/file/encoder.py
+-rw-r--r--   0        0        0     8901 2024-05-13 23:22:43.371944 sc_file-3.3.0/scfile/file/mcsa/decoder.py
+-rw-r--r--   0        0        0      682 2024-03-26 21:28:59.419991 sc_file-3.3.0/scfile/file/mcsa/flags.py
+-rw-r--r--   0        0        0      153 2024-03-20 03:27:16.317139 sc_file-3.3.0/scfile/file/mcsa/versions.py
+-rw-r--r--   0        0        0      611 2024-05-13 23:14:47.772239 sc_file-3.3.0/scfile/file/mic/decoder.py
+-rw-r--r--   0        0        0     4511 2024-05-13 23:22:43.371944 sc_file-3.3.0/scfile/file/ms3d/ascii/encoder.py
+-rw-r--r--   0        0        0     5306 2024-05-13 23:22:43.372941 sc_file-3.3.0/scfile/file/ms3d/bin/encoder.py
+-rw-r--r--   0        0        0     2189 2024-05-13 23:22:43.372941 sc_file-3.3.0/scfile/file/obj/encoder.py
+-rw-r--r--   0        0        0      694 2024-04-27 19:31:59.469317 sc_file-3.3.0/scfile/file/ol/converter/base.py
+-rw-r--r--   0        0        0      189 2024-03-20 03:27:16.318139 sc_file-3.3.0/scfile/file/ol/converter/bgra8.py
+-rw-r--r--   0        0        0      244 2024-03-20 03:27:16.318139 sc_file-3.3.0/scfile/file/ol/converter/rgba32f.py
+-rw-r--r--   0        0        0     3864 2024-05-13 23:14:05.625616 sc_file-3.3.0/scfile/file/ol/decoder.py
+-rw-r--r--   0        0        0      144 2024-03-20 03:27:16.319140 sc_file-3.3.0/scfile/file/ol/formats.py
+-rw-r--r--   0        0        0      295 2024-05-13 23:14:04.340618 sc_file-3.3.0/scfile/file/png/encoder.py
+-rw-r--r--   0        0        0        0 2024-03-20 03:27:16.319140 sc_file-3.3.0/scfile/io/__init__.py
+-rw-r--r--   0        0        0     1578 2024-05-13 23:14:02.689615 sc_file-3.3.0/scfile/io/base.py
+-rw-r--r--   0        0        0      261 2024-05-13 23:14:00.719522 sc_file-3.3.0/scfile/io/binary.py
+-rw-r--r--   0        0        0     1980 2024-05-13 23:13:33.800137 sc_file-3.3.0/scfile/io/mcsa.py
+-rw-r--r--   0        0        0      405 2024-05-13 23:13:32.331505 sc_file-3.3.0/scfile/io/ol.py
+-rw-r--r--   0        0        0      122 2024-03-26 21:28:59.420991 sc_file-3.3.0/scfile/types.py
+-rw-r--r--   0        0        0     4550 2024-05-13 23:22:43.372941 sc_file-3.3.0/scfile/utils/convert.py
+-rw-r--r--   0        0        0     4250 2024-05-13 23:22:43.373943 sc_file-3.3.0/scfile/utils/model.py
+-rw-r--r--   0        0        0     6388 1970-01-01 00:00:00.000000 sc_file-3.3.0/setup.py
+-rw-r--r--   0        0        0     5771 1970-01-01 00:00:00.000000 sc_file-3.3.0/PKG-INFO
```

### Comparing `sc_file-3.2.0/LICENSE` & `sc_file-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sc_file-3.2.0/pyproject.toml` & `sc_file-3.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "sc-file"
-version = "3.2.0"
+version = "3.3.0"
 description = "Utility & Library for decoding stalcraft assets"
-authors = ["onejeuu <bloodtrail@beber1k.ru>"]
+authors = ["onejeuu <mail@66rk.ru>"]
 
 license = "MIT"
 readme = "README.md"
 
 homepage = "https://github.com/onejeuu/sc-file"
 repository = "https://github.com/onejeuu/sc-file"
 documentation = "https://github.com/onejeuu/sc-file/?tab=readme-ov-file#usage-1"
@@ -22,12 +22,12 @@
 
 [tool.poetry.group.dev.dependencies]
 pyinstaller = "^6.0.0"
 rich = "^13.0.0"
 pytest = "^8.1.1"
 
 [tool.poetry.scripts]
-build = "build:build"
+build = "scripts.build:build"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sc_file-3.2.0/README.md` & `sc_file-3.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 > Do not use game assets directly. \
 > Any changes in game client can be detected.
 
 You can use executable program from [Releases](https://github.com/onejeuu/sc-file/releases) page.
 
 # 📁 Formats
 
-| Type    | Source format | Output format |
-| ------- | ------------- | ------------- |
-| Model   | .mcsa         | .obj          |
-| Model   | .mcvd         | .obj          |
-| Texture | .ol           | .dds          |
-| Image   | .mic          | .png          |
+| Type    | Source        | Output           |
+| ------- | ------------- | ---------------- |
+| Model   | .mcsa / .mcvd | .obj, .txt, ms3d |
+| Texture | .ol           | .dds             |
+| Image   | .mic          | .png             |
 
 Model versions supported: 7.0, 8.0, 10.0
 
+Model animations (`.mcvd`) currently supports only meshes
+
 Texture formats supported: DXT1, DXT3, DXT5, RGBA8, BGRA8, RGBA32F, DXN_XY
 
 Texture formats unsupported: Cubemaps (hdri, sky)
 
 # 💻 CLI Utility
 
 ## Usage
@@ -128,14 +129,18 @@
 
 # Output path is optional.
 # Defaults to source path with new suffix.
 convert.mcsa_to_obj("path/to/model.mcsa", "path/to/model.obj")
 convert.ol_to_dds("path/to/texture.ol", "path/to/texture.dds")
 convert.mic_to_png("path/to/image.mic", "path/to/image.png")
 
+# Skeleton support via MilkShape3D
+convert.mcsa_to_ms3d("path/to/model.mcsa", "path/to/model.ms3d")
+convert.mcsa_to_ms3d_ascii("path/to/model.mcsa", "path/to/model.txt")
+
 # Or determinate it automatically
 convert.auto("path/to/model.mcsa")
 ```
 
 ### Advanced
 
 Default
```

### Comparing `sc_file-3.2.0/scfile/consts.py` & `sc_file-3.3.0/scfile/consts.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     """
     Big-Endian Output File Signature.
     List[Integer].
     """
 
     DDS = [0x44, 0x44, 0x53, 0x20]
     PNG = [0x89, 0x50, 0x4E, 0x47]
+    MS3D = [0x4D, 0x53, 0x33, 0x44]
 
 
 class Factor:
     """
     Integer range.
     """
```

### Comparing `sc_file-3.2.0/scfile/enums.py` & `sc_file-3.3.0/scfile/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 
 
 class FileSuffix(StrEnum):
     DDS = auto()
     MCSA = auto()
     MCVD = auto()
     MIC = auto()
+    MS3D = auto()
     OBJ = auto()
     OL = auto()
     PNG = auto()
+    TXT = auto()
 
 
 class FileMode(StrEnum):
     RB = READ = auto()
     WB = WRITE = auto()
     AB = APPEND = auto()
     PLUS = "+"
```

### Comparing `sc_file-3.2.0/scfile/exceptions/basic.py` & `sc_file-3.3.0/scfile/exceptions/basic.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.2.0/scfile/exceptions/decode.py` & `sc_file-3.3.0/scfile/exceptions/decode.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.2.0/scfile/exceptions/mcsa.py` & `sc_file-3.3.0/scfile/exceptions/mcsa.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.2.0/scfile/exceptions/ol.py` & `sc_file-3.3.0/scfile/exceptions/ol.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.2.0/scfile/file/base.py` & `sc_file-3.3.0/scfile/file/base.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.2.0/scfile/file/dds/encoder.py` & `sc_file-3.3.0/scfile/file/dds/encoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.2.0/scfile/file/dds/structure.py` & `sc_file-3.3.0/scfile/file/dds/structure.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.2.0/scfile/file/decoder.py` & `sc_file-3.3.0/scfile/file/decoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.2.0/scfile/file/encoder.py` & `sc_file-3.3.0/scfile/file/encoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     @property
     def b(self):
         """Bytes buffer abbreviation."""
         return self._buffer
 
     @property
     def magic(self) -> Optional[list[int]]:
-        """Optional file magic value (4 bytes)."""
+        """Optional file magic value."""
         return None
 
     @property
     def content(self) -> bytes:
         """Buffer content bytes."""
         return self.b.getvalue()
```

### Comparing `sc_file-3.2.0/scfile/file/mcsa/decoder.py` & `sc_file-3.3.0/scfile/file/mcsa/decoder.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 from scfile import exceptions as exc
-from scfile.consts import Factor, McsaSize, Signature
+from scfile.consts import Factor, McsaModel, McsaSize, Signature
 from scfile.enums import ByteOrder
 from scfile.enums import StructFormat as F
 from scfile.file.data import ModelData
 from scfile.file.decoder import FileDecoder
+from scfile.file.ms3d.ascii.encoder import Ms3dAsciiEncoder
+from scfile.file.ms3d.bin.encoder import Ms3dBinEncoder
 from scfile.file.obj.encoder import ObjEncoder
 from scfile.io.mcsa import McsaFileIO
-from scfile.utils.model import Mesh, Model
+from scfile.utils.model import Bone, Mesh, Model, Vertex
 
 from .flags import Flag, McsaFlags
 from .versions import SUPPORTED_VERSIONS, VERSION_FLAGS
 
 
 class McsaDecoder(FileDecoder[McsaFileIO, ModelData]):
     def to_obj(self):
         return self.convert_to(ObjEncoder)
 
+    def to_ms3d_ascii(self):
+        return self.convert_to(Ms3dAsciiEncoder)
+
+    def to_ms3d(self):
+        return self.convert_to(Ms3dBinEncoder)
+
     @property
     def opener(self):
         return McsaFileIO
 
     @property
     def order(self):
         return ByteOrder.LITTLE
@@ -32,14 +40,17 @@
         return ModelData(self.model)
 
     def parse(self):
         self._create_model()
         self._parse_header()
         self._parse_meshes()
 
+        if self.flags[Flag.SKELETON]:
+            self._parse_skeleton()
+
     def _create_model(self):
         self.model = Model()
 
     def _parse_header(self):
         self._parse_version()
         self._parse_flags()
         self._parse_scales()
@@ -56,14 +67,15 @@
 
         if not self.flags_count:
             raise exc.McsaUnsupportedVersion(self.path, self.version)
 
         for index in range(self.flags_count):
             self.flags[index] = self.f.readb(F.BOOL)
 
+        self.model.flags.skeleton = self.flags[Flag.SKELETON]
         self.model.flags.texture = self.flags[Flag.TEXTURE]
         self.model.flags.normals = self.flags[Flag.NORMALS]
 
     def _parse_scales(self):
         self.model.scale.position = self.f.readb(F.F32)
 
         if self.flags[Flag.TEXTURE]:
@@ -197,21 +209,43 @@
             case 1 | 2:
                 self._parse_bone_packed()
             case 3 | 4:
                 self._parse_bone_plains()
             case _:
                 raise exc.McsaUnknownLinkCount(self.path, self.count.links)
 
-    def _parse_bone_packed(self):
-        # Still no export support yet
+    def _parse_bone_packed(self) -> None:
+        # Unused
         self._skip_vertices(size=4)
+        return
 
-    def _parse_bone_plains(self):
-        # Still no export support yet
+        for vertex in self.mesh.vertices:
+            self._parse_bone_id(vertex, 2)
+            self._parse_bone_weight(vertex, 2)
+
+    def _parse_bone_plains(self) -> None:
+        # Unused
         self._skip_vertices(size=8)
+        return
+
+        for vertex in self.mesh.vertices:
+            self._parse_bone_id(vertex, 4)
+
+        for vertex in self.mesh.vertices:
+            self._parse_bone_weight(vertex, 4)
+
+    def _parse_bone_id(self, vertex: Vertex, size: int) -> None:
+        for index in range(size):
+            bone_id = self.f.readb(F.U8)
+            vertex.bone.ids[index] = self.mesh.bones.get(bone_id, McsaModel.ROOT_BONE_ID)
+
+    def _parse_bone_weight(self, vertex: Vertex, size: int) -> None:
+        for index in range(size):
+            bone_weight = self.f.readb(F.U8)
+            vertex.bone.weights[index] = bone_weight / Factor.U8
 
     def _parse_colors(self):
         # Quite useless
         self._skip_vertices(size=4)
         return
 
         # Could be rgba, but not that important
@@ -227,9 +261,36 @@
 
         for polygon, (a, b, c) in zip(self.mesh.polygons, abc):
             polygon.a = a
             polygon.b = b
             polygon.c = c
 
     def _parse_skeleton(self):
-        # Still no export support yet
-        return
+        bones_count = self.f.readb(F.U8)
+
+        for index in range(bones_count):
+            self._parse_bone(index)
+
+        self.model.skeleton.convert_to_local()
+
+    def _parse_bone(self, index: int) -> None:
+        self.bone = Bone()
+
+        self.bone.name = self.f.readstring()
+
+        parent_id = self.f.readb(F.U8)
+        self.bone.parent_id = parent_id if parent_id != index else McsaModel.ROOT_BONE_ID
+
+        self._parse_bone_position()
+        self._parse_bone_rotation()
+
+        self.model.skeleton.bones.append(self.bone)
+
+    def _parse_bone_position(self):
+        self.bone.position.x = self.f.readb(F.F32)
+        self.bone.position.y = self.f.readb(F.F32)
+        self.bone.position.z = self.f.readb(F.F32)
+
+    def _parse_bone_rotation(self):
+        self.bone.rotation.x = self.f.readb(F.F32)
+        self.bone.rotation.y = self.f.readb(F.F32)
+        self.bone.rotation.z = self.f.readb(F.F32)
```

### Comparing `sc_file-3.2.0/scfile/file/mcsa/flags.py` & `sc_file-3.3.0/scfile/file/mcsa/flags.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.2.0/scfile/file/mic/decoder.py` & `sc_file-3.3.0/scfile/file/mic/decoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.2.0/scfile/file/obj/encoder.py` & `sc_file-3.3.0/scfile/file/obj/encoder.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,17 +7,15 @@
     FLOAT_FORMAT = ".6f"
 
     def serialize(self):
         self.model = self.data.model
         self.flags = self.data.model.flags
 
         self.model.ensure_unique_names()
-
-        # In obj vertex indexes 1-based
-        self.offset = 1
+        self.model.convert_polygons_to_global(start=1)
 
         for mesh in self.model.meshes:
             self.b.writes(f"o {mesh.name}\n")
 
             self._add_geometric_vertices(mesh)
 
             if self.flags.texture:
@@ -44,25 +42,22 @@
     def _add_vertex_normals(self, mesh: Mesh):
         f = self.FLOAT_FORMAT
         self._write_vertex_data(
             [f"vn {v.normals.x:{f}} {v.normals.y:{f}} {v.normals.z:{f}}" for v in mesh.vertices]
         )
 
     def _add_polygonal_faces(self, mesh: Mesh):
-        self._write_vertex_data([f"f {self._polygon_to_faces(p)}" for p in mesh.polygons])
-
-        # Vertex id in mcsa are local to each mesh.
-        self.offset += mesh.offset
+        self._write_vertex_data([f"f {self._polygon_to_faces(p)}" for p in mesh.global_polygons])
 
     def _write_vertex_data(self, data: list[str]):
         self.b.writes("\n".join(data))
         self.b.write(b"\n\n")
 
     def _polygon_to_faces(self, polygon: Polygon):
-        a, b, c = polygon.a + self.offset, polygon.b + self.offset, polygon.c + self.offset
+        a, b, c = polygon.a, polygon.b, polygon.c
 
         if self.flags.texture and self.flags.normals:
             return f"{a}/{a}/{a} {b}/{b}/{b} {c}/{c}/{c}"
 
         if self.flags.texture:
             return f"{a}/{a} {b}/{b} {c}/{c}"
```

### Comparing `sc_file-3.2.0/scfile/file/ol/converter/base.py` & `sc_file-3.3.0/scfile/file/ol/converter/base.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.2.0/scfile/file/ol/decoder.py` & `sc_file-3.3.0/scfile/file/ol/decoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.2.0/scfile/io/base.py` & `sc_file-3.3.0/scfile/io/base.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.2.0/scfile/io/mcsa.py` & `sc_file-3.3.0/scfile/io/mcsa.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.2.0/scfile/utils/convert.py` & `sc_file-3.3.0/scfile/utils/convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,46 +5,64 @@
 from scfile.enums import FileSuffix
 from scfile.file.dds.encoder import DdsEncoder
 from scfile.file.decoder import FileDecoder
 from scfile.file.encoder import FileEncoder
 from scfile.file.mcsa.decoder import McsaDecoder
 from scfile.file.mic.decoder import MicDecoder
 from scfile.file.obj.encoder import ObjEncoder
+from scfile.file.ms3d.bin.encoder import Ms3dBinEncoder
+from scfile.file.ms3d.ascii.encoder import Ms3dAsciiEncoder
 from scfile.file.ol.decoder import OlDecoder
 from scfile.file.png.encoder import PngEncoder
 from scfile.types import PathLike
 
 
-def mcsa_to_obj(source: PathLike, output: Optional[PathLike] = None):
+def mcsa_to_ms3d(source: PathLike, output: Optional[PathLike] = None):
     """
-    Converting `.mcsa` file to `.obj`.
+    Converting `.mcsa` file to `.ms3d`.
 
     Args:
         source: Full path to `.mcsa` file.
-        output (optional): Full path to output `.obj` file.
+        output (optional): Full path to output `.ms3d` file.
         Defaults to source path with new suffix.
 
     Example:
-        `mcsa_to_obj("C:/file.mcsa", "C:/file.obj")`
+        `mcsa_to_ms3d("C:/file.mcsa", "C:/file.ms3d")`
     """
 
-    _convert(source, output, McsaDecoder, ObjEncoder, FileSuffix.OBJ)
+    _convert(source, output, McsaDecoder, Ms3dBinEncoder, FileSuffix.MS3D)
 
 
-def mcvd_to_obj(source: PathLike, output: Optional[PathLike] = None):
+def mcsa_to_ms3d_ascii(source: PathLike, output: Optional[PathLike] = None):
     """
-    Converting `.mcvd` file to `.obj`.
+    Converting `.mcsa` file to `.txt`.
 
     Args:
-        source: Full path to `.mcvd` file.
+        source: Full path to `.mcsa` file.
+        output (optional): Full path to output `.txt` file.
+        Defaults to source path with new suffix.
+
+    Example:
+        `mcsa_to_ms3d_ascii("C:/file.mcsa", "C:/file.txt")`
+    """
+
+    _convert(source, output, McsaDecoder, Ms3dAsciiEncoder, FileSuffix.TXT)
+
+
+def mcsa_to_obj(source: PathLike, output: Optional[PathLike] = None):
+    """
+    Converting `.mcsa` file to `.obj`.
+
+    Args:
+        source: Full path to `.mcsa` file.
         output (optional): Full path to output `.obj` file.
         Defaults to source path with new suffix.
 
     Example:
-        `mcvd_to_obj("C:/file.mcvd", "C:/file.obj")`
+        `mcsa_to_obj("C:/file.mcsa", "C:/file.obj")`
     """
 
     _convert(source, output, McsaDecoder, ObjEncoder, FileSuffix.OBJ)
 
 
 def mic_to_png(source: PathLike, output: Optional[PathLike] = None):
     """
@@ -95,17 +113,19 @@
     """
 
     path = Path(source)
 
     match path.suffix.lstrip("."):
         case FileSuffix.MCSA:
             mcsa_to_obj(source, output)
+            mcsa_to_ms3d_ascii(source, output)
 
         case FileSuffix.MCVD:
-            mcvd_to_obj(source, output)
+            mcsa_to_obj(source, output)
+            mcsa_to_ms3d_ascii(source, output)
 
         case FileSuffix.MIC:
             mic_to_png(source, output)
 
         case FileSuffix.OL:
             ol_to_dds(source, output)
```

### Comparing `sc_file-3.2.0/setup.py` & `sc_file-3.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['scfile',
+ 'scfile.cli',
  'scfile.exceptions',
  'scfile.file',
  'scfile.file.dds',
  'scfile.file.mcsa',
  'scfile.file.mic',
+ 'scfile.file.ms3d.ascii',
+ 'scfile.file.ms3d.bin',
  'scfile.file.obj',
  'scfile.file.ol',
  'scfile.file.ol.converter',
  'scfile.file.png',
  'scfile.io',
  'scfile.utils']
 
@@ -21,23 +24,23 @@
 install_requires = \
 ['click>=8.1.7,<9.0.0',
  'lz4>=4.3.2,<5.0.0',
  'numpy>=1.26.3,<2.0.0',
  'quicktex>=0.2.0,<0.3.0']
 
 entry_points = \
-{'console_scripts': ['build = build:build']}
+{'console_scripts': ['build = scripts.build:build']}
 
 setup_kwargs = {
     'name': 'sc-file',
-    'version': '3.2.0',
+    'version': '3.3.0',
     'description': 'Utility & Library for decoding stalcraft assets',
-    'long_description': '# SC FILE\n\nUtility and Library for decoding and converting stalcraft assets files, such as models and textures into well-known formats.\n\nDesigned for artworks creation and the like.\n\n> [!NOTE]\n> There is not and will not be encoding back into game formats.\n\n> [!WARNING]\n> Do not use game assets directly. \\\n> Any changes in game client can be detected.\n\nYou can use executable program from [Releases](https://github.com/onejeuu/sc-file/releases) page.\n\n# 📁 Formats\n\n| Type    | Source format | Output format |\n| ------- | ------------- | ------------- |\n| Model   | .mcsa         | .obj          |\n| Model   | .mcvd         | .obj          |\n| Texture | .ol           | .dds          |\n| Image   | .mic          | .png          |\n\nModel versions supported: 7.0, 8.0, 10.0\n\nTexture formats supported: DXT1, DXT3, DXT5, RGBA8, BGRA8, RGBA32F, DXN_XY\n\nTexture formats unsupported: Cubemaps (hdri, sky)\n\n# 💻 CLI Utility\n\n## Usage\n\nFrom bash:\n\n```bash\nscfile [FILES]... [OPTIONS]\n```\n\n> [!TIP]\n> You can just drag and drop one or multiple files onto `scfile.exe`.\n\n## Arguments\n\n- `FILES`: **List of file paths to be converted**. Multiple files should be separated by **spaces**. Accepts both full and relative paths. **Does not accept directory**.\n\n## Options\n\n- `-O`, `--output`: **One path to output file or directory**. Can be specified multiple times for different output files or directories. If not specified, file will be saved in same directory with a new suffix. You can specify multiple `FILES` and a single `--output` directory.\n\n## Examples\n\n1. Convert a single file:\n\n   ```bash\n   scfile file.mcsa\n   ```\n\n   _Will be saved in same directory with a new suffix._\n\n2. Convert a single file with a specified path or name:\n\n   ```bash\n   scfile file.mcsa --output path/to/file.obj\n   ```\n\n3. Convert multiple files to a specified directory:\n\n   ```bash\n   scfile file1.mcsa file2.mcsa --output path/to/dir\n   ```\n\n4. Convert multiple files with explicitly specified output files:\n\n   ```bash\n   scfile file1.mcsa file2.mcsa -O 1.obj -O 2.obj\n   ```\n\n   _If count of `FILES` and `--output` is different, as many files as possible will be converted._\n\n5. Convert all `.mcsa` files in current directory:\n\n   ```bash\n   scfile *.mcsa\n   ```\n\n   _In this case, `--output` accepts only a directory. Subdirectories are not included._\n\n6. Convert all `.mcsa` files with subdirectories to a specified directory:\n\n   ```bash\n   scfile **/*.mcsa -O path/to/dir\n   ```\n\n   _In this case, `--output` accepts only a directory. With `--output` specified, directory structure is not duplicated._\n\n# 📚 Library\n\n## Install\n\n### Pip\n\n```bash\npip install sc-file -U\n```\n\n### Manual\n\n```bash\ngit clone git@github.com:onejeuu/sc-file.git\n```\n\n```bash\ncd sc-file\n```\n\n```bash\npoetry install\n```\n\n## Usage\n\n### Simple\n\n```python\nfrom scfile import convert\n\n# Output path is optional.\n# Defaults to source path with new suffix.\nconvert.mcsa_to_obj("path/to/model.mcsa", "path/to/model.obj")\nconvert.ol_to_dds("path/to/texture.ol", "path/to/texture.dds")\nconvert.mic_to_png("path/to/image.mic", "path/to/image.png")\n\n# Or determinate it automatically\nconvert.auto("path/to/model.mcsa")\n```\n\n### Advanced\n\nDefault\n\n```python\nfrom scfile.file.data import ModelData\nfrom scfile.file.mcsa.decoder import McsaDecoder\nfrom scfile.file.obj.encoder import ObjEncoder\n\nmcsa = McsaDecoder("model.mcsa")\ndata: ModelData = mcsa.decode()\nmcsa.close() # ? Necessary to close\n\nobj = ObjEncoder(data)\nobj.encode().save("model.obj") # ? Encoder closes after saving\n```\n\nUse encoded content bytes\n\n```python\nobj = ObjEncoder(data)\nobj.encode()\n\nwith open("model.obj", "wb") as fp:\n    fp.write(obj.content)\n\nobj.close() # ? Necessary to close\n```\n\nUse convert methods\n\n```python\nmcsa = McsaDecoder("model.mcsa")\nmcsa.convert_to(ObjEncoder).save("model.obj")\nmcsa.close() # ? Necessary to close\n```\n\n```python\nmcsa = McsaDecoder("model.mcsa")\nmcsa.to_obj().save("model.obj")\nmcsa.close() # ? Necessary to close\n```\n\nUse context manager\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    data: ModelData = mcsa.decode()\n\nwith ObjEncoder(data) as obj:\n    obj.encode().save("model.obj")\n```\n\nUse context manager + convert methods\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    mcsa.to_obj().save("model.obj")\n```\n\nSave multiple copies\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    with mcsa.to_obj() as obj:\n        obj.save_as("model_1.obj")\n        obj.save_as("model_2.obj")\n```\n\n# 🛠️ Build\n\n> [!IMPORTANT]\n> You will need [poetry](https://python-poetry.org) to do compilation.\n\n> [!TIP]\n> Recommended to create virtual environment.\n>\n> ```bash\n> poetry shell\n> ```\n\nThen install dependencies:\n\n```bash\npoetry install\n```\n\nAnd run script to compile:\n\n```bash\npoetry run build\n```\n\nExecutable file will be created in `/dist` directory.\n',
+    'long_description': '# SC FILE\n\nUtility and Library for decoding and converting stalcraft assets files, such as models and textures into well-known formats.\n\nDesigned for artworks creation and the like.\n\n> [!NOTE]\n> There is not and will not be encoding back into game formats.\n\n> [!WARNING]\n> Do not use game assets directly. \\\n> Any changes in game client can be detected.\n\nYou can use executable program from [Releases](https://github.com/onejeuu/sc-file/releases) page.\n\n# 📁 Formats\n\n| Type    | Source        | Output           |\n| ------- | ------------- | ---------------- |\n| Model   | .mcsa / .mcvd | .obj, .txt, ms3d |\n| Texture | .ol           | .dds             |\n| Image   | .mic          | .png             |\n\nModel versions supported: 7.0, 8.0, 10.0\n\nModel animations (`.mcvd`) currently supports only meshes\n\nTexture formats supported: DXT1, DXT3, DXT5, RGBA8, BGRA8, RGBA32F, DXN_XY\n\nTexture formats unsupported: Cubemaps (hdri, sky)\n\n# 💻 CLI Utility\n\n## Usage\n\nFrom bash:\n\n```bash\nscfile [FILES]... [OPTIONS]\n```\n\n> [!TIP]\n> You can just drag and drop one or multiple files onto `scfile.exe`.\n\n## Arguments\n\n- `FILES`: **List of file paths to be converted**. Multiple files should be separated by **spaces**. Accepts both full and relative paths. **Does not accept directory**.\n\n## Options\n\n- `-O`, `--output`: **One path to output file or directory**. Can be specified multiple times for different output files or directories. If not specified, file will be saved in same directory with a new suffix. You can specify multiple `FILES` and a single `--output` directory.\n\n## Examples\n\n1. Convert a single file:\n\n   ```bash\n   scfile file.mcsa\n   ```\n\n   _Will be saved in same directory with a new suffix._\n\n2. Convert a single file with a specified path or name:\n\n   ```bash\n   scfile file.mcsa --output path/to/file.obj\n   ```\n\n3. Convert multiple files to a specified directory:\n\n   ```bash\n   scfile file1.mcsa file2.mcsa --output path/to/dir\n   ```\n\n4. Convert multiple files with explicitly specified output files:\n\n   ```bash\n   scfile file1.mcsa file2.mcsa -O 1.obj -O 2.obj\n   ```\n\n   _If count of `FILES` and `--output` is different, as many files as possible will be converted._\n\n5. Convert all `.mcsa` files in current directory:\n\n   ```bash\n   scfile *.mcsa\n   ```\n\n   _In this case, `--output` accepts only a directory. Subdirectories are not included._\n\n6. Convert all `.mcsa` files with subdirectories to a specified directory:\n\n   ```bash\n   scfile **/*.mcsa -O path/to/dir\n   ```\n\n   _In this case, `--output` accepts only a directory. With `--output` specified, directory structure is not duplicated._\n\n# 📚 Library\n\n## Install\n\n### Pip\n\n```bash\npip install sc-file -U\n```\n\n### Manual\n\n```bash\ngit clone git@github.com:onejeuu/sc-file.git\n```\n\n```bash\ncd sc-file\n```\n\n```bash\npoetry install\n```\n\n## Usage\n\n### Simple\n\n```python\nfrom scfile import convert\n\n# Output path is optional.\n# Defaults to source path with new suffix.\nconvert.mcsa_to_obj("path/to/model.mcsa", "path/to/model.obj")\nconvert.ol_to_dds("path/to/texture.ol", "path/to/texture.dds")\nconvert.mic_to_png("path/to/image.mic", "path/to/image.png")\n\n# Skeleton support via MilkShape3D\nconvert.mcsa_to_ms3d("path/to/model.mcsa", "path/to/model.ms3d")\nconvert.mcsa_to_ms3d_ascii("path/to/model.mcsa", "path/to/model.txt")\n\n# Or determinate it automatically\nconvert.auto("path/to/model.mcsa")\n```\n\n### Advanced\n\nDefault\n\n```python\nfrom scfile.file.data import ModelData\nfrom scfile.file.mcsa.decoder import McsaDecoder\nfrom scfile.file.obj.encoder import ObjEncoder\n\nmcsa = McsaDecoder("model.mcsa")\ndata: ModelData = mcsa.decode()\nmcsa.close() # ? Necessary to close\n\nobj = ObjEncoder(data)\nobj.encode().save("model.obj") # ? Encoder closes after saving\n```\n\nUse encoded content bytes\n\n```python\nobj = ObjEncoder(data)\nobj.encode()\n\nwith open("model.obj", "wb") as fp:\n    fp.write(obj.content)\n\nobj.close() # ? Necessary to close\n```\n\nUse convert methods\n\n```python\nmcsa = McsaDecoder("model.mcsa")\nmcsa.convert_to(ObjEncoder).save("model.obj")\nmcsa.close() # ? Necessary to close\n```\n\n```python\nmcsa = McsaDecoder("model.mcsa")\nmcsa.to_obj().save("model.obj")\nmcsa.close() # ? Necessary to close\n```\n\nUse context manager\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    data: ModelData = mcsa.decode()\n\nwith ObjEncoder(data) as obj:\n    obj.encode().save("model.obj")\n```\n\nUse context manager + convert methods\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    mcsa.to_obj().save("model.obj")\n```\n\nSave multiple copies\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    with mcsa.to_obj() as obj:\n        obj.save_as("model_1.obj")\n        obj.save_as("model_2.obj")\n```\n\n# 🛠️ Build\n\n> [!IMPORTANT]\n> You will need [poetry](https://python-poetry.org) to do compilation.\n\n> [!TIP]\n> Recommended to create virtual environment.\n>\n> ```bash\n> poetry shell\n> ```\n\nThen install dependencies:\n\n```bash\npoetry install\n```\n\nAnd run script to compile:\n\n```bash\npoetry run build\n```\n\nExecutable file will be created in `/dist` directory.\n',
     'author': 'onejeuu',
-    'author_email': 'bloodtrail@beber1k.ru',
+    'author_email': 'mail@66rk.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/onejeuu/sc-file',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
```

### Comparing `sc_file-3.2.0/PKG-INFO` & `sc_file-3.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: sc-file
-Version: 3.2.0
+Version: 3.3.0
 Summary: Utility & Library for decoding stalcraft assets
 Home-page: https://github.com/onejeuu/sc-file
 License: MIT
 Author: onejeuu
-Author-email: bloodtrail@beber1k.ru
+Author-email: mail@66rk.ru
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: lz4 (>=4.3.2,<5.0.0)
 Requires-Dist: numpy (>=1.26.3,<2.0.0)
@@ -31,23 +31,24 @@
 > Do not use game assets directly. \
 > Any changes in game client can be detected.
 
 You can use executable program from [Releases](https://github.com/onejeuu/sc-file/releases) page.
 
 # 📁 Formats
 
-| Type    | Source format | Output format |
-| ------- | ------------- | ------------- |
-| Model   | .mcsa         | .obj          |
-| Model   | .mcvd         | .obj          |
-| Texture | .ol           | .dds          |
-| Image   | .mic          | .png          |
+| Type    | Source        | Output           |
+| ------- | ------------- | ---------------- |
+| Model   | .mcsa / .mcvd | .obj, .txt, ms3d |
+| Texture | .ol           | .dds             |
+| Image   | .mic          | .png             |
 
 Model versions supported: 7.0, 8.0, 10.0
 
+Model animations (`.mcvd`) currently supports only meshes
+
 Texture formats supported: DXT1, DXT3, DXT5, RGBA8, BGRA8, RGBA32F, DXN_XY
 
 Texture formats unsupported: Cubemaps (hdri, sky)
 
 # 💻 CLI Utility
 
 ## Usage
@@ -148,14 +149,18 @@
 
 # Output path is optional.
 # Defaults to source path with new suffix.
 convert.mcsa_to_obj("path/to/model.mcsa", "path/to/model.obj")
 convert.ol_to_dds("path/to/texture.ol", "path/to/texture.dds")
 convert.mic_to_png("path/to/image.mic", "path/to/image.png")
 
+# Skeleton support via MilkShape3D
+convert.mcsa_to_ms3d("path/to/model.mcsa", "path/to/model.ms3d")
+convert.mcsa_to_ms3d_ascii("path/to/model.mcsa", "path/to/model.txt")
+
 # Or determinate it automatically
 convert.auto("path/to/model.mcsa")
 ```
 
 ### Advanced
 
 Default
```

