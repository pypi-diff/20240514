# Comparing `tmp/rlbot_flatbuffers-0.3.4.tar.gz` & `tmp/rlbot_flatbuffers-0.3.5.tar.gz`

## Comparing `rlbot_flatbuffers-0.3.4.tar` & `rlbot_flatbuffers-0.3.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 rlbot_flatbuffers-0.3.4/Cargo.toml
--rw-r--r--   0     1001      127     1070 2024-05-08 22:16:03.000000 rlbot_flatbuffers-0.3.4/LICENSE
--rw-r--r--   0     1001      127      479 2024-05-08 22:16:03.000000 rlbot_flatbuffers-0.3.4/README.md
--rw-r--r--   0     1001      127    61447 2024-05-08 22:16:03.000000 rlbot_flatbuffers-0.3.4/build.rs
--rw-r--r--   0     1001      127      182 2024-05-08 22:16:05.000000 rlbot_flatbuffers-0.3.4/flatbuffers-schema/README.md
--rw-r--r--   0     1001      127      401 2024-05-08 22:16:05.000000 rlbot_flatbuffers-0.3.4/flatbuffers-schema/comms.fbs
--rw-r--r--   0     1001      127     1932 2024-05-08 22:16:05.000000 rlbot_flatbuffers-0.3.4/flatbuffers-schema/event.fbs
--rwxr-xr-x   0     1001      127  6685928 2024-05-08 22:16:05.000000 rlbot_flatbuffers-0.3.4/flatbuffers-schema/flatc
--rw-r--r--   0     1001      127  3488256 2024-05-08 22:16:05.000000 rlbot_flatbuffers-0.3.4/flatbuffers-schema/flatc.exe
--rwxr-xr-x   0     1001      127  6896752 2024-05-08 22:16:05.000000 rlbot_flatbuffers-0.3.4/flatbuffers-schema/flatc_mac
--rw-r--r--   0     1001      127     1281 2024-05-08 22:16:05.000000 rlbot_flatbuffers-0.3.4/flatbuffers-schema/gamestate.fbs
--rw-r--r--   0     1001      127     5824 2024-05-08 22:16:05.000000 rlbot_flatbuffers-0.3.4/flatbuffers-schema/matchstart.fbs
--rw-r--r--   0     1001      127     1162 2024-05-08 22:16:05.000000 rlbot_flatbuffers-0.3.4/flatbuffers-schema/rendering.fbs
--rw-r--r--   0     1001      127     6296 2024-05-08 22:16:05.000000 rlbot_flatbuffers-0.3.4/flatbuffers-schema/rlbot.fbs
--rw-r--r--   0     1001      127     5365 2024-05-08 22:16:03.000000 rlbot_flatbuffers-0.3.4/src/lib.rs
--rw-r--r--   0     1001      127    13114 2024-05-08 22:16:03.000000 rlbot_flatbuffers-0.3.4/Cargo.lock
--rw-r--r--   0     1001      127      418 2024-05-08 22:16:03.000000 rlbot_flatbuffers-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 rlbot_flatbuffers-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 rlbot_flatbuffers-0.3.5/Cargo.toml
+-rw-r--r--   0     1001      127     1070 2024-05-14 21:23:39.000000 rlbot_flatbuffers-0.3.5/LICENSE
+-rw-r--r--   0     1001      127      479 2024-05-14 21:23:39.000000 rlbot_flatbuffers-0.3.5/README.md
+-rw-r--r--   0     1001      127    61922 2024-05-14 21:23:39.000000 rlbot_flatbuffers-0.3.5/build.rs
+-rw-r--r--   0     1001      127      182 2024-05-14 21:23:40.000000 rlbot_flatbuffers-0.3.5/flatbuffers-schema/README.md
+-rw-r--r--   0     1001      127      401 2024-05-14 21:23:40.000000 rlbot_flatbuffers-0.3.5/flatbuffers-schema/comms.fbs
+-rw-r--r--   0     1001      127     1932 2024-05-14 21:23:40.000000 rlbot_flatbuffers-0.3.5/flatbuffers-schema/event.fbs
+-rwxr-xr-x   0     1001      127  6685928 2024-05-14 21:23:41.000000 rlbot_flatbuffers-0.3.5/flatbuffers-schema/flatc
+-rw-r--r--   0     1001      127  3488256 2024-05-14 21:23:41.000000 rlbot_flatbuffers-0.3.5/flatbuffers-schema/flatc.exe
+-rwxr-xr-x   0     1001      127  6896752 2024-05-14 21:23:41.000000 rlbot_flatbuffers-0.3.5/flatbuffers-schema/flatc_mac
+-rw-r--r--   0     1001      127     1281 2024-05-14 21:23:41.000000 rlbot_flatbuffers-0.3.5/flatbuffers-schema/gamestate.fbs
+-rw-r--r--   0     1001      127     5824 2024-05-14 21:23:41.000000 rlbot_flatbuffers-0.3.5/flatbuffers-schema/matchstart.fbs
+-rw-r--r--   0     1001      127     1162 2024-05-14 21:23:41.000000 rlbot_flatbuffers-0.3.5/flatbuffers-schema/rendering.fbs
+-rw-r--r--   0     1001      127     6296 2024-05-14 21:23:41.000000 rlbot_flatbuffers-0.3.5/flatbuffers-schema/rlbot.fbs
+-rw-r--r--   0     1001      127     5543 2024-05-14 21:23:39.000000 rlbot_flatbuffers-0.3.5/src/lib.rs
+-rw-r--r--   0     1001      127    13114 2024-05-14 21:23:39.000000 rlbot_flatbuffers-0.3.5/Cargo.lock
+-rw-r--r--   0     1001      127      418 2024-05-14 21:23:39.000000 rlbot_flatbuffers-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 rlbot_flatbuffers-0.3.5/PKG-INFO
```

### Comparing `rlbot_flatbuffers-0.3.4/Cargo.toml` & `rlbot_flatbuffers-0.3.5/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rlbot-flatbuffers-py"
-version = "0.3.4"
+version = "0.3.5"
 edition = "2021"
 description = "A Python module implemented in Rust for serializing and deserializing RLBot's flatbuffers"
 repository = "https://github.com/VirxEC/rlbot-flatbuffers-py"
 license = "MIT"
 readme = "README.md"
 exclude = [".github", "pytest.py", "rustfmt.toml", ".gitignore", ".gitmodules"]
 publish = false
