# Comparing `tmp/quokka_sharp-0.0.9.tar.gz` & `tmp/quokka_sharp-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quokka_sharp-0.0.9.tar", last modified: Wed Feb 28 17:21:23 2024, max compression
+gzip compressed data, was "quokka_sharp-1.0.0.tar", last modified: Tue May 14 16:14:17 2024, max compression
```

## Comparing `quokka_sharp-0.0.9.tar` & `quokka_sharp-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 meij     (1596456755) 208802054        0 2024-02-28 17:21:23.757800 quokka_sharp-0.0.9/
--rw-r--r--   0 meij     (1596456755) 208802054      760 2024-02-28 17:21:23.757518 quokka_sharp-0.0.9/PKG-INFO
-drwxr-xr-x   0 meij     (1596456755) 208802054        0 2024-02-28 17:21:23.753909 quokka_sharp-0.0.9/quokka_sharp/
--rw-r--r--   0 meij     (1596456755) 208802054       76 2024-02-28 17:12:12.000000 quokka_sharp-0.0.9/quokka_sharp/__init__.py
--rw-r--r--   0 meij     (1596456755) 208802054     4047 2024-02-28 17:18:34.000000 quokka_sharp-0.0.9/quokka_sharp/ecmc.py
-drwxr-xr-x   0 meij     (1596456755) 208802054        0 2024-02-28 17:21:23.757035 quokka_sharp-0.0.9/quokka_sharp/encoding/
--rw-r--r--   0 meij     (1596456755) 208802054      138 2024-02-16 14:29:26.000000 quokka_sharp-0.0.9/quokka_sharp/encoding/__init__.py
--rw-r--r--   0 meij     (1596456755) 208802054     9090 2024-02-15 09:34:01.000000 quokka_sharp-0.0.9/quokka_sharp/encoding/cliffordt2cnf.py
--rw-r--r--   0 meij     (1596456755) 208802054     8910 2024-02-18 14:22:12.000000 quokka_sharp-0.0.9/quokka_sharp/encoding/cliffordt2cnf_py_codegen.py
--rw-r--r--   0 meij     (1596456755) 208802054     3293 2024-02-15 17:19:49.000000 quokka_sharp-0.0.9/quokka_sharp/encoding/cnf.py
--rw-r--r--   0 meij     (1596456755) 208802054     1115 2024-01-31 13:15:02.000000 quokka_sharp-0.0.9/quokka_sharp/encoding/memory.py
--rw-r--r--   0 meij     (1596456755) 208802054     4061 2024-02-28 16:39:25.000000 quokka_sharp-0.0.9/quokka_sharp/encoding/qasm2cnf.py
--rw-r--r--   0 meij     (1596456755) 208802054     6155 2024-02-27 11:17:06.000000 quokka_sharp-0.0.9/quokka_sharp/encoding/qasm_parser.py
--rw-r--r--   0 meij     (1596456755) 208802054     2839 2024-02-28 17:20:31.000000 quokka_sharp-0.0.9/quokka_sharp/qcmc.py
-drwxr-xr-x   0 meij     (1596456755) 208802054        0 2024-02-28 17:21:23.754909 quokka_sharp-0.0.9/quokka_sharp.egg-info/
--rw-r--r--   0 meij     (1596456755) 208802054      760 2024-02-28 17:21:23.000000 quokka_sharp-0.0.9/quokka_sharp.egg-info/PKG-INFO
--rw-r--r--   0 meij     (1596456755) 208802054      509 2024-02-28 17:21:23.000000 quokka_sharp-0.0.9/quokka_sharp.egg-info/SOURCES.txt
--rw-r--r--   0 meij     (1596456755) 208802054        1 2024-02-28 17:21:23.000000 quokka_sharp-0.0.9/quokka_sharp.egg-info/dependency_links.txt
--rw-r--r--   0 meij     (1596456755) 208802054       12 2024-02-28 17:21:23.000000 quokka_sharp-0.0.9/quokka_sharp.egg-info/requires.txt
--rw-r--r--   0 meij     (1596456755) 208802054       13 2024-02-28 17:21:23.000000 quokka_sharp-0.0.9/quokka_sharp.egg-info/top_level.txt
--rw-r--r--   0 meij     (1596456755) 208802054       38 2024-02-28 17:21:23.757854 quokka_sharp-0.0.9/setup.cfg
--rw-r--r--   0 meij     (1596456755) 208802054     1059 2024-02-28 17:20:58.000000 quokka_sharp-0.0.9/setup.py
+drwxr-xr-x   0 meij     (1596456755) VUW\Domain Users (208802054)        0 2024-05-14 16:14:17.723086 quokka_sharp-1.0.0/
+-rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)      733 2024-05-14 16:14:17.722772 quokka_sharp-1.0.0/PKG-INFO
+drwxr-xr-x   0 meij     (1596456755) VUW\Domain Users (208802054)        0 2024-05-14 16:14:17.719165 quokka_sharp-1.0.0/quokka_sharp/
+-rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)      207 2024-03-18 14:38:39.000000 quokka_sharp-1.0.0/quokka_sharp/__init__.py
+-rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)     2224 2024-04-18 11:56:40.000000 quokka_sharp-1.0.0/quokka_sharp/ecmc.py
+drwxr-xr-x   0 meij     (1596456755) VUW\Domain Users (208802054)        0 2024-05-14 16:14:17.722043 quokka_sharp-1.0.0/quokka_sharp/encoding/
+-rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)      139 2024-03-18 14:38:30.000000 quokka_sharp-1.0.0/quokka_sharp/encoding/__init__.py
+-rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)     9064 2024-05-14 15:44:03.000000 quokka_sharp-1.0.0/quokka_sharp/encoding/cliffordt2cnf.py
+-rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)     4227 2024-04-05 11:20:57.000000 quokka_sharp-1.0.0/quokka_sharp/encoding/cnf.py
+-rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)     1115 2024-01-31 13:15:02.000000 quokka_sharp-1.0.0/quokka_sharp/encoding/memory.py
+-rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)     4439 2024-05-14 15:58:43.000000 quokka_sharp-1.0.0/quokka_sharp/encoding/qasm2cnf.py
+-rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)     5994 2024-03-18 12:57:29.000000 quokka_sharp-1.0.0/quokka_sharp/encoding/qasm_parser.py
+-rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)     1216 2024-04-20 09:44:17.000000 quokka_sharp-1.0.0/quokka_sharp/qcmc.py
+drwxr-xr-x   0 meij     (1596456755) VUW\Domain Users (208802054)        0 2024-05-14 16:14:17.722461 quokka_sharp-1.0.0/quokka_sharp.egg-info/
+-rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)      733 2024-05-14 16:14:17.000000 quokka_sharp-1.0.0/quokka_sharp.egg-info/PKG-INFO
+-rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)      424 2024-05-14 16:14:17.000000 quokka_sharp-1.0.0/quokka_sharp.egg-info/SOURCES.txt
+-rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)        1 2024-05-14 16:14:17.000000 quokka_sharp-1.0.0/quokka_sharp.egg-info/dependency_links.txt
+-rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)       13 2024-05-14 16:14:17.000000 quokka_sharp-1.0.0/quokka_sharp.egg-info/top_level.txt
+-rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)       38 2024-05-14 16:14:17.723158 quokka_sharp-1.0.0/setup.cfg
+-rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)     1046 2024-05-14 16:13:40.000000 quokka_sharp-1.0.0/setup.py
```

### Comparing `quokka_sharp-0.0.9/quokka_sharp/encoding/cliffordt2cnf.py` & `quokka_sharp-1.0.0/quokka_sharp/encoding/cliffordt2cnf.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
     cnf.vars.z[k] = Z
     cnf.vars.r = R
 
 # Equivalent(R, r ^ (x[k] & z[k] & ~Z))
 # x[k] | (Equivalent(Z, z[k]))
 # Equivalent(u, x[k])
