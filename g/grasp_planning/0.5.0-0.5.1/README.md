# Comparing `tmp/grasp_planning-0.5.0.tar.gz` & `tmp/grasp_planning-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grasp_planning-0.5.0.tar", max compression
+gzip compressed data, was "grasp_planning-0.5.1.tar", max compression
```

## Comparing `grasp_planning-0.5.0.tar` & `grasp_planning-0.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1676 2024-05-13 14:58:14.750519 grasp_planning-0.5.0/README.md
--rw-r--r--   0        0        0      123 2024-05-07 16:34:01.834623 grasp_planning-0.5.0/grasp_planning/__init__.py
--rw-r--r--   0        0        0     1335 2024-05-13 14:27:59.161140 grasp_planning-0.5.0/grasp_planning/constraints/__pycache__/collision_constraint.cpython-38.pyc
--rw-r--r--   0        0        0      799 2024-05-13 12:55:10.134092 grasp_planning-0.5.0/grasp_planning/constraints/__pycache__/constraint_template.cpython-38.pyc
--rw-r--r--   0        0        0      411 2024-05-08 08:43:17.328729 grasp_planning-0.5.0/grasp_planning/constraints/__pycache__/constraints.cpython-38.pyc
--rw-r--r--   0        0        0     1331 2024-05-13 12:55:10.134092 grasp_planning-0.5.0/grasp_planning/constraints/__pycache__/grasp_pos_constraint.cpython-38.pyc
--rw-r--r--   0        0        0     1528 2024-05-13 13:10:01.879282 grasp_planning-0.5.0/grasp_planning/constraints/__pycache__/grasp_rot_constraint.cpython-38.pyc
--rw-r--r--   0        0        0     1557 2024-05-09 15:57:33.554280 grasp_planning-0.5.0/grasp_planning/constraints/__pycache__/manipulation_constraint.cpython-38.pyc
--rw-r--r--   0        0        0      888 2024-05-13 14:27:19.884832 grasp_planning-0.5.0/grasp_planning/constraints/collision_constraint.py
--rw-r--r--   0        0        0      226 2024-05-13 12:54:20.897417 grasp_planning-0.5.0/grasp_planning/constraints/constraint_template.py
--rw-r--r--   0        0        0      252 2024-05-08 08:42:32.500427 grasp_planning-0.5.0/grasp_planning/constraints/constraints.py
--rw-r--r--   0        0        0     1057 2024-05-13 12:38:19.452309 grasp_planning-0.5.0/grasp_planning/constraints/grasp_pos_constraint.py
--rw-r--r--   0        0        0     1334 2024-05-13 13:10:00.135267 grasp_planning-0.5.0/grasp_planning/constraints/grasp_rot_constraint.py
--rw-r--r--   0        0        0     1059 2024-05-09 15:55:53.313730 grasp_planning-0.5.0/grasp_planning/constraints/manipulation_constraint.py
--rw-r--r--   0        0        0      219 2024-05-07 16:34:48.974947 grasp_planning-0.5.0/grasp_planning/cost/__pycache__/costs.cpython-38.pyc
--rw-r--r--   0        0        0     1344 2024-05-13 08:32:20.007123 grasp_planning-0.5.0/grasp_planning/cost/__pycache__/squared_acc_cost.cpython-38.pyc
--rw-r--r--   0        0        0       65 2024-05-07 16:34:01.834623 grasp_planning-0.5.0/grasp_planning/cost/costs.py
--rw-r--r--   0        0        0        0 2024-05-02 12:00:02.772313 grasp_planning-0.5.0/grasp_planning/cost/dist_to_home.py
--rw-r--r--   0        0        0     1439 2024-05-13 08:29:45.664854 grasp_planning-0.5.0/grasp_planning/cost/squared_acc_cost.py
--rw-r--r--   0        0        0     5689 2024-05-13 14:30:35.090364 grasp_planning-0.5.0/grasp_planning/solver/__pycache__/gomp_planner.cpython-38.pyc
--rw-r--r--   0        0        0     2203 2024-05-13 13:26:57.783698 grasp_planning-0.5.0/grasp_planning/solver/__pycache__/robot_model.cpython-38.pyc
--rw-r--r--   0        0        0     7077 2024-05-13 14:30:31.766338 grasp_planning-0.5.0/grasp_planning/solver/gomp_planner.py
--rw-r--r--   0        0        0     1875 2024-05-13 13:26:55.591679 grasp_planning-0.5.0/grasp_planning/solver/robot_model.py
--rw-r--r--   0        0        0      450 2024-05-13 14:54:58.605033 grasp_planning-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2318 1970-01-01 00:00:00.000000 grasp_planning-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1711 2024-05-14 12:21:39.645718 grasp_planning-0.5.1/README.md
+-rw-r--r--   0        0        0      123 2024-05-07 16:34:01.834623 grasp_planning-0.5.1/grasp_planning/__init__.py
+-rw-r--r--   0        0        0     1335 2024-05-13 14:27:59.161140 grasp_planning-0.5.1/grasp_planning/constraints/__pycache__/collision_constraint.cpython-38.pyc
+-rw-r--r--   0        0        0      799 2024-05-13 12:55:10.134092 grasp_planning-0.5.1/grasp_planning/constraints/__pycache__/constraint_template.cpython-38.pyc
+-rw-r--r--   0        0        0      411 2024-05-08 08:43:17.328729 grasp_planning-0.5.1/grasp_planning/constraints/__pycache__/constraints.cpython-38.pyc
+-rw-r--r--   0        0        0     1331 2024-05-13 12:55:10.134092 grasp_planning-0.5.1/grasp_planning/constraints/__pycache__/grasp_pos_constraint.cpython-38.pyc
+-rw-r--r--   0        0        0     1528 2024-05-13 13:10:01.879282 grasp_planning-0.5.1/grasp_planning/constraints/__pycache__/grasp_rot_constraint.cpython-38.pyc
+-rw-r--r--   0        0        0     1557 2024-05-09 15:57:33.554280 grasp_planning-0.5.1/grasp_planning/constraints/__pycache__/manipulation_constraint.cpython-38.pyc
+-rw-r--r--   0        0        0      888 2024-05-13 14:27:19.884832 grasp_planning-0.5.1/grasp_planning/constraints/collision_constraint.py
+-rw-r--r--   0        0        0      226 2024-05-13 12:54:20.897417 grasp_planning-0.5.1/grasp_planning/constraints/constraint_template.py
+-rw-r--r--   0        0        0      252 2024-05-08 08:42:32.500427 grasp_planning-0.5.1/grasp_planning/constraints/constraints.py
+-rw-r--r--   0        0        0     1057 2024-05-13 12:38:19.452309 grasp_planning-0.5.1/grasp_planning/constraints/grasp_pos_constraint.py
+-rw-r--r--   0        0        0     1334 2024-05-13 13:10:00.135267 grasp_planning-0.5.1/grasp_planning/constraints/grasp_rot_constraint.py
+-rw-r--r--   0        0        0     1059 2024-05-09 15:55:53.313730 grasp_planning-0.5.1/grasp_planning/constraints/manipulation_constraint.py
+-rw-r--r--   0        0        0      219 2024-05-07 16:34:48.974947 grasp_planning-0.5.1/grasp_planning/cost/__pycache__/costs.cpython-38.pyc
+-rw-r--r--   0        0        0     1344 2024-05-13 08:32:20.007123 grasp_planning-0.5.1/grasp_planning/cost/__pycache__/squared_acc_cost.cpython-38.pyc
+-rw-r--r--   0        0        0       65 2024-05-07 16:34:01.834623 grasp_planning-0.5.1/grasp_planning/cost/costs.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:00:02.772313 grasp_planning-0.5.1/grasp_planning/cost/dist_to_home.py
+-rw-r--r--   0        0        0     1439 2024-05-13 08:29:45.664854 grasp_planning-0.5.1/grasp_planning/cost/squared_acc_cost.py
+-rw-r--r--   0        0        0     5969 2024-05-14 13:19:55.752368 grasp_planning-0.5.1/grasp_planning/solver/__pycache__/gomp_planner.cpython-38.pyc
+-rw-r--r--   0        0        0     2203 2024-05-13 13:26:57.783698 grasp_planning-0.5.1/grasp_planning/solver/__pycache__/robot_model.cpython-38.pyc
+-rw-r--r--   0        0        0     7650 2024-05-14 13:19:53.464393 grasp_planning-0.5.1/grasp_planning/solver/gomp_planner.py
+-rw-r--r--   0        0        0     1875 2024-05-13 13:26:55.591679 grasp_planning-0.5.1/grasp_planning/solver/robot_model.py
+-rw-r--r--   0        0        0      450 2024-05-14 13:21:33.811293 grasp_planning-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2353 1970-01-01 00:00:00.000000 grasp_planning-0.5.1/PKG-INFO
```

### Comparing `grasp_planning-0.5.0/README.md` & `grasp_planning-0.5.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -42,7 +42,10 @@
 start = time.time()
 planner.update_constraints_params(T_W_Obj, T_W_Obst)
 x, solver_flag = planner.solve()
 end = time.time()
 print(f"Computational time: {end-start}" )
 print(f"Solver status: {solver_flag}" )
 ```
+
+## ToDo
+- [ ] removing constraints
```

### Comparing `grasp_planning-0.5.0/grasp_planning/constraints/__pycache__/collision_constraint.cpython-38.pyc` & `grasp_planning-0.5.1/grasp_planning/constraints/__pycache__/collision_constraint.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.0/grasp_planning/constraints/__pycache__/constraint_template.cpython-38.pyc` & `grasp_planning-0.5.1/grasp_planning/constraints/__pycache__/constraint_template.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.0/grasp_planning/constraints/__pycache__/grasp_pos_constraint.cpython-38.pyc` & `grasp_planning-0.5.1/grasp_planning/constraints/__pycache__/grasp_pos_constraint.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.0/grasp_planning/constraints/__pycache__/grasp_rot_constraint.cpython-38.pyc` & `grasp_planning-0.5.1/grasp_planning/constraints/__pycache__/grasp_rot_constraint.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.0/grasp_planning/constraints/__pycache__/manipulation_constraint.cpython-38.pyc` & `grasp_planning-0.5.1/grasp_planning/constraints/__pycache__/manipulation_constraint.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.0/grasp_planning/constraints/collision_constraint.py` & `grasp_planning-0.5.1/grasp_planning/constraints/collision_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.0/grasp_planning/constraints/grasp_pos_constraint.py` & `grasp_planning-0.5.1/grasp_planning/constraints/grasp_pos_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.0/grasp_planning/constraints/grasp_rot_constraint.py` & `grasp_planning-0.5.1/grasp_planning/constraints/grasp_rot_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.0/grasp_planning/constraints/manipulation_constraint.py` & `grasp_planning-0.5.1/grasp_planning/constraints/manipulation_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.0/grasp_planning/cost/__pycache__/squared_acc_cost.cpython-38.pyc` & `grasp_planning-0.5.1/grasp_planning/cost/__pycache__/squared_acc_cost.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.0/grasp_planning/cost/squared_acc_cost.py` & `grasp_planning-0.5.1/grasp_planning/cost/squared_acc_cost.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.0/grasp_planning/solver/__pycache__/gomp_planner.cpython-38.pyc` & `grasp_planning-0.5.1/grasp_planning/solver/__pycache__/gomp_planner.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 13 14:30:31 2024 UTC, .py size: 7077 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,356 +1,374 @@
-00000000: 550d 0d0a 0000 0000 0724 4266 a51b 0000  U........$Bf....
+00000000: 550d 0d0a 0000 0000 f964 4366 e21d 0000  U........dCf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c04 5a05 6400 6402 6c06 6d07 5a08  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c0b 6d0c 5a0c 0100 6400 6405 6c0d  d.l.m.Z...d.d.l.
 00000070: 5400 4700 6406 6407 8400 6407 8302 5a0e  T.G.d.d...d...Z.
 00000080: 6401 5300 2908 e900 0000 004e 2901 da08  d.S.)......N)...
 00000090: 526f 7461 7469 6f6e 2901 da13 526f 626f  Rotation)...Robo
 000000a0: 744b 696e 656d 6174 6963 4d6f 6465 6c29  tKinematicModel)
 000000b0: 01da 0e53 7175 6172 6564 4163 6343 6f73  ...SquaredAccCos
 000000c0: 7429 01da 012a 6300 0000 0000 0000 0000  t)...*c.........
 000000d0: 0000 0000 0000 0004 0000 0040 0000 0073  ...........@...s
