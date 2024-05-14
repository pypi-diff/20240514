# Comparing `tmp/crutil-2.1.0.tar.gz` & `tmp/crutil-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crutil-2.1.0.tar", last modified: Mon May 13 12:52:01 2024, max compression
+gzip compressed data, was "crutil-2.1.1.tar", last modified: Mon May 13 15:23:11 2024, max compression
```

## Comparing `crutil-2.1.0.tar` & `crutil-2.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 12:52:01.397836 crutil-2.1.0/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1050 2022-11-13 15:45:04.000000 crutil-2.1.0/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)      311 2024-05-10 17:03:57.000000 crutil-2.1.0/MANIFEST.in
--rw-rw-r--   0 tom       (1000) tom       (1000)      254 2024-05-13 12:52:01.397836 crutil-2.1.0/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     1497 2024-05-10 20:13:14.000000 crutil-2.1.0/README.md
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 12:52:01.393836 crutil-2.1.0/crutil.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)      254 2024-05-13 12:52:01.000000 crutil-2.1.0/crutil.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      546 2024-05-13 12:52:01.000000 crutil-2.1.0/crutil.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-05-13 12:52:01.000000 crutil-2.1.0/crutil.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       19 2024-05-13 12:52:01.000000 crutil-2.1.0/crutil.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        7 2024-05-13 12:52:01.000000 crutil-2.1.0/crutil.egg-info/top_level.txt
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 12:52:01.393836 crutil-2.1.0/scripts/
--rw-rw-r--   0 tom       (1000) tom       (1000)      442 2024-05-10 20:15:10.000000 crutil-2.1.0/scripts/crutil-compile
--rw-rw-r--   0 tom       (1000) tom       (1000)      446 2024-05-10 20:15:44.000000 crutil-2.1.0/scripts/crutil-install
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2024-05-13 12:52:01.397836 crutil-2.1.0/setup.cfg
--rw-rw-r--   0 tom       (1000) tom       (1000)      955 2024-05-10 20:14:09.000000 crutil-2.1.0/setup.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 12:52:01.393836 crutil-2.1.0/source/
--rw-rw-r--   0 tom       (1000) tom       (1000)      256 2024-05-10 17:11:30.000000 crutil-2.1.0/source/__init__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 12:52:01.389836 crutil-2.1.0/source/c/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 12:52:01.397836 crutil-2.1.0/source/c/combinatorics/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1262 2024-05-10 17:03:57.000000 crutil-2.1.0/source/c/combinatorics/main.c
--rw-rw-r--   0 tom       (1000) tom       (1000)     1925 2024-05-10 17:03:57.000000 crutil-2.1.0/source/c_utils.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2073 2024-05-10 17:03:57.000000 crutil-2.1.0/source/collatz.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1044 2024-05-10 23:28:53.000000 crutil-2.1.0/source/combinatorics.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3816 2024-05-11 01:22:56.000000 crutil-2.1.0/source/primes.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 12:52:01.389836 crutil-2.1.0/source/rust/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 12:52:01.397836 crutil-2.1.0/source/rust/hosker_collatz/
--rw-rw-r--   0 tom       (1000) tom       (1000)      165 2024-05-09 11:22:59.000000 crutil-2.1.0/source/rust/hosker_collatz/Cargo.toml
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 12:52:01.397836 crutil-2.1.0/source/rust/hosker_collatz/src/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1618 2024-05-09 11:22:59.000000 crutil-2.1.0/source/rust/hosker_collatz/src/lib.rs
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 12:52:01.397836 crutil-2.1.0/source/rust/hosker_primes/
--rw-rw-r--   0 tom       (1000) tom       (1000)      261 2024-04-25 17:35:09.000000 crutil-2.1.0/source/rust/hosker_primes/Cargo.toml
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 12:52:01.397836 crutil-2.1.0/source/rust/hosker_primes/src/
--rw-rw-r--   0 tom       (1000) tom       (1000)     3369 2024-04-26 18:27:50.000000 crutil-2.1.0/source/rust/hosker_primes/src/lib.rs
--rw-rw-r--   0 tom       (1000) tom       (1000)     2631 2024-05-10 17:03:57.000000 crutil-2.1.0/source/rust_utils.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1172 2024-05-10 23:57:12.000000 crutil-2.1.0/source/utils.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 15:23:11.495926 crutil-2.1.1/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1050 2022-11-13 15:45:04.000000 crutil-2.1.1/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)      311 2024-05-10 17:03:57.000000 crutil-2.1.1/MANIFEST.in
+-rw-rw-r--   0 tom       (1000) tom       (1000)      254 2024-05-13 15:23:11.495926 crutil-2.1.1/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1497 2024-05-10 20:13:14.000000 crutil-2.1.1/README.md
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 15:23:11.495926 crutil-2.1.1/crutil.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      254 2024-05-13 15:23:11.000000 crutil-2.1.1/crutil.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)      546 2024-05-13 15:23:11.000000 crutil-2.1.1/crutil.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-05-13 15:23:11.000000 crutil-2.1.1/crutil.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       19 2024-05-13 15:23:11.000000 crutil-2.1.1/crutil.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        7 2024-05-13 15:23:11.000000 crutil-2.1.1/crutil.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 15:23:11.495926 crutil-2.1.1/scripts/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      442 2024-05-10 20:15:10.000000 crutil-2.1.1/scripts/crutil-compile
+-rw-rw-r--   0 tom       (1000) tom       (1000)      446 2024-05-10 20:15:44.000000 crutil-2.1.1/scripts/crutil-install
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2024-05-13 15:23:11.495926 crutil-2.1.1/setup.cfg
+-rw-rw-r--   0 tom       (1000) tom       (1000)      955 2024-05-13 15:21:48.000000 crutil-2.1.1/setup.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 15:23:11.495926 crutil-2.1.1/source/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      256 2024-05-10 17:11:30.000000 crutil-2.1.1/source/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 15:23:11.491926 crutil-2.1.1/source/c/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 15:23:11.495926 crutil-2.1.1/source/c/combinatorics/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1262 2024-05-10 17:03:57.000000 crutil-2.1.1/source/c/combinatorics/main.c
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1925 2024-05-10 17:03:57.000000 crutil-2.1.1/source/c_utils.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2031 2024-05-13 13:28:30.000000 crutil-2.1.1/source/collatz.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1008 2024-05-13 13:32:24.000000 crutil-2.1.1/source/combinatorics.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3716 2024-05-13 13:23:33.000000 crutil-2.1.1/source/primes.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 15:23:11.491926 crutil-2.1.1/source/rust/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 15:23:11.495926 crutil-2.1.1/source/rust/hosker_collatz/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      165 2024-05-09 11:22:59.000000 crutil-2.1.1/source/rust/hosker_collatz/Cargo.toml
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 15:23:11.495926 crutil-2.1.1/source/rust/hosker_collatz/src/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1618 2024-05-09 11:22:59.000000 crutil-2.1.1/source/rust/hosker_collatz/src/lib.rs
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 15:23:11.495926 crutil-2.1.1/source/rust/hosker_primes/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      261 2024-04-25 17:35:09.000000 crutil-2.1.1/source/rust/hosker_primes/Cargo.toml
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 15:23:11.495926 crutil-2.1.1/source/rust/hosker_primes/src/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3369 2024-04-26 18:27:50.000000 crutil-2.1.1/source/rust/hosker_primes/src/lib.rs
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2631 2024-05-10 17:03:57.000000 crutil-2.1.1/source/rust_utils.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1179 2024-05-13 13:17:35.000000 crutil-2.1.1/source/utils.py
```

### Comparing `crutil-2.1.0/LICENSE` & `crutil-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crutil-2.1.0/README.md` & `crutil-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `crutil-2.1.0/crutil.egg-info/SOURCES.txt` & `crutil-2.1.1/crutil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crutil-2.1.0/setup.py` & `crutil-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 # Non-standard imports.
 from setuptools import setup
 
 # Local constants.
 PACKAGE_NAME = "crutil"
-VERSION = "2.1.0"
+VERSION = "2.1.1"
 DESCRIPTION = "C and Rust utility functions"
 GIT_URL_STEM = "https://github.com/tomhosker"
 AUTHOR = "Tom Hosker"
 AUTHOR_EMAIL = "tomdothosker@gmail.com"
 SCRIPT_PATHS = ("scripts/crutil-install", "scripts/crutil-compile")
 INSTALL_REQUIRES = ("hosker_utils", "sympy")
 INCLUDE_PACKAGE_DATA = True
```