```

### Comparing `rlbot_flatbuffers-0.3.4/LICENSE` & `rlbot_flatbuffers-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.4/build.rs` & `rlbot_flatbuffers-0.3.5/build.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1134,24 +1134,35 @@
             self.write_str("            Err(e) => Err(flat_err_to_py(e)),");
             self.write_str("        }");
         }
 
         self.write_str("    }");
     }
 
+    fn generate_enum_hash_method(&mut self) {
+        self.write_str("    pub fn __hash__(&self) -> u64 {");
+        self.write_str("        crate::hash_u64(*self as u64)");
+        self.write_str("    }");
+    }
+
     fn generate_py_methods(&mut self) {
         self.write_str("#[pymethods]");
         self.write_string(format!("impl {} {{", self.struct_name));
 
         self.generate_new_method();
         self.write_str("");
         self.generate_str_method();
         self.write_str("");
         self.generate_repr_method();
 
+        if self.bind_type == PythonBindType::Enum {
+            self.write_str("");
+            self.generate_enum_hash_method();
+        }
+
         if self.bind_type != PythonBindType::Union {
             self.write_str("");
             self.generate_pack_method();
             self.write_str("");
             self.generate_unpack_method();
         }
 
@@ -1354,15 +1365,17 @@
             }
 
             file_contents.push(Cow::Borrowed(""));
 
             if is_enum {
                 file_contents.push(Cow::Borrowed("    def __init__(self, value: int = 0):"));
                 file_contents.push(Cow::Borrowed("        \"\"\""));
-                file_contents.push(Cow::Borrowed("        :raises ValueError: If the `value` is not a valid enum value"));
+                file_contents.push(Cow::Borrowed(
+                    "        :raises ValueError: If the `value` is not a valid enum value",
+                ));
                 file_contents.push(Cow::Borrowed("        \"\"\""));
             } else {
                 file_contents.push(Cow::Borrowed("    def __init__("));
                 file_contents.push(Cow::Borrowed("        self,"));
 
                 let mut i = 0;
                 for variable_info in types {
@@ -1401,14 +1414,15 @@
 
                 file_contents.push(Cow::Borrowed("    ): ..."));
             }
         }
 
         file_contents.push(Cow::Borrowed("    def __str__(self) -> str: ..."));
         file_contents.push(Cow::Borrowed("    def __repr__(self) -> str: ..."));
+        file_contents.push(Cow::Borrowed("    def __hash__(self) -> str: ..."));
 
         if is_enum {
             file_contents.push(Cow::Borrowed("    def __int__(self) -> int: ..."));
             file_contents.push(Cow::Owned(format!(
                 "    def __richcmp__(self, other: {type_name}, op: int) -> bool: ..."
             )));
         }