-000000e0: a800 0000 6500 5a01 6400 5a02 6503 6a04  ....e.Z.d.Z.e.j.
+000000e0: aa00 0000 6500 5a01 6400 5a02 6503 6a04  ....e.Z.d.Z.e.j.
 000000f0: 6401 1b00 6402 6403 6603 6404 6405 9c01  d...d.d.f.d.d...
 00000100: 6406 6407 8405 5a05 6429 6506 6404 6409  d.d...Z.d)e.d.d.
 00000110: 9c02 640a 640b 8405 5a07 6503 6a08 6404  ..d.d...Z.e.j.d.
 00000120: 640c 9c02 640d 640e 8404 5a09 640f 6410  d...d.d...Z.d.d.
 00000130: 8400 5a0a 6411 6412 8400 5a0b 642a 6413  ..Z.d.d...Z.d*d.
 00000140: 6414 8401 5a0c 642b 6416 6417 8401 5a0d  d...Z.d+d.d...Z.
 00000150: 6418 6419 8400 5a0e 642c 641b 641c 8401  d.d...Z.d,d.d...
 00000160: 5a0f 642d 641e 641f 8401 5a10 642e 6420  Z.d-d.d...Z.d.d 
 00000170: 6421 8401 5a11 642f 6425 6426 8401 5a12  d!..Z.d/d%d&..Z.