### Comparing `crutil-2.1.0/source/c/combinatorics/main.c` & `crutil-2.1.1/source/c/combinatorics/main.c`

 * *Files identical despite different names*

### Comparing `crutil-2.1.0/source/c_utils.py` & `crutil-2.1.1/source/c_utils.py`

 * *Files identical despite different names*

### Comparing `crutil-2.1.0/source/collatz.py` & `crutil-2.1.1/source/collatz.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This code interfaces with the "collatz" Rust library.
 """
 
 # Standard imports.
 from ctypes import c_int32
 
 # Local imports.
-from .utils import make_contact_template
+from .utils import make_contact_template, refine_ffunc
 from .rust_utils import get_local_rust_library, MAX_I32
 
 # Local constants.
 RUST_LIB = get_local_rust_library("hosker_collatz")
 
 #############
 # FUNCTIONS #
@@ -38,17 +38,15 @@
     return result
 
 def count_collatz_steps(num: int) -> int:
     """ Count the number of Collatz steps required to reach 1, given a starting
     point. """
     if num > MAX_I32:
         return count_collatz_steps_large(num)
-    rust_func = RUST_LIB.count_collatz_steps
-    rust_func.argtypes = [c_int32]
-    rust_func.restype = c_int32
+    rust_func = refine_ffunc(RUST_LIB.count_collatz_steps, [c_int32], c_int32)
     result = rust_func(num)
     return result
 
 def max_collatz_steps_under_large(limit: int) -> int:
     """ As below, but suitable for large integers. """
     result = 1
     current_max = 0
@@ -62,12 +60,11 @@
 
 def max_collatz_steps_under(limit: int) -> int:
     """ Find the maximum number of Collatz steps required to reach 1, if one
     uses all the numbers between 1 and a given limit (inclusive) as starting
     points. """
     if limit > MAX_I32:
         return max_collatz_steps_under_large(limit)
-    rust_func = RUST_LIB.max_collatz_steps_under
-    rust_func.argtypes = [c_int32]
-    rust_func.restype = c_int32
+    rust_func = \
+        refine_ffunc(RUST_LIB.max_collatz_steps_under, [c_int32], c_int32)
     result = rust_func(limit)
     return result
```

### Comparing `crutil-2.1.0/source/combinatorics.py` & `crutil-2.1.1/source/combinatorics.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This code interfaces with the "combinatorics" C library.
 """
 
 # Standard import.
 from ctypes import c_void_p, c_char_p, c_int32, cast
 
 # Local imports.