-def T2CNF(cnf, k):
+def T2CNF(cnf, k, w):
     r = cnf.vars.r
     x = cnf.vars.x
     z = cnf.vars.z
     R = cnf.add_var()
     Z = cnf.add_var()
     cnf.add_clause([ R, -r,  x[k]])
     cnf.add_clause([ R, -r,  z[k]])
@@ -123,23 +123,23 @@
 
     cnf.add_clause([ Z,  x[k], -z[k]])
     cnf.add_clause([-Z,  x[k],  z[k]])
 
     u = cnf.add_var()
     cnf.add_clause([ u, -x[k]])
     cnf.add_clause([-u,  x[k]])
-    cnf.add_weight(u, 0.707106781186548)
+    cnf.add_weight(u, w)
 
     cnf.vars.z[k] = Z
     cnf.vars.r = R
 
 # Equivalent(R, r ^ (Z & x[k] & ~z[k]))
 # x[k] | (Equivalent(Z, z[k]))
 # Equivalent(u, x[k])
-def Tdg2CNF(cnf, k):
+def Tdg2CNF(cnf, k, w):
     r = cnf.vars.r
     x = cnf.vars.x
     z = cnf.vars.z
     R = cnf.add_var()
     Z = cnf.add_var()
     cnf.add_clause([ R,  Z, -r])
     cnf.add_clause([ R, -r,  x[k]])