-00000180: 6427 6428 8400 5a13 6404 5300 2930 da04  d'd(..Z.d.S.)0..
-00000190: 474f 4d50 e904 0000 00da 0577 6f72 6c64  GOMP.......world
-000001a0: 5a0a 746f 6f6c 5f66 7261 6d65 4e29 01da  Z.tool_frameN)..
-000001b0: 0672 6574 7572 6e63 0600 0000 0000 0000  .returnc........
-000001c0: 0000 0000 0600 0000 0500 0000 4300 0000  ............C...
-000001d0: 73aa 0000 0064 007c 005f 0064 007c 005f  s....d.|._.d.|._
-000001e0: 0174 026a 0364 0174 0464 028d 027c 005f  .t.j.d.t.d...|._
-000001f0: 0574 067c 027c 047c 0583 037c 005f 077c  .t.|.|.|...|._.|
-00000200: 006a 076a 087c 005f 0864 037c 005f 097c  .j.j.|._.d.|._.|
-00000210: 006a 087c 005f 0a7c 017c 005f 0b7c 037c  .j.|._.|.|._.|.|
-00000220: 005f 0c74 0d6a 0ea0 0f64 047c 006a 0a7c  ._.t.j...d.|.j.|
-00000230: 006a 0ba1 037c 005f 1064 007c 005f 1164  .j...|._.d.|._.d
-00000240: 007c 005f 1264 055c 027c 005f 137c 005f  .|._.d.\.|._.|._
-00000250: 1467 007c 005f 1574 0d6a 0ea0 0f64 0664  .g.|._.t.j...d.d
-00000260: 0164 01a1 037c 005f 1674 0d6a 0ea0 0f64  .d...|._.t.j...d
-00000270: 0764 0164 01a1 037c 005f 1764 0053 0029  .d.d...|._.d.S.)
-00000280: 084e 7207 0000 00a9 01da 0564 7479 7065  .Nr........dtype
-00000290: e906 0000 00da 0178 2902 4e4e 5a0b 7061  .......x).NNZ.pa
-000002a0: 7261 6d5f 6772 6173 705a 0a70 6172 616d  ram_graspZ.param
-000002b0: 5f6f 6273 7429 18da 0954 5f57 5f47 7261  _obst)...T_W_Gra
-000002c0: 7370 da07 545f 575f 4f62 6ada 026e 70da  sp..T_W_Obj..np.
-000002d0: 0365 7965 da05 666c 6f61 74da 0b54 5f4f  .eye..float..T_O
-000002e0: 626a 5f47 7261 7370 7203 0000 00da 0c5f  bj_Graspr......_
-000002f0: 726f 626f 745f 6d6f 6465 6cda 066e 5f64  robot_model..n_d
-00000300: 6f66 735a 166d 616e 6970 756c 6174 696f  ofsZ.manipulatio
-00000310: 6e5f 6672 616d 655f 6469 6dda 0578 5f64  n_frame_dim..x_d
-00000320: 696d da0b 6e5f 7761 7970 6f69 6e74 73da  im..n_waypoints.
-00000330: 0574 6865 7461 da02 6361 5a02 5358 5a03  .theta..caZ.SXZ.
-00000340: 7379 6d72 0d00 0000 da06 785f 696e 6974  symr......x_init
-00000350: 5a0a 5f6f 626a 6563 7469 7665 da0e 6c5f  Z._objective..l_
-00000360: 6a6f 696e 745f 6c69 6d69 7473 da0e 755f  joint_limits..u_
-00000370: 6a6f 696e 745f 6c69 6d69 7473 da06 675f  joint_limits..g_
-00000380: 6c69 7374 da0e 7061 7261 6d5f 6772 6173  list..param_gras
-00000390: 705f 6361 da0d 7061 7261 6d5f 6f62 7374  p_ca..param_obst
-000003a0: 5f63 6129 06da 0473 656c 6672 1700 0000  _ca)...selfr....
-000003b0: 5a04 7572 6466 7218 0000 005a 0972 6f6f  Z.urdfr....Z.roo
-000003c0: 745f 6c69 6e6b 5a08 656e 645f 6c69 6e6b  t_linkZ.end_link
-000003d0: a900 7221 0000 00fa 482f 686f 6d65 2f74  ..r!....H/home/t
-000003e0: 6f6d 6173 2f44 6573 6b74 6f70 2f67 7261  omas/Desktop/gra
-000003f0: 7370 5f70 6c61 6e6e 696e 672f 6772 6173  sp_planning/gras
-00000400: 705f 706c 616e 6e69 6e67 2f73 6f6c 7665  p_planning/solve
-00000410: 722f 676f 6d70 5f70 6c61 6e6e 6572 2e70  r/gomp_planner.p
-00000420: 79da 085f 5f69 6e69 745f 5f0a 0000 0073  y..__init__....s
-00000430: 2000 0000 0002 0601 0601 1003 0e01 0a01   ...............
-00000440: 0601 0801 0601 0603 1601 0602 0601 0c01  ................
-00000450: 0602 1201 7a0d 474f 4d50 2e5f 5f69 6e69  ....z.GOMP.__ini
-00000460: 745f 5f54 2902 7218 0000 0072 0900 0000  t__T).r....r....
-00000470: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
-00000480: 0005 0000 0043 0000 0073 9600 0000 7400  .....C...s....t.
-00000490: 6a01 6401 7402 6402 8d02 7c00 5f03 7c02  j.d.t.d...|._.|.
-000004a0: 7244 7404 6a05 6403 6404 6405 7c01 6703  rDt.j.d.d.d.|.g.
-000004b0: 6406 6407 8d03 a006 a100 7d03 7400 a007  d.d.......}.t...
-000004c0: 7400 a008 7c01 a101 6408 a102 7c00 5f09  t...|...d...|._.
-000004d0: 6e2a 7404 6a05 6403 7400 6a0a 6405 7c01  n*t.j.d.t.j.d.|.
-000004e0: 6703 6409 6407 8d03 a006 a100 7d03 7400  g.d.d.......}.t.
-000004f0: a007 7c01 6408 a102 7c00 5f09 7c03 7c00  ..|.d...|._.|.|.
-00000500: 6a03 640a 640b 8502 640a 640b 8502 6602  j.d.d...d.d...f.
-00000510: 3c00 7c00 6a0b 7c00 6a03 1000 7c00 5f0c  <.|.j.|.j...|._.
-00000520: 640a 5300 290c 7a48 0a20 2020 2020 2020  d.S.).zH.       
-00000530: 204f 626a 6563 7420 6861 7320 746f 2068   Object has to h
-00000540: 6176 6520 7a2d 6178 6973 2061 6c69 676e  ave z-axis align
-00000550: 6564 2077 6974 6820 7468 6520 776f 726c  ed with the worl
-00000560: 6420 6672 616d 650a 2020 2020 2020 2020  d frame.        
-00000570: 7207 0000 0072 0a00 0000 da03 7879 7ae9  r....r......xyz.
-00000580: b400 0000 7201 0000 0054 2901 da07 6465  ....r....T)...de
-00000590: 6772 6565 73e9 0200 0000 464e e903 0000  grees.....FN....
-000005a0: 0029 0d72 1000 0000 7211 0000 0072 1200  .).r....r....r..
-000005b0: 0000 7213 0000 00da 0152 5a0a 6672 6f6d  ..r......RZ.from
-000005c0: 5f65 756c 6572 5a09 6173 5f6d 6174 7269  _eulerZ.as_matri
-000005d0: 78da 0572 6f75 6e64 5a07 6465 6732 7261  x..roundZ.deg2ra
-000005e0: 6472 1800 0000 da02 7069 720f 0000 0072  dr......pir....r
-000005f0: 0e00 0000 2904 7220 0000 0072 1800 0000  ....).r ...r....
-00000600: 7226 0000 005a 0b52 5f4f 626a 5f47 7261  r&...Z.R_Obj_Gra
-00000610: 7370 7221 0000 0072 2100 0000 7222 0000  spr!...r!...r"..
-00000620: 00da 1075 7064 6174 655f 6772 6173 705f  ...update_grasp_
-00000630: 444f 4625 0000 0073 1000 0000 0004 1001  DOF%...s........
-00000640: 0401 1a01 1602 1c01 0e01 1601 7a15 474f  ............z.GO
-00000650: 4d50 2e75 7064 6174 655f 6772 6173 705f  MP.update_grasp_
-00000660: 444f 4629 0272 0f00 0000 7209 0000 0063  DOF).r....r....c
-00000670: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000680: 0200 0000 4300 0000 730a 0000 007c 017c  ....C...s....|.|
-00000690: 005f 0064 0153 0029 027a 2f0a 2020 2020  ._.d.S.).z/.    
-000006a0: 2020 2020 5570 6461 7465 206f 626a 6563      Update objec
-000006b0: 7420 616e 6420 6772 6173 7020 706f 7365  t and grasp pose
-000006c0: 730a 2020 2020 2020 2020 4e29 0172 0f00  s.        N).r..
-000006d0: 0000 2902 7220 0000 0072 0f00 0000 7221  ..).r ...r....r!
-000006e0: 0000 0072 2100 0000 7222 0000 00da 1275  ...r!...r".....u
-000006f0: 7064 6174 655f 6f62 6a65 6374 5f70 6f73  pdate_object_pos
-00000700: 6533 0000 0073 0200 0000 0004 7a17 474f  e3...s......z.GO
-00000710: 4d50 2e75 7064 6174 655f 6f62 6a65 6374  MP.update_object
-00000720: 5f70 6f73 6563 0100 0000 0000 0000 0000  _posec..........
-00000730: 0000 0200 0000 0600 0000 4300 0000 7354  ..........C...sT
-00000740: 0000 0074 006a 01a0 027c 006a 0364 0164  ...t.j...|.j.d.d
-00000750: 0285 0264 0164 0285 0266 0219 00a1 01a0  ...d.d...f......
-00000760: 0464 03a1 017d 0174 05a0 067c 006a 0364  .d...}.t...|.j.d
-00000770: 0164 0285 0264 0266 0219 0064 0164 0185  .d...d.f...d.d..
-00000780: 0264 0166 0219 007c 0166 02a1 017c 005f  .d.f...|.f...|._
-00000790: 077c 006a 0753 0029 047a 360a 2020 2020  .|.j.S.).z6.    
-000007a0: 2020 2020 436f 6e76 6572 7420 545f 575f      Convert T_W_
-000007b0: 4772 6173 7020 696e 746f 205b 782c 792c  Grasp into [x,y,
-000007c0: 7a2c 722c 702c 795d 0a20 2020 2020 2020  z,r,p,y].       
-000007d0: 204e 7228 0000 0072 2400 0000 2908 da02   Nr(...r$...)...
-000007e0: 7363 7202 0000 005a 0b66 726f 6d5f 6d61  scr....Z.from_ma
-000007f0: 7472 6978 720e 0000 005a 0861 735f 6575  trixr....Z.as_eu
-00000800: 6c65 7272 1000 0000 5a06 7673 7461 636b  lerr....Z.vstack
-00000810: 5a0d 545f 575f 4772 6173 705f 7270 7929  Z.T_W_Grasp_rpy)
-00000820: 0272 2000 0000 5a0d 525f 575f 4772 6173  .r ...Z.R_W_Gras
-00000830: 705f 7270 7972 2100 0000 7221 0000 0072  p_rpyr!...r!...r
-00000840: 2200 0000 da0a 5f67 7261 7370 3272 7079  "....._grasp2rpy
-00000850: 3900 0000 7306 0000 0000 0424 012a 017a  9...s......$.*.z
-00000860: 0f47 4f4d 502e 5f67 7261 7370 3272 7079  .GOMP._grasp2rpy
-00000870: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000880: 0004 0000 0043 0000 0073 1400 0000 7400  .....C...s....t.
-00000890: a001 7c01 7c00 6a02 a102 7c00 5f03 6400  ..|.|.j...|._.d.
-000008a0: 5300 a901 4e29 0472 1000 0000 5a04 7469  S...N).r....Z.ti
-000008b0: 6c65 7217 0000 0072 1a00 0000 2902 7220  ler....r....).r 
-000008c0: 0000 00da 0171 7221 0000 0072 2100 0000  .....qr!...r!...
-000008d0: 7222 0000 00da 0e73 6574 5f69 6e69 745f  r".....set_init_
-000008e0: 6775 6573 7342 0000 0073 0200 0000 0001  guessB...s......
-000008f0: 7a13 474f 4d50 2e73 6574 5f69 6e69 745f  z.GOMP.set_init_
-00000900: 6775 6573 7363 0300 0000 0000 0000 0000  guessc..........
-00000910: 0000 0500 0000 0500 0000 4300 0000 7302  ..........C...s.
-00000920: 0100 007c 006a 0064 006b 0873 147c 006a  ...|.j.d.k.s.|.j
-00000930: 0164 006b 0872 ca74 02a0 037c 006a 047c  .d.k.r.t...|.j.|
-00000940: 006a 0566 0264 01a1 027c 005f 0074 02a0  .j.f.d...|._.t..
-00000950: 037c 006a 047c 006a 0566 0264 02a1 027c  .|.j.|.j.f.d...|
-00000960: 005f 017c 006a 06a0 07a1 007d 0374 087c  ._.|.j.....}.t.|
-00000970: 006a 0583 0144 005d 747d 047c 0364 0064  .j...D.]t}.|.d.d
-00000980: 0085 0264 0366 0219 007c 006a 0064 007c  ...d.f...|.j.d.|
-00000990: 006a 0985 027c 0466 023c 007c 0364 0064  .j...|.f.<.|.d.d
-000009a0: 0085 0264 0466 0219 007c 006a 0164 007c  ...d.f...|.j.d.|
-000009b0: 006a 0985 027c 0466 023c 0064 0574 026a  .j...|.f.<.d.t.j
-000009c0: 0a14 007c 006a 0064 0664 0085 027c 0466  ...|.j.d.d...|.f
-000009d0: 023c 0064 0774 026a 0a14 007c 006a 0164  .<.d.t.j...|.j.d
-000009e0: 0664 0085 027c 0466 023c 0071 547c 017c  .d...|.f.<.qT|.|
-000009f0: 006a 0064 0064 0085 0264 0366 023c 007c  .j.d.d...d.f.<.|
-00000a00: 017c 006a 0164 0064 0085 0264 0366 023c  .|.j.d.d...d.f.<
-00000a10: 007c 0264 006b 0372 fe74 0b64 0883 0101  .|.d.k.r.t.d....
-00000a20: 0064 0053 0029 094e 6700 0000 0000 0059  .d.S.).Ng......Y
-00000a30: c067 0000 0000 0000 5940 7201 0000 00e9  .g......Y@r.....
-00000a40: 0100 0000 e9fe ffff ffe9 fdff ffff 7227  ..............r'
-00000a50: 0000 007a 2c46 696e 616c 2062 6f75 6e64  ...z,Final bound
-00000a60: 6172 7920 636f 6e64 6974 696f 6e20 6973  ary condition is
-00000a70: 206e 6f74 2069 6d70 6c65 6d65 6e74 6564   not implemented
-00000a80: 2e29 0c72 1b00 0000 721c 0000 0072 1000  .).r....r....r..
-00000a90: 0000 5a04 6675 6c6c 7216 0000 0072 1700  ..Z.fullr....r..
-00000aa0: 0000 7214 0000 005a 1467 6574 5f6a 6f69  ..r....Z.get_joi
-00000ab0: 6e74 5f70 6f73 5f6c 696d 6974 73da 0572  nt_pos_limits..r
-00000ac0: 616e 6765 7215 0000 0072 2b00 0000 da05  anger....r+.....
-00000ad0: 7072 696e 7429 0572 2000 0000 da07 715f  print).r .....q_
-00000ae0: 7374 6172 745a 0571 5f65 6e64 5a0c 6a6f  startZ.q_endZ.jo
-00000af0: 696e 745f 6c69 6d69 7473 da01 7472 2100  int_limits..tr!.
-00000b00: 0000 7221 0000 0072 2200 0000 da17 7365  ..r!...r".....se
-00000b10: 745f 626f 756e 6461 7279 5f63 6f6e 6469  t_boundary_condi
-00000b20: 7469 6f6e 7345 0000 0073 1a00 0000 0001  tionsE...s......
-00000b30: 1402 1601 1603 0a01 0e01 2001 2001 1801  .......... . ...
-00000b40: 1a04 1201 1202 0801 7a1c 474f 4d50 2e73  ........z.GOMP.s
-00000b50: 6574 5f62 6f75 6e64 6172 795f 636f 6e64  et_boundary_cond
-00000b60: 6974 696f 6e73 4663 0200 0000 0000 0000  itionsFc........
-00000b70: 0000 0000 0c00 0000 0900 0000 4300 0000  ............C...
-00000b80: 73de 0000 007c 006a 00a0 0164 01a1 017d  s....|.j...d...}
-00000b90: 0274 027c 006a 037c 006a 0464 0264 038d  .t.|.j.|.j.d.d..
-00000ba0: 037d 037c 03a0 057c 02a1 017d 0474 06a0  .}.|...|...}.t..
-00000bb0: 07a1 0074 06a0 07a1 0074 06a0 07a1 0003  ...t.....t......
-00000bc0: 0002 007d 057c 005f 087c 005f 097c 006a  ...}.|._.|._.|.j
-00000bd0: 0a44 005d 3e7d 067c 06a0 0ba1 005c 037d  .D.]>}.|.....\.}
-00000be0: 077d 087d 0974 06a0 077c 057c 07a1 027d  .}.}.t...|.|...}
-00000bf0: 0574 06a0 077c 006a 087c 08a1 027c 005f  .t...|.j.|...|._
-00000c00: 0874 06a0 077c 006a 097c 09a1 027c 005f  .t...|.j.|...|._
-00000c10: 0971 4e69 007d 0a64 047c 0a64 053c 007c  .qNi.}.d.|.d.<.|
-00000c20: 0173 ae64 067c 0a64 073c 0064 067c 0a64  .s.d.|.d.<.d.|.d
-00000c30: 083c 0074 06a0 077c 006a 0c7c 006a 0da1  .<.t...|.j.|.j..
-00000c40: 027d 0b74 06a0 0e64 0964 0a7c 027c 047c  .}.t...d.d.|.|.|
-00000c50: 057c 0b64 0b9c 047c 0aa1 047c 005f 0f64  .|.d...|...|._.d
-00000c60: 0053 0029 0c4e a902 e9ff ffff ff72 3300  .S.).N.......r3.
-00000c70: 0000 5429 015a 0b6d 616e 6970 5f66 7261  ..T).Z.manip_fra
-00000c80: 6d65 67fc a9f1 d24d 6250 3f7a 1469 706f  meg....MbP?z.ipo
-00000c90: 7074 2e61 6363 6570 7461 626c 655f 746f  pt.acceptable_to
-00000ca0: 6c72 0100 0000 7a11 6970 6f70 742e 7072  lr....z.ipopt.pr
-00000cb0: 696e 745f 6c65 7665 6c5a 0a70 7269 6e74  int_levelZ.print
-00000cc0: 5f74 696d 65da 0673 6f6c 7665 725a 0569  _time..solverZ.i
-00000cd0: 706f 7074 2904 720d 0000 00da 0166 da01  popt).r......f..
-00000ce0: 67da 0170 2910 720d 0000 00da 0772 6573  g..p).r......res
-00000cf0: 6861 7065 7204 0000 0072 1700 0000 7216  haper....r....r.
-00000d00: 0000 005a 0965 7661 6c5f 636f 7374 7219  ...Z.eval_costr.
-00000d10: 0000 00da 0776 6572 7463 6174 da04 675f  .....vertcat..g_
-00000d20: 6c62 da04 675f 7562 721d 0000 005a 0e67  lb..g_ubr....Z.g
-00000d30: 6574 5f63 6f6e 7374 7261 696e 7472 1e00  et_constraintr..
-00000d40: 0000 721f 0000 005a 066e 6c70 736f 6c72  ..r....Z.nlpsolr
-00000d50: 3d00 0000 290c 7220 0000 00da 0776 6572  =...).r .....ver
-00000d60: 626f 7365 5a0c 785f 6361 5f66 6c61 7474  boseZ.x_ca_flatt
-00000d70: 656e 5a04 636f 7374 5a09 6f62 6a65 6374  enZ.costZ.object
-00000d80: 6976 6572 3f00 0000 5a06 675f 7465 726d  iver?...Z.g_term
-00000d90: da02 6774 7243 0000 0072 4400 0000 da07  ..gtrC...rD.....
-00000da0: 6f70 7469 6f6e 735a 0f70 6172 616d 735f  optionsZ.params_
-00000db0: 6f70 7469 6d5f 6361 7221 0000 0072 2100  optim_car!...r!.
-00000dc0: 0000 7222 0000 00da 0d73 6574 7570 5f70  ..r".....setup_p
-00000dd0: 726f 626c 656d 5d00 0000 7320 0000 0000  roblem]...s ....
-00000de0: 040c 0512 010a 0220 010a 010e 010c 0110  ....... ........
-00000df0: 0112 0404 0108 0104 0108 0108 0210 017a  ...............z
-00000e00: 1247 4f4d 502e 7365 7475 705f 7072 6f62  .GOMP.setup_prob
-00000e10: 6c65 6d63 0100 0000 0000 0000 0000 0000  lemc............
-00000e20: 0400 0000 0900 0000 4300 0000 735e 0000  ........C...s^..
-00000e30: 007c 006a 007c 006a 017c 006a 027c 006a  .|.j.|.j.|.j.|.j
-00000e40: 037c 006a 046a 0564 0164 0264 038d 027c  .|.j.j.d.d.d...|
-00000e50: 006a 066a 0564 0164 0264 038d 027c 006a  .j.j.d.d.d...|.j
-00000e60: 0764 048d 067d 017c 006a 00a0 08a1 0064  .d...}.|.j.....d
-00000e70: 0519 007d 027c 006a 00a0 08a1 0064 0619  ...}.|.j.....d..
-00000e80: 007d 037c 0164 0719 007c 0266 0253 0029  .}.|.d...|.f.S.)
-00000e90: 084e 723b 0000 00da 0146 2901 da05 6f72  .Nr;.....F)...or
-00000ea0: 6465 7229 065a 0278 305a 036c 6267 5a03  der).Z.x0Z.lbgZ.
-00000eb0: 7562 675a 036c 6278 5a03 7562 7872 4000  ubgZ.lbxZ.ubxr@.
-00000ec0: 0000 5a07 7375 6363 6573 735a 0d72 6574  ..Z.successZ.ret
-00000ed0: 7572 6e5f 7374 6174 7573 720d 0000 0029  urn_statusr....)
-00000ee0: 0972 3d00 0000 721a 0000 0072 4300 0000  .r=...r....rC...
-00000ef0: 7244 0000 0072 1b00 0000 7241 0000 0072  rD...r....rA...r
-00000f00: 1c00 0000 da10 7061 7261 6d73 5f6f 7074  ......params_opt
-00000f10: 696d 5f6e 756d 5a05 7374 6174 7329 0472  im_numZ.stats).r
-00000f20: 2000 0000 da06 7265 7375 6c74 5a0c 7375   .....resultZ.su
-00000f30: 6363 6573 735f 666c 6167 5a0b 7375 6363  ccess_flagZ.succ
-00000f40: 6573 735f 6d73 6772 2100 0000 7221 0000  ess_msgr!...r!..
-00000f50: 0072 2200 0000 da05 736f 6c76 657d 0000  .r".....solve}..
-00000f60: 0073 1400 0000 0001 0801 0401 0401 0e01  .s..............
-00000f70: 0e01 04fb 0606 0e01 0e01 7a0a 474f 4d50  ..........z.GOMP
-00000f80: 2e73 6f6c 7665 e700 0000 0000 0000 0063  .solve.........c
-00000f90: 0300 0000 0000 0000 0000 0000 0300 0000  ................
-00000fa0: 0800 0000 4300 0000 7322 0000 007c 006a  ....C...s"...|.j
-00000fb0: 00a0 0174 027c 006a 037c 006a 047c 017c  ...t.|.j.|.j.|.|
-00000fc0: 006a 057c 0283 05a1 0101 0064 0053 0072  .j.|.......d.S.r
-00000fd0: 3000 0000 2906 721d 0000 00da 0661 7070  0...).r......app
-00000fe0: 656e 645a 1247 7261 7370 506f 7343 6f6e  endZ.GraspPosCon
-00000ff0: 7374 7261 696e 7472 1400 0000 720d 0000  straintr....r...
-00001000: 0072 1e00 0000 a903 7220 0000 00da 0b77  .r......r .....w
-00001010: 6179 706f 696e 745f 4944 da09 746f 6c65  aypoint_ID..tole
-00001020: 7261 6e63 6572 2100 0000 7221 0000 0072  rancer!...r!...r
-00001030: 2200 0000 da19 5f61 6464 5f67 7261 7370  "....._add_grasp
-00001040: 5f70 6f73 5f63 6f6e 7374 7261 696e 7488  _pos_constraint.
-00001050: 0000 0073 0c00 0000 0001 0c01 0401 0201  ...s............
-00001060: 0401 02fc 7a1e 474f 4d50 2e5f 6164 645f  ....z.GOMP._add_
-00001070: 6772 6173 705f 706f 735f 636f 6e73 7472  grasp_pos_constr
-00001080: 6169 6e74 e79a 9999 9999 99b9 3f63 0300  aint........?c..
-00001090: 0000 0000 0000 0000 0000 0300 0000 0900  ................
-000010a0: 0000 4300 0000 7326 0000 007c 006a 00a0  ..C...s&...|.j..
-000010b0: 0174 027c 006a 037c 006a 047c 017c 006a  .t.|.j.|.j.|.|.j
-000010c0: 057c 006a 067c 0283 06a1 0101 0064 0053  .|.j.|.......d.S
-000010d0: 0072 3000 0000 2907 721d 0000 0072 4f00  .r0...).r....rO.
-000010e0: 0000 5a12 4772 6173 7052 6f74 436f 6e73  ..Z.GraspRotCons
-000010f0: 7472 6169 6e74 7214 0000 0072 0d00 0000  traintr....r....
-00001100: 721e 0000 0072 1800 0000 7250 0000 0072  r....r....rP...r
-00001110: 2100 0000 7221 0000 0072 2200 0000 da19  !...r!...r".....
-00001120: 5f61 6464 5f67 7261 7370 5f72 6f74 5f63  _add_grasp_rot_c
-00001130: 6f6e 7374 7261 696e 748f 0000 0073 0e00  onstraint....s..
-00001140: 0000 0001 0c01 0401 0201 0401 0401 02fb  ................
-00001150: 7a1e 474f 4d50 2e5f 6164 645f 6772 6173  z.GOMP._add_gras
-00001160: 705f 726f 745f 636f 6e73 7472 6169 6e74  p_rot_constraint
-00001170: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-00001180: 0004 0000 0043 0000 0073 1c00 0000 7c00  .....C...s....|.
-00001190: a000 7c01 7c02 a102 0100 7c00 a001 7c01  ..|.|.....|...|.
-000011a0: 7c02 a102 0100 6400 5300 7230 0000 0029  |.....d.S.r0...)
-000011b0: 0272 5300 0000 7255 0000 0072 5000 0000  .rS...rU...rP...
-000011c0: 7221 0000 0072 2100 0000 7222 0000 00da  r!...r!...r"....
-000011d0: 1461 6464 5f67 7261 7370 5f63 6f6e 7374  .add_grasp_const
-000011e0: 7261 696e 7497 0000 0073 0400 0000 0001  raint....s......
-000011f0: 0c01 7a19 474f 4d50 2e61 6464 5f67 7261  ..z.GOMP.add_gra
-00001200: 7370 5f63 6f6e 7374 7261 696e 74e7 0000  sp_constraint...
-00001210: 0000 0000 e03f e79a 9999 9999 99c9 3fe7  .....?........?.
-00001220: 7b14 ae47 e17a 843f 6306 0000 0000 0000  {..G.z.?c.......
-00001230: 0000 0000 0006 0000 000c 0000 0043 0000  .............C..
-00001240: 0073 2a00 0000 7c00 6a00 a001 7402 7c00  .s*...|.j...t.|.
-00001250: 6a03 7c00 6a04 7c01 7c00 6a05 7c02 7c03  j.|.j.|.|.j.|.|.
-00001260: 7c04 7c05 6401 8d08 a101 0100 6400 5300  |.|.d.......d.S.
-00001270: 2902 4e29 085a 0572 6f62 6f74 5a04 715f  ).N).Z.robotZ.q_
-00001280: 6361 7251 0000 0072 1f00 0000 5a09 6c69  carQ...r....Z.li
-00001290: 6e6b 5f6e 616d 65da 0672 5f6c 696e 6bda  nk_name..r_link.
-000012a0: 0672 5f6f 6273 7472 5200 0000 2906 721d  .r_obstrR...).r.
-000012b0: 0000 0072 4f00 0000 5a13 436f 6c6c 6973  ...rO...Z.Collis
-000012c0: 696f 6e43 6f6e 7374 7261 696e 7472 1400  ionConstraintr..
-000012d0: 0000 720d 0000 0072 1f00 0000 2906 7220  ..r....r....).r 
-000012e0: 0000 0072 5100 0000 da0a 6368 696c 645f  ...rQ.....child_
-000012f0: 6c69 6e6b 725a 0000 0072 5b00 0000 7252  linkrZ...r[...rR
-00001300: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
-00001310: 0000 da18 6164 645f 636f 6c6c 6973 696f  ....add_collisio
-00001320: 6e5f 636f 6e73 7472 6169 6e74 9b00 0000  n_constraint....
-00001330: 7312 0000 0000 010c 0104 0102 0104 0102  s...............
-00001340: 0102 0102 0102 f97a 1d47 4f4d 502e 6164  .......z.GOMP.ad
-00001350: 645f 636f 6c6c 6973 696f 6e5f 636f 6e73  d_collision_cons
-00001360: 7472 6169 6e74 6303 0000 0000 0000 0000  traintc.........
-00001370: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
-00001380: 2c00 0000 7c00 a000 7c01 a101 0100 7c00  ,...|...|.....|.
-00001390: 6a01 7c00 6a02 6401 6402 8d02 0100 7403  j.|.j.d.d.....t.
-000013a0: a004 7c01 7c02 a102 7c00 5f05 6400 5300  ..|.|...|._.d.S.
-000013b0: 2903 4e46 2902 7218 0000 0072 2600 0000  ).NF).r....r&...
-000013c0: 2906 722d 0000 0072 2c00 0000 7218 0000  ).r-...r,...r...
-000013d0: 0072 1900 0000 7242 0000 0072 4b00 0000  .r....rB...rK...
-000013e0: 2903 7220 0000 0072 0f00 0000 da08 545f  ).r ...r......T_
-000013f0: 575f 4f62 7374 7221 0000 0072 2100 0000  W_Obstr!...r!...
-00001400: 7222 0000 00da 1975 7064 6174 655f 636f  r".....update_co
-00001410: 6e73 7472 6169 6e74 735f 7061 7261 6d73  nstraints_params
-00001420: a500 0000 7306 0000 0000 010a 0110 037a  ....s..........z
-00001430: 1e47 4f4d 502e 7570 6461 7465 5f63 6f6e  .GOMP.update_con
-00001440: 7374 7261 696e 7473 5f70 6172 616d 7329  straints_params)
-00001450: 0154 2901 4e29 0146 2901 724e 0000 0029  .T).N).F).rN...)
-00001460: 0172 5400 0000 2901 724e 0000 0029 0372  .rT...).rN...).r
-00001470: 5700 0000 7258 0000 0072 5900 0000 2914  W...rX...rY...).
-00001480: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00001490: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-000014a0: 6d65 5f5f 7210 0000 0072 2b00 0000 7223  me__r....r+...r#
-000014b0: 0000 0072 1200 0000 722c 0000 00da 0561  ...r....r,.....a
-000014c0: 7272 6179 722d 0000 0072 2f00 0000 7232  rrayr-...r/...r2
-000014d0: 0000 0072 3a00 0000 7248 0000 0072 4d00  ...r:...rH...rM.
-000014e0: 0000 7253 0000 0072 5500 0000 7256 0000  ..rS...rU...rV..
-000014f0: 0072 5d00 0000 725f 0000 0072 2100 0000  .r]...r_...r!...
-00001500: 7221 0000 0072 2100 0000 7222 0000 0072  r!...r!...r"...r
-00001510: 0600 0000 0900 0000 731a 0000 0008 011c  ........s.......
-00001520: 1b12 0e12 0608 0908 030a 180a 2008 0b0a  ............ ...
-00001530: 070a 080a 040a 0a72 0600 0000 290f da05  .......r....)...
-00001540: 6e75 6d70 7972 1000 0000 5a06 6361 7361  numpyr....Z.casa
-00001550: 6469 7219 0000 005a 0e73 7061 7469 616c  dir....Z.spatial
-00001560: 5f63 6173 6164 6972 2e00 0000 5a17 7363  _casadir....Z.sc
-00001570: 6970 792e 7370 6174 6961 6c2e 7472 616e  ipy.spatial.tran
-00001580: 7366 6f72 6d72 0200 0000 7229 0000 005a  sformr....r)...Z
-00001590: 2167 7261 7370 5f70 6c61 6e6e 696e 672e  !grasp_planning.
-000015a0: 736f 6c76 6572 2e72 6f62 6f74 5f6d 6f64  solver.robot_mod
-000015b0: 656c 7203 0000 005a 1967 7261 7370 5f70  elr....Z.grasp_p
-000015c0: 6c61 6e6e 696e 672e 636f 7374 2e63 6f73  lanning.cost.cos
-000015d0: 7473 7204 0000 005a 2667 7261 7370 5f70  tsr....Z&grasp_p
-000015e0: 6c61 6e6e 696e 672e 636f 6e73 7472 6169  lanning.constrai
-000015f0: 6e74 732e 636f 6e73 7472 6169 6e74 7372  nts.constraintsr
-00001600: 0600 0000 7221 0000 0072 2100 0000 7221  ....r!...r!...r!
-00001610: 0000 0072 2200 0000 da08 3c6d 6f64 756c  ...r".....<modul
-00001620: 653e 0100 0000 730e 0000 0008 0108 0108  e>....s.........
-00001630: 010c 010c 010c 0108 02                   .........
+00000180: 6430 6427 6428 8401 5a13 6404 5300 2931  d0d'd(..Z.d.S.)1
+00000190: da04 474f 4d50 e904 0000 00da 0577 6f72  ..GOMP.......wor
+000001a0: 6c64 5a0a 746f 6f6c 5f66 7261 6d65 4e29  ldZ.tool_frameN)
+000001b0: 01da 0672 6574 7572 6e63 0600 0000 0000  ...returnc......
+000001c0: 0000 0000 0000 0600 0000 0500 0000 4300  ..............C.
+000001d0: 0000 73c0 0000 0064 007c 005f 0064 007c  ..s....d.|._.d.|
+000001e0: 005f 0174 026a 0364 0174 0464 028d 027c  ._.t.j.d.t.d...|
+000001f0: 005f 0574 067c 027c 047c 0583 037c 005f  ._.t.|.|.|...|._
+00000200: 077c 006a 076a 087c 005f 0864 037c 005f  .|.j.j.|._.d.|._
+00000210: 097c 006a 087c 005f 0a7c 017c 005f 0b7c  .|.j.|._.|.|._.|
+00000220: 037c 005f 0c74 0d6a 0ea0 0f64 047c 006a  .|._.t.j...d.|.j
+00000230: 0a7c 006a 0ba1 037c 005f 1064 007c 005f  .|.j...|._.d.|._
+00000240: 1164 007c 005f 1264 055c 027c 005f 137c  .d.|._.d.\.|._.|
+00000250: 005f 1467 007c 005f 1574 0d6a 0ea0 0f64  ._.g.|._.t.j...d
+00000260: 0664 0164 01a1 037c 005f 1674 0d6a 0ea0  .d.d...|._.t.j..
+00000270: 0f64 0764 0164 01a1 037c 005f 1764 087c  .d.d.d...|._.d.|
+00000280: 005f 1874 0da0 19a1 007c 005f 1a67 007c  ._.t.....|._.g.|
+00000290: 005f 1b64 0053 0029 094e 7207 0000 00a9  ._.d.S.).Nr.....
+000002a0: 01da 0564 7479 7065 e906 0000 00da 0178  ...dtype.......x
+000002b0: 2902 4e4e 5a0b 7061 7261 6d5f 6772 6173  ).NNZ.param_gras
+000002c0: 705a 0a70 6172 616d 5f6f 6273 7446 291c  pZ.param_obstF).
+000002d0: da09 545f 575f 4772 6173 70da 0754 5f57  ..T_W_Grasp..T_W
+000002e0: 5f4f 626a da02 6e70 da03 6579 65da 0566  _Obj..np..eye..f
+000002f0: 6c6f 6174 da0b 545f 4f62 6a5f 4772 6173  loat..T_Obj_Gras
+00000300: 7072 0300 0000 da0c 5f72 6f62 6f74 5f6d  pr......_robot_m
+00000310: 6f64 656c da06 6e5f 646f 6673 5a16 6d61  odel..n_dofsZ.ma
+00000320: 6e69 7075 6c61 7469 6f6e 5f66 7261 6d65  nipulation_frame
+00000330: 5f64 696d da05 785f 6469 6dda 0b6e 5f77  _dim..x_dim..n_w
+00000340: 6179 706f 696e 7473 da05 7468 6574 61da  aypoints..theta.
+00000350: 0263 615a 0253 585a 0373 796d 720d 0000  .caZ.SXZ.symr...
+00000360: 00da 0678 5f69 6e69 745a 0a5f 6f62 6a65  ...x_initZ._obje
+00000370: 6374 6976 65da 0e6c 5f6a 6f69 6e74 5f6c  ctive..l_joint_l
+00000380: 696d 6974 73da 0e75 5f6a 6f69 6e74 5f6c  imits..u_joint_l
+00000390: 696d 6974 73da 0667 5f6c 6973 74da 0e70  imits..g_list..p
+000003a0: 6172 616d 5f67 7261 7370 5f63 61da 0d70  aram_grasp_ca..p
+000003b0: 6172 616d 5f6f 6273 745f 6361 da0f 5f63  aram_obst_ca.._c
+000003c0: 6f6c 6c69 7369 6f6e 5f66 6c61 67da 0776  ollision_flag..v
+000003d0: 6572 7463 6174 da0e 7061 7261 6d5f 6f70  ertcat..param_op
+000003e0: 7469 6d5f 6361 da0d 7061 7261 6d5f 6361  tim_ca..param_ca
+000003f0: 5f6c 6973 7429 06da 0473 656c 6672 1700  _list)...selfr..
+00000400: 0000 5a04 7572 6466 7218 0000 005a 0972  ..Z.urdfr....Z.r
+00000410: 6f6f 745f 6c69 6e6b 5a08 656e 645f 6c69  oot_linkZ.end_li
+00000420: 6e6b a900 7225 0000 00fa 482f 686f 6d65  nk..r%....H/home
+00000430: 2f74 6f6d 6173 2f44 6573 6b74 6f70 2f67  /tomas/Desktop/g
+00000440: 7261 7370 5f70 6c61 6e6e 696e 672f 6772  rasp_planning/gr
+00000450: 6173 705f 706c 616e 6e69 6e67 2f73 6f6c  asp_planning/sol
+00000460: 7665 722f 676f 6d70 5f70 6c61 6e6e 6572  ver/gomp_planner
+00000470: 2e70 79da 085f 5f69 6e69 745f 5f0a 0000  .py..__init__...
+00000480: 0073 2600 0000 0002 0601 0601 1003 0e01  .s&.............
+00000490: 0a01 0601 0801 0601 0603 1601 0602 0601  ................
+000004a0: 0c01 0602 1201 1201 0601 0a01 7a0d 474f  ............z.GO
+000004b0: 4d50 2e5f 5f69 6e69 745f 5f54 2902 7218  MP.__init__T).r.
+000004c0: 0000 0072 0900 0000 6303 0000 0000 0000  ...r....c.......
+000004d0: 0000 0000 0004 0000 0005 0000 0043 0000  .............C..
+000004e0: 0073 9600 0000 7400 6a01 6401 7402 6402  .s....t.j.d.t.d.
+000004f0: 8d02 7c00 5f03 7c02 7244 7404 6a05 6403  ..|._.|.rDt.j.d.
+00000500: 6404 6405 7c01 6703 6406 6407 8d03 a006  d.d.|.g.d.d.....
+00000510: a100 7d03 7400 a007 7400 a008 7c01 a101  ..}.t...t...|...
+00000520: 6408 a102 7c00 5f09 6e2a 7404 6a05 6403  d...|._.n*t.j.d.
+00000530: 7400 6a0a 6405 7c01 6703 6409 6407 8d03  t.j.d.|.g.d.d...
+00000540: a006 a100 7d03 7400 a007 7c01 6408 a102  ....}.t...|.d...
+00000550: 7c00 5f09 7c03 7c00 6a03 640a 640b 8502  |._.|.|.j.d.d...
+00000560: 640a 640b 8502 6602 3c00 7c00 6a0b 7c00  d.d...f.<.|.j.|.
+00000570: 6a03 1000 7c00 5f0c 640a 5300 290c 7a48  j...|._.d.S.).zH
+00000580: 0a20 2020 2020 2020 204f 626a 6563 7420  .        Object 
+00000590: 6861 7320 746f 2068 6176 6520 7a2d 6178  has to have z-ax
+000005a0: 6973 2061 6c69 676e 6564 2077 6974 6820  is aligned with 
+000005b0: 7468 6520 776f 726c 6420 6672 616d 650a  the world frame.
+000005c0: 2020 2020 2020 2020 7207 0000 0072 0a00          r....r..
+000005d0: 0000 da03 7879 7ae9 b400 0000 7201 0000  ....xyz.....r...
+000005e0: 0054 2901 da07 6465 6772 6565 73e9 0200  .T)...degrees...
+000005f0: 0000 464e e903 0000 0029 0d72 1000 0000  ..FN.....).r....
+00000600: 7211 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
+00000610: 0152 5a0a 6672 6f6d 5f65 756c 6572 5a09  .RZ.from_eulerZ.
+00000620: 6173 5f6d 6174 7269 78da 0572 6f75 6e64  as_matrix..round
+00000630: 5a07 6465 6732 7261 6472 1800 0000 da02  Z.deg2radr......
+00000640: 7069 720f 0000 0072 0e00 0000 2904 7224  pir....r....).r$
+00000650: 0000 0072 1800 0000 722a 0000 005a 0b52  ...r....r*...Z.R
+00000660: 5f4f 626a 5f47 7261 7370 7225 0000 0072  _Obj_Graspr%...r
+00000670: 2500 0000 7226 0000 00da 1075 7064 6174  %...r&.....updat
+00000680: 655f 6772 6173 705f 444f 4627 0000 0073  e_grasp_DOF'...s
+00000690: 1000 0000 0004 1001 0401 1a01 1602 1c01  ................
+000006a0: 0e01 1601 7a15 474f 4d50 2e75 7064 6174  ....z.GOMP.updat
+000006b0: 655f 6772 6173 705f 444f 4629 0272 0f00  e_grasp_DOF).r..
+000006c0: 0000 7209 0000 0063 0200 0000 0000 0000  ..r....c........
+000006d0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
+000006e0: 730a 0000 007c 017c 005f 0064 0153 0029  s....|.|._.d.S.)
+000006f0: 027a 2f0a 2020 2020 2020 2020 5570 6461  .z/.        Upda
+00000700: 7465 206f 626a 6563 7420 616e 6420 6772  te object and gr
+00000710: 6173 7020 706f 7365 730a 2020 2020 2020  asp poses.      
+00000720: 2020 4e29 0172 0f00 0000 2902 7224 0000    N).r....).r$..
+00000730: 0072 0f00 0000 7225 0000 0072 2500 0000  .r....r%...r%...
+00000740: 7226 0000 00da 1275 7064 6174 655f 6f62  r&.....update_ob
+00000750: 6a65 6374 5f70 6f73 6535 0000 0073 0200  ject_pose5...s..
+00000760: 0000 0004 7a17 474f 4d50 2e75 7064 6174  ....z.GOMP.updat
+00000770: 655f 6f62 6a65 6374 5f70 6f73 6563 0100  e_object_posec..
+00000780: 0000 0000 0000 0000 0000 0200 0000 0600  ................
+00000790: 0000 4300 0000 7354 0000 0074 006a 01a0  ..C...sT...t.j..
+000007a0: 027c 006a 0364 0164 0285 0264 0164 0285  .|.j.d.d...d.d..
+000007b0: 0266 0219 00a1 01a0 0464 03a1 017d 0174  .f.......d...}.t
+000007c0: 05a0 067c 006a 0364 0164 0285 0264 0266  ...|.j.d.d...d.f
+000007d0: 0219 0064 0164 0185 0264 0166 0219 007c  ...d.d...d.f...|
+000007e0: 0166 02a1 017c 005f 077c 006a 0753 0029  .f...|._.|.j.S.)
+000007f0: 047a 360a 2020 2020 2020 2020 436f 6e76  .z6.        Conv
+00000800: 6572 7420 545f 575f 4772 6173 7020 696e  ert T_W_Grasp in
+00000810: 746f 205b 782c 792c 7a2c 722c 702c 795d  to [x,y,z,r,p,y]
+00000820: 0a20 2020 2020 2020 204e 722c 0000 0072  .        Nr,...r
+00000830: 2800 0000 2908 da02 7363 7202 0000 005a  (...)...scr....Z
+00000840: 0b66 726f 6d5f 6d61 7472 6978 720e 0000  .from_matrixr...
+00000850: 005a 0861 735f 6575 6c65 7272 1000 0000  .Z.as_eulerr....
+00000860: 5a06 7673 7461 636b 5a0d 545f 575f 4772  Z.vstackZ.T_W_Gr
+00000870: 6173 705f 7270 7929 0272 2400 0000 5a0d  asp_rpy).r$...Z.
+00000880: 525f 575f 4772 6173 705f 7270 7972 2500  R_W_Grasp_rpyr%.
+00000890: 0000 7225 0000 0072 2600 0000 da0a 5f67  ..r%...r&....._g
+000008a0: 7261 7370 3272 7079 3b00 0000 7306 0000  rasp2rpy;...s...
+000008b0: 0000 0424 012a 017a 0f47 4f4d 502e 5f67  ...$.*.z.GOMP._g
+000008c0: 7261 7370 3272 7079 6302 0000 0000 0000  rasp2rpyc.......
+000008d0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+000008e0: 0073 1400 0000 7400 a001 7c01 7c00 6a02  .s....t...|.|.j.
+000008f0: a102 7c00 5f03 6400 5300 a901 4e29 0472  ..|._.d.S...N).r
+00000900: 1000 0000 5a04 7469 6c65 7217 0000 0072  ....Z.tiler....r
+00000910: 1a00 0000 2902 7224 0000 00da 0171 7225  ....).r$.....qr%
+00000920: 0000 0072 2500 0000 7226 0000 00da 0e73  ...r%...r&.....s
+00000930: 6574 5f69 6e69 745f 6775 6573 7344 0000  et_init_guessD..
+00000940: 0073 0200 0000 0001 7a13 474f 4d50 2e73  .s......z.GOMP.s
+00000950: 6574 5f69 6e69 745f 6775 6573 7363 0300  et_init_guessc..
+00000960: 0000 0000 0000 0000 0000 0500 0000 0500  ................
+00000970: 0000 4300 0000 7302 0100 007c 006a 0064  ..C...s....|.j.d
+00000980: 006b 0873 147c 006a 0164 006b 0872 ca74  .k.s.|.j.d.k.r.t
+00000990: 02a0 037c 006a 047c 006a 0566 0264 01a1  ...|.j.|.j.f.d..
+000009a0: 027c 005f 0074 02a0 037c 006a 047c 006a  .|._.t...|.j.|.j
+000009b0: 0566 0264 02a1 027c 005f 017c 006a 06a0  .f.d...|._.|.j..
+000009c0: 07a1 007d 0374 087c 006a 0583 0144 005d  ...}.t.|.j...D.]
+000009d0: 747d 047c 0364 0064 0085 0264 0366 0219  t}.|.d.d...d.f..
+000009e0: 007c 006a 0064 007c 006a 0985 027c 0466  .|.j.d.|.j...|.f
+000009f0: 023c 007c 0364 0064 0085 0264 0466 0219  .<.|.d.d...d.f..
+00000a00: 007c 006a 0164 007c 006a 0985 027c 0466  .|.j.d.|.j...|.f
+00000a10: 023c 0064 0574 026a 0a14 007c 006a 0064  .<.d.t.j...|.j.d
+00000a20: 0664 0085 027c 0466 023c 0064 0774 026a  .d...|.f.<.d.t.j
+00000a30: 0a14 007c 006a 0164 0664 0085 027c 0466  ...|.j.d.d...|.f
+00000a40: 023c 0071 547c 017c 006a 0064 0064 0085  .<.qT|.|.j.d.d..
+00000a50: 0264 0366 023c 007c 017c 006a 0164 0064  .d.f.<.|.|.j.d.d
+00000a60: 0085 0264 0366 023c 007c 0264 006b 0372  ...d.f.<.|.d.k.r
+00000a70: fe74 0b64 0883 0101 0064 0053 0029 094e  .t.d.....d.S.).N
+00000a80: 6700 0000 0000 0059 c067 0000 0000 0000  g......Y.g......
+00000a90: 5940 7201 0000 00e9 0100 0000 e9fe ffff  Y@r.............
+00000aa0: ffe9 fdff ffff 722b 0000 007a 2c46 696e  ......r+...z,Fin
+00000ab0: 616c 2062 6f75 6e64 6172 7920 636f 6e64  al boundary cond
+00000ac0: 6974 696f 6e20 6973 206e 6f74 2069 6d70  ition is not imp
+00000ad0: 6c65 6d65 6e74 6564 2e29 0c72 1b00 0000  lemented.).r....
+00000ae0: 721c 0000 0072 1000 0000 5a04 6675 6c6c  r....r....Z.full
+00000af0: 7216 0000 0072 1700 0000 7214 0000 005a  r....r....r....Z
+00000b00: 1467 6574 5f6a 6f69 6e74 5f70 6f73 5f6c  .get_joint_pos_l
+00000b10: 696d 6974 73da 0572 616e 6765 7215 0000  imits..ranger...
+00000b20: 0072 2f00 0000 da05 7072 696e 7429 0572  .r/.....print).r
+00000b30: 2400 0000 da07 715f 7374 6172 745a 0571  $.....q_startZ.q
+00000b40: 5f65 6e64 5a0c 6a6f 696e 745f 6c69 6d69  _endZ.joint_limi
+00000b50: 7473 da01 7472 2500 0000 7225 0000 0072  ts..tr%...r%...r
+00000b60: 2600 0000 da17 7365 745f 626f 756e 6461  &.....set_bounda
+00000b70: 7279 5f63 6f6e 6469 7469 6f6e 7347 0000  ry_conditionsG..
+00000b80: 0073 1a00 0000 0001 1402 1601 1603 0a01  .s..............
+00000b90: 0e01 2001 2001 1801 1a04 1201 1202 0801  .. . ...........
+00000ba0: 7a1c 474f 4d50 2e73 6574 5f62 6f75 6e64  z.GOMP.set_bound
+00000bb0: 6172 795f 636f 6e64 6974 696f 6e73 4663  ary_conditionsFc
+00000bc0: 0200 0000 0000 0000 0000 0000 0c00 0000  ................
+00000bd0: 0900 0000 4300 0000 7324 0100 007c 006a  ....C...s$...|.j
+00000be0: 00a0 0164 01a1 017d 0274 027c 006a 037c  ...d...}.t.|.j.|
+00000bf0: 006a 0464 0264 038d 037d 037c 03a0 057c  .j.d.d...}.|...|
+00000c00: 02a1 017d 0474 06a0 07a1 0074 06a0 07a1  ...}.t.....t....
+00000c10: 0074 06a0 07a1 0003 0002 007d 057c 005f  .t.........}.|._
+00000c20: 087c 005f 097c 006a 0a44 005d 3e7d 067c  .|._.|.j.D.]>}.|
+00000c30: 06a0 0ba1 005c 037d 077d 087d 0974 06a0  .....\.}.}.}.t..
+00000c40: 077c 057c 07a1 027d 0574 06a0 077c 006a  .|.|...}.t...|.j
+00000c50: 087c 08a1 027c 005f 0874 06a0 077c 006a  .|...|._.t...|.j
+00000c60: 097c 09a1 027c 005f 0971 4e7c 006a 0c72  .|...|._.qN|.j.r
+00000c70: a27c 006a 0da0 0e7c 006a 0fa1 0101 0074  .|.j...|.j.....t
+00000c80: 06a0 077c 006a 0d64 0419 00a1 017c 005f  ...|.j.d.....|._
+00000c90: 1074 1164 0574 127c 006a 0d83 0183 0244  .t.d.t.|.j.....D
+00000ca0: 005d 1a7d 0a74 06a0 077c 006a 107c 006a  .].}.t...|.j.|.j
+00000cb0: 0d7c 0a19 00a1 027c 005f 1071 c469 007d  .|.....|._.q.i.}
+00000cc0: 0b64 067c 0b64 073c 007c 0190 0173 0264  .d.|.d.<.|...s.d
+00000cd0: 047c 0b64 083c 0064 047c 0b64 093c 0074  .|.d.<.d.|.d.<.t
+00000ce0: 06a0 1364 0a64 0b7c 027c 047c 057c 006a  ...d.d.|.|.|.|.j
+00000cf0: 1064 0c9c 047c 0ba1 047c 005f 1464 0053  .d...|...|._.d.S
+00000d00: 0029 0d4e a902 e9ff ffff ff72 3700 0000  .).N.......r7...
+00000d10: 5429 015a 0b6d 616e 6970 5f66 7261 6d65  T).Z.manip_frame
+00000d20: 7201 0000 0072 3700 0000 67fc a9f1 d24d  r....r7...g....M
+00000d30: 6250 3f7a 1469 706f 7074 2e61 6363 6570  bP?z.ipopt.accep
+00000d40: 7461 626c 655f 746f 6c7a 1169 706f 7074  table_tolz.ipopt
+00000d50: 2e70 7269 6e74 5f6c 6576 656c 5a0a 7072  .print_levelZ.pr
+00000d60: 696e 745f 7469 6d65 da06 736f 6c76 6572  int_time..solver
+00000d70: 5a05 6970 6f70 7429 0472 0d00 0000 da01  Z.ipopt).r......
+00000d80: 66da 0167 da01 7029 1572 0d00 0000 da07  f..g..p).r......
+00000d90: 7265 7368 6170 6572 0400 0000 7217 0000  reshaper....r...
+00000da0: 0072 1600 0000 5a09 6576 616c 5f63 6f73  .r....Z.eval_cos
+00000db0: 7472 1900 0000 7221 0000 00da 0467 5f6c  tr....r!.....g_l
+00000dc0: 62da 0467 5f75 6272 1d00 0000 5a0e 6765  b..g_ubr....Z.ge
+00000dd0: 745f 636f 6e73 7472 6169 6e74 7220 0000  t_constraintr ..
+00000de0: 0072 2300 0000 da06 6170 7065 6e64 721f  .r#.....appendr.
+00000df0: 0000 0072 2200 0000 723a 0000 00da 036c  ...r"...r:.....l
+00000e00: 656e 5a06 6e6c 7073 6f6c 7241 0000 0029  enZ.nlpsolrA...)
+00000e10: 0c72 2400 0000 da07 7665 7262 6f73 655a  .r$.....verboseZ
+00000e20: 0c78 5f63 615f 666c 6174 7465 6e5a 0463  .x_ca_flattenZ.c
+00000e30: 6f73 745a 096f 626a 6563 7469 7665 7243  ostZ.objectiverC
+00000e40: 0000 005a 0667 5f74 6572 6dda 0267 7472  ...Z.g_term..gtr
+00000e50: 4600 0000 7247 0000 00da 0169 da07 6f70  F...rG.....i..op
+00000e60: 7469 6f6e 7372 2500 0000 7225 0000 0072  tionsr%...r%...r
+00000e70: 2600 0000 da0d 7365 7475 705f 7072 6f62  &.....setup_prob
+00000e80: 6c65 6d5f 0000 0073 2800 0000 0004 0c05  lem_...s(.......
+00000e90: 1201 0a02 2001 0a01 0e01 0c01 1001 1202  .... ...........
+00000ea0: 0601 0e03 1201 1401 1802 0401 0801 0601  ................
+00000eb0: 0801 0802 7a12 474f 4d50 2e73 6574 7570  ....z.GOMP.setup
+00000ec0: 5f70 726f 626c 656d 6301 0000 0000 0000  _problemc.......
+00000ed0: 0000 0000 0004 0000 0009 0000 0043 0000  .............C..
+00000ee0: 0073 6e00 0000 7c00 6a00 7c00 6a01 7c00  .sn...|.j.|.j.|.
+00000ef0: 6a02 7c00 6a03 7c00 6a04 6a05 6401 6402  j.|.j.|.j.j.d.d.
+00000f00: 6403 8d02 7c00 6a06 6a05 6401 6402 6403  d...|.j.j.d.d.d.
+00000f10: 8d02 7c00 6a07 6404 8d06 7d01 7c00 6a00  ..|.j.d...}.|.j.
+00000f20: a008 a100 6405 1900 7d02 7c00 6a00 a008  ....d...}.|.j...
+00000f30: a100 6406 1900 7d03 7409 a005 7c01 6407  ..d...}.t...|.d.
+00000f40: 1900 7c00 6a0a 7c00 6a0b 6602 a102 7c02  ..|.j.|.j.f...|.
+00000f50: 6602 5300 2908 4e72 3f00 0000 da01 4629  f.S.).Nr?.....F)
+00000f60: 01da 056f 7264 6572 2906 5a02 7830 5a03  ...order).Z.x0Z.
+00000f70: 6c62 675a 0375 6267 5a03 6c62 785a 0375  lbgZ.ubgZ.lbxZ.u
+00000f80: 6278 7244 0000 005a 0773 7563 6365 7373  bxrD...Z.success
+00000f90: 5a0d 7265 7475 726e 5f73 7461 7475 7372  Z.return_statusr
+00000fa0: 0d00 0000 290c 7241 0000 0072 1a00 0000  ....).rA...r....
+00000fb0: 7246 0000 0072 4700 0000 721b 0000 0072  rF...rG...r....r
+00000fc0: 4500 0000 721c 0000 00da 1070 6172 616d  E...r......param
+00000fd0: 735f 6f70 7469 6d5f 6e75 6d5a 0573 7461  s_optim_numZ.sta
+00000fe0: 7473 7210 0000 0072 1500 0000 7217 0000  tsr....r....r...
+00000ff0: 0029 0472 2400 0000 da06 7265 7375 6c74  .).r$.....result
+00001000: 5a0c 7375 6363 6573 735f 666c 6167 5a0b  Z.success_flagZ.
+00001010: 7375 6363 6573 735f 6d73 6772 2500 0000  success_msgr%...
+00001020: 7225 0000 0072 2600 0000 da05 736f 6c76  r%...r&.....solv
+00001030: 6584 0000 0073 1400 0000 0001 0801 0401  e....s..........
+00001040: 0401 0e01 0e01 04fb 0607 0e01 0e01 7a0a  ..............z.
+00001050: 474f 4d50 2e73 6f6c 7665 e700 0000 0000  GOMP.solve......
+00001060: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
+00001070: 0300 0000 0800 0000 4300 0000 7322 0000  ........C...s"..
+00001080: 007c 006a 00a0 0174 027c 006a 037c 006a  .|.j...t.|.j.|.j
+00001090: 047c 017c 006a 057c 0283 05a1 0101 0064  .|.|.j.|.......d
+000010a0: 0053 0072 3400 0000 2906 721d 0000 0072  .S.r4...).r....r
+000010b0: 4800 0000 5a12 4772 6173 7050 6f73 436f  H...Z.GraspPosCo
+000010c0: 6e73 7472 6169 6e74 7214 0000 0072 0d00  nstraintr....r..
+000010d0: 0000 721e 0000 00a9 0372 2400 0000 da0b  ..r......r$.....
+000010e0: 7761 7970 6f69 6e74 5f49 44da 0974 6f6c  waypoint_ID..tol
+000010f0: 6572 616e 6365 7225 0000 0072 2500 0000  erancer%...r%...
+00001100: 7226 0000 00da 195f 6164 645f 6772 6173  r&....._add_gras
+00001110: 705f 706f 735f 636f 6e73 7472 6169 6e74  p_pos_constraint
+00001120: 9000 0000 730c 0000 0000 010c 0104 0102  ....s...........
+00001130: 0104 0102 fc7a 1e47 4f4d 502e 5f61 6464  .....z.GOMP._add
+00001140: 5f67 7261 7370 5f70 6f73 5f63 6f6e 7374  _grasp_pos_const
+00001150: 7261 696e 74e7 9a99 9999 9999 b93f 6303  raint........?c.
+00001160: 0000 0000 0000 0000 0000 0003 0000 0009  ................
+00001170: 0000 0043 0000 0073 2600 0000 7c00 6a00  ...C...s&...|.j.
+00001180: a001 7402 7c00 6a03 7c00 6a04 7c01 7c00  ..t.|.j.|.j.|.|.
+00001190: 6a05 7c00 6a06 7c02 8306 a101 0100 6400  j.|.j.|.......d.
+000011a0: 5300 7234 0000 0029 0772 1d00 0000 7248  S.r4...).r....rH
+000011b0: 0000 005a 1247 7261 7370 526f 7443 6f6e  ...Z.GraspRotCon
+000011c0: 7374 7261 696e 7472 1400 0000 720d 0000  straintr....r...
+000011d0: 0072 1e00 0000 7218 0000 0072 5500 0000  .r....r....rU...
+000011e0: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
+000011f0: 195f 6164 645f 6772 6173 705f 726f 745f  ._add_grasp_rot_
+00001200: 636f 6e73 7472 6169 6e74 9700 0000 730e  constraint....s.
+00001210: 0000 0000 010c 0104 0102 0104 0104 0102  ................
+00001220: fb7a 1e47 4f4d 502e 5f61 6464 5f67 7261  .z.GOMP._add_gra
+00001230: 7370 5f72 6f74 5f63 6f6e 7374 7261 696e  sp_rot_constrain
+00001240: 7463 0300 0000 0000 0000 0000 0000 0300  tc..............
+00001250: 0000 0400 0000 4300 0000 732a 0000 007c  ......C...s*...|
+00001260: 00a0 007c 017c 02a1 0201 007c 00a0 017c  ...|.|.....|...|
+00001270: 017c 02a1 0201 007c 006a 02a0 037c 006a  .|.....|.j...|.j
+00001280: 04a1 0101 0064 0053 0072 3400 0000 2905  .....d.S.r4...).
+00001290: 7258 0000 0072 5a00 0000 7223 0000 0072  rX...rZ...r#...r
+000012a0: 4800 0000 721e 0000 0072 5500 0000 7225  H...r....rU...r%
+000012b0: 0000 0072 2500 0000 7226 0000 00da 1461  ...r%...r&.....a
+000012c0: 6464 5f67 7261 7370 5f63 6f6e 7374 7261  dd_grasp_constra
+000012d0: 696e 749f 0000 0073 0600 0000 0001 0c01  int....s........
+000012e0: 0c01 7a19 474f 4d50 2e61 6464 5f67 7261  ..z.GOMP.add_gra
+000012f0: 7370 5f63 6f6e 7374 7261 696e 74e7 0000  sp_constraint...
+00001300: 0000 0000 e03f e79a 9999 9999 99c9 3fe7  .....?........?.
+00001310: 7b14 ae47 e17a 843f 6306 0000 0000 0000  {..G.z.?c.......
+00001320: 0000 0000 0006 0000 000c 0000 0043 0000  .............C..
+00001330: 0073 3000 0000 6401 7c00 5f00 7c00 6a01  .s0...d.|._.|.j.
+00001340: a002 7403 7c00 6a04 7c00 6a05 7c01 7c00  ..t.|.j.|.j.|.|.
+00001350: 6a06 7c02 7c03 7c04 7c05 6402 8d08 a101  j.|.|.|.|.d.....
+00001360: 0100 6400 5300 2903 4e54 2908 5a05 726f  ..d.S.).NT).Z.ro
+00001370: 626f 745a 0471 5f63 6172 5600 0000 721f  botZ.q_carV...r.
+00001380: 0000 005a 096c 696e 6b5f 6e61 6d65 da06  ...Z.link_name..
+00001390: 725f 6c69 6e6b da06 725f 6f62 7374 7257  r_link..r_obstrW
+000013a0: 0000 0029 0772 2000 0000 721d 0000 0072  ...).r ...r....r
+000013b0: 4800 0000 5a13 436f 6c6c 6973 696f 6e43  H...Z.CollisionC
+000013c0: 6f6e 7374 7261 696e 7472 1400 0000 720d  onstraintr....r.
+000013d0: 0000 0072 1f00 0000 2906 7224 0000 0072  ...r....).r$...r
+000013e0: 5600 0000 da0a 6368 696c 645f 6c69 6e6b  V.....child_link
+000013f0: 725f 0000 0072 6000 0000 7257 0000 0072  r_...r`...rW...r
+00001400: 2500 0000 7225 0000 0072 2600 0000 da18  %...r%...r&.....
+00001410: 6164 645f 636f 6c6c 6973 696f 6e5f 636f  add_collision_co
+00001420: 6e73 7472 6169 6e74 a400 0000 7314 0000  nstraint....s...
+00001430: 0000 0106 010c 0104 0102 0104 0102 0102  ................
+00001440: 0102 0102 f97a 1d47 4f4d 502e 6164 645f  .....z.GOMP.add_
+00001450: 636f 6c6c 6973 696f 6e5f 636f 6e73 7472  collision_constr
+00001460: 6169 6e74 6303 0000 0000 0000 0000 0000  aintc...........
+00001470: 0003 0000 0004 0000 0043 0000 0073 3a00  .........C...s:.
+00001480: 0000 7c00 a000 7c01 a101 0100 7c00 6a01  ..|...|.....|.j.
+00001490: 7c00 6a02 6401 6402 8d02 0100 7c00 6a03  |.j.d.d.....|.j.
+000014a0: 7230 7404 a005 7c01 7c02 a102 7c00 5f06  r0t...|.|...|._.
+000014b0: 6e06 7c01 7c00 5f06 6400 5300 2903 4e46  n.|.|._.d.S.).NF
+000014c0: 2902 7218 0000 0072 2a00 0000 2907 7231  ).r....r*...).r1
+000014d0: 0000 0072 3000 0000 7218 0000 0072 2000  ...r0...r....r .
+000014e0: 0000 7219 0000 0072 2100 0000 7251 0000  ..r....r!...rQ..
+000014f0: 0029 0372 2400 0000 720f 0000 00da 0854  .).r$...r......T
+00001500: 5f57 5f4f 6273 7472 2500 0000 7225 0000  _W_Obstr%...r%..
+00001510: 0072 2600 0000 da19 7570 6461 7465 5f63  .r&.....update_c
+00001520: 6f6e 7374 7261 696e 7473 5f70 6172 616d  onstraints_param
+00001530: 73af 0000 0073 0a00 0000 0001 0a01 1002  s....s..........
+00001540: 0601 1002 7a1e 474f 4d50 2e75 7064 6174  ....z.GOMP.updat
+00001550: 655f 636f 6e73 7472 6169 6e74 735f 7061  e_constraints_pa
+00001560: 7261 6d73 2901 5429 014e 2901 4629 0172  rams).T).N).F).r
+00001570: 5400 0000 2901 7259 0000 0029 0172 5400  T...).rY...).rT.
+00001580: 0000 2903 725c 0000 0072 5d00 0000 725e  ..).r\...r]...r^
+00001590: 0000 0029 014e 2914 da08 5f5f 6e61 6d65  ...).N)...__name
+000015a0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+000015b0: 5f5f 7175 616c 6e61 6d65 5f5f 7210 0000  __qualname__r...
+000015c0: 0072 2f00 0000 7227 0000 0072 1200 0000  .r/...r'...r....
+000015d0: 7230 0000 00da 0561 7272 6179 7231 0000  r0.....arrayr1..
+000015e0: 0072 3300 0000 7236 0000 0072 3e00 0000  .r3...r6...r>...
+000015f0: 724e 0000 0072 5300 0000 7258 0000 0072  rN...rS...rX...r
+00001600: 5a00 0000 725b 0000 0072 6200 0000 7264  Z...r[...rb...rd
+00001610: 0000 0072 2500 0000 7225 0000 0072 2500  ...r%...r%...r%.
+00001620: 0000 7226 0000 0072 0600 0000 0900 0000  ..r&...r........
+00001630: 731a 0000 0008 011c 1d12 0e12 0608 0908  s...............
+00001640: 030a 180a 2508 0c0a 070a 080a 050a 0b72  ....%..........r
+00001650: 0600 0000 290f da05 6e75 6d70 7972 1000  ....)...numpyr..
+00001660: 0000 5a06 6361 7361 6469 7219 0000 005a  ..Z.casadir....Z
+00001670: 0e73 7061 7469 616c 5f63 6173 6164 6972  .spatial_casadir
+00001680: 3200 0000 5a17 7363 6970 792e 7370 6174  2...Z.scipy.spat
+00001690: 6961 6c2e 7472 616e 7366 6f72 6d72 0200  ial.transformr..
+000016a0: 0000 722d 0000 005a 2167 7261 7370 5f70  ..r-...Z!grasp_p
+000016b0: 6c61 6e6e 696e 672e 736f 6c76 6572 2e72  lanning.solver.r
+000016c0: 6f62 6f74 5f6d 6f64 656c 7203 0000 005a  obot_modelr....Z
+000016d0: 1967 7261 7370 5f70 6c61 6e6e 696e 672e  .grasp_planning.
+000016e0: 636f 7374 2e63 6f73 7473 7204 0000 005a  cost.costsr....Z
+000016f0: 2667 7261 7370 5f70 6c61 6e6e 696e 672e  &grasp_planning.
+00001700: 636f 6e73 7472 6169 6e74 732e 636f 6e73  constraints.cons
+00001710: 7472 6169 6e74 7372 0600 0000 7225 0000  traintsr....r%..
+00001720: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
+00001730: da08 3c6d 6f64 756c 653e 0100 0000 730e  ..<module>....s.
+00001740: 0000 0008 0108 0108 010c 010c 010c 0108  ................
+00001750: 02                                       .
```