-from .utils import make_contact_template
+from .utils import make_contact_template, refine_ffunc
 from .c_utils import get_local_c_library
 
 # Local constants.
 CLIB = get_local_c_library("combinatorics")
 
 #############
 # FUNCTIONS #
@@ -19,22 +19,18 @@
 def make_contact():
     """ Prove that you can access this library. """
     return make_contact_template(CLIB)
 
 def free_string(string_pointer: c_char_p):
     """ Calling this, after having called a C function which returns a string,
     prevents memory leaks. """
-    cfunc = CLIB.free_string
-    cfunc.argtypes = [c_char_p]
-    cfunc.restype = None
+    cfunc = refine_ffunc(CLIB.free_string, [c_char_p], None)
     cfunc(string_pointer)
 
 def factorial(num: int) -> int:
     """ Return num!. """
-    cfunc = CLIB.factorial
-    cfunc.argtypes = [c_int32]
-    cfunc.restype = c_void_p
+    cfunc = refine_ffunc(CLIB.factorial, [c_int32], c_void_p)
     raw_pointer = cfunc(num)
     string_pointer = cast(raw_pointer, c_char_p)
     result = int(string_pointer.value.decode())
     free_string(string_pointer)
     return result
```

### Comparing `crutil-2.1.0/source/primes.py` & `crutil-2.1.1/source/primes.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import warnings
 from ctypes import c_char_p, c_int32, c_void_p, cast
 
 # Non-standard imports.
 import sympy
 
 # Local imports.
-from .utils import make_contact_template, int_to_bool, refine_func
+from .utils import make_contact_template, int_to_bool, refine_ffunc
 from .rust_utils import get_local_rust_library, rusticate_int, MAX_I32
 
 # Local constants.
 RUST_LIB = get_local_rust_library("hosker_primes")
 MAX_DIGITS = 100
 BIGINT_DIGIT_LIST_C_TYPE = c_int32*MAX_DIGITS
 MAX_PRIME_ORDINAL_I32 = 105097565
@@ -25,65 +25,68 @@
 
 def make_contact():
     """ Prove that you can access this library. """
     return make_contact_template(RUST_LIB)
 
 def is_prime_i32(number: int) -> bool:
     """ Determine whether a given 32-bit integer is prime. """
-    rust_func = refine_func(RUST_LIB.is_prime_i32, [c_int32], c_int32)
+    rust_func = refine_ffunc(RUST_LIB.is_prime_i32, [c_int32], c_int32)
     rust_result = rust_func(number)
     result = int_to_bool(rust_result)
     return result
 
 def is_prime_bigint_rust(number: int) -> bool:
     """
     Determine whether an arbitrarily large number is prime, where that
     arbitrarily large number is represented by a list of "digits", and where
     each of those "digits" represents a power of 2**32, rather than of 10.
 
     IMPORTANT: This function is SLOWER than sympy.isprime(n).
     """
     bigint_digit_list, _ = rusticate_int(number)
     c_array = BIGINT_DIGIT_LIST_C_TYPE(*bigint_digit_list)