```

### Comparing `rlbot_flatbuffers-0.3.4/flatbuffers-schema/event.fbs` & `rlbot_flatbuffers-0.3.5/flatbuffers-schema/event.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.4/flatbuffers-schema/flatc` & `rlbot_flatbuffers-0.3.5/flatbuffers-schema/flatc`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.4/flatbuffers-schema/flatc.exe` & `rlbot_flatbuffers-0.3.5/flatbuffers-schema/flatc.exe`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.4/flatbuffers-schema/flatc_mac` & `rlbot_flatbuffers-0.3.5/flatbuffers-schema/flatc_mac`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.4/flatbuffers-schema/gamestate.fbs` & `rlbot_flatbuffers-0.3.5/flatbuffers-schema/gamestate.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.4/flatbuffers-schema/matchstart.fbs` & `rlbot_flatbuffers-0.3.5/flatbuffers-schema/matchstart.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.4/flatbuffers-schema/rendering.fbs` & `rlbot_flatbuffers-0.3.5/flatbuffers-schema/rendering.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.4/flatbuffers-schema/rlbot.fbs` & `rlbot_flatbuffers-0.3.5/flatbuffers-schema/rlbot.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.4/src/lib.rs` & `rlbot_flatbuffers-0.3.5/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -10,25 +10,34 @@
 pub mod generated;
 
 #[allow(clippy::enum_variant_names)]
 mod python;
 
 use pyo3::{create_exception, exceptions::PyValueError, prelude::*, types::PyBytes, PyClass};
 use python::*;
-use std::panic::Location;
+use std::{
+    hash::{DefaultHasher, Hash, Hasher},
+    panic::Location,
+};
 
 create_exception!(rlbot_flatbuffers, InvalidFlatbuffer, PyValueError, "Invalid FlatBuffer");
 
 #[track_caller]
 pub fn flat_err_to_py(err: flatbuffers::InvalidFlatbuffer) -> PyErr {
     let caller = Location::caller();
     let err_msg = format!("Can't make flatbuffer @ \"rlbot_flatbuffers/{}\":\n  {err}", caller.file());
     InvalidFlatbuffer::new_err(err_msg)
 }
 
+pub fn hash_u64(num: u64) -> u64 {
+    let mut hasher = DefaultHasher::new();
+    num.hash(&mut hasher);
+    hasher.finish()
+}
+
 pub trait FromGil<T> {
     fn from_gil(py: Python, obj: T) -> Self;
 }
 
 pub trait IntoGil<T>: Sized {
     fn into_gil(self, py: Python) -> T;
 }
```

### Comparing `rlbot_flatbuffers-0.3.4/Cargo.lock` & `rlbot_flatbuffers-0.3.5/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c124f12ade4e670107b132722d0ad1a5c9790bcbc1b265336369ea05626b4498"
 dependencies = [
  "attribute-derive-macro",
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "attribute-derive-macro"
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b217a07446e0fb086f83401a98297e2d81492122f5874db5391bd270a185f88"
@@ -23,15 +23,15 @@
  "collection_literals",
  "interpolator",
  "proc-macro-error",
  "proc-macro-utils",
  "proc-macro2",
  "quote",
  "quote-use",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
@@ -64,15 +64,15 @@
 name = "derive-where"
 version = "1.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62d671cc41a825ebabc75757b62d3d168c577f9149b2d49ece1dad1f72119d25"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "flatbuffers"
 version = "24.3.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8add37afff2d4ffa83bc748a70b4b1370984f6980768554182424ef71447c35f"
@@ -94,15 +94,15 @@
 name = "get-size-derive"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "13a1bcfb855c1f340d5913ab542e36f25a1c56f57de79022928297632435dec2"
 dependencies = [
  "attribute-derive",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
@@ -266,28 +266,28 @@
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
@@ -299,41 +299,41 @@
 name = "quote-use"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a7b5abe3fe82fdeeb93f44d66a7b444dedf2e4827defb0a8e69c437b2de2ef94"
 dependencies = [
  "quote",
  "quote-use-macros",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "quote-use-macros"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "97ea44c7e20f16017a76a245bb42188517e13d16dcb1aa18044bc406cdc3f4af"
 dependencies = [
  "derive-where",
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
  "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "rlbot-flatbuffers-py"
-version = "0.3.4"
+version = "0.3.5"
 dependencies = [
  "flatbuffers",
  "get-size",
  "pyo3",
  "serde",
 ]
 
@@ -371,15 +371,15 @@
 name = "serde_derive"
 version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c5e405930b9796f1c00bee880d03fc7e0bb4b9a11afc776885ffe84320da2865"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
@@ -392,17 +392,17 @@
 dependencies = [
  "proc-macro2",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.61"
+version = "2.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c993ed8ccba56ae856363b1845da7266a7cb78e1d146c8a32d54b45a8b831fc9"
+checksum = "bf5be731623ca1a1fb7d8be6f261a3be6d3e2337b8a1f97be944d020c8fcb704"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
```

### Comparing `rlbot_flatbuffers-0.3.4/PKG-INFO` & `rlbot_flatbuffers-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rlbot_flatbuffers
-Version: 0.3.4
+Version: 0.3.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: A Python module implemented in Rust for serializing and deserializing RLBot's flatbuffers
 License: MIT
 Requires-Python: >=3.10
```