### Comparing `grasp_planning-0.5.0/grasp_planning/solver/__pycache__/robot_model.cpython-38.pyc` & `grasp_planning-0.5.1/grasp_planning/solver/__pycache__/robot_model.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.0/grasp_planning/solver/gomp_planner.py` & `grasp_planning-0.5.1/grasp_planning/solver/gomp_planner.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,17 @@
         
         self._objective = None
         self.l_joint_limits, self.u_joint_limits = None, None
         self.g_list = []
 
         self.param_grasp_ca = ca.SX.sym("param_grasp", 4, 4)
         self.param_obst_ca = ca.SX.sym("param_obst", 4, 4)
-
+        self._collision_flag = False
+        self.param_optim_ca = ca.vertcat()
+        self.param_ca_list = []
 
 
     def update_grasp_DOF(self, theta: float, degrees=True) -> None:
         """
         Object has to have z-axis aligned with the world frame
         """
         self.T_Obj_Grasp = np.eye(4, dtype=float)
@@ -105,37 +107,43 @@
         g, self.g_lb, self.g_ub = ca.vertcat(), ca.vertcat(), ca.vertcat()
         for g_term in self.g_list:
             gt, g_lb, g_ub = g_term.get_constraint()
             g = ca.vertcat(g, gt)
             self.g_lb = ca.vertcat(self.g_lb, g_lb)
             self.g_ub = ca.vertcat(self.g_ub, g_ub)
 