-    rust_func = refine_func(RUST_LIB.is_prime_bigint, [BIGINT_DIGIT_LIST_C_TYPE] 
-    rust_func = RUST_LIB.is_prime_bigint
-    rust_func.argtypes = [BIGINT_DIGIT_LIST_C_TYPE]
-    rust_func.restype = c_int32
+    rust_func = \
+        refine_ffunc(
+            RUST_LIB.is_prime_bigint,
+            [BIGINT_DIGIT_LIST_C_TYPE],
+            c_int32
+        )
     rust_result = rust_func(c_array)
     result = int_to_bool(rust_result)
     return result
 
 def is_prime(number: int) -> bool:
     """ Combine the i32 and BigInt methods into one. """
     if number < MAX_I32:
         return is_prime_i32(number)
     return sympy.isprime(number)
 
 def free_string(string_pointer: c_char_p):
     """ Calling this, after having called a Rust function which returns a
     string, prevents memory leaks. """
-    rust_func = RUST_LIB.free_string
-    rust_func.argtypes = [c_char_p]
-    rust_func.restype = None
+    rust_func = refine_ffunc(RUST_LIB.free_string, [c_char_p], None)
     rust_func(string_pointer)
 
 def echo_big_integer(big_integer: int) -> int:
     """
     This function passes an arbitrarily large integer to Rust, and then receives
     exactly the same integer back from Rust, and returns that integer.
 
     Obviously, on its own this serves no earthly purpose, but it might
     demonstrate one means of passing an arbitrarily large integer from Rust
     to Python, which is not straightforward.
     """
     bigint_digit_list, _ = rusticate_int(big_integer)
     c_array = BIGINT_DIGIT_LIST_C_TYPE(*bigint_digit_list)
-    rust_func = RUST_LIB.echo_big_integer
-    rust_func.argtypes = [BIGINT_DIGIT_LIST_C_TYPE]
-    rust_func.restype = c_void_p
+    rust_func = \
+        refine_ffunc(
+            RUST_LIB.echo_big_integer,
+            [BIGINT_DIGIT_LIST_C_TYPE],
+            c_void_p
+        )
     raw_pointer = rust_func(c_array)
     string_pointer = cast(raw_pointer, c_char_p)
     result = int(string_pointer.value.decode())
     free_string(string_pointer)
     return result
 
 def nth_prime_i32(ordinal: int) -> int:
@@ -92,17 +95,15 @@
     if ordinal > MAX_PRIME_ORDINAL_I32:
         warnings.warn(
             f"The prime with {ordinal} cannot be represented in 32 bits. "+
             f"The largest prime representable in 32 bits is {MAX_I32}, with "+
             f"ordinal {MAX_PRIME_ORDINAL_I32}."
         )
         return None
-    rust_func = RUST_LIB.nth_prime_i32
-    rust_func.argtypes = [c_int32]
-    rust_func.restype = c_int32
+    rust_func = refine_ffunc(RUST_LIB.nth_prime_i32, [c_int32], c_int32)
     result = rust_func(ordinal)
     return result
 
 def nth_prime(ordinal: int) -> int:
     """ As above, but for an arbitrarily large ordinal. """
     if ordinal < MAX_PRIME_ORDINAL_I32:
         return nth_prime_i32(ordinal)
```

### Comparing `crutil-2.1.0/source/rust/hosker_collatz/src/lib.rs` & `crutil-2.1.1/source/rust/hosker_collatz/src/lib.rs`

 * *Files identical despite different names*

### Comparing `crutil-2.1.0/source/rust/hosker_primes/src/lib.rs` & `crutil-2.1.1/source/rust/hosker_primes/src/lib.rs`

 * *Files identical despite different names*

### Comparing `crutil-2.1.0/source/rust_utils.py` & `crutil-2.1.1/source/rust_utils.py`

 * *Files identical despite different names*

### Comparing `crutil-2.1.0/source/utils.py` & `crutil-2.1.1/source/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,31 +20,31 @@
 class CRUtilBadBooleanInteger(Exception):
     """ A custom exception. """
 
 #############
 # FUNCTIONS #
 #############
 
-def refine_func(func, argtypes, restype):
-    """ Assign argument types and a return type to a ctypes function in one
-    line. """
+def refine_ffunc(func, argtypes, restype):
+    """ Assign argument types and a return type to a ctypes foreign function in
+    one line. """
     func.argtypes = argtypes
     func.restype = restype
     return func
 
 def make_contact_template(library):
     """ Prove that you can access the library in question. """
     try:
-        func = refine_func(library.make_contact, [], None)
+        func = refine_ffunc(library.make_contact, [], None)
         library.make_contact(LUCKY_INT)
     except:
         traceback.print_exc()
         return False
     return True
 
 def int_to_bool(integer):
     """ Convert an integer representation of a boolean into a boolean. """
     if integer == TRUE_INT:
         return True
     if integer == FALSE_INT:
         return False
-    raise CRUtilBadBooleanInteger("Bad boolean integer: "+str(integer))
+    raise CRUtilBadBooleanInteger(f"Bad boolean integer: {integer}")
```

