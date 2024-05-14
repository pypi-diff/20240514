# Comparing `tmp/iregexp_check-0.1.2.tar.gz` & `tmp/iregexp_check-0.1.3.tar.gz`

## Comparing `iregexp_check-0.1.2.tar` & `iregexp_check-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0     1001      127      308 2024-05-14 10:28:14.000000 iregexp_check-0.1.2/crates/iregexp/Cargo.toml
--rw-r--r--   0     1001      127      229 2024-05-14 10:28:14.000000 iregexp_check-0.1.2/crates/iregexp/README.md
--rw-r--r--   0     1001      127     1977 2024-05-14 10:28:14.000000 iregexp_check-0.1.2/crates/iregexp/src/iregexp.pest
--rw-r--r--   0     1001      127      501 2024-05-14 10:28:14.000000 iregexp_check-0.1.2/crates/iregexp/src/lib.rs
--rw-r--r--   0     1001      127     7313 2024-05-14 10:28:14.000000 iregexp_check-0.1.2/crates/iregexp/src/parser.rs
--rw-r--r--   0        0        0      327 1970-01-01 00:00:00.000000 iregexp_check-0.1.2/crates/python/Cargo.toml
--rw-r--r--   0     1001      127      686 2024-05-14 10:28:14.000000 iregexp_check-0.1.2/crates/python/.gitignore
--rw-r--r--   0     1001      127      283 2024-05-14 10:28:14.000000 iregexp_check-0.1.2/crates/python/README.md
--rw-r--r--   0     1001      127       37 2024-05-14 10:28:14.000000 iregexp_check-0.1.2/crates/python/i_regexp.pyi
--rw-r--r--   0     1001      127        0 2024-05-14 10:28:14.000000 iregexp_check-0.1.2/crates/python/py.typed
--rw-r--r--   0     1001      127       15 2024-05-14 10:28:14.000000 iregexp_check-0.1.2/crates/python/requirements.txt
--rw-r--r--   0     1001      127      370 2024-05-14 10:28:14.000000 iregexp_check-0.1.2/crates/python/src/lib.rs
--rw-r--r--   0     1001      127    11900 2024-05-14 10:28:14.000000 iregexp_check-0.1.2/Cargo.lock
--rw-r--r--   0        0        0       87 1970-01-01 00:00:00.000000 iregexp_check-0.1.2/Cargo.toml
--rw-r--r--   0        0        0     1148 1970-01-01 00:00:00.000000 iregexp_check-0.1.2/pyproject.toml
--rw-r--r--   0     1001      127      283 2024-05-14 10:28:14.000000 iregexp_check-0.1.2/README.md
--rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 iregexp_check-0.1.2/PKG-INFO
+-rw-r--r--   0     1001      127      308 2024-05-14 14:27:43.000000 iregexp_check-0.1.3/crates/iregexp/Cargo.toml
+-rw-r--r--   0     1001      127      229 2024-05-14 14:27:43.000000 iregexp_check-0.1.3/crates/iregexp/README.md
+-rw-r--r--   0     1001      127     1977 2024-05-14 14:27:43.000000 iregexp_check-0.1.3/crates/iregexp/src/iregexp.pest
+-rw-r--r--   0     1001      127      501 2024-05-14 14:27:43.000000 iregexp_check-0.1.3/crates/iregexp/src/lib.rs
+-rw-r--r--   0     1001      127     7313 2024-05-14 14:27:43.000000 iregexp_check-0.1.3/crates/iregexp/src/parser.rs
+-rw-r--r--   0        0        0      327 1970-01-01 00:00:00.000000 iregexp_check-0.1.3/crates/python/Cargo.toml
+-rw-r--r--   0     1001      127      686 2024-05-14 14:27:43.000000 iregexp_check-0.1.3/crates/python/.gitignore
+-rw-r--r--   0     1001      127      283 2024-05-14 14:27:43.000000 iregexp_check-0.1.3/crates/python/README.md
+-rw-r--r--   0     1001      127       37 2024-05-14 14:27:43.000000 iregexp_check-0.1.3/crates/python/iregexp_check.pyi
+-rw-r--r--   0     1001      127        0 2024-05-14 14:27:43.000000 iregexp_check-0.1.3/crates/python/py.typed
+-rw-r--r--   0     1001      127       15 2024-05-14 14:27:43.000000 iregexp_check-0.1.3/crates/python/requirements.txt
+-rw-r--r--   0     1001      127      370 2024-05-14 14:27:43.000000 iregexp_check-0.1.3/crates/python/src/lib.rs
+-rw-r--r--   0     1001      127    11900 2024-05-14 14:27:43.000000 iregexp_check-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0       87 1970-01-01 00:00:00.000000 iregexp_check-0.1.3/Cargo.toml
+-rw-r--r--   0        0        0     1148 1970-01-01 00:00:00.000000 iregexp_check-0.1.3/pyproject.toml
+-rw-r--r--   0     1001      127      283 2024-05-14 14:27:43.000000 iregexp_check-0.1.3/README.md
+-rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 iregexp_check-0.1.3/PKG-INFO
```

### Comparing `iregexp_check-0.1.2/crates/iregexp/src/iregexp.pest` & `iregexp_check-0.1.3/crates/iregexp/src/iregexp.pest`

 * *Files identical despite different names*

### Comparing `iregexp_check-0.1.2/crates/iregexp/src/parser.rs` & `iregexp_check-0.1.3/crates/iregexp/src/parser.rs`

 * *Files identical despite different names*

### Comparing `iregexp_check-0.1.2/crates/python/.gitignore` & `iregexp_check-0.1.3/crates/python/.gitignore`

 * *Files identical despite different names*

### Comparing `iregexp_check-0.1.2/Cargo.lock` & `iregexp_check-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "i_regexp"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "iregexp",
  "pyo3",
 ]
 
 [[package]]
 name = "indoc"
```

### Comparing `iregexp_check-0.1.2/pyproject.toml` & `iregexp_check-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iregexp_check-0.1.2/PKG-INFO` & `iregexp_check-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: iregexp-check
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3.8
```