+        if self._collision_flag:
+            self.param_ca_list.append(self.param_obst_ca)
+
 
+        self.param_optim_ca = ca.vertcat(self.param_ca_list[0])
+        for i in range(1, len(self.param_ca_list)):
+            self.param_optim_ca = ca.vertcat(self.param_optim_ca, self.param_ca_list[i])
 
         options = {}
         options["ipopt.acceptable_tol"] = 1e-3
         if not verbose:
             options["ipopt.print_level"] = 0
             options["print_time"] = 0
 
-        params_optim_ca = ca.vertcat(self.param_grasp_ca, self.param_obst_ca)
-        self.solver = ca.nlpsol('solver', 'ipopt', {'x': x_ca_flatten, 'f': objective, 'g': g, 'p': params_optim_ca}, options)
+        self.solver = ca.nlpsol('solver', 'ipopt', {'x': x_ca_flatten, 'f': objective, 'g': g, 'p': self.param_optim_ca}, options)
     
 
         
     def solve(self):
         result = self.solver(x0=self.x_init,
                              lbg=self.g_lb,
                              ubg=self.g_ub,
                              lbx=self.l_joint_limits.reshape((-1,1), order='F'),
                              ubx=self.u_joint_limits.reshape((-1,1), order='F'),
                              p=self.params_optim_num)