@@ -152,15 +152,15 @@
 
     cnf.add_clause([ Z,  x[k], -z[k]])
     cnf.add_clause([-Z,  x[k],  z[k]])
 
     u = cnf.add_var()
     cnf.add_clause([ u, -x[k]])
     cnf.add_clause([-u,  x[k]])
-    cnf.add_weight(u, 0.707106781186548)
+    cnf.add_weight(u, w)
 
     cnf.vars.z[k] = Z
     cnf.vars.r = R
 
 # Equivalent(R, r ^ (x[c] & z[t] & (z[c] ^ ~x[t])))
 # Equivalent(X, x[c] ^ x[t])
 # Equivalent(Z, z[c] ^ z[t])
```

### Comparing `quokka_sharp-0.0.9/quokka_sharp/encoding/memory.py` & `quokka_sharp-1.0.0/quokka_sharp/encoding/memory.py`

 * *Files identical despite different names*

### Comparing `quokka_sharp-0.0.9/quokka_sharp/encoding/qasm2cnf.py` & `quokka_sharp-1.0.0/quokka_sharp/encoding/qasm2cnf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from .cnf import Variables, CNF
 from .cliffordt2cnf import *
 from .qasm_parser import Circuit
 import math
+from decimal import Decimal, getcontext
 
+# set the precision of rotation angles
+getcontext().prec = 32
 
-def convert_to_float(frac_str):
+def frac_to_float(frac_str):
     sign = 0
     if "-" in frac_str:
         sign = 1
         frac_str = frac_str.replace("-",'')
     try:
         return float(frac_str)
     except:
@@ -26,37 +29,37 @@
             piflag = 1
             num = num.replace("pi",'')
             num = num.replace("*",'')
             num = float(num)
         if piflag == 1:
             return math.pow(-1,sign) * num / denom * math.pi
         else:
-            return math.pow(-1,sign) * num / denom
+            return Decimal(math.pow(-1,sign) * num / denom)
 
 def get_angle(angle):
     try:
         if "/" in angle:
-            theta = convert_to_float(angle)
+            theta = frac_to_float(angle)
         else:
             theta_str = angle
             if 'pi' in theta_str:
                 theta = theta_str.replace('*', '')
                 theta = theta.replace('pi', '')
                 theta = float(theta) * math.pi
             else:
-                theta = float(theta_str)
+                theta = Decimal(float(theta_str))
         return theta
     except:
         raise Exception(angle, "is not supported")
 
 def get_cos_sin(theta):
-    res_cos = math.cos(theta)
+    res_cos = str(Decimal(math.cos(theta)))
     if abs(res_cos) < 1e-15:
         res_cos = 0
-    res_sin = math.sin(theta)
+    res_sin = str(Decimal(math.sin(theta)))
     if abs(res_sin) < 1e-15:
         res_sin = 0
     return [res_cos, res_sin]
 
 def QASM2CNF(circuit : Circuit) -> CNF:
 
     cnf = CNF(circuit.n)
@@ -75,26 +78,32 @@
         elif gate == 'z':
             k = int(element[1]) - 1
             Z2CNF(cnf,k)
         elif gate == 'cx':
             j = int(element[1]) - 1
             k = int(element[2]) - 1
             CNOT2CNF(cnf,j,k)