+        
         success_flag = self.solver.stats()["success"]
         success_msg = self.solver.stats()["return_status"]
-        return result['x'], success_flag
+        return  np.reshape(result['x'], (self.n_dofs, self.n_waypoints)), success_flag
 
     def _add_grasp_pos_constraint(self, waypoint_ID, tolerance=0.0):
         self.g_list.append(GraspPosConstraint(self._robot_model, 
                                               self.x, 
                                               waypoint_ID, 
                                               self.param_grasp_ca, 
                                               tolerance))
@@ -147,24 +155,28 @@
                                               self.param_grasp_ca, 
                                               self.theta, 
                                               tolerance))
 
     def add_grasp_constraint(self, waypoint_ID, tolerance=0.0):
         self._add_grasp_pos_constraint(waypoint_ID, tolerance)
         self._add_grasp_rot_constraint(waypoint_ID, tolerance)
+        self.param_ca_list.append(self.param_grasp_ca)
 
     def add_collision_constraint(self, waypoint_ID, child_link, r_link=0.5, r_obst=0.2, tolerance=0.01):
+        self._collision_flag = True
         self.g_list.append(CollisionConstraint(robot=self._robot_model,
                                                 q_ca=self.x,
                                                 waypoint_ID=waypoint_ID,
                                                 param_obst_ca=self.param_obst_ca,
                                                 link_name=child_link,
                                                 r_link= r_link,
                                                 r_obst= r_obst,
                                                 tolerance=tolerance))
 
-    def update_constraints_params(self, T_W_Obj, T_W_Obst):
+    def update_constraints_params(self, T_W_Obj, T_W_Obst=None):
         self.update_object_pose(T_W_Obj)
         self.update_grasp_DOF(theta=self.theta, degrees=False)
 
-      
-        self.params_optim_num = ca.vertcat(T_W_Obj, T_W_Obst)
+        if self._collision_flag:
+            self.params_optim_num = ca.vertcat(T_W_Obj, T_W_Obst)
+        else:
+            self.params_optim_num = T_W_Obj
```

### Comparing `grasp_planning-0.5.0/grasp_planning/solver/robot_model.py` & `grasp_planning-0.5.1/grasp_planning/solver/robot_model.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.0/PKG-INFO` & `grasp_planning-0.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grasp_planning
-Version: 0.5.0
+Version: 0.5.1
 Summary: "Grasp and Motion Planning Python Package."
 License: MIT
 Author: Tomas Merva
 Author-email: tmerva7@gmail.com
 Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -62,7 +62,9 @@
 planner.update_constraints_params(T_W_Obj, T_W_Obst)
 x, solver_flag = planner.solve()
 end = time.time()
 print(f"Computational time: {end-start}" )
 print(f"Solver status: {solver_flag}" )
 ```
 
+## ToDo
+- [ ] removing constraints
```