+        elif gate == 'cz':
+            j = int(element[1]) - 1
+            k = int(element[2]) - 1
+            CZ2CNF(cnf,j,k)            
         elif gate == 's':
             k = int(element[1]) - 1
             S2CNF(cnf,k)
         elif gate == 'tdg':
             k = int(element[1]) - 1
-            Tdg2CNF(cnf,k)
+            w = str(Decimal(1/2).sqrt())
+            Tdg2CNF(cnf,k, w)
         elif gate == 'sdg':
             k = int(element[1]) - 1
             Sdg2CNF(cnf,k)
         elif gate == 't':
             k = int(element[1]) - 1
-            T2CNF(cnf,k)
+            w = str(Decimal(1/2).sqrt())
+            T2CNF(cnf, k, w)
         elif gate[0] == 'r':
             angle = get_angle(element[1])
             k = int(element[2]) - 1
             if gate == 'rx':
                 [res_cos, res_sin] = get_cos_sin(angle)
                 RX2CNF(cnf,k, res_cos, res_sin)
             elif gate == 'rz':
@@ -121,15 +130,15 @@
             T2CNF(cnf,qubitc2)
             T2CNF(cnf,qubitr)
             CNOT2CNF(cnf,qubitc1,qubitc2)
             H2CNF(cnf,qubitr)
             T2CNF(cnf,qubitc1)
             Tdg2CNF(cnf,qubitc2)
             CNOT2CNF(cnf,qubitc1,qubitc2)
-        elif gate == 'm':
-            cnf.rightProjectZXi(True, 0)
-        elif gate == 'mm':
-            cnf.rightProjectAllZero()
+        # elif gate == 'm':
+        #     cnf.rightProjectZXi(True, 0)
+        # elif gate == 'mm':
+        #     cnf.rightProjectAllZero()
         else:
             raise Exception(str(gate) + " undefined."+ str(element))
 
     return cnf
```

### Comparing `quokka_sharp-0.0.9/quokka_sharp/encoding/qasm_parser.py` & `quokka_sharp-1.0.0/quokka_sharp/encoding/qasm_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             if gate in HermiGates:
                 pass
             elif NHermitGates.get(gate) != None:
                 self.circ[idx][0] = NHermitGates[gate]
             else:
                 raise Exception("Gate "+ gate[0] +" dagger not supported.")
 
-    def merge(self, other):
+    def append(self, other):
         assert(self.translate_ccx == other.translate_ccx)
         self.circ.extend( other.circ )
         self.n = self.n
         self.tgate = self.tgate + other.tgate
 
 def get_num(s):
     num = ''
@@ -125,18 +125,14 @@
             qubit = get_num(line[1])
             circuit.add_single(gate, qubit)
 
         elif gate == 'rz(pi)' or gate == 'rz(-pi)' or gate == 'rz(1.0*pi)':
             qubit = get_num(line[1])
             circuit.add_single('z',qubit)
 
-        elif gate == 'rx(pi/2)' or gate == 'rx(-0.5*pi)' or gate == 'rx(0.5*pi)':
-            qubit = get_num(line[1])
-            circuit.add_single('y',qubit)
-
         elif gate == 's' or gate == "rz(0.5*pi)" or gate == "rz(pi/2)":
             qubit = get_num(line[1])
             circuit.add_single("s", qubit)
         
         elif gate == 'sdg' or gate == 'rz(-0.5*pi)' or gate == "rz(-pi/2)":
             qubit = get_num(line[1])
             circuit.add_single("sdg", qubit)
```

### Comparing `quokka_sharp-0.0.9/setup.py` & `quokka_sharp-1.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.9'
+VERSION = '1.0.0'
 DESCRIPTION = 'Quokka Sharp'
 LONG_DESCRIPTION = '''
                     Quokka Sharp for simulating and equivalence checking 
                     of quantum circuits based on weighted model counting.
                     You have to intall a weighted model counting tool first.
                     '''
 
@@ -21,10 +21,10 @@
             "Programming Language :: Python :: 3",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Operating System :: MacOS :: MacOS X",
             "Operating System :: Microsoft :: Windows"  
     ],
-    install_requires=["sympy>=1.12"],
+    install_requires=[],
     include_package_data=True
 )
```

