# Comparing `tmp/tgqSim-0.1.6.tar.gz` & `tmp/tgqSim-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgqSim-0.1.6.tar", last modified: Tue May 14 00:55:31 2024, max compression
+gzip compressed data, was "tgqSim-0.1.7.tar", last modified: Tue May 14 03:32:09 2024, max compression
```

## Comparing `tgqSim-0.1.6.tar` & `tgqSim-0.1.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 00:55:31.461296 tgqSim-0.1.6/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-14 00:55:30.000000 tgqSim-0.1.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-14 00:55:30.000000 tgqSim-0.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      747 2024-05-14 00:55:31.461296 tgqSim-0.1.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-14 00:55:30.000000 tgqSim-0.1.6/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 00:55:31.461296 tgqSim-0.1.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1151 2024-05-14 00:55:30.000000 tgqSim-0.1.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 00:55:31.458296 tgqSim-0.1.6/tgqSim/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 00:55:31.460296 tgqSim-0.1.6/tgqSim/GateSimulation/
--rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-14 00:55:30.000000 tgqSim-0.1.6/tgqSim/GateSimulation/DoubleGate.py
--rw-rw-rw-   0 root         (0) root         (0)     5413 2024-05-14 00:55:30.000000 tgqSim-0.1.6/tgqSim/GateSimulation/SingleGate.py
--rw-rw-rw-   0 root         (0) root         (0)     3537 2024-05-14 00:55:30.000000 tgqSim-0.1.6/tgqSim/GateSimulation/TripleGate.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-14 00:55:30.000000 tgqSim-0.1.6/tgqSim/GateSimulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22122 2024-05-14 00:55:30.000000 tgqSim-0.1.6/tgqSim/QuantumCircuit.py
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-14 00:55:30.000000 tgqSim-0.1.6/tgqSim/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18468 2024-05-14 00:55:30.000000 tgqSim-0.1.6/tgqSim/draw_circuit_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 00:55:31.460296 tgqSim-0.1.6/tgqSim/lib/
--rw-rw-rw-   0 root         (0) root         (0)    61896 2024-05-14 00:55:30.000000 tgqSim-0.1.6/tgqSim/lib/cuda_11-8_tgq_simulator.so
--rw-rw-rw-   0 root         (0) root         (0)    73408 2024-05-14 00:55:30.000000 tgqSim-0.1.6/tgqSim/lib/cuda_12-4_tgq_simulator.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 00:55:31.459296 tgqSim-0.1.6/tgqSim.egg-info/
--rw-r--r--   0 root         (0) root         (0)      747 2024-05-14 00:55:31.000000 tgqSim-0.1.6/tgqSim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      478 2024-05-14 00:55:31.000000 tgqSim-0.1.6/tgqSim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 00:55:31.000000 tgqSim-0.1.6/tgqSim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2024-05-14 00:55:31.000000 tgqSim-0.1.6/tgqSim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-14 00:55:31.000000 tgqSim-0.1.6/tgqSim.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 03:32:09.865350 tgqSim-0.1.7/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-14 03:32:07.000000 tgqSim-0.1.7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-14 03:32:07.000000 tgqSim-0.1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      747 2024-05-14 03:32:09.865350 tgqSim-0.1.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-14 03:32:07.000000 tgqSim-0.1.7/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 03:32:09.865350 tgqSim-0.1.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1151 2024-05-14 03:32:08.000000 tgqSim-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 03:32:09.864350 tgqSim-0.1.7/tgqSim/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 03:32:09.864350 tgqSim-0.1.7/tgqSim/GateSimulation/
+-rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-14 03:32:07.000000 tgqSim-0.1.7/tgqSim/GateSimulation/DoubleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)     5413 2024-05-14 03:32:07.000000 tgqSim-0.1.7/tgqSim/GateSimulation/SingleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3537 2024-05-14 03:32:07.000000 tgqSim-0.1.7/tgqSim/GateSimulation/TripleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-14 03:32:07.000000 tgqSim-0.1.7/tgqSim/GateSimulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22122 2024-05-14 03:32:07.000000 tgqSim-0.1.7/tgqSim/QuantumCircuit.py
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-14 03:32:08.000000 tgqSim-0.1.7/tgqSim/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18468 2024-05-14 03:32:07.000000 tgqSim-0.1.7/tgqSim/draw_circuit_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 03:32:09.865350 tgqSim-0.1.7/tgqSim/lib/
+-rw-rw-rw-   0 root         (0) root         (0)    61896 2024-05-14 03:32:07.000000 tgqSim-0.1.7/tgqSim/lib/cuda_11-8_tgq_simulator.so
+-rw-rw-rw-   0 root         (0) root         (0)    73456 2024-05-14 03:32:07.000000 tgqSim-0.1.7/tgqSim/lib/cuda_12-4_tgq_simulator.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 03:32:09.864350 tgqSim-0.1.7/tgqSim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      747 2024-05-14 03:32:09.000000 tgqSim-0.1.7/tgqSim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      478 2024-05-14 03:32:09.000000 tgqSim-0.1.7/tgqSim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 03:32:09.000000 tgqSim-0.1.7/tgqSim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-14 03:32:09.000000 tgqSim-0.1.7/tgqSim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-14 03:32:09.000000 tgqSim-0.1.7/tgqSim.egg-info/top_level.txt
```

### Comparing `tgqSim-0.1.6/LICENSE` & `tgqSim-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.6/PKG-INFO` & `tgqSim-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgqSim
-Version: 0.1.6
+Version: 0.1.7
 Summary: TGQ量子模拟器
 Home-page: UNKNOWN
 Author: tiangongqs
 License: MIT
 Keywords: tgq,quantum,simulator
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `tgqSim-0.1.6/setup.py` & `tgqSim-0.1.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='tgqSim',
-    version='0.1.6',
+    version='0.1.7',
     description='TGQ量子模拟器',  # 包描述
     long_description="Python for quantum simulation http://www.tiangongqs.com",  # 详细描述
     long_description_content_type='text/markdown',
     author='tiangongqs',  # 作者姓名
     license='MIT',  # 许可证
     package=find_packages(),
     include_package_data=True,
```

### Comparing `tgqSim-0.1.6/tgqSim/GateSimulation/DoubleGate.py` & `tgqSim-0.1.7/tgqSim/GateSimulation/DoubleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.6/tgqSim/GateSimulation/SingleGate.py` & `tgqSim-0.1.7/tgqSim/GateSimulation/SingleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.6/tgqSim/GateSimulation/TripleGate.py` & `tgqSim-0.1.7/tgqSim/GateSimulation/TripleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.6/tgqSim/QuantumCircuit.py` & `tgqSim-0.1.7/tgqSim/QuantumCircuit.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.6/tgqSim/draw_circuit_tools.py` & `tgqSim-0.1.7/tgqSim/draw_circuit_tools.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.6/tgqSim/lib/cuda_11-8_tgq_simulator.so` & `tgqSim-0.1.7/tgqSim/lib/cuda_11-8_tgq_simulator.so`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.6/tgqSim/lib/cuda_12-4_tgq_simulator.so` & `tgqSim-0.1.7/tgqSim/lib/cuda_12-4_tgq_simulator.so`

 * *Files 2% similar despite different names*

#### readelf --wide --file-header {}

```diff
@@ -4,17 +4,17 @@
   Data:                              2's complement, little endian
   Version:                           1 (current)
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              DYN (Shared object file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
-  Entry point address:               0x1f50
+  Entry point address:               0x1fa0
   Start of program headers:          64 (bytes into file)
-  Start of section headers:          71168 (bytes into file)
+  Start of section headers:          71216 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           56 (bytes)
   Number of program headers:         6
   Size of section headers:           64 (bytes)
   Number of section headers:         35
   Section header string table index: 34
```

#### readelf --wide --program-header {}

```diff
@@ -1,18 +1,18 @@
 
 Elf file type is DYN (Shared object file)
-Entry point 0x1f50
+Entry point 0x1fa0
 There are 6 program headers, starting at offset 64
 
 Program Headers:
   Type           Offset   VirtAddr           PhysAddr           FileSiz  MemSiz   Flg Align
-  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x00b5d4 0x00b5d4 R E 0x200000
-  LOAD           0x00bd60 0x000000000020bd60 0x000000000020bd60 0x0004e0 0x0004f0 RW  0x200000
+  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x00b664 0x00b664 R E 0x200000
+  LOAD           0x00bd60 0x000000000020bd60 0x000000000020bd60 0x0004e8 0x0004f8 RW  0x200000
   DYNAMIC        0x00bd78 0x000000000020bd78 0x000000000020bd78 0x000230 0x000230 RW  0x8
-  GNU_EH_FRAME   0x00ad58 0x000000000000ad58 0x000000000000ad58 0x0001ac 0x0001ac R   0x4
+  GNU_EH_FRAME   0x00ade8 0x000000000000ade8 0x000000000000ade8 0x0001ac 0x0001ac R   0x4
   GNU_STACK      0x000000 0x0000000000000000 0x0000000000000000 0x000000 0x000000 RW  0x10
   GNU_RELRO      0x00bd60 0x000000000020bd60 0x000000000020bd60 0x0002a0 0x0002a0 R   0x1
 
  Section to Segment mapping:
   Segment Sections...
    00     .hash .dynsym .dynstr .gnu.version .gnu.version_r .rela.dyn .rela.plt .init .plt .text .fini .rodata .nv_fatbin .eh_frame_hdr .eh_frame 
    01     .init_array .fini_array .dynamic .got .got.plt .data .nvFatBinSegment .bss
```

#### readelf --wide --sections {}

```diff
@@ -1,44 +1,44 @@
-There are 35 section headers, starting at offset 0x11600:
+There are 35 section headers, starting at offset 0x11630:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
-  [ 1] .hash             HASH            0000000000000190 000190 000254 04   A  2   0  8
-  [ 2] .dynsym           DYNSYM          00000000000003e8 0003e8 000780 18   A  3   1  8
-  [ 3] .dynstr           STRTAB          0000000000000b68 000b68 000710 00   A  0   0  1
-  [ 4] .gnu.version      VERSYM          0000000000001278 001278 0000a0 02   A  2   0  2
-  [ 5] .gnu.version_r    VERNEED         0000000000001318 001318 000060 00   A  3   3  8
-  [ 6] .rela.dyn         RELA            0000000000001378 001378 000180 18   A  2   0  8
-  [ 7] .rela.plt         RELA            00000000000014f8 0014f8 000618 18  AI  2  20  8
-  [ 8] .init             PROGBITS        0000000000001b10 001b10 000017 00  AX  0   0  4
-  [ 9] .plt              PROGBITS        0000000000001b30 001b30 000420 10  AX  0   0 16
-  [10] .text             PROGBITS        0000000000001f50 001f50 002a9e 00  AX  0   0 16
-  [11] .fini             PROGBITS        00000000000049f0 0049f0 000009 00  AX  0   0  4
-  [12] .rodata           PROGBITS        0000000000004a00 004a00 0002f8 00   A  0   0 16
-  [13] .nv_fatbin        PROGBITS        0000000000004cf8 004cf8 006060 00   A  0   0  8
-  [14] .eh_frame_hdr     PROGBITS        000000000000ad58 00ad58 0001ac 00   A  0   0  4
-  [15] .eh_frame         PROGBITS        000000000000af08 00af08 0006cc 00   A  0   0  8
+  [ 1] .hash             HASH            0000000000000190 000190 000258 04   A  2   0  8
+  [ 2] .dynsym           DYNSYM          00000000000003e8 0003e8 000798 18   A  3   1  8
+  [ 3] .dynstr           STRTAB          0000000000000b80 000b80 000717 00   A  0   0  1
+  [ 4] .gnu.version      VERSYM          0000000000001298 001298 0000a2 02   A  2   0  2
+  [ 5] .gnu.version_r    VERNEED         0000000000001340 001340 000060 00   A  3   3  8
+  [ 6] .rela.dyn         RELA            00000000000013a0 0013a0 000180 18   A  2   0  8
+  [ 7] .rela.plt         RELA            0000000000001520 001520 000630 18  AI  2  20  8
+  [ 8] .init             PROGBITS        0000000000001b50 001b50 000017 00  AX  0   0  4
+  [ 9] .plt              PROGBITS        0000000000001b70 001b70 000430 10  AX  0   0 16
+  [10] .text             PROGBITS        0000000000001fa0 001fa0 002abe 00  AX  0   0 16
+  [11] .fini             PROGBITS        0000000000004a60 004a60 000009 00  AX  0   0  4
+  [12] .rodata           PROGBITS        0000000000004a70 004a70 000318 00   A  0   0 16
+  [13] .nv_fatbin        PROGBITS        0000000000004d88 004d88 006060 00   A  0   0  8
+  [14] .eh_frame_hdr     PROGBITS        000000000000ade8 00ade8 0001ac 00   A  0   0  4
+  [15] .eh_frame         PROGBITS        000000000000af98 00af98 0006cc 00   A  0   0  8
   [16] .init_array       INIT_ARRAY      000000000020bd60 00bd60 000010 08  WA  0   0  8
   [17] .fini_array       FINI_ARRAY      000000000020bd70 00bd70 000008 08  WA  0   0  8
   [18] .dynamic          DYNAMIC         000000000020bd78 00bd78 000230 10  WA  3   0  8
   [19] .got              PROGBITS        000000000020bfa8 00bfa8 000058 08  WA  0   0  8
-  [20] .got.plt          PROGBITS        000000000020c000 00c000 000220 08  WA  0   0  8
-  [21] .data             PROGBITS        000000000020c220 00c220 000008 00  WA  0   0  8
-  [22] .nvFatBinSegment  PROGBITS        000000000020c228 00c228 000018 00  WA  0   0  8
-  [23] .bss              NOBITS          000000000020c240 00c240 000010 00  WA  0   0  8
-  [24] .comment          PROGBITS        0000000000000000 00c240 000011 01  MS  0   0  1
+  [20] .got.plt          PROGBITS        000000000020c000 00c000 000228 08  WA  0   0  8
+  [21] .data             PROGBITS        000000000020c228 00c228 000008 00  WA  0   0  8
+  [22] .nvFatBinSegment  PROGBITS        000000000020c230 00c230 000018 00  WA  0   0  8
+  [23] .bss              NOBITS          000000000020c248 00c248 000010 00  WA  0   0  8
+  [24] .comment          PROGBITS        0000000000000000 00c248 000011 01  MS  0   0  1
   [25] .debug_aranges    PROGBITS        0000000000000000 00c260 0000b0 00      0   0 16
   [26] .debug_info       PROGBITS        0000000000000000 00c310 001ef4 00      0   0  1
   [27] .debug_abbrev     PROGBITS        0000000000000000 00e204 000386 00      0   0  1
   [28] .debug_line       PROGBITS        0000000000000000 00e58a 0004b1 00      0   0  1
   [29] .debug_str        PROGBITS        0000000000000000 00ea3b 0012f9 01  MS  0   0  1
   [30] .debug_loc        PROGBITS        0000000000000000 00fd34 000039 00      0   0  1
   [31] .debug_ranges     PROGBITS        0000000000000000 00fd70 000080 00      0   0 16
-  [32] .symtab           SYMTAB          0000000000000000 00fdf0 000d08 18     33  60  8
-  [33] .strtab           STRTAB          0000000000000000 010af8 0009bd 00      0   0  1
-  [34] .shstrtab         STRTAB          0000000000000000 0114b5 00014b 00      0   0  1
+  [32] .symtab           SYMTAB          0000000000000000 00fdf0 000d20 18     33  60  8
+  [33] .strtab           STRTAB          0000000000000000 010b10 0009d1 00      0   0  1
+  [34] .shstrtab         STRTAB          0000000000000000 0114e1 00014b 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

#### readelf --wide --symbols {}

```diff
@@ -1,225 +1,227 @@
 
-Symbol table '.dynsym' contains 80 entries:
+Symbol table '.dynsym' contains 81 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
-     1: 0000000000002550   105 FUNC    GLOBAL DEFAULT   10 _Z11cphase_gateP6float2f
-     2: 0000000000003670   662 FUNC    GLOBAL DEFAULT   10 execute_circuit
-     3: 0000000000002440   117 FUNC    GLOBAL DEFAULT   10 _Z7ad_gateP6float2f
-     4: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaMalloc@libcudart.so.12 (2)
-     5: 00000000000033b0    47 FUNC    GLOBAL DEFAULT   10 _Z4hashPKc
-     6: 00000000000023c0   120 FUNC    GLOBAL DEFAULT   10 _Z7pd_gateP6float2f
-     7: 00000000000044e0   201 FUNC    GLOBAL DEFAULT   10 _Z50__device_stub__Z18actionOnTripleGateP6float2S0_mPmP6float2S0_mPm
-     8: 0000000000002110    22 FUNC    GLOBAL DEFAULT   10 _Z6y_gateP6float2
-     9: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaLaunchKernel@libcudart.so.12 (2)
-    10: 0000000000002940   101 FUNC    GLOBAL DEFAULT   10 _Z22toff_gate_target_smallP6float2
-    11: 00000000000020d0     5 FUNC    GLOBAL DEFAULT   10 _Z7comparePKvS0_
-    12: 000000000020c240     0 NOTYPE  GLOBAL DEFAULT   22 _edata
-    13: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND rand@GLIBC_2.2.5 (3)
-    14: 0000000000003030   416 FUNC    GLOBAL DEFAULT   10 _Z23fred_gate_control_smallP6float2
-    15: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaUnregisterFatBinary@libcudart.so.12 (2)
-    16: 0000000000002e90   416 FUNC    GLOBAL DEFAULT   10 _Z21fred_gate_control_midP6float2
-    17: 0000000000002600    51 FUNC    GLOBAL DEFAULT   10 _Z23cnot_gate_control_smallP6float2
-    18: 0000000000002260   106 FUNC    GLOBAL DEFAULT   10 _Z7ry_gateP6float2f
-    19: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND sincosf@GLIBC_2.2.5 (4)
-    20: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5 (3)
-    21: 0000000000002cf0   416 FUNC    GLOBAL DEFAULT   10 _Z21fred_gate_control_bigP6float2
-    22: 00000000000028f0    65 FUNC    GLOBAL DEFAULT   10 _Z8syc_gateP6float2
-    23: 0000000000002680   197 FUNC    GLOBAL DEFAULT   10 _Z8rxx_gateP6float2f
-    24: 00000000000029b0   402 FUNC    GLOBAL DEFAULT   10 _Z20toff_gate_target_midP6float2
-    25: 0000000000002820   194 FUNC    GLOBAL DEFAULT   10 _Z8rzz_gateP6float2f
-    26: 0000000000004030  1190 FUNC    GLOBAL DEFAULT   10 doubleGateAction
-    27: 00000000000033e0    82 FUNC    GLOBAL DEFAULT   10 _Z9isInArrayPPKcPci
-    28: 00000000000025c0    51 FUNC    GLOBAL DEFAULT   10 _Z21cnot_gate_control_bigP6float2
-    29: 00000000000020f0    23 FUNC    GLOBAL DEFAULT   10 _Z6x_gateP6float2
-    30: 0000000000003240    65 FUNC    GLOBAL DEFAULT   10 _Z20generate_binary_dataf
-    31: 0000000000002150    23 FUNC    GLOBAL DEFAULT   10 _Z6s_gateP6float2
-    32: 0000000000002330   131 FUNC    GLOBAL DEFAULT   10 _Z11damp_i_gateP6float2f
-    33: 0000000000002500    65 FUNC    GLOBAL DEFAULT   10 _Z10iswap_gateP6float2
-    34: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_atexit@GLIBC_2.2.5 (3)
-    35: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFatBinary@libcudart.so.12 (2)
-    36: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND time@GLIBC_2.2.5 (3)
-    37: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND srand@GLIBC_2.2.5 (3)
-    38: 0000000000002190    23 FUNC    GLOBAL DEFAULT   10 _Z6t_gateP6float2
-    39: 0000000000003470   510 FUNC    GLOBAL DEFAULT   10 _Z13normalizationP6float2i
-    40: 0000000000002130    23 FUNC    GLOBAL DEFAULT   10 _Z6z_gateP6float2
-    41: 0000000000004020     5 FUNC    GLOBAL DEFAULT   10 _Z19actionOnDoubleQubitP6float2S0_mPm
-    42: 0000000000003f50   201 FUNC    GLOBAL DEFAULT   10 _Z51__device_stub__Z19actionOnDoubleQubitP6float2S0_mPmP6float2S0_mPm
-    43: 0000000000003290   286 FUNC    GLOBAL DEFAULT   10 _Z7getprobP6float2Pfm
-    44: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free@GLIBC_2.2.5 (3)
-    45: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaMemcpy@libcudart.so.12 (2)
-    46: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND exit@GLIBC_2.2.5 (3)
-    47: 00000000000021b0    23 FUNC    GLOBAL DEFAULT   10 _Z8tdg_gateP6float2
-    48: 0000000000002640    58 FUNC    GLOBAL DEFAULT   10 _Z7cz_gateP6float2
-    49: 00000000000045b0     5 FUNC    GLOBAL DEFAULT   10 _Z18actionOnTripleGateP6float2S0_mPm
-    50: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND malloc@GLIBC_2.2.5 (3)
-    51: 000000000020c250     0 NOTYPE  GLOBAL DEFAULT   23 _end
-    52: 0000000000003910   201 FUNC    GLOBAL DEFAULT   10 _Z51__device_stub__Z19actionOnSingleQubitP6float2S0_mPmP6float2S0_mPm
-    53: 0000000000003440    33 FUNC    GLOBAL DEFAULT   10 _Z14getArrayLengthPi
-    54: 0000000000002170    23 FUNC    GLOBAL DEFAULT   10 _Z8sdg_gateP6float2
-    55: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strcmp@GLIBC_2.2.5 (3)
-    56: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFunction@libcudart.so.12 (2)
-    57: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaFree@libcudart.so.12 (2)
-    58: 0000000000002b50   416 FUNC    GLOBAL DEFAULT   10 _Z20toff_gate_target_bigP6float2
-    59: 0000000000002750   200 FUNC    GLOBAL DEFAULT   10 _Z8ryy_gateP6float2f
-    60: 000000000020c240     0 NOTYPE  GLOBAL DEFAULT   23 __bss_start
-    61: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND puts@GLIBC_2.2.5 (3)
-    62: 00000000000039f0  1373 FUNC    GLOBAL DEFAULT   10 singleGateAction
-    63: 00000000000039e0     5 FUNC    GLOBAL DEFAULT   10 _Z19actionOnSingleQubitP6float2S0_mPm
-    64: 00000000000031d0   107 FUNC    GLOBAL DEFAULT   10 _Z11identityMatP6float2i
-    65: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaPopCallConfiguration@libcudart.so.12 (2)
-    66: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaDeviceSynchronize@libcudart.so.12 (2)
-    67: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
-    68: 00000000000022d0    94 FUNC    GLOBAL DEFAULT   10 _Z7rz_gateP6float2f
-    69: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaPushCallConfiguration@libcudart.so.12 (2)
-    70: 00000000000021d0    22 FUNC    GLOBAL DEFAULT   10 _Z6h_gateP6float2
-    71: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND sqrtf@GLIBC_2.2.5 (4)
-    72: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFatBinaryEnd@libcudart.so.12 (2)
-    73: 00000000000045c0  1049 FUNC    GLOBAL DEFAULT   10 tripleGateAction
-    74: 00000000000024c0    51 FUNC    GLOBAL DEFAULT   10 _Z9swap_gateP6float2
-    75: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
-    76: 00000000000021f0    97 FUNC    GLOBAL DEFAULT   10 _Z7rx_gateP6float2f
-    77: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND qsort@GLIBC_2.2.5 (3)
-    78: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
-    79: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaSetDevice@libcudart.so.12 (2)
+     1: 00000000000025a0   105 FUNC    GLOBAL DEFAULT   10 _Z11cphase_gateP6float2f
+     2: 00000000000036c0   662 FUNC    GLOBAL DEFAULT   10 execute_circuit
+     3: 0000000000002490   117 FUNC    GLOBAL DEFAULT   10 _Z7ad_gateP6float2f
+     4: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND printf@GLIBC_2.2.5 (2)
+     5: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaMalloc@libcudart.so.12 (3)
+     6: 0000000000003400    47 FUNC    GLOBAL DEFAULT   10 _Z4hashPKc
+     7: 0000000000002410   120 FUNC    GLOBAL DEFAULT   10 _Z7pd_gateP6float2f
+     8: 0000000000004550   201 FUNC    GLOBAL DEFAULT   10 _Z50__device_stub__Z18actionOnTripleGateP6float2S0_mPmP6float2S0_mPm
+     9: 0000000000002160    22 FUNC    GLOBAL DEFAULT   10 _Z6y_gateP6float2
+    10: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaLaunchKernel@libcudart.so.12 (3)
+    11: 0000000000002990   101 FUNC    GLOBAL DEFAULT   10 _Z22toff_gate_target_smallP6float2
+    12: 0000000000002120     5 FUNC    GLOBAL DEFAULT   10 _Z7comparePKvS0_
+    13: 000000000020c248     0 NOTYPE  GLOBAL DEFAULT   22 _edata
+    14: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND rand@GLIBC_2.2.5 (2)
+    15: 0000000000003080   416 FUNC    GLOBAL DEFAULT   10 _Z23fred_gate_control_smallP6float2
+    16: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaUnregisterFatBinary@libcudart.so.12 (3)
+    17: 0000000000002ee0   416 FUNC    GLOBAL DEFAULT   10 _Z21fred_gate_control_midP6float2
+    18: 0000000000002650    51 FUNC    GLOBAL DEFAULT   10 _Z23cnot_gate_control_smallP6float2
+    19: 00000000000022b0   106 FUNC    GLOBAL DEFAULT   10 _Z7ry_gateP6float2f
+    20: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND sincosf@GLIBC_2.2.5 (4)
+    21: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5 (2)
+    22: 0000000000002d40   416 FUNC    GLOBAL DEFAULT   10 _Z21fred_gate_control_bigP6float2
+    23: 0000000000002940    65 FUNC    GLOBAL DEFAULT   10 _Z8syc_gateP6float2
+    24: 00000000000026d0   197 FUNC    GLOBAL DEFAULT   10 _Z8rxx_gateP6float2f
+    25: 0000000000002a00   402 FUNC    GLOBAL DEFAULT   10 _Z20toff_gate_target_midP6float2
+    26: 0000000000002870   194 FUNC    GLOBAL DEFAULT   10 _Z8rzz_gateP6float2f
+    27: 0000000000004080  1227 FUNC    GLOBAL DEFAULT   10 doubleGateAction
+    28: 0000000000003430    82 FUNC    GLOBAL DEFAULT   10 _Z9isInArrayPPKcPci
+    29: 0000000000002610    51 FUNC    GLOBAL DEFAULT   10 _Z21cnot_gate_control_bigP6float2
+    30: 0000000000002140    23 FUNC    GLOBAL DEFAULT   10 _Z6x_gateP6float2
+    31: 0000000000003290    65 FUNC    GLOBAL DEFAULT   10 _Z20generate_binary_dataf
+    32: 00000000000021a0    23 FUNC    GLOBAL DEFAULT   10 _Z6s_gateP6float2
+    33: 0000000000002380   131 FUNC    GLOBAL DEFAULT   10 _Z11damp_i_gateP6float2f
+    34: 0000000000002550    65 FUNC    GLOBAL DEFAULT   10 _Z10iswap_gateP6float2
+    35: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_atexit@GLIBC_2.2.5 (2)
+    36: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFatBinary@libcudart.so.12 (3)
+    37: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND time@GLIBC_2.2.5 (2)
+    38: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND srand@GLIBC_2.2.5 (2)
+    39: 00000000000021e0    23 FUNC    GLOBAL DEFAULT   10 _Z6t_gateP6float2
+    40: 00000000000034c0   510 FUNC    GLOBAL DEFAULT   10 _Z13normalizationP6float2i
+    41: 0000000000002180    23 FUNC    GLOBAL DEFAULT   10 _Z6z_gateP6float2
+    42: 0000000000004070     5 FUNC    GLOBAL DEFAULT   10 _Z19actionOnDoubleQubitP6float2S0_mPm
+    43: 0000000000003fa0   201 FUNC    GLOBAL DEFAULT   10 _Z51__device_stub__Z19actionOnDoubleQubitP6float2S0_mPmP6float2S0_mPm
+    44: 00000000000032e0   286 FUNC    GLOBAL DEFAULT   10 _Z7getprobP6float2Pfm
+    45: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free@GLIBC_2.2.5 (2)
+    46: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaMemcpy@libcudart.so.12 (3)
+    47: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND exit@GLIBC_2.2.5 (2)
+    48: 0000000000002200    23 FUNC    GLOBAL DEFAULT   10 _Z8tdg_gateP6float2
+    49: 0000000000002690    58 FUNC    GLOBAL DEFAULT   10 _Z7cz_gateP6float2
+    50: 0000000000004620     5 FUNC    GLOBAL DEFAULT   10 _Z18actionOnTripleGateP6float2S0_mPm
+    51: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND malloc@GLIBC_2.2.5 (2)
+    52: 000000000020c258     0 NOTYPE  GLOBAL DEFAULT   23 _end
+    53: 0000000000003960   201 FUNC    GLOBAL DEFAULT   10 _Z51__device_stub__Z19actionOnSingleQubitP6float2S0_mPmP6float2S0_mPm
+    54: 0000000000003490    33 FUNC    GLOBAL DEFAULT   10 _Z14getArrayLengthPi
+    55: 00000000000021c0    23 FUNC    GLOBAL DEFAULT   10 _Z8sdg_gateP6float2
+    56: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strcmp@GLIBC_2.2.5 (2)
+    57: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFunction@libcudart.so.12 (3)
+    58: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaFree@libcudart.so.12 (3)
+    59: 0000000000002ba0   416 FUNC    GLOBAL DEFAULT   10 _Z20toff_gate_target_bigP6float2
+    60: 00000000000027a0   200 FUNC    GLOBAL DEFAULT   10 _Z8ryy_gateP6float2f
+    61: 000000000020c248     0 NOTYPE  GLOBAL DEFAULT   23 __bss_start
+    62: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND puts@GLIBC_2.2.5 (2)
+    63: 0000000000003a40  1373 FUNC    GLOBAL DEFAULT   10 singleGateAction
+    64: 0000000000003a30     5 FUNC    GLOBAL DEFAULT   10 _Z19actionOnSingleQubitP6float2S0_mPm
+    65: 0000000000003220   107 FUNC    GLOBAL DEFAULT   10 _Z11identityMatP6float2i
+    66: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaPopCallConfiguration@libcudart.so.12 (3)
+    67: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaDeviceSynchronize@libcudart.so.12 (3)
+    68: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
+    69: 0000000000002320    94 FUNC    GLOBAL DEFAULT   10 _Z7rz_gateP6float2f
+    70: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaPushCallConfiguration@libcudart.so.12 (3)
+    71: 0000000000002220    22 FUNC    GLOBAL DEFAULT   10 _Z6h_gateP6float2
+    72: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND sqrtf@GLIBC_2.2.5 (4)
+    73: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFatBinaryEnd@libcudart.so.12 (3)
+    74: 0000000000004630  1049 FUNC    GLOBAL DEFAULT   10 tripleGateAction
+    75: 0000000000002510    51 FUNC    GLOBAL DEFAULT   10 _Z9swap_gateP6float2
+    76: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
+    77: 0000000000002240    97 FUNC    GLOBAL DEFAULT   10 _Z7rx_gateP6float2f
+    78: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND qsort@GLIBC_2.2.5 (2)
+    79: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
+    80: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaSetDevice@libcudart.so.12 (3)
 
-Symbol table '.symtab' contains 139 entries:
+Symbol table '.symtab' contains 140 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000190     0 SECTION LOCAL  DEFAULT    1 .hash
      2: 00000000000003e8     0 SECTION LOCAL  DEFAULT    2 .dynsym
-     3: 0000000000000b68     0 SECTION LOCAL  DEFAULT    3 .dynstr
-     4: 0000000000001278     0 SECTION LOCAL  DEFAULT    4 .gnu.version
-     5: 0000000000001318     0 SECTION LOCAL  DEFAULT    5 .gnu.version_r
-     6: 0000000000001378     0 SECTION LOCAL  DEFAULT    6 .rela.dyn
-     7: 00000000000014f8     0 SECTION LOCAL  DEFAULT    7 .rela.plt
-     8: 0000000000001b10     0 SECTION LOCAL  DEFAULT    8 .init
-     9: 0000000000001b30     0 SECTION LOCAL  DEFAULT    9 .plt
-    10: 0000000000001f50     0 SECTION LOCAL  DEFAULT   10 .text
-    11: 00000000000049f0     0 SECTION LOCAL  DEFAULT   11 .fini
-    12: 0000000000004a00     0 SECTION LOCAL  DEFAULT   12 .rodata
-    13: 0000000000004cf8     0 SECTION LOCAL  DEFAULT   13 .nv_fatbin
-    14: 000000000000ad58     0 SECTION LOCAL  DEFAULT   14 .eh_frame_hdr
-    15: 000000000000af08     0 SECTION LOCAL  DEFAULT   15 .eh_frame
+     3: 0000000000000b80     0 SECTION LOCAL  DEFAULT    3 .dynstr
+     4: 0000000000001298     0 SECTION LOCAL  DEFAULT    4 .gnu.version
+     5: 0000000000001340     0 SECTION LOCAL  DEFAULT    5 .gnu.version_r
+     6: 00000000000013a0     0 SECTION LOCAL  DEFAULT    6 .rela.dyn
+     7: 0000000000001520     0 SECTION LOCAL  DEFAULT    7 .rela.plt
+     8: 0000000000001b50     0 SECTION LOCAL  DEFAULT    8 .init
+     9: 0000000000001b70     0 SECTION LOCAL  DEFAULT    9 .plt
+    10: 0000000000001fa0     0 SECTION LOCAL  DEFAULT   10 .text
+    11: 0000000000004a60     0 SECTION LOCAL  DEFAULT   11 .fini
+    12: 0000000000004a70     0 SECTION LOCAL  DEFAULT   12 .rodata
+    13: 0000000000004d88     0 SECTION LOCAL  DEFAULT   13 .nv_fatbin
+    14: 000000000000ade8     0 SECTION LOCAL  DEFAULT   14 .eh_frame_hdr
+    15: 000000000000af98     0 SECTION LOCAL  DEFAULT   15 .eh_frame
     16: 000000000020bd60     0 SECTION LOCAL  DEFAULT   16 .init_array
     17: 000000000020bd70     0 SECTION LOCAL  DEFAULT   17 .fini_array
     18: 000000000020bd78     0 SECTION LOCAL  DEFAULT   18 .dynamic
     19: 000000000020bfa8     0 SECTION LOCAL  DEFAULT   19 .got
     20: 000000000020c000     0 SECTION LOCAL  DEFAULT   20 .got.plt
-    21: 000000000020c220     0 SECTION LOCAL  DEFAULT   21 .data
-    22: 000000000020c228     0 SECTION LOCAL  DEFAULT   22 .nvFatBinSegment
-    23: 000000000020c240     0 SECTION LOCAL  DEFAULT   23 .bss
+    21: 000000000020c228     0 SECTION LOCAL  DEFAULT   21 .data
+    22: 000000000020c230     0 SECTION LOCAL  DEFAULT   22 .nvFatBinSegment
+    23: 000000000020c248     0 SECTION LOCAL  DEFAULT   23 .bss
     24: 0000000000000000     0 SECTION LOCAL  DEFAULT   24 .comment
     25: 0000000000000000     0 SECTION LOCAL  DEFAULT   25 .debug_aranges
     26: 0000000000000000     0 SECTION LOCAL  DEFAULT   26 .debug_info
     27: 0000000000000000     0 SECTION LOCAL  DEFAULT   27 .debug_abbrev
     28: 0000000000000000     0 SECTION LOCAL  DEFAULT   28 .debug_line
     29: 0000000000000000     0 SECTION LOCAL  DEFAULT   29 .debug_str
     30: 0000000000000000     0 SECTION LOCAL  DEFAULT   30 .debug_loc
     31: 0000000000000000     0 SECTION LOCAL  DEFAULT   31 .debug_ranges
-    32: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS tmpxft_00004acc_00000000-6_tgq_simulator.cudafe1.cpp
-    33: 00000000000050b8     0 NOTYPE  LOCAL  DEFAULT   13 fatbinData
-    34: 00000000000020e0    12 FUNC    LOCAL  DEFAULT   10 _ZL26__cudaUnregisterBinaryUtilv
-    35: 000000000020c248     8 OBJECT  LOCAL  DEFAULT   23 _ZL20__cudaFatCubinHandle
-    36: 0000000000001f50   186 FUNC    LOCAL  DEFAULT   10 _ZL24__sti____cudaRegisterAllv
-    37: 000000000020c228    24 OBJECT  LOCAL  DEFAULT   22 _ZL15__fatDeviceText
+    32: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS tmpxft_00005715_00000000-6_tgq_simulator.cudafe1.cpp
+    33: 0000000000005148     0 NOTYPE  LOCAL  DEFAULT   13 fatbinData
+    34: 0000000000002130    12 FUNC    LOCAL  DEFAULT   10 _ZL26__cudaUnregisterBinaryUtilv
+    35: 000000000020c250     8 OBJECT  LOCAL  DEFAULT   23 _ZL20__cudaFatCubinHandle
+    36: 0000000000001fa0   186 FUNC    LOCAL  DEFAULT   10 _ZL24__sti____cudaRegisterAllv
+    37: 000000000020c230    24 OBJECT  LOCAL  DEFAULT   22 _ZL15__fatDeviceText
     38: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
-    39: 0000000000002010     0 FUNC    LOCAL  DEFAULT   10 deregister_tm_clones
-    40: 0000000000002040     0 FUNC    LOCAL  DEFAULT   10 register_tm_clones
-    41: 0000000000002080     0 FUNC    LOCAL  DEFAULT   10 __do_global_dtors_aux
-    42: 000000000020c240     1 OBJECT  LOCAL  DEFAULT   23 completed.7311
+    39: 0000000000002060     0 FUNC    LOCAL  DEFAULT   10 deregister_tm_clones
+    40: 0000000000002090     0 FUNC    LOCAL  DEFAULT   10 register_tm_clones
+    41: 00000000000020d0     0 FUNC    LOCAL  DEFAULT   10 __do_global_dtors_aux
+    42: 000000000020c248     1 OBJECT  LOCAL  DEFAULT   23 completed.7311
     43: 000000000020bd70     0 OBJECT  LOCAL  DEFAULT   17 __do_global_dtors_aux_fini_array_entry
-    44: 00000000000020c0     0 FUNC    LOCAL  DEFAULT   10 frame_dummy
+    44: 0000000000002110     0 FUNC    LOCAL  DEFAULT   10 frame_dummy
     45: 000000000020bd60     0 OBJECT  LOCAL  DEFAULT   16 __frame_dummy_init_array_entry
     46: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS link.stub
-    47: 0000000000004cf8     0 NOTYPE  LOCAL  DEFAULT   13 fatbinData
+    47: 0000000000004d88     0 NOTYPE  LOCAL  DEFAULT   13 fatbinData
     48: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS atexit.c
     49: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
-    50: 000000000000b5d0     0 OBJECT  LOCAL  DEFAULT   15 __FRAME_END__
+    50: 000000000000b660     0 OBJECT  LOCAL  DEFAULT   15 __FRAME_END__
     51: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS 
-    52: 000000000000ad58     0 NOTYPE  LOCAL  DEFAULT   14 __GNU_EH_FRAME_HDR
-    53: 000000000020c220     0 OBJECT  LOCAL  DEFAULT   21 __dso_handle
-    54: 00000000000049e0    14 FUNC    LOCAL  DEFAULT   10 atexit
-    55: 00000000000049f0     0 FUNC    LOCAL  DEFAULT   11 _fini
-    56: 0000000000001b10     0 FUNC    LOCAL  DEFAULT    8 _init
+    52: 000000000000ade8     0 NOTYPE  LOCAL  DEFAULT   14 __GNU_EH_FRAME_HDR
+    53: 000000000020c228     0 OBJECT  LOCAL  DEFAULT   21 __dso_handle
+    54: 0000000000004a50    14 FUNC    LOCAL  DEFAULT   10 atexit
+    55: 0000000000004a60     0 FUNC    LOCAL  DEFAULT   11 _fini
+    56: 0000000000001b50     0 FUNC    LOCAL  DEFAULT    8 _init
     57: 000000000020bd78     0 OBJECT  LOCAL  DEFAULT   18 _DYNAMIC
-    58: 000000000020c228     0 OBJECT  LOCAL  DEFAULT   22 __TMC_END__
+    58: 000000000020c230     0 OBJECT  LOCAL  DEFAULT   22 __TMC_END__
     59: 000000000020c000     0 OBJECT  LOCAL  DEFAULT   20 _GLOBAL_OFFSET_TABLE_
-    60: 0000000000002550   105 FUNC    GLOBAL DEFAULT   10 _Z11cphase_gateP6float2f
-    61: 0000000000003670   662 FUNC    GLOBAL DEFAULT   10 execute_circuit
-    62: 0000000000002440   117 FUNC    GLOBAL DEFAULT   10 _Z7ad_gateP6float2f
-    63: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaMalloc@@libcudart.so.12
-    64: 00000000000033b0    47 FUNC    GLOBAL DEFAULT   10 _Z4hashPKc
-    65: 00000000000023c0   120 FUNC    GLOBAL DEFAULT   10 _Z7pd_gateP6float2f
-    66: 00000000000044e0   201 FUNC    GLOBAL DEFAULT   10 _Z50__device_stub__Z18actionOnTripleGateP6float2S0_mPmP6float2S0_mPm
-    67: 0000000000002110    22 FUNC    GLOBAL DEFAULT   10 _Z6y_gateP6float2
-    68: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaLaunchKernel@@libcudart.so.12
-    69: 0000000000002940   101 FUNC    GLOBAL DEFAULT   10 _Z22toff_gate_target_smallP6float2
-    70: 00000000000020d0     5 FUNC    GLOBAL DEFAULT   10 _Z7comparePKvS0_
-    71: 000000000020c240     0 NOTYPE  GLOBAL DEFAULT   22 _edata
-    72: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND rand@@GLIBC_2.2.5
-    73: 0000000000003030   416 FUNC    GLOBAL DEFAULT   10 _Z23fred_gate_control_smallP6float2
-    74: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaUnregisterFatBinary@@libcudart.so.12
-    75: 0000000000002e90   416 FUNC    GLOBAL DEFAULT   10 _Z21fred_gate_control_midP6float2
-    76: 0000000000002600    51 FUNC    GLOBAL DEFAULT   10 _Z23cnot_gate_control_smallP6float2
-    77: 0000000000002260   106 FUNC    GLOBAL DEFAULT   10 _Z7ry_gateP6float2f
-    78: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND sincosf@@GLIBC_2.2.5
-    79: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@@GLIBC_2.2.5
-    80: 0000000000002cf0   416 FUNC    GLOBAL DEFAULT   10 _Z21fred_gate_control_bigP6float2
-    81: 00000000000028f0    65 FUNC    GLOBAL DEFAULT   10 _Z8syc_gateP6float2
-    82: 0000000000002680   197 FUNC    GLOBAL DEFAULT   10 _Z8rxx_gateP6float2f
-    83: 00000000000029b0   402 FUNC    GLOBAL DEFAULT   10 _Z20toff_gate_target_midP6float2
-    84: 0000000000002820   194 FUNC    GLOBAL DEFAULT   10 _Z8rzz_gateP6float2f
-    85: 0000000000004030  1190 FUNC    GLOBAL DEFAULT   10 doubleGateAction
-    86: 00000000000033e0    82 FUNC    GLOBAL DEFAULT   10 _Z9isInArrayPPKcPci
-    87: 00000000000025c0    51 FUNC    GLOBAL DEFAULT   10 _Z21cnot_gate_control_bigP6float2
-    88: 00000000000020f0    23 FUNC    GLOBAL DEFAULT   10 _Z6x_gateP6float2
-    89: 0000000000003240    65 FUNC    GLOBAL DEFAULT   10 _Z20generate_binary_dataf
-    90: 0000000000002150    23 FUNC    GLOBAL DEFAULT   10 _Z6s_gateP6float2
-    91: 0000000000002330   131 FUNC    GLOBAL DEFAULT   10 _Z11damp_i_gateP6float2f
-    92: 0000000000002500    65 FUNC    GLOBAL DEFAULT   10 _Z10iswap_gateP6float2
-    93: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_atexit@@GLIBC_2.2.5
-    94: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFatBinary@@libcudart.so.12
-    95: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND time@@GLIBC_2.2.5
-    96: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND srand@@GLIBC_2.2.5
-    97: 0000000000002190    23 FUNC    GLOBAL DEFAULT   10 _Z6t_gateP6float2
-    98: 0000000000003470   510 FUNC    GLOBAL DEFAULT   10 _Z13normalizationP6float2i
-    99: 0000000000002130    23 FUNC    GLOBAL DEFAULT   10 _Z6z_gateP6float2
-   100: 0000000000004020     5 FUNC    GLOBAL DEFAULT   10 _Z19actionOnDoubleQubitP6float2S0_mPm
-   101: 0000000000003f50   201 FUNC    GLOBAL DEFAULT   10 _Z51__device_stub__Z19actionOnDoubleQubitP6float2S0_mPmP6float2S0_mPm
-   102: 0000000000003290   286 FUNC    GLOBAL DEFAULT   10 _Z7getprobP6float2Pfm
-   103: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free@@GLIBC_2.2.5
-   104: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaMemcpy@@libcudart.so.12
-   105: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND exit@@GLIBC_2.2.5
-   106: 00000000000021b0    23 FUNC    GLOBAL DEFAULT   10 _Z8tdg_gateP6float2
-   107: 0000000000002640    58 FUNC    GLOBAL DEFAULT   10 _Z7cz_gateP6float2
-   108: 00000000000045b0     5 FUNC    GLOBAL DEFAULT   10 _Z18actionOnTripleGateP6float2S0_mPm
-   109: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND malloc@@GLIBC_2.2.5
-   110: 000000000020c250     0 NOTYPE  GLOBAL DEFAULT   23 _end
-   111: 0000000000003910   201 FUNC    GLOBAL DEFAULT   10 _Z51__device_stub__Z19actionOnSingleQubitP6float2S0_mPmP6float2S0_mPm
-   112: 0000000000003440    33 FUNC    GLOBAL DEFAULT   10 _Z14getArrayLengthPi
-   113: 0000000000002170    23 FUNC    GLOBAL DEFAULT   10 _Z8sdg_gateP6float2
-   114: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strcmp@@GLIBC_2.2.5
-   115: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFunction@@libcudart.so.12
-   116: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaFree@@libcudart.so.12
-   117: 0000000000002b50   416 FUNC    GLOBAL DEFAULT   10 _Z20toff_gate_target_bigP6float2
-   118: 0000000000002750   200 FUNC    GLOBAL DEFAULT   10 _Z8ryy_gateP6float2f
-   119: 000000000020c240     0 NOTYPE  GLOBAL DEFAULT   23 __bss_start
-   120: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND puts@@GLIBC_2.2.5
-   121: 00000000000039f0  1373 FUNC    GLOBAL DEFAULT   10 singleGateAction
-   122: 00000000000039e0     5 FUNC    GLOBAL DEFAULT   10 _Z19actionOnSingleQubitP6float2S0_mPm
-   123: 00000000000031d0   107 FUNC    GLOBAL DEFAULT   10 _Z11identityMatP6float2i
-   124: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaPopCallConfiguration@@libcudart.so.12
-   125: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaDeviceSynchronize@@libcudart.so.12
-   126: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
-   127: 00000000000022d0    94 FUNC    GLOBAL DEFAULT   10 _Z7rz_gateP6float2f
-   128: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaPushCallConfiguration@@libcudart.so.12
-   129: 00000000000021d0    22 FUNC    GLOBAL DEFAULT   10 _Z6h_gateP6float2
-   130: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND sqrtf@@GLIBC_2.2.5
-   131: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFatBinaryEnd@@libcudart.so.12
-   132: 00000000000045c0  1049 FUNC    GLOBAL DEFAULT   10 tripleGateAction
-   133: 00000000000024c0    51 FUNC    GLOBAL DEFAULT   10 _Z9swap_gateP6float2
-   134: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
-   135: 00000000000021f0    97 FUNC    GLOBAL DEFAULT   10 _Z7rx_gateP6float2f
-   136: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND qsort@@GLIBC_2.2.5
-   137: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
-   138: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaSetDevice@@libcudart.so.12
+    60: 00000000000025a0   105 FUNC    GLOBAL DEFAULT   10 _Z11cphase_gateP6float2f
+    61: 00000000000036c0   662 FUNC    GLOBAL DEFAULT   10 execute_circuit
+    62: 0000000000002490   117 FUNC    GLOBAL DEFAULT   10 _Z7ad_gateP6float2f
+    63: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND printf@@GLIBC_2.2.5
+    64: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaMalloc@@libcudart.so.12
+    65: 0000000000003400    47 FUNC    GLOBAL DEFAULT   10 _Z4hashPKc
+    66: 0000000000002410   120 FUNC    GLOBAL DEFAULT   10 _Z7pd_gateP6float2f
+    67: 0000000000004550   201 FUNC    GLOBAL DEFAULT   10 _Z50__device_stub__Z18actionOnTripleGateP6float2S0_mPmP6float2S0_mPm
+    68: 0000000000002160    22 FUNC    GLOBAL DEFAULT   10 _Z6y_gateP6float2
+    69: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaLaunchKernel@@libcudart.so.12
+    70: 0000000000002990   101 FUNC    GLOBAL DEFAULT   10 _Z22toff_gate_target_smallP6float2
+    71: 0000000000002120     5 FUNC    GLOBAL DEFAULT   10 _Z7comparePKvS0_
+    72: 000000000020c248     0 NOTYPE  GLOBAL DEFAULT   22 _edata
+    73: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND rand@@GLIBC_2.2.5
+    74: 0000000000003080   416 FUNC    GLOBAL DEFAULT   10 _Z23fred_gate_control_smallP6float2
+    75: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaUnregisterFatBinary@@libcudart.so.12
+    76: 0000000000002ee0   416 FUNC    GLOBAL DEFAULT   10 _Z21fred_gate_control_midP6float2
+    77: 0000000000002650    51 FUNC    GLOBAL DEFAULT   10 _Z23cnot_gate_control_smallP6float2
+    78: 00000000000022b0   106 FUNC    GLOBAL DEFAULT   10 _Z7ry_gateP6float2f
+    79: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND sincosf@@GLIBC_2.2.5
+    80: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@@GLIBC_2.2.5
+    81: 0000000000002d40   416 FUNC    GLOBAL DEFAULT   10 _Z21fred_gate_control_bigP6float2
+    82: 0000000000002940    65 FUNC    GLOBAL DEFAULT   10 _Z8syc_gateP6float2
+    83: 00000000000026d0   197 FUNC    GLOBAL DEFAULT   10 _Z8rxx_gateP6float2f
+    84: 0000000000002a00   402 FUNC    GLOBAL DEFAULT   10 _Z20toff_gate_target_midP6float2
+    85: 0000000000002870   194 FUNC    GLOBAL DEFAULT   10 _Z8rzz_gateP6float2f
+    86: 0000000000004080  1227 FUNC    GLOBAL DEFAULT   10 doubleGateAction
+    87: 0000000000003430    82 FUNC    GLOBAL DEFAULT   10 _Z9isInArrayPPKcPci
+    88: 0000000000002610    51 FUNC    GLOBAL DEFAULT   10 _Z21cnot_gate_control_bigP6float2
+    89: 0000000000002140    23 FUNC    GLOBAL DEFAULT   10 _Z6x_gateP6float2
+    90: 0000000000003290    65 FUNC    GLOBAL DEFAULT   10 _Z20generate_binary_dataf
+    91: 00000000000021a0    23 FUNC    GLOBAL DEFAULT   10 _Z6s_gateP6float2
+    92: 0000000000002380   131 FUNC    GLOBAL DEFAULT   10 _Z11damp_i_gateP6float2f
+    93: 0000000000002550    65 FUNC    GLOBAL DEFAULT   10 _Z10iswap_gateP6float2
+    94: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_atexit@@GLIBC_2.2.5
+    95: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFatBinary@@libcudart.so.12
+    96: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND time@@GLIBC_2.2.5
+    97: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND srand@@GLIBC_2.2.5
+    98: 00000000000021e0    23 FUNC    GLOBAL DEFAULT   10 _Z6t_gateP6float2
+    99: 00000000000034c0   510 FUNC    GLOBAL DEFAULT   10 _Z13normalizationP6float2i
+   100: 0000000000002180    23 FUNC    GLOBAL DEFAULT   10 _Z6z_gateP6float2
+   101: 0000000000004070     5 FUNC    GLOBAL DEFAULT   10 _Z19actionOnDoubleQubitP6float2S0_mPm
+   102: 0000000000003fa0   201 FUNC    GLOBAL DEFAULT   10 _Z51__device_stub__Z19actionOnDoubleQubitP6float2S0_mPmP6float2S0_mPm
+   103: 00000000000032e0   286 FUNC    GLOBAL DEFAULT   10 _Z7getprobP6float2Pfm
+   104: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free@@GLIBC_2.2.5
+   105: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaMemcpy@@libcudart.so.12
+   106: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND exit@@GLIBC_2.2.5
+   107: 0000000000002200    23 FUNC    GLOBAL DEFAULT   10 _Z8tdg_gateP6float2
+   108: 0000000000002690    58 FUNC    GLOBAL DEFAULT   10 _Z7cz_gateP6float2
+   109: 0000000000004620     5 FUNC    GLOBAL DEFAULT   10 _Z18actionOnTripleGateP6float2S0_mPm
+   110: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND malloc@@GLIBC_2.2.5
+   111: 000000000020c258     0 NOTYPE  GLOBAL DEFAULT   23 _end
+   112: 0000000000003960   201 FUNC    GLOBAL DEFAULT   10 _Z51__device_stub__Z19actionOnSingleQubitP6float2S0_mPmP6float2S0_mPm
+   113: 0000000000003490    33 FUNC    GLOBAL DEFAULT   10 _Z14getArrayLengthPi
+   114: 00000000000021c0    23 FUNC    GLOBAL DEFAULT   10 _Z8sdg_gateP6float2
+   115: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strcmp@@GLIBC_2.2.5
+   116: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFunction@@libcudart.so.12
+   117: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaFree@@libcudart.so.12
+   118: 0000000000002ba0   416 FUNC    GLOBAL DEFAULT   10 _Z20toff_gate_target_bigP6float2
+   119: 00000000000027a0   200 FUNC    GLOBAL DEFAULT   10 _Z8ryy_gateP6float2f
+   120: 000000000020c248     0 NOTYPE  GLOBAL DEFAULT   23 __bss_start
+   121: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND puts@@GLIBC_2.2.5
+   122: 0000000000003a40  1373 FUNC    GLOBAL DEFAULT   10 singleGateAction
+   123: 0000000000003a30     5 FUNC    GLOBAL DEFAULT   10 _Z19actionOnSingleQubitP6float2S0_mPm
+   124: 0000000000003220   107 FUNC    GLOBAL DEFAULT   10 _Z11identityMatP6float2i
+   125: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaPopCallConfiguration@@libcudart.so.12
+   126: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaDeviceSynchronize@@libcudart.so.12
+   127: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
+   128: 0000000000002320    94 FUNC    GLOBAL DEFAULT   10 _Z7rz_gateP6float2f
+   129: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaPushCallConfiguration@@libcudart.so.12
+   130: 0000000000002220    22 FUNC    GLOBAL DEFAULT   10 _Z6h_gateP6float2
+   131: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND sqrtf@@GLIBC_2.2.5
+   132: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFatBinaryEnd@@libcudart.so.12
+   133: 0000000000004630  1049 FUNC    GLOBAL DEFAULT   10 tripleGateAction
+   134: 0000000000002510    51 FUNC    GLOBAL DEFAULT   10 _Z9swap_gateP6float2
+   135: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
+   136: 0000000000002240    97 FUNC    GLOBAL DEFAULT   10 _Z7rx_gateP6float2f
+   137: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND qsort@@GLIBC_2.2.5
+   138: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
+   139: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaSetDevice@@libcudart.so.12
```

#### readelf --wide --relocs {}

```diff
@@ -1,87 +1,88 @@
 
-Relocation section '.rela.dyn' at offset 0x1378 contains 16 entries:
+Relocation section '.rela.dyn' at offset 0x13a0 contains 16 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-000000000020bd60  0000000000000008 R_X86_64_RELATIVE                         20c0
-000000000020bd68  0000000000000008 R_X86_64_RELATIVE                         1f50
-000000000020bd70  0000000000000008 R_X86_64_RELATIVE                         2080
-000000000020c220  0000000000000008 R_X86_64_RELATIVE                         20c220
-000000000020c230  0000000000000008 R_X86_64_RELATIVE                         50b8
-000000000020bfa8  0000000b00000006 R_X86_64_GLOB_DAT      00000000000020d0 _Z7comparePKvS0_ + 0
-000000000020bfb0  0000001400000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
-000000000020bfb8  0000001a00000006 R_X86_64_GLOB_DAT      0000000000004030 doubleGateAction + 0
-000000000020bfc0  0000002900000006 R_X86_64_GLOB_DAT      0000000000004020 _Z19actionOnDoubleQubitP6float2S0_mPm + 0
-000000000020bfc8  0000003100000006 R_X86_64_GLOB_DAT      00000000000045b0 _Z18actionOnTripleGateP6float2S0_mPm + 0
-000000000020bfd0  0000003e00000006 R_X86_64_GLOB_DAT      00000000000039f0 singleGateAction + 0
-000000000020bfd8  0000003f00000006 R_X86_64_GLOB_DAT      00000000000039e0 _Z19actionOnSingleQubitP6float2S0_mPm + 0
-000000000020bfe0  0000004300000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
-000000000020bfe8  0000004900000006 R_X86_64_GLOB_DAT      00000000000045c0 tripleGateAction + 0
-000000000020bff0  0000004b00000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
-000000000020bff8  0000004e00000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
+000000000020bd60  0000000000000008 R_X86_64_RELATIVE                         2110
+000000000020bd68  0000000000000008 R_X86_64_RELATIVE                         1fa0
+000000000020bd70  0000000000000008 R_X86_64_RELATIVE                         20d0
+000000000020c228  0000000000000008 R_X86_64_RELATIVE                         20c228
+000000000020c238  0000000000000008 R_X86_64_RELATIVE                         5148
+000000000020bfa8  0000000c00000006 R_X86_64_GLOB_DAT      0000000000002120 _Z7comparePKvS0_ + 0
+000000000020bfb0  0000001500000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
+000000000020bfb8  0000001b00000006 R_X86_64_GLOB_DAT      0000000000004080 doubleGateAction + 0
+000000000020bfc0  0000002a00000006 R_X86_64_GLOB_DAT      0000000000004070 _Z19actionOnDoubleQubitP6float2S0_mPm + 0
+000000000020bfc8  0000003200000006 R_X86_64_GLOB_DAT      0000000000004620 _Z18actionOnTripleGateP6float2S0_mPm + 0
+000000000020bfd0  0000003f00000006 R_X86_64_GLOB_DAT      0000000000003a40 singleGateAction + 0
+000000000020bfd8  0000004000000006 R_X86_64_GLOB_DAT      0000000000003a30 _Z19actionOnSingleQubitP6float2S0_mPm + 0
+000000000020bfe0  0000004400000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
+000000000020bfe8  0000004a00000006 R_X86_64_GLOB_DAT      0000000000004630 tripleGateAction + 0
+000000000020bff0  0000004c00000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
+000000000020bff8  0000004f00000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
 
-Relocation section '.rela.plt' at offset 0x14f8 contains 65 entries:
+Relocation section '.rela.plt' at offset 0x1520 contains 66 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-000000000020c018  0000000100000007 R_X86_64_JUMP_SLOT     0000000000002550 _Z11cphase_gateP6float2f + 0
-000000000020c020  0000000300000007 R_X86_64_JUMP_SLOT     0000000000002440 _Z7ad_gateP6float2f + 0
-000000000020c028  0000000400000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaMalloc@libcudart.so.12 + 0
-000000000020c030  0000000500000007 R_X86_64_JUMP_SLOT     00000000000033b0 _Z4hashPKc + 0
-000000000020c038  0000000600000007 R_X86_64_JUMP_SLOT     00000000000023c0 _Z7pd_gateP6float2f + 0
-000000000020c040  0000000700000007 R_X86_64_JUMP_SLOT     00000000000044e0 _Z50__device_stub__Z18actionOnTripleGateP6float2S0_mPmP6float2S0_mPm + 0
-000000000020c048  0000000800000007 R_X86_64_JUMP_SLOT     0000000000002110 _Z6y_gateP6float2 + 0
-000000000020c050  0000000900000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaLaunchKernel@libcudart.so.12 + 0
-000000000020c058  0000000a00000007 R_X86_64_JUMP_SLOT     0000000000002940 _Z22toff_gate_target_smallP6float2 + 0
-000000000020c060  0000000d00000007 R_X86_64_JUMP_SLOT     0000000000000000 rand@GLIBC_2.2.5 + 0
-000000000020c068  0000000e00000007 R_X86_64_JUMP_SLOT     0000000000003030 _Z23fred_gate_control_smallP6float2 + 0
-000000000020c070  0000000f00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaUnregisterFatBinary@libcudart.so.12 + 0
-000000000020c078  0000001000000007 R_X86_64_JUMP_SLOT     0000000000002e90 _Z21fred_gate_control_midP6float2 + 0
-000000000020c080  0000001100000007 R_X86_64_JUMP_SLOT     0000000000002600 _Z23cnot_gate_control_smallP6float2 + 0
-000000000020c088  0000001200000007 R_X86_64_JUMP_SLOT     0000000000002260 _Z7ry_gateP6float2f + 0
-000000000020c090  0000001300000007 R_X86_64_JUMP_SLOT     0000000000000000 sincosf@GLIBC_2.2.5 + 0
-000000000020c098  0000001400000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
-000000000020c0a0  0000001500000007 R_X86_64_JUMP_SLOT     0000000000002cf0 _Z21fred_gate_control_bigP6float2 + 0
-000000000020c0a8  0000001600000007 R_X86_64_JUMP_SLOT     00000000000028f0 _Z8syc_gateP6float2 + 0
-000000000020c0b0  0000001700000007 R_X86_64_JUMP_SLOT     0000000000002680 _Z8rxx_gateP6float2f + 0
-000000000020c0b8  0000001800000007 R_X86_64_JUMP_SLOT     00000000000029b0 _Z20toff_gate_target_midP6float2 + 0
-000000000020c0c0  0000001900000007 R_X86_64_JUMP_SLOT     0000000000002820 _Z8rzz_gateP6float2f + 0
-000000000020c0c8  0000001b00000007 R_X86_64_JUMP_SLOT     00000000000033e0 _Z9isInArrayPPKcPci + 0
-000000000020c0d0  0000001c00000007 R_X86_64_JUMP_SLOT     00000000000025c0 _Z21cnot_gate_control_bigP6float2 + 0
-000000000020c0d8  0000001d00000007 R_X86_64_JUMP_SLOT     00000000000020f0 _Z6x_gateP6float2 + 0
-000000000020c0e0  0000001f00000007 R_X86_64_JUMP_SLOT     0000000000002150 _Z6s_gateP6float2 + 0
-000000000020c0e8  0000002000000007 R_X86_64_JUMP_SLOT     0000000000002330 _Z11damp_i_gateP6float2f + 0
-000000000020c0f0  0000002100000007 R_X86_64_JUMP_SLOT     0000000000002500 _Z10iswap_gateP6float2 + 0
-000000000020c0f8  0000002200000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_atexit@GLIBC_2.2.5 + 0
-000000000020c100  0000002300000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaRegisterFatBinary@libcudart.so.12 + 0
-000000000020c108  0000002400000007 R_X86_64_JUMP_SLOT     0000000000000000 time@GLIBC_2.2.5 + 0
-000000000020c110  0000002500000007 R_X86_64_JUMP_SLOT     0000000000000000 srand@GLIBC_2.2.5 + 0
-000000000020c118  0000002600000007 R_X86_64_JUMP_SLOT     0000000000002190 _Z6t_gateP6float2 + 0
-000000000020c120  0000002700000007 R_X86_64_JUMP_SLOT     0000000000003470 _Z13normalizationP6float2i + 0
-000000000020c128  0000002800000007 R_X86_64_JUMP_SLOT     0000000000002130 _Z6z_gateP6float2 + 0
-000000000020c130  0000002900000007 R_X86_64_JUMP_SLOT     0000000000004020 _Z19actionOnDoubleQubitP6float2S0_mPm + 0
-000000000020c138  0000002a00000007 R_X86_64_JUMP_SLOT     0000000000003f50 _Z51__device_stub__Z19actionOnDoubleQubitP6float2S0_mPmP6float2S0_mPm + 0
-000000000020c140  0000002c00000007 R_X86_64_JUMP_SLOT     0000000000000000 free@GLIBC_2.2.5 + 0
-000000000020c148  0000002d00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaMemcpy@libcudart.so.12 + 0
-000000000020c150  0000002e00000007 R_X86_64_JUMP_SLOT     0000000000000000 exit@GLIBC_2.2.5 + 0
-000000000020c158  0000002f00000007 R_X86_64_JUMP_SLOT     00000000000021b0 _Z8tdg_gateP6float2 + 0
-000000000020c160  0000003000000007 R_X86_64_JUMP_SLOT     0000000000002640 _Z7cz_gateP6float2 + 0
-000000000020c168  0000003100000007 R_X86_64_JUMP_SLOT     00000000000045b0 _Z18actionOnTripleGateP6float2S0_mPm + 0
-000000000020c170  0000003200000007 R_X86_64_JUMP_SLOT     0000000000000000 malloc@GLIBC_2.2.5 + 0
-000000000020c178  0000003400000007 R_X86_64_JUMP_SLOT     0000000000003910 _Z51__device_stub__Z19actionOnSingleQubitP6float2S0_mPmP6float2S0_mPm + 0
-000000000020c180  0000003500000007 R_X86_64_JUMP_SLOT     0000000000003440 _Z14getArrayLengthPi + 0
-000000000020c188  0000003600000007 R_X86_64_JUMP_SLOT     0000000000002170 _Z8sdg_gateP6float2 + 0
-000000000020c190  0000003700000007 R_X86_64_JUMP_SLOT     0000000000000000 strcmp@GLIBC_2.2.5 + 0
-000000000020c198  0000003800000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaRegisterFunction@libcudart.so.12 + 0
-000000000020c1a0  0000003900000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaFree@libcudart.so.12 + 0
-000000000020c1a8  0000003a00000007 R_X86_64_JUMP_SLOT     0000000000002b50 _Z20toff_gate_target_bigP6float2 + 0
-000000000020c1b0  0000003b00000007 R_X86_64_JUMP_SLOT     0000000000002750 _Z8ryy_gateP6float2f + 0
-000000000020c1b8  0000003d00000007 R_X86_64_JUMP_SLOT     0000000000000000 puts@GLIBC_2.2.5 + 0
-000000000020c1c0  0000003f00000007 R_X86_64_JUMP_SLOT     00000000000039e0 _Z19actionOnSingleQubitP6float2S0_mPm + 0
-000000000020c1c8  0000004100000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaPopCallConfiguration@libcudart.so.12 + 0
-000000000020c1d0  0000004200000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaDeviceSynchronize@libcudart.so.12 + 0
-000000000020c1d8  0000004400000007 R_X86_64_JUMP_SLOT     00000000000022d0 _Z7rz_gateP6float2f + 0
-000000000020c1e0  0000004500000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaPushCallConfiguration@libcudart.so.12 + 0
-000000000020c1e8  0000004600000007 R_X86_64_JUMP_SLOT     00000000000021d0 _Z6h_gateP6float2 + 0
-000000000020c1f0  0000004700000007 R_X86_64_JUMP_SLOT     0000000000000000 sqrtf@GLIBC_2.2.5 + 0
-000000000020c1f8  0000004800000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaRegisterFatBinaryEnd@libcudart.so.12 + 0
-000000000020c200  0000004a00000007 R_X86_64_JUMP_SLOT     00000000000024c0 _Z9swap_gateP6float2 + 0
-000000000020c208  0000004c00000007 R_X86_64_JUMP_SLOT     00000000000021f0 _Z7rx_gateP6float2f + 0
-000000000020c210  0000004d00000007 R_X86_64_JUMP_SLOT     0000000000000000 qsort@GLIBC_2.2.5 + 0
-000000000020c218  0000004f00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaSetDevice@libcudart.so.12 + 0
+000000000020c018  0000000100000007 R_X86_64_JUMP_SLOT     00000000000025a0 _Z11cphase_gateP6float2f + 0
+000000000020c020  0000000300000007 R_X86_64_JUMP_SLOT     0000000000002490 _Z7ad_gateP6float2f + 0
+000000000020c028  0000000400000007 R_X86_64_JUMP_SLOT     0000000000000000 printf@GLIBC_2.2.5 + 0
+000000000020c030  0000000500000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaMalloc@libcudart.so.12 + 0
+000000000020c038  0000000600000007 R_X86_64_JUMP_SLOT     0000000000003400 _Z4hashPKc + 0
+000000000020c040  0000000700000007 R_X86_64_JUMP_SLOT     0000000000002410 _Z7pd_gateP6float2f + 0
+000000000020c048  0000000800000007 R_X86_64_JUMP_SLOT     0000000000004550 _Z50__device_stub__Z18actionOnTripleGateP6float2S0_mPmP6float2S0_mPm + 0
+000000000020c050  0000000900000007 R_X86_64_JUMP_SLOT     0000000000002160 _Z6y_gateP6float2 + 0
+000000000020c058  0000000a00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaLaunchKernel@libcudart.so.12 + 0
+000000000020c060  0000000b00000007 R_X86_64_JUMP_SLOT     0000000000002990 _Z22toff_gate_target_smallP6float2 + 0
+000000000020c068  0000000e00000007 R_X86_64_JUMP_SLOT     0000000000000000 rand@GLIBC_2.2.5 + 0
+000000000020c070  0000000f00000007 R_X86_64_JUMP_SLOT     0000000000003080 _Z23fred_gate_control_smallP6float2 + 0
+000000000020c078  0000001000000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaUnregisterFatBinary@libcudart.so.12 + 0
+000000000020c080  0000001100000007 R_X86_64_JUMP_SLOT     0000000000002ee0 _Z21fred_gate_control_midP6float2 + 0
+000000000020c088  0000001200000007 R_X86_64_JUMP_SLOT     0000000000002650 _Z23cnot_gate_control_smallP6float2 + 0
+000000000020c090  0000001300000007 R_X86_64_JUMP_SLOT     00000000000022b0 _Z7ry_gateP6float2f + 0
+000000000020c098  0000001400000007 R_X86_64_JUMP_SLOT     0000000000000000 sincosf@GLIBC_2.2.5 + 0
+000000000020c0a0  0000001500000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
+000000000020c0a8  0000001600000007 R_X86_64_JUMP_SLOT     0000000000002d40 _Z21fred_gate_control_bigP6float2 + 0
+000000000020c0b0  0000001700000007 R_X86_64_JUMP_SLOT     0000000000002940 _Z8syc_gateP6float2 + 0
+000000000020c0b8  0000001800000007 R_X86_64_JUMP_SLOT     00000000000026d0 _Z8rxx_gateP6float2f + 0
+000000000020c0c0  0000001900000007 R_X86_64_JUMP_SLOT     0000000000002a00 _Z20toff_gate_target_midP6float2 + 0
+000000000020c0c8  0000001a00000007 R_X86_64_JUMP_SLOT     0000000000002870 _Z8rzz_gateP6float2f + 0
+000000000020c0d0  0000001c00000007 R_X86_64_JUMP_SLOT     0000000000003430 _Z9isInArrayPPKcPci + 0
+000000000020c0d8  0000001d00000007 R_X86_64_JUMP_SLOT     0000000000002610 _Z21cnot_gate_control_bigP6float2 + 0
+000000000020c0e0  0000001e00000007 R_X86_64_JUMP_SLOT     0000000000002140 _Z6x_gateP6float2 + 0
+000000000020c0e8  0000002000000007 R_X86_64_JUMP_SLOT     00000000000021a0 _Z6s_gateP6float2 + 0
+000000000020c0f0  0000002100000007 R_X86_64_JUMP_SLOT     0000000000002380 _Z11damp_i_gateP6float2f + 0
+000000000020c0f8  0000002200000007 R_X86_64_JUMP_SLOT     0000000000002550 _Z10iswap_gateP6float2 + 0
+000000000020c100  0000002300000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_atexit@GLIBC_2.2.5 + 0
+000000000020c108  0000002400000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaRegisterFatBinary@libcudart.so.12 + 0
+000000000020c110  0000002500000007 R_X86_64_JUMP_SLOT     0000000000000000 time@GLIBC_2.2.5 + 0
+000000000020c118  0000002600000007 R_X86_64_JUMP_SLOT     0000000000000000 srand@GLIBC_2.2.5 + 0
+000000000020c120  0000002700000007 R_X86_64_JUMP_SLOT     00000000000021e0 _Z6t_gateP6float2 + 0
+000000000020c128  0000002800000007 R_X86_64_JUMP_SLOT     00000000000034c0 _Z13normalizationP6float2i + 0
+000000000020c130  0000002900000007 R_X86_64_JUMP_SLOT     0000000000002180 _Z6z_gateP6float2 + 0
+000000000020c138  0000002a00000007 R_X86_64_JUMP_SLOT     0000000000004070 _Z19actionOnDoubleQubitP6float2S0_mPm + 0
+000000000020c140  0000002b00000007 R_X86_64_JUMP_SLOT     0000000000003fa0 _Z51__device_stub__Z19actionOnDoubleQubitP6float2S0_mPmP6float2S0_mPm + 0
+000000000020c148  0000002d00000007 R_X86_64_JUMP_SLOT     0000000000000000 free@GLIBC_2.2.5 + 0
+000000000020c150  0000002e00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaMemcpy@libcudart.so.12 + 0
+000000000020c158  0000002f00000007 R_X86_64_JUMP_SLOT     0000000000000000 exit@GLIBC_2.2.5 + 0
+000000000020c160  0000003000000007 R_X86_64_JUMP_SLOT     0000000000002200 _Z8tdg_gateP6float2 + 0
+000000000020c168  0000003100000007 R_X86_64_JUMP_SLOT     0000000000002690 _Z7cz_gateP6float2 + 0
+000000000020c170  0000003200000007 R_X86_64_JUMP_SLOT     0000000000004620 _Z18actionOnTripleGateP6float2S0_mPm + 0
+000000000020c178  0000003300000007 R_X86_64_JUMP_SLOT     0000000000000000 malloc@GLIBC_2.2.5 + 0
+000000000020c180  0000003500000007 R_X86_64_JUMP_SLOT     0000000000003960 _Z51__device_stub__Z19actionOnSingleQubitP6float2S0_mPmP6float2S0_mPm + 0
+000000000020c188  0000003600000007 R_X86_64_JUMP_SLOT     0000000000003490 _Z14getArrayLengthPi + 0
+000000000020c190  0000003700000007 R_X86_64_JUMP_SLOT     00000000000021c0 _Z8sdg_gateP6float2 + 0
+000000000020c198  0000003800000007 R_X86_64_JUMP_SLOT     0000000000000000 strcmp@GLIBC_2.2.5 + 0
+000000000020c1a0  0000003900000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaRegisterFunction@libcudart.so.12 + 0
+000000000020c1a8  0000003a00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaFree@libcudart.so.12 + 0
+000000000020c1b0  0000003b00000007 R_X86_64_JUMP_SLOT     0000000000002ba0 _Z20toff_gate_target_bigP6float2 + 0
+000000000020c1b8  0000003c00000007 R_X86_64_JUMP_SLOT     00000000000027a0 _Z8ryy_gateP6float2f + 0
+000000000020c1c0  0000003e00000007 R_X86_64_JUMP_SLOT     0000000000000000 puts@GLIBC_2.2.5 + 0
+000000000020c1c8  0000004000000007 R_X86_64_JUMP_SLOT     0000000000003a30 _Z19actionOnSingleQubitP6float2S0_mPm + 0
+000000000020c1d0  0000004200000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaPopCallConfiguration@libcudart.so.12 + 0
+000000000020c1d8  0000004300000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaDeviceSynchronize@libcudart.so.12 + 0
+000000000020c1e0  0000004500000007 R_X86_64_JUMP_SLOT     0000000000002320 _Z7rz_gateP6float2f + 0
+000000000020c1e8  0000004600000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaPushCallConfiguration@libcudart.so.12 + 0
+000000000020c1f0  0000004700000007 R_X86_64_JUMP_SLOT     0000000000002220 _Z6h_gateP6float2 + 0
+000000000020c1f8  0000004800000007 R_X86_64_JUMP_SLOT     0000000000000000 sqrtf@GLIBC_2.2.5 + 0
+000000000020c200  0000004900000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaRegisterFatBinaryEnd@libcudart.so.12 + 0
+000000000020c208  0000004b00000007 R_X86_64_JUMP_SLOT     0000000000002510 _Z9swap_gateP6float2 + 0
+000000000020c210  0000004d00000007 R_X86_64_JUMP_SLOT     0000000000002240 _Z7rx_gateP6float2f + 0
+000000000020c218  0000004e00000007 R_X86_64_JUMP_SLOT     0000000000000000 qsort@GLIBC_2.2.5 + 0
+000000000020c220  0000005000000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaSetDevice@libcudart.so.12 + 0
```

#### readelf --wide --dynamic {}

```diff
@@ -5,30 +5,30 @@
  0x0000000000000001 (NEEDED)             Shared library: [librt.so.1]
  0x0000000000000001 (NEEDED)             Shared library: [libpthread.so.0]
  0x0000000000000001 (NEEDED)             Shared library: [libdl.so.2]
  0x0000000000000001 (NEEDED)             Shared library: [libstdc++.so.6]
  0x0000000000000001 (NEEDED)             Shared library: [libm.so.6]
  0x0000000000000001 (NEEDED)             Shared library: [libgcc_s.so.1]
  0x0000000000000001 (NEEDED)             Shared library: [libc.so.6]
- 0x000000000000000c (INIT)               0x1b10
- 0x000000000000000d (FINI)               0x49f0
+ 0x000000000000000c (INIT)               0x1b50
+ 0x000000000000000d (FINI)               0x4a60
  0x0000000000000019 (INIT_ARRAY)         0x20bd60
  0x000000000000001b (INIT_ARRAYSZ)       16 (bytes)
  0x000000000000001a (FINI_ARRAY)         0x20bd70
  0x000000000000001c (FINI_ARRAYSZ)       8 (bytes)
  0x0000000000000004 (HASH)               0x190
- 0x0000000000000005 (STRTAB)             0xb68
+ 0x0000000000000005 (STRTAB)             0xb80
  0x0000000000000006 (SYMTAB)             0x3e8
- 0x000000000000000a (STRSZ)              1808 (bytes)
+ 0x000000000000000a (STRSZ)              1815 (bytes)
  0x000000000000000b (SYMENT)             24 (bytes)
  0x0000000000000003 (PLTGOT)             0x20c000
- 0x0000000000000002 (PLTRELSZ)           1560 (bytes)
+ 0x0000000000000002 (PLTRELSZ)           1584 (bytes)
  0x0000000000000014 (PLTREL)             RELA
- 0x0000000000000017 (JMPREL)             0x14f8
- 0x0000000000000007 (RELA)               0x1378
+ 0x0000000000000017 (JMPREL)             0x1520
+ 0x0000000000000007 (RELA)               0x13a0
  0x0000000000000008 (RELASZ)             384 (bytes)
  0x0000000000000009 (RELAENT)            24 (bytes)
- 0x000000006ffffffe (VERNEED)            0x1318
+ 0x000000006ffffffe (VERNEED)            0x1340
  0x000000006fffffff (VERNEEDNUM)         3
- 0x000000006ffffff0 (VERSYM)             0x1278
+ 0x000000006ffffff0 (VERSYM)             0x1298
  0x000000006ffffff9 (RELACOUNT)          5
  0x0000000000000000 (NULL)               0x0
```

#### readelf --wide --version-info {}

```diff
@@ -1,32 +1,33 @@
 
-Version symbols section '.gnu.version' contains 80 entries:
- Addr: 0x0000000000001278  Offset: 0x00001278  Link: 2 (.dynsym)
+Version symbols section '.gnu.version' contains 81 entries:
+ Addr: 0x0000000000001298  Offset: 0x00001298  Link: 2 (.dynsym)
   000:   0 (*local*)       1 (*global*)      1 (*global*)      1 (*global*)   
-  004:   2 (libcudart.so.12)     1 (*global*)      1 (*global*)      1 (*global*)   
-  008:   1 (*global*)      2 (libcudart.so.12)     1 (*global*)      1 (*global*)   
-  00c:   1 (*global*)      3 (GLIBC_2.2.5)   1 (*global*)      2 (libcudart.so.12)  
-  010:   1 (*global*)      1 (*global*)      1 (*global*)      4 (GLIBC_2.2.5)
-  014:   3 (GLIBC_2.2.5)   1 (*global*)      1 (*global*)      1 (*global*)   
+  004:   2 (GLIBC_2.2.5)   3 (libcudart.so.12)     1 (*global*)      1 (*global*)   
+  008:   1 (*global*)      1 (*global*)      3 (libcudart.so.12)     1 (*global*)   
+  00c:   1 (*global*)      1 (*global*)      2 (GLIBC_2.2.5)   1 (*global*)   
+  010:   3 (libcudart.so.12)     1 (*global*)      1 (*global*)      1 (*global*)   
+  014:   4 (GLIBC_2.2.5)   2 (GLIBC_2.2.5)   1 (*global*)      1 (*global*)   
   018:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   01c:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
-  020:   1 (*global*)      1 (*global*)      3 (GLIBC_2.2.5)   2 (libcudart.so.12)  
-  024:   3 (GLIBC_2.2.5)   3 (GLIBC_2.2.5)   1 (*global*)      1 (*global*)   
+  020:   1 (*global*)      1 (*global*)      1 (*global*)      2 (GLIBC_2.2.5)
+  024:   3 (libcudart.so.12)     2 (GLIBC_2.2.5)   2 (GLIBC_2.2.5)   1 (*global*)   
   028:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
-  02c:   3 (GLIBC_2.2.5)   2 (libcudart.so.12)     3 (GLIBC_2.2.5)   1 (*global*)   
-  030:   1 (*global*)      1 (*global*)      3 (GLIBC_2.2.5)   1 (*global*)   
-  034:   1 (*global*)      1 (*global*)      1 (*global*)      3 (GLIBC_2.2.5)
-  038:   2 (libcudart.so.12)     2 (libcudart.so.12)     1 (*global*)      1 (*global*)   
-  03c:   1 (*global*)      3 (GLIBC_2.2.5)   1 (*global*)      1 (*global*)   
-  040:   1 (*global*)      2 (libcudart.so.12)     2 (libcudart.so.12)     0 (*local*)    
-  044:   1 (*global*)      2 (libcudart.so.12)     1 (*global*)      4 (GLIBC_2.2.5)
-  048:   2 (libcudart.so.12)     1 (*global*)      1 (*global*)      0 (*local*)    
-  04c:   1 (*global*)      3 (GLIBC_2.2.5)   0 (*local*)       2 (libcudart.so.12)  
+  02c:   1 (*global*)      2 (GLIBC_2.2.5)   3 (libcudart.so.12)     2 (GLIBC_2.2.5)
+  030:   1 (*global*)      1 (*global*)      1 (*global*)      2 (GLIBC_2.2.5)
+  034:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
+  038:   2 (GLIBC_2.2.5)   3 (libcudart.so.12)     3 (libcudart.so.12)     1 (*global*)   
+  03c:   1 (*global*)      1 (*global*)      2 (GLIBC_2.2.5)   1 (*global*)   
+  040:   1 (*global*)      1 (*global*)      3 (libcudart.so.12)     3 (libcudart.so.12)  
+  044:   0 (*local*)       1 (*global*)      3 (libcudart.so.12)     1 (*global*)   
+  048:   4 (GLIBC_2.2.5)   3 (libcudart.so.12)     1 (*global*)      1 (*global*)   
+  04c:   0 (*local*)       1 (*global*)      2 (GLIBC_2.2.5)   0 (*local*)    
+  050:   3 (libcudart.so.12)  
 
 Version needs section '.gnu.version_r' contains 3 entries:
- Addr: 0x0000000000001318  Offset: 0x00001318  Link: 3 (.dynstr)
+ Addr: 0x0000000000001340  Offset: 0x00001340  Link: 3 (.dynstr)
   000000: Version: 1  File: libm.so.6  Cnt: 1
   0x0010:   Name: GLIBC_2.2.5  Flags: none  Version: 4
-  0x0020: Version: 1  File: libc.so.6  Cnt: 1
-  0x0030:   Name: GLIBC_2.2.5  Flags: none  Version: 3
-  0x0040: Version: 1  File: libcudart.so.12  Cnt: 1
-  0x0050:   Name: libcudart.so.12  Flags: none  Version: 2
+  0x0020: Version: 1  File: libcudart.so.12  Cnt: 1
+  0x0030:   Name: libcudart.so.12  Flags: none  Version: 3
+  0x0040: Version: 1  File: libc.so.6  Cnt: 1
+  0x0050:   Name: GLIBC_2.2.5  Flags: none  Version: 2
```

#### readelf --wide --debug-dump=rawline {}

```diff
@@ -28,28 +28,28 @@
   1	../sysdeps/x86_64
 
  The File Name Table (offset 0x2e):
   Entry	Dir	Time	Size	Name
   1	1	0	0	crti.S
 
  Line Number Statements:
-  [0x00000039]  Extended opcode 2: set Address to 0x1b10
+  [0x00000039]  Extended opcode 2: set Address to 0x1b50
   [0x00000044]  Advance Line by 65 to 66
   [0x00000047]  Copy
-  [0x00000048]  Special opcode 63: advance Address by 4 to 0x1b14 and Line by 2 to 68
-  [0x00000049]  Special opcode 104: advance Address by 7 to 0x1b1b and Line by 1 to 69
-  [0x0000004a]  Special opcode 48: advance Address by 3 to 0x1b1e and Line by 1 to 70
-  [0x0000004b]  Special opcode 34: advance Address by 2 to 0x1b20 and Line by 1 to 71
-  [0x0000004c]  Advance PC by 2 to 0x1b22
+  [0x00000048]  Special opcode 63: advance Address by 4 to 0x1b54 and Line by 2 to 68
+  [0x00000049]  Special opcode 104: advance Address by 7 to 0x1b5b and Line by 1 to 69
+  [0x0000004a]  Special opcode 48: advance Address by 3 to 0x1b5e and Line by 1 to 70
+  [0x0000004b]  Special opcode 34: advance Address by 2 to 0x1b60 and Line by 1 to 71
+  [0x0000004c]  Advance PC by 2 to 0x1b62
   [0x0000004e]  Extended opcode 1: End of Sequence
 
-  [0x00000051]  Extended opcode 2: set Address to 0x49f0
+  [0x00000051]  Extended opcode 2: set Address to 0x4a60
   [0x0000005c]  Advance Line by 83 to 84
   [0x0000005f]  Copy
-  [0x00000060]  Advance PC by 4 to 0x49f4
+  [0x00000060]  Advance PC by 4 to 0x4a64
   [0x00000062]  Extended opcode 1: End of Sequence
 
 
   Offset:                      0x65
   Length:                      999
   DWARF Version:               2
   Prologue Length:             965
@@ -138,23 +138,23 @@
   37	13	0	0	internaltypes.h
   38	13	0	0	pthread-functions.h
   39	13	0	0	libc-lockP.h
   40	0	0	0	exit.h
 
  Line Number Statements:
   [0x00000434]  Set column to 1
-  [0x00000436]  Extended opcode 2: set Address to 0x49e0
+  [0x00000436]  Extended opcode 2: set Address to 0x4a50
   [0x00000441]  Advance Line by 44 to 45
   [0x00000443]  Copy
   [0x00000444]  Set column to 3
-  [0x00000446]  Special opcode 6: advance Address by 0 to 0x49e0 and Line by 1 to 46 (view 1)
+  [0x00000446]  Special opcode 6: advance Address by 0 to 0x4a50 and Line by 1 to 46 (view 1)
   [0x00000447]  Set column to 10
   [0x00000449]  Set is_stmt to 0
   [0x0000044a]  Copy (view 2)
-  [0x0000044b]  Advance PC by 14 to 0x49ee
+  [0x0000044b]  Advance PC by 14 to 0x4a5e
   [0x0000044d]  Extended opcode 1: End of Sequence
 
 
   Offset:                      0x450
   Length:                      93
   DWARF Version:               2
   Prologue Length:             47
@@ -182,22 +182,22 @@
   1	../sysdeps/x86_64
 
  The File Name Table (offset 0x47e):
   Entry	Dir	Time	Size	Name
   1	1	0	0	crtn.S
 
  Line Number Statements:
-  [0x00000489]  Extended opcode 2: set Address to 0x1b22
+  [0x00000489]  Extended opcode 2: set Address to 0x1b62
   [0x00000494]  Advance Line by 39 to 40
   [0x00000496]  Copy
-  [0x00000497]  Special opcode 62: advance Address by 4 to 0x1b26 and Line by 1 to 41
-  [0x00000498]  Advance PC by 1 to 0x1b27
+  [0x00000497]  Special opcode 62: advance Address by 4 to 0x1b66 and Line by 1 to 41
+  [0x00000498]  Advance PC by 1 to 0x1b67
   [0x0000049a]  Extended opcode 1: End of Sequence
 
-  [0x0000049d]  Extended opcode 2: set Address to 0x49f4
+  [0x0000049d]  Extended opcode 2: set Address to 0x4a64
   [0x000004a8]  Advance Line by 43 to 44
   [0x000004aa]  Copy
-  [0x000004ab]  Special opcode 62: advance Address by 4 to 0x49f8 and Line by 1 to 45
-  [0x000004ac]  Advance PC by 1 to 0x49f9
+  [0x000004ab]  Special opcode 62: advance Address by 4 to 0x4a68 and Line by 1 to 45
+  [0x000004ac]  Advance PC by 1 to 0x4a69
   [0x000004ae]  Extended opcode 1: End of Sequence
```

#### readelf --wide --debug-dump=info {}

```diff
@@ -18,15 +18,15 @@
    Abbrev Offset: 0x12
    Pointer Size:  8
  <0><5a>: Abbrev Number: 1 (DW_TAG_compile_unit)
     <5b>   DW_AT_producer    : (strp) (offset: 0x987): GNU C11 9.3.0 -mtune=generic -march=x86-64 -g -O2 -std=gnu11 -fgnu89-inline -fmerge-all-constants -frounding-math -fno-stack-protector -fmath-errno -fPIC -ftls-model=initial-exec
     <5f>   DW_AT_language    : (data1) 12	(ANSI C99)
     <60>   DW_AT_name        : (strp) (offset: 0x763): atexit.c
     <64>   DW_AT_comp_dir    : (strp) (offset: 0x4b2): /opt/glibc-2.31/stdlib
-    <68>   DW_AT_low_pc      : (addr) 0x49e0
+    <68>   DW_AT_low_pc      : (addr) 0x4a50
     <70>   DW_AT_high_pc     : (data8) 0xe
     <78>   DW_AT_stmt_list   : (sec_offset) 0x65
  <1><7c>: Abbrev Number: 2 (DW_TAG_base_type)
     <7d>   DW_AT_byte_size   : (data1) 8
     <7e>   DW_AT_encoding    : (data1) 5	(signed)
     <7f>   DW_AT_name        : (strp) (offset: 0x890): long int
  <1><83>: Abbrev Number: 3 (DW_TAG_typedef)
@@ -3992,28 +3992,28 @@
     <1e4c>   DW_AT_external    : (flag_present) 1
     <1e4c>   DW_AT_name        : (strp) (offset: 0x5e8): atexit
     <1e50>   DW_AT_decl_file   : (data1) 1
     <1e51>   DW_AT_decl_line   : (data1) 44
     <1e52>   DW_AT_decl_column : (data1) 1
     <1e53>   DW_AT_prototyped  : (flag_present) 1
     <1e53>   DW_AT_type        : (ref4) <0x96>, int
-    <1e57>   DW_AT_low_pc      : (addr) 0x49e0
+    <1e57>   DW_AT_low_pc      : (addr) 0x4a50
     <1e5f>   DW_AT_high_pc     : (data8) 0xe
     <1e67>   DW_AT_frame_base  : (exprloc) 1 byte block: 9c 	(DW_OP_call_frame_cfa)
     <1e69>   DW_AT_GNU_all_call_sites: (flag_present) 1
     <1e69>   DW_AT_sibling     : (ref4) <0x1e98>
  <2><1e6d>: Abbrev Number: 57 (DW_TAG_formal_parameter)
     <1e6e>   DW_AT_name        : (strp) (offset: 0x29c): func
     <1e72>   DW_AT_decl_file   : (data1) 1
     <1e73>   DW_AT_decl_line   : (data1) 44
     <1e74>   DW_AT_decl_column : (data1) 16
     <1e75>   DW_AT_type        : (ref4) <0xac4>
     <1e79>   DW_AT_location    : (sec_offset) 0 (location list)
  <2><1e7d>: Abbrev Number: 58 (DW_TAG_GNU_call_site)
-    <1e7e>   DW_AT_low_pc      : (addr) 0x49ee
+    <1e7e>   DW_AT_low_pc      : (addr) 0x4a5e
     <1e86>   DW_AT_GNU_tail_call: (flag_present) 1
     <1e86>   DW_AT_abstract_origin: (ref4) <0x1e98>
  <3><1e8a>: Abbrev Number: 59 (DW_TAG_GNU_call_site_parameter)
     <1e8b>   DW_AT_location    : (exprloc) 1 byte block: 55 	(DW_OP_reg5 (rdi))
     <1e8d>   DW_AT_GNU_call_site_value: (exprloc) 3 byte block: f3 1 55 	(DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)))
  <3><1e91>: Abbrev Number: 59 (DW_TAG_GNU_call_site_parameter)
     <1e92>   DW_AT_location    : (exprloc) 1 byte block: 54 	(DW_OP_reg4 (rsi))
```

#### readelf --wide --debug-dump=aranges {}

```diff
@@ -3,30 +3,30 @@
   Length:                   60
   Version:                  2
   Offset into .debug_info:  0
   Pointer Size:             8
   Segment Size:             0
 
     Address            Length
-    0000000000001b10 0000000000000012
-    00000000000049f0 0000000000000004
+    0000000000001b50 0000000000000012
+    0000000000004a60 0000000000000004
     0000000000000000 0000000000000000
   Length:                   44
   Version:                  2
   Offset into .debug_info:  0x4f
   Pointer Size:             8
   Segment Size:             0
 
     Address            Length
-    00000000000049e0 000000000000000e
+    0000000000004a50 000000000000000e
     0000000000000000 0000000000000000
   Length:                   60
   Version:                  2
   Offset into .debug_info:  0x1ea5
   Pointer Size:             8
   Segment Size:             0
 
     Address            Length
-    0000000000001b22 0000000000000005
-    00000000000049f4 0000000000000005
+    0000000000001b62 0000000000000005
+    0000000000004a64 0000000000000005
     0000000000000000 0000000000000000
```

#### readelf --wide --debug-dump=frames {}

```diff
@@ -9,714 +9,714 @@
   Return address column: 16
   Augmentation data:     1b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_offset: r16 (rip) at cfa-8
   DW_CFA_nop
   DW_CFA_nop
 
-00000018 0000000000000024 0000001c FDE cie=00000000 pc=0000000000001b30..0000000000001f50
+00000018 0000000000000024 0000001c FDE cie=00000000 pc=0000000000001b70..0000000000001fa0
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 6 to 0000000000001b36
+  DW_CFA_advance_loc: 6 to 0000000000001b76
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 10 to 0000000000001b40
+  DW_CFA_advance_loc: 10 to 0000000000001b80
   DW_CFA_def_cfa_expression (DW_OP_breg7 (rsp): 8; DW_OP_breg16 (rip): 0; DW_OP_lit15; DW_OP_and; DW_OP_lit11; DW_OP_ge; DW_OP_lit3; DW_OP_shl; DW_OP_plus)
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000040 0000000000000014 00000044 FDE cie=00000000 pc=00000000000020d0..00000000000020d5
+00000040 0000000000000014 00000044 FDE cie=00000000 pc=0000000000002120..0000000000002125
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000058 0000000000000014 0000005c FDE cie=00000000 pc=00000000000020e0..00000000000020ec
+00000058 0000000000000014 0000005c FDE cie=00000000 pc=0000000000002130..000000000000213c
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000070 0000000000000014 00000074 FDE cie=00000000 pc=00000000000020f0..0000000000002107
+00000070 0000000000000014 00000074 FDE cie=00000000 pc=0000000000002140..0000000000002157
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000088 0000000000000014 0000008c FDE cie=00000000 pc=0000000000002110..0000000000002126
+00000088 0000000000000014 0000008c FDE cie=00000000 pc=0000000000002160..0000000000002176
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000000a0 0000000000000014 000000a4 FDE cie=00000000 pc=0000000000002130..0000000000002147
+000000a0 0000000000000014 000000a4 FDE cie=00000000 pc=0000000000002180..0000000000002197
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000000b8 0000000000000014 000000bc FDE cie=00000000 pc=0000000000002150..0000000000002167
+000000b8 0000000000000014 000000bc FDE cie=00000000 pc=00000000000021a0..00000000000021b7
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000000d0 0000000000000014 000000d4 FDE cie=00000000 pc=0000000000002170..0000000000002187
+000000d0 0000000000000014 000000d4 FDE cie=00000000 pc=00000000000021c0..00000000000021d7
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000000e8 0000000000000014 000000ec FDE cie=00000000 pc=0000000000002190..00000000000021a7
+000000e8 0000000000000014 000000ec FDE cie=00000000 pc=00000000000021e0..00000000000021f7
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000100 0000000000000014 00000104 FDE cie=00000000 pc=00000000000021b0..00000000000021c7
+00000100 0000000000000014 00000104 FDE cie=00000000 pc=0000000000002200..0000000000002217
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000118 0000000000000014 0000011c FDE cie=00000000 pc=00000000000021d0..00000000000021e6
+00000118 0000000000000014 0000011c FDE cie=00000000 pc=0000000000002220..0000000000002236
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000130 000000000000001c 00000134 FDE cie=00000000 pc=00000000000021f0..0000000000002251
-  DW_CFA_advance_loc: 1 to 00000000000021f1
+00000130 000000000000001c 00000134 FDE cie=00000000 pc=0000000000002240..00000000000022a1
+  DW_CFA_advance_loc: 1 to 0000000000002241
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r3 (rbx) at cfa-16
-  DW_CFA_advance_loc: 7 to 00000000000021f8
+  DW_CFA_advance_loc: 7 to 0000000000002248
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc1: 87 to 000000000000224f
+  DW_CFA_advance_loc1: 87 to 000000000000229f
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 0000000000002250
+  DW_CFA_advance_loc: 1 to 00000000000022a0
   DW_CFA_def_cfa_offset: 8
 
-00000150 000000000000001c 00000154 FDE cie=00000000 pc=0000000000002260..00000000000022ca
-  DW_CFA_advance_loc: 1 to 0000000000002261
+00000150 000000000000001c 00000154 FDE cie=00000000 pc=00000000000022b0..000000000000231a
+  DW_CFA_advance_loc: 1 to 00000000000022b1
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r3 (rbx) at cfa-16
-  DW_CFA_advance_loc: 7 to 0000000000002268
+  DW_CFA_advance_loc: 7 to 00000000000022b8
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc1: 96 to 00000000000022c8
+  DW_CFA_advance_loc1: 96 to 0000000000002318
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 00000000000022c9
+  DW_CFA_advance_loc: 1 to 0000000000002319
   DW_CFA_def_cfa_offset: 8
 
-00000170 000000000000001c 00000174 FDE cie=00000000 pc=00000000000022d0..000000000000232e
-  DW_CFA_advance_loc: 1 to 00000000000022d1
+00000170 000000000000001c 00000174 FDE cie=00000000 pc=0000000000002320..000000000000237e
+  DW_CFA_advance_loc: 1 to 0000000000002321
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r3 (rbx) at cfa-16
-  DW_CFA_advance_loc: 7 to 00000000000022d8
+  DW_CFA_advance_loc: 7 to 0000000000002328
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc1: 84 to 000000000000232c
+  DW_CFA_advance_loc1: 84 to 000000000000237c
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 000000000000232d
+  DW_CFA_advance_loc: 1 to 000000000000237d
   DW_CFA_def_cfa_offset: 8
 
-00000190 0000000000000014 00000194 FDE cie=00000000 pc=0000000000002330..00000000000023b3
-  DW_CFA_advance_loc1: 84 to 0000000000002384
+00000190 0000000000000014 00000194 FDE cie=00000000 pc=0000000000002380..0000000000002403
+  DW_CFA_advance_loc1: 84 to 00000000000023d4
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 46 to 00000000000023b2
+  DW_CFA_advance_loc: 46 to 0000000000002402
   DW_CFA_def_cfa_offset: 8
 
-000001a8 0000000000000014 000001ac FDE cie=00000000 pc=00000000000023c0..0000000000002438
-  DW_CFA_advance_loc1: 76 to 000000000000240c
+000001a8 0000000000000014 000001ac FDE cie=00000000 pc=0000000000002410..0000000000002488
+  DW_CFA_advance_loc1: 76 to 000000000000245c
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 43 to 0000000000002437
+  DW_CFA_advance_loc: 43 to 0000000000002487
   DW_CFA_def_cfa_offset: 8
 
-000001c0 000000000000001c 000001c4 FDE cie=00000000 pc=0000000000002440..00000000000024b5
-  DW_CFA_advance_loc: 36 to 0000000000002464
+000001c0 000000000000001c 000001c4 FDE cie=00000000 pc=0000000000002490..0000000000002505
+  DW_CFA_advance_loc: 36 to 00000000000024b4
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 51 to 0000000000002497
+  DW_CFA_advance_loc: 51 to 00000000000024e7
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000000000002498
+  DW_CFA_advance_loc: 1 to 00000000000024e8
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000001e0 0000000000000014 000001e4 FDE cie=00000000 pc=00000000000024c0..00000000000024f3
+000001e0 0000000000000014 000001e4 FDE cie=00000000 pc=0000000000002510..0000000000002543
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000001f8 0000000000000014 000001fc FDE cie=00000000 pc=0000000000002500..0000000000002541
+000001f8 0000000000000014 000001fc FDE cie=00000000 pc=0000000000002550..0000000000002591
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000210 000000000000001c 00000214 FDE cie=00000000 pc=0000000000002550..00000000000025b9
-  DW_CFA_advance_loc: 1 to 0000000000002551
+00000210 000000000000001c 00000214 FDE cie=00000000 pc=00000000000025a0..0000000000002609
+  DW_CFA_advance_loc: 1 to 00000000000025a1
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r3 (rbx) at cfa-16
-  DW_CFA_advance_loc: 7 to 0000000000002558
+  DW_CFA_advance_loc: 7 to 00000000000025a8
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc1: 95 to 00000000000025b7
+  DW_CFA_advance_loc1: 95 to 0000000000002607
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 00000000000025b8
+  DW_CFA_advance_loc: 1 to 0000000000002608
   DW_CFA_def_cfa_offset: 8
 
-00000230 0000000000000014 00000234 FDE cie=00000000 pc=00000000000025c0..00000000000025f3
+00000230 0000000000000014 00000234 FDE cie=00000000 pc=0000000000002610..0000000000002643
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000248 0000000000000014 0000024c FDE cie=00000000 pc=0000000000002600..0000000000002633
+00000248 0000000000000014 0000024c FDE cie=00000000 pc=0000000000002650..0000000000002683
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000260 0000000000000014 00000264 FDE cie=00000000 pc=0000000000002640..000000000000267a
+00000260 0000000000000014 00000264 FDE cie=00000000 pc=0000000000002690..00000000000026ca
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000278 000000000000001c 0000027c FDE cie=00000000 pc=0000000000002680..0000000000002745
-  DW_CFA_advance_loc: 1 to 0000000000002681
+00000278 000000000000001c 0000027c FDE cie=00000000 pc=00000000000026d0..0000000000002795
+  DW_CFA_advance_loc: 1 to 00000000000026d1
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r3 (rbx) at cfa-16
-  DW_CFA_advance_loc: 7 to 0000000000002688
+  DW_CFA_advance_loc: 7 to 00000000000026d8
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc1: 187 to 0000000000002743
+  DW_CFA_advance_loc1: 187 to 0000000000002793
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 0000000000002744
+  DW_CFA_advance_loc: 1 to 0000000000002794
   DW_CFA_def_cfa_offset: 8
 
-00000298 000000000000001c 0000029c FDE cie=00000000 pc=0000000000002750..0000000000002818
-  DW_CFA_advance_loc: 1 to 0000000000002751
+00000298 000000000000001c 0000029c FDE cie=00000000 pc=00000000000027a0..0000000000002868
+  DW_CFA_advance_loc: 1 to 00000000000027a1
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r3 (rbx) at cfa-16
-  DW_CFA_advance_loc: 7 to 0000000000002758
+  DW_CFA_advance_loc: 7 to 00000000000027a8
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc1: 190 to 0000000000002816
+  DW_CFA_advance_loc1: 190 to 0000000000002866
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 0000000000002817
+  DW_CFA_advance_loc: 1 to 0000000000002867
   DW_CFA_def_cfa_offset: 8
 
-000002b8 000000000000001c 000002bc FDE cie=00000000 pc=0000000000002820..00000000000028e2
-  DW_CFA_advance_loc: 1 to 0000000000002821
+000002b8 000000000000001c 000002bc FDE cie=00000000 pc=0000000000002870..0000000000002932
+  DW_CFA_advance_loc: 1 to 0000000000002871
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r3 (rbx) at cfa-16
-  DW_CFA_advance_loc: 7 to 0000000000002828
+  DW_CFA_advance_loc: 7 to 0000000000002878
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc1: 184 to 00000000000028e0
+  DW_CFA_advance_loc1: 184 to 0000000000002930
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 00000000000028e1
+  DW_CFA_advance_loc: 1 to 0000000000002931
   DW_CFA_def_cfa_offset: 8
 
-000002d8 0000000000000014 000002dc FDE cie=00000000 pc=00000000000028f0..0000000000002931
+000002d8 0000000000000014 000002dc FDE cie=00000000 pc=0000000000002940..0000000000002981
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000002f0 0000000000000014 000002f4 FDE cie=00000000 pc=0000000000002940..00000000000029a5
+000002f0 0000000000000014 000002f4 FDE cie=00000000 pc=0000000000002990..00000000000029f5
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000308 0000000000000014 0000030c FDE cie=00000000 pc=00000000000029b0..0000000000002b42
+00000308 0000000000000014 0000030c FDE cie=00000000 pc=0000000000002a00..0000000000002b92
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000320 0000000000000014 00000324 FDE cie=00000000 pc=0000000000002b50..0000000000002cf0
+00000320 0000000000000014 00000324 FDE cie=00000000 pc=0000000000002ba0..0000000000002d40
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000338 0000000000000014 0000033c FDE cie=00000000 pc=0000000000002cf0..0000000000002e90
+00000338 0000000000000014 0000033c FDE cie=00000000 pc=0000000000002d40..0000000000002ee0
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000350 0000000000000014 00000354 FDE cie=00000000 pc=0000000000002e90..0000000000003030
+00000350 0000000000000014 00000354 FDE cie=00000000 pc=0000000000002ee0..0000000000003080
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000368 0000000000000014 0000036c FDE cie=00000000 pc=0000000000003030..00000000000031d0
+00000368 0000000000000014 0000036c FDE cie=00000000 pc=0000000000003080..0000000000003220
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000380 0000000000000014 00000384 FDE cie=00000000 pc=00000000000031d0..000000000000323b
+00000380 0000000000000014 00000384 FDE cie=00000000 pc=0000000000003220..000000000000328b
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000398 0000000000000014 0000039c FDE cie=00000000 pc=0000000000003240..0000000000003281
-  DW_CFA_advance_loc: 4 to 0000000000003244
+00000398 0000000000000014 0000039c FDE cie=00000000 pc=0000000000003290..00000000000032d1
+  DW_CFA_advance_loc: 4 to 0000000000003294
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 60 to 0000000000003280
+  DW_CFA_advance_loc: 60 to 00000000000032d0
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
 
-000003b0 0000000000000014 000003b4 FDE cie=00000000 pc=0000000000003290..00000000000033ae
+000003b0 0000000000000014 000003b4 FDE cie=00000000 pc=00000000000032e0..00000000000033fe
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000003c8 0000000000000014 000003cc FDE cie=00000000 pc=00000000000033b0..00000000000033df
+000003c8 0000000000000014 000003cc FDE cie=00000000 pc=0000000000003400..000000000000342f
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000003e0 000000000000003c 000003e4 FDE cie=00000000 pc=00000000000033e0..0000000000003432
-  DW_CFA_advance_loc: 9 to 00000000000033e9
+000003e0 000000000000003c 000003e4 FDE cie=00000000 pc=0000000000003430..0000000000003482
+  DW_CFA_advance_loc: 9 to 0000000000003439
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r12 (r12) at cfa-16
-  DW_CFA_advance_loc: 6 to 00000000000033ef
+  DW_CFA_advance_loc: 6 to 000000000000343f
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r6 (rbp) at cfa-24
-  DW_CFA_advance_loc: 4 to 00000000000033f3
+  DW_CFA_advance_loc: 4 to 0000000000003443
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r3 (rbx) at cfa-32
-  DW_CFA_advance_loc: 38 to 0000000000003419
+  DW_CFA_advance_loc: 38 to 0000000000003469
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 6 to 000000000000341f
+  DW_CFA_advance_loc: 6 to 000000000000346f
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000003421
+  DW_CFA_advance_loc: 2 to 0000000000003471
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 7 to 0000000000003428
+  DW_CFA_advance_loc: 7 to 0000000000003478
   DW_CFA_restore_state
-  DW_CFA_advance_loc: 1 to 0000000000003429
+  DW_CFA_advance_loc: 1 to 0000000000003479
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 3 to 000000000000342c
+  DW_CFA_advance_loc: 3 to 000000000000347c
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000342e
+  DW_CFA_advance_loc: 2 to 000000000000347e
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 000000000000342f
+  DW_CFA_advance_loc: 1 to 000000000000347f
   DW_CFA_restore: r3 (rbx)
   DW_CFA_restore: r6 (rbp)
   DW_CFA_restore: r12 (r12)
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000420 0000000000000014 00000424 FDE cie=00000000 pc=0000000000003440..0000000000003461
+00000420 0000000000000014 00000424 FDE cie=00000000 pc=0000000000003490..00000000000034b1
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000438 0000000000000014 0000043c FDE cie=00000000 pc=0000000000003470..000000000000366e
+00000438 0000000000000014 0000043c FDE cie=00000000 pc=00000000000034c0..00000000000036be
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000450 000000000000004c 00000454 FDE cie=00000000 pc=0000000000003670..0000000000003906
-  DW_CFA_advance_loc: 2 to 0000000000003672
+00000450 000000000000004c 00000454 FDE cie=00000000 pc=00000000000036c0..0000000000003956
+  DW_CFA_advance_loc: 2 to 00000000000036c2
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 19 to 0000000000003685
+  DW_CFA_advance_loc: 19 to 00000000000036d5
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 19 to 0000000000003698
+  DW_CFA_advance_loc: 19 to 00000000000036e8
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 18 to 00000000000036aa
+  DW_CFA_advance_loc: 18 to 00000000000036fa
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 18 to 00000000000036bc
+  DW_CFA_advance_loc: 18 to 000000000000370c
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 16 to 00000000000036cc
+  DW_CFA_advance_loc: 16 to 000000000000371c
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 38 to 00000000000036f2
+  DW_CFA_advance_loc: 38 to 0000000000003742
   DW_CFA_def_cfa_offset: 288
-  DW_CFA_advance_loc2: 477 to 00000000000038cf
+  DW_CFA_advance_loc2: 477 to 000000000000391f
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 00000000000038d0
+  DW_CFA_advance_loc: 1 to 0000000000003920
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 00000000000038d1
+  DW_CFA_advance_loc: 1 to 0000000000003921
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 00000000000038d3
+  DW_CFA_advance_loc: 2 to 0000000000003923
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000038d5
+  DW_CFA_advance_loc: 2 to 0000000000003925
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000038d7
+  DW_CFA_advance_loc: 2 to 0000000000003927
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000038d9
+  DW_CFA_advance_loc: 2 to 0000000000003929
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 7 to 00000000000038e0
+  DW_CFA_advance_loc: 7 to 0000000000003930
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000004a0 000000000000002c 000004a4 FDE cie=00000000 pc=0000000000003910..00000000000039d9
-  DW_CFA_advance_loc: 7 to 0000000000003917
+000004a0 000000000000002c 000004a4 FDE cie=00000000 pc=0000000000003960..0000000000003a29
+  DW_CFA_advance_loc: 7 to 0000000000003967
   DW_CFA_def_cfa_offset: 144
-  DW_CFA_advance_loc1: 144 to 00000000000039a7
+  DW_CFA_advance_loc1: 144 to 00000000000039f7
   DW_CFA_def_cfa_offset: 152
-  DW_CFA_advance_loc: 11 to 00000000000039b2
+  DW_CFA_advance_loc: 11 to 0000000000003a02
   DW_CFA_def_cfa_offset: 160
-  DW_CFA_advance_loc: 30 to 00000000000039d0
+  DW_CFA_advance_loc: 30 to 0000000000003a20
   DW_CFA_def_cfa_offset: 152
-  DW_CFA_advance_loc: 1 to 00000000000039d1
+  DW_CFA_advance_loc: 1 to 0000000000003a21
   DW_CFA_def_cfa_offset: 144
-  DW_CFA_advance_loc: 7 to 00000000000039d8
+  DW_CFA_advance_loc: 7 to 0000000000003a28
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000004d0 0000000000000014 000004d4 FDE cie=00000000 pc=00000000000039e0..00000000000039e5
+000004d0 0000000000000014 000004d4 FDE cie=00000000 pc=0000000000003a30..0000000000003a35
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000004e8 000000000000004c 000004ec FDE cie=00000000 pc=00000000000039f0..0000000000003f4d
-  DW_CFA_advance_loc: 2 to 00000000000039f2
+000004e8 000000000000004c 000004ec FDE cie=00000000 pc=0000000000003a40..0000000000003f9d
+  DW_CFA_advance_loc: 2 to 0000000000003a42
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 9 to 00000000000039fb
+  DW_CFA_advance_loc: 9 to 0000000000003a4b
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 17 to 0000000000003a0c
+  DW_CFA_advance_loc: 17 to 0000000000003a5c
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 13 to 0000000000003a19
+  DW_CFA_advance_loc: 13 to 0000000000003a69
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 15 to 0000000000003a28
+  DW_CFA_advance_loc: 15 to 0000000000003a78
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 16 to 0000000000003a38
+  DW_CFA_advance_loc: 16 to 0000000000003a88
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 50 to 0000000000003a6a
+  DW_CFA_advance_loc: 50 to 0000000000003aba
   DW_CFA_def_cfa_offset: 256
-  DW_CFA_advance_loc2: 709 to 0000000000003d2f
+  DW_CFA_advance_loc2: 709 to 0000000000003d7f
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 0000000000003d33
+  DW_CFA_advance_loc: 4 to 0000000000003d83
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000003d34
+  DW_CFA_advance_loc: 1 to 0000000000003d84
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000003d36
+  DW_CFA_advance_loc: 2 to 0000000000003d86
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000003d38
+  DW_CFA_advance_loc: 2 to 0000000000003d88
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000003d3a
+  DW_CFA_advance_loc: 2 to 0000000000003d8a
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000003d3c
+  DW_CFA_advance_loc: 2 to 0000000000003d8c
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 12 to 0000000000003d48
+  DW_CFA_advance_loc: 12 to 0000000000003d98
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000538 000000000000002c 0000053c FDE cie=00000000 pc=0000000000003f50..0000000000004019
-  DW_CFA_advance_loc: 7 to 0000000000003f57
+00000538 000000000000002c 0000053c FDE cie=00000000 pc=0000000000003fa0..0000000000004069
+  DW_CFA_advance_loc: 7 to 0000000000003fa7
   DW_CFA_def_cfa_offset: 144
-  DW_CFA_advance_loc1: 144 to 0000000000003fe7
+  DW_CFA_advance_loc1: 144 to 0000000000004037
   DW_CFA_def_cfa_offset: 152
-  DW_CFA_advance_loc: 11 to 0000000000003ff2
+  DW_CFA_advance_loc: 11 to 0000000000004042
   DW_CFA_def_cfa_offset: 160
-  DW_CFA_advance_loc: 30 to 0000000000004010
+  DW_CFA_advance_loc: 30 to 0000000000004060
   DW_CFA_def_cfa_offset: 152
-  DW_CFA_advance_loc: 1 to 0000000000004011
+  DW_CFA_advance_loc: 1 to 0000000000004061
   DW_CFA_def_cfa_offset: 144
-  DW_CFA_advance_loc: 7 to 0000000000004018
+  DW_CFA_advance_loc: 7 to 0000000000004068
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000568 0000000000000014 0000056c FDE cie=00000000 pc=0000000000004020..0000000000004025
+00000568 0000000000000014 0000056c FDE cie=00000000 pc=0000000000004070..0000000000004075
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000580 000000000000004c 00000584 FDE cie=00000000 pc=0000000000004030..00000000000044d6
-  DW_CFA_advance_loc: 2 to 0000000000004032
+00000580 000000000000004c 00000584 FDE cie=00000000 pc=0000000000004080..000000000000454b
+  DW_CFA_advance_loc: 2 to 0000000000004082
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 9 to 000000000000403b
+  DW_CFA_advance_loc: 9 to 000000000000408b
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 17 to 000000000000404c
+  DW_CFA_advance_loc: 17 to 000000000000409c
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 15 to 000000000000405b
+  DW_CFA_advance_loc: 15 to 00000000000040ab
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 13 to 0000000000004068
+  DW_CFA_advance_loc: 16 to 00000000000040bb
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 16 to 0000000000004078
+  DW_CFA_advance_loc: 13 to 00000000000040c8
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 22 to 000000000000408e
+  DW_CFA_advance_loc: 22 to 00000000000040de
   DW_CFA_def_cfa_offset: 224
-  DW_CFA_advance_loc2: 674 to 0000000000004330
+  DW_CFA_advance_loc2: 698 to 0000000000004398
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 0000000000004334
+  DW_CFA_advance_loc: 4 to 000000000000439c
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000004335
+  DW_CFA_advance_loc: 1 to 000000000000439d
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000004337
+  DW_CFA_advance_loc: 2 to 000000000000439f
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000004339
+  DW_CFA_advance_loc: 2 to 00000000000043a1
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000433b
+  DW_CFA_advance_loc: 2 to 00000000000043a3
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000433d
+  DW_CFA_advance_loc: 2 to 00000000000043a5
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 11 to 0000000000004348
+  DW_CFA_advance_loc: 11 to 00000000000043b0
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000005d0 000000000000002c 000005d4 FDE cie=00000000 pc=00000000000044e0..00000000000045a9
-  DW_CFA_advance_loc: 7 to 00000000000044e7
+000005d0 000000000000002c 000005d4 FDE cie=00000000 pc=0000000000004550..0000000000004619
+  DW_CFA_advance_loc: 7 to 0000000000004557
   DW_CFA_def_cfa_offset: 144
-  DW_CFA_advance_loc1: 144 to 0000000000004577
+  DW_CFA_advance_loc1: 144 to 00000000000045e7
   DW_CFA_def_cfa_offset: 152
-  DW_CFA_advance_loc: 11 to 0000000000004582
+  DW_CFA_advance_loc: 11 to 00000000000045f2
   DW_CFA_def_cfa_offset: 160
-  DW_CFA_advance_loc: 30 to 00000000000045a0
+  DW_CFA_advance_loc: 30 to 0000000000004610
   DW_CFA_def_cfa_offset: 152
-  DW_CFA_advance_loc: 1 to 00000000000045a1
+  DW_CFA_advance_loc: 1 to 0000000000004611
   DW_CFA_def_cfa_offset: 144
-  DW_CFA_advance_loc: 7 to 00000000000045a8
+  DW_CFA_advance_loc: 7 to 0000000000004618
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000600 0000000000000014 00000604 FDE cie=00000000 pc=00000000000045b0..00000000000045b5
+00000600 0000000000000014 00000604 FDE cie=00000000 pc=0000000000004620..0000000000004625
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000618 000000000000004c 0000061c FDE cie=00000000 pc=00000000000045c0..00000000000049d9
-  DW_CFA_advance_loc: 2 to 00000000000045c2
+00000618 000000000000004c 0000061c FDE cie=00000000 pc=0000000000004630..0000000000004a49
+  DW_CFA_advance_loc: 2 to 0000000000004632
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 9 to 00000000000045cb
+  DW_CFA_advance_loc: 9 to 000000000000463b
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 13 to 00000000000045d8
+  DW_CFA_advance_loc: 13 to 0000000000004648
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 5 to 00000000000045dd
+  DW_CFA_advance_loc: 5 to 000000000000464d
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 00000000000045de
+  DW_CFA_advance_loc: 1 to 000000000000464e
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 4 to 00000000000045e2
+  DW_CFA_advance_loc: 4 to 0000000000004652
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 7 to 00000000000045e9
+  DW_CFA_advance_loc: 7 to 0000000000004659
   DW_CFA_def_cfa_offset: 160
-  DW_CFA_advance_loc2: 595 to 000000000000483c
+  DW_CFA_advance_loc2: 595 to 00000000000048ac
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 0000000000004840
+  DW_CFA_advance_loc: 4 to 00000000000048b0
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000004841
+  DW_CFA_advance_loc: 1 to 00000000000048b1
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000004843
+  DW_CFA_advance_loc: 2 to 00000000000048b3
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000004845
+  DW_CFA_advance_loc: 2 to 00000000000048b5
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000004847
+  DW_CFA_advance_loc: 2 to 00000000000048b7
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000004849
+  DW_CFA_advance_loc: 2 to 00000000000048b9
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 7 to 0000000000004850
+  DW_CFA_advance_loc: 7 to 00000000000048c0
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000668 0000000000000044 0000066c FDE cie=00000000 pc=0000000000001f50..000000000000200a
-  DW_CFA_advance_loc: 1 to 0000000000001f51
+00000668 0000000000000044 0000066c FDE cie=00000000 pc=0000000000001fa0..000000000000205a
+  DW_CFA_advance_loc: 1 to 0000000000001fa1
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 14 to 0000000000001f5f
+  DW_CFA_advance_loc: 14 to 0000000000001faf
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 11 to 0000000000001f6a
+  DW_CFA_advance_loc: 11 to 0000000000001fba
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 15 to 0000000000001f79
+  DW_CFA_advance_loc: 15 to 0000000000001fc9
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 12 to 0000000000001f85
+  DW_CFA_advance_loc: 12 to 0000000000001fd5
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 16 to 0000000000001f95
+  DW_CFA_advance_loc: 16 to 0000000000001fe5
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 8 to 0000000000001f9d
+  DW_CFA_advance_loc: 8 to 0000000000001fed
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 22 to 0000000000001fb3
+  DW_CFA_advance_loc: 22 to 0000000000002003
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 5 to 0000000000001fb8
+  DW_CFA_advance_loc: 5 to 0000000000002008
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000001fba
+  DW_CFA_advance_loc: 2 to 000000000000200a
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 9 to 0000000000001fc3
+  DW_CFA_advance_loc: 9 to 0000000000002013
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 8 to 0000000000001fcb
+  DW_CFA_advance_loc: 8 to 000000000000201b
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 22 to 0000000000001fe1
+  DW_CFA_advance_loc: 22 to 0000000000002031
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 5 to 0000000000001fe6
+  DW_CFA_advance_loc: 5 to 0000000000002036
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000001fe8
+  DW_CFA_advance_loc: 2 to 0000000000002038
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 16 to 0000000000001ff8
+  DW_CFA_advance_loc: 16 to 0000000000002048
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 13 to 0000000000002005
+  DW_CFA_advance_loc: 13 to 0000000000002055
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
 
-000006b0 0000000000000014 000006b4 FDE cie=00000000 pc=00000000000049e0..00000000000049ee
+000006b0 0000000000000014 000006b4 FDE cie=00000000 pc=0000000000004a50..0000000000004a5e
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
```

#### readelf --wide --debug-dump=loc {}

```diff
@@ -1,7 +1,7 @@
 Contents of the .debug_loc section:
 
     Offset   Begin            End              Expression
-    00000000 00000000000049e0 00000000000049ed (DW_OP_reg5 (rdi))
-    00000013 00000000000049ed 00000000000049ee (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
+    00000000 0000000000004a50 0000000000004a5d (DW_OP_reg5 (rdi))
+    00000013 0000000000004a5d 0000000000004a5e (DW_OP_GNU_entry_value: (DW_OP_reg5 (rdi)); DW_OP_stack_value)
     00000029 <End of list>
```

#### readelf --wide --debug-dump=ranges {}

```diff
@@ -3,30 +3,30 @@
   Length:                   60
   Version:                  2
   Offset into .debug_info:  0
   Pointer Size:             8
   Segment Size:             0
 
     Address            Length
-    0000000000001b10 0000000000000012
-    00000000000049f0 0000000000000004
+    0000000000001b50 0000000000000012
+    0000000000004a60 0000000000000004
     0000000000000000 0000000000000000
   Length:                   44
   Version:                  2
   Offset into .debug_info:  0x4f
   Pointer Size:             8
   Segment Size:             0
 
     Address            Length
-    00000000000049e0 000000000000000e
+    0000000000004a50 000000000000000e
     0000000000000000 0000000000000000
   Length:                   60
   Version:                  2
   Offset into .debug_info:  0x1ea5
   Pointer Size:             8
   Segment Size:             0
 
     Address            Length
-    0000000000001b22 0000000000000005
-    00000000000049f4 0000000000000005
+    0000000000001b62 0000000000000005
+    0000000000004a64 0000000000000005
     0000000000000000 0000000000000000
```

#### strings --all --bytes=8 {}

```diff
@@ -73,15 +73,16 @@
 __cxa_atexit
 __bss_start
 GLIBC_2.2.5
 []A\A]A^A_
 []A\A]A^A_
 []A\A]A^A_
 []A\A]A^A_
-Must be have two action position!
+pos_array_size = %d
+Must be have two action position!, gateName: %s
 action position must be different!
 Must be have three action position!
 _Z18actionOnTripleGateP6float2S0_mPm
 _Z19actionOnDoubleQubitP6float2S0_mPm
 _Z19actionOnSingleQubitP6float2S0_mPm
 .shstrtab
 .symtab_shndx
@@ -469,15 +470,15 @@
 ptr___pthread_cond_init
 __exit_funcs
 ptr__pthread_cleanup_pop_restore
 _Unwind_Exception_Cleanup_Fn
 __routine
 __pthread_mutex_s
 __mon_yday
-tmpxft_00004acc_00000000-6_tgq_simulator.cudafe1.cpp
+tmpxft_00005715_00000000-6_tgq_simulator.cudafe1.cpp
 fatbinData
 _ZL26__cudaUnregisterBinaryUtilv
 _ZL20__cudaFatCubinHandle
 _ZL24__sti____cudaRegisterAllv
 _ZL15__fatDeviceText
 crtstuff.c
 deregister_tm_clones
@@ -493,14 +494,15 @@
 __dso_handle
 _DYNAMIC
 __TMC_END__
 _GLOBAL_OFFSET_TABLE_
 _Z11cphase_gateP6float2f
 execute_circuit
 _Z7ad_gateP6float2f
+printf@@GLIBC_2.2.5
 cudaMalloc@@libcudart.so.12
 _Z4hashPKc
 _Z7pd_gateP6float2f
 _Z50__device_stub__Z18actionOnTripleGateP6float2S0_mPmP6float2S0_mPm
 _Z6y_gateP6float2
 cudaLaunchKernel@@libcudart.so.12
 _Z22toff_gate_target_smallP6float2
```

#### readelf --wide --decompress --hex-dump=.hash {}

```diff
@@ -1,41 +1,41 @@
 
 Hex dump of section '.hash':
-  0x00000190 43000000 50000000 00000000 3b000000 C...P.......;...
-  0x000001a0 00000000 00000000 0b000000 00000000 ................
-  0x000001b0 00000000 1a000000 00000000 00000000 ................
-  0x000001c0 4e000000 00000000 49000000 15000000 N.......I.......
-  0x000001d0 00000000 48000000 01000000 41000000 ....H.......A...
-  0x000001e0 22000000 29000000 31000000 24000000 "...)...1...$...
-  0x000001f0 28000000 00000000 43000000 00000000 (.......C.......
-  0x00000200 4d000000 46000000 00000000 33000000 M...F.......3...
-  0x00000210 00000000 08000000 39000000 0a000000 ........9.......
-  0x00000220 3d000000 4b000000 17000000 42000000 =...K.......B...
-  0x00000230 0e000000 35000000 1e000000 20000000 ....5....... ...
-  0x00000240 44000000 36000000 16000000 23000000 D...6.......#...
-  0x00000250 00000000 10000000 00000000 3c000000 ............<...
-  0x00000260 00000000 4f000000 2d000000 18000000 ....O...-.......
-  0x00000270 00000000 00000000 00000000 3f000000 ............?...
-  0x00000280 25000000 2e000000 34000000 2c000000 %.......4...,...
-  0x00000290 40000000 1f000000 4c000000 4a000000 @.......L...J...
+  0x00000190 43000000 51000000 00000000 3c000000 C...Q.......<...
+  0x000001a0 00000000 00000000 0c000000 00000000 ................
+  0x000001b0 00000000 1b000000 00000000 00000000 ................
+  0x000001c0 4f000000 00000000 4a000000 16000000 O.......J.......
+  0x000001d0 00000000 49000000 01000000 42000000 ....I.......B...
+  0x000001e0 23000000 2a000000 32000000 25000000 #...*...2...%...
+  0x000001f0 29000000 00000000 44000000 00000000 ).......D.......
+  0x00000200 4e000000 47000000 00000000 34000000 N...G.......4...
+  0x00000210 00000000 09000000 3a000000 0b000000 ........:.......
+  0x00000220 3e000000 4c000000 18000000 43000000 >...L.......C...
+  0x00000230 0f000000 36000000 1f000000 21000000 ....6.......!...
+  0x00000240 45000000 37000000 17000000 24000000 E...7.......$...
+  0x00000250 00000000 11000000 00000000 3d000000 ............=...
+  0x00000260 00000000 50000000 2e000000 19000000 ....P...........
+  0x00000270 00000000 00000000 00000000 40000000 ............@...
+  0x00000280 26000000 2f000000 35000000 2d000000 &.../...5...-...
+  0x00000290 41000000 20000000 4d000000 4b000000 A... ...M...K...
   0x000002a0 00000000 00000000 00000000 00000000 ................
   0x000002b0 00000000 00000000 00000000 00000000 ................
-  0x000002c0 00000000 00000000 05000000 00000000 ................
+  0x000002c0 00000000 00000000 00000000 06000000 ................
   0x000002d0 00000000 00000000 00000000 00000000 ................
-  0x000002e0 00000000 0d000000 00000000 00000000 ................
+  0x000002e0 00000000 00000000 0e000000 00000000 ................
   0x000002f0 00000000 00000000 00000000 00000000 ................
-  0x00000300 14000000 00000000 00000000 00000000 ................
-  0x00000310 00000000 11000000 00000000 00000000 ................
-  0x00000320 1c000000 1b000000 04000000 02000000 ................
-  0x00000330 00000000 00000000 00000000 00000000 ................
-  0x00000340 06000000 00000000 0f000000 00000000 ................
-  0x00000350 00000000 2a000000 12000000 00000000 ....*...........
-  0x00000360 00000000 27000000 30000000 00000000 ....'...0.......
-  0x00000370 00000000 00000000 03000000 00000000 ................
-  0x00000380 1d000000 00000000 00000000 00000000 ................
-  0x00000390 38000000 3a000000 2f000000 0c000000 8...:.../.......
-  0x000003a0 00000000 32000000 07000000 00000000 ....2...........
-  0x000003b0 09000000 2b000000 26000000 00000000 ....+...&.......
-  0x000003c0 3e000000 37000000 45000000 19000000 >...7...E.......
-  0x000003d0 00000000 00000000 13000000 47000000 ............G...
-  0x000003e0 21000000                            !...
+  0x00000300 00000000 15000000 00000000 00000000 ................
+  0x00000310 04000000 00000000 12000000 00000000 ................
+  0x00000320 00000000 1d000000 1c000000 05000000 ................
+  0x00000330 02000000 00000000 00000000 00000000 ................
+  0x00000340 00000000 07000000 00000000 10000000 ................
+  0x00000350 00000000 00000000 2b000000 13000000 ........+.......
+  0x00000360 00000000 00000000 28000000 31000000 ........(...1...
+  0x00000370 00000000 00000000 00000000 03000000 ................
+  0x00000380 00000000 1e000000 00000000 00000000 ................
+  0x00000390 00000000 39000000 3b000000 30000000 ....9...;...0...
+  0x000003a0 0d000000 00000000 33000000 08000000 ........3.......
+  0x000003b0 00000000 0a000000 2c000000 27000000 ........,...'...
+  0x000003c0 00000000 3f000000 38000000 46000000 ....?...8...F...
+  0x000003d0 1a000000 00000000 00000000 14000000 ................
+  0x000003e0 48000000 22000000                   H..."...
```

#### readelf --wide --decompress --hex-dump=.dynstr {}

```diff
@@ -1,116 +1,117 @@
 
 Hex dump of section '.dynstr':
-  0x00000b68 005f5f67 6d6f6e5f 73746172 745f5f00 .__gmon_start__.
-  0x00000b78 5f49544d 5f646572 65676973 74657254 _ITM_deregisterT
-  0x00000b88 4d436c6f 6e655461 626c6500 5f49544d MCloneTable._ITM
-  0x00000b98 5f726567 69737465 72544d43 6c6f6e65 _registerTMClone
-  0x00000ba8 5461626c 65005f5f 6378615f 66696e61 Table.__cxa_fina
-  0x00000bb8 6c697a65 005f5a37 636f6d70 61726550 lize._Z7compareP
-  0x00000bc8 4b765330 5f005f5f 63756461 556e7265 KvS0_.__cudaUnre
-  0x00000bd8 67697374 65724661 7442696e 61727900 gisterFatBinary.
-  0x00000be8 5f5a3678 5f676174 65503666 6c6f6174 _Z6x_gateP6float
-  0x00000bf8 32005f5a 36795f67 61746550 36666c6f 2._Z6y_gateP6flo
-  0x00000c08 61743200 5f5a367a 5f676174 65503666 at2._Z6z_gateP6f
-  0x00000c18 6c6f6174 32005f5a 36735f67 61746550 loat2._Z6s_gateP
-  0x00000c28 36666c6f 61743200 5f5a3873 64675f67 6float2._Z8sdg_g
-  0x00000c38 61746550 36666c6f 61743200 5f5a3674 ateP6float2._Z6t
-  0x00000c48 5f676174 65503666 6c6f6174 32005f5a _gateP6float2._Z
-  0x00000c58 38746467 5f676174 65503666 6c6f6174 8tdg_gateP6float
-  0x00000c68 32005f5a 36685f67 61746550 36666c6f 2._Z6h_gateP6flo
-  0x00000c78 61743200 5f5a3772 785f6761 74655036 at2._Z7rx_gateP6
-  0x00000c88 666c6f61 74326600 73696e63 6f736600 float2f.sincosf.
-  0x00000c98 5f5a3772 795f6761 74655036 666c6f61 _Z7ry_gateP6floa
-  0x00000ca8 74326600 5f5a3772 7a5f6761 74655036 t2f._Z7rz_gateP6
-  0x00000cb8 666c6f61 74326600 5f5a3131 64616d70 float2f._Z11damp
-  0x00000cc8 5f695f67 61746550 36666c6f 61743266 _i_gateP6float2f
-  0x00000cd8 00737172 7466005f 5a377064 5f676174 .sqrtf._Z7pd_gat
-  0x00000ce8 65503666 6c6f6174 3266005f 5a376164 eP6float2f._Z7ad
-  0x00000cf8 5f676174 65503666 6c6f6174 3266005f _gateP6float2f._
-  0x00000d08 5a397377 61705f67 61746550 36666c6f Z9swap_gateP6flo
-  0x00000d18 61743200 5f5a3130 69737761 705f6761 at2._Z10iswap_ga
-  0x00000d28 74655036 666c6f61 7432005f 5a313163 teP6float2._Z11c
-  0x00000d38 70686173 655f6761 74655036 666c6f61 phase_gateP6floa
-  0x00000d48 74326600 5f5a3231 636e6f74 5f676174 t2f._Z21cnot_gat
-  0x00000d58 655f636f 6e74726f 6c5f6269 67503666 e_control_bigP6f
-  0x00000d68 6c6f6174 32005f5a 3233636e 6f745f67 loat2._Z23cnot_g
-  0x00000d78 6174655f 636f6e74 726f6c5f 736d616c ate_control_smal
-  0x00000d88 6c503666 6c6f6174 32005f5a 37637a5f lP6float2._Z7cz_
-  0x00000d98 67617465 5036666c 6f617432 005f5a38 gateP6float2._Z8
-  0x00000da8 7278785f 67617465 5036666c 6f617432 rxx_gateP6float2
-  0x00000db8 66005f5a 38727979 5f676174 65503666 f._Z8ryy_gateP6f
-  0x00000dc8 6c6f6174 3266005f 5a38727a 7a5f6761 loat2f._Z8rzz_ga
-  0x00000dd8 74655036 666c6f61 74326600 5f5a3873 teP6float2f._Z8s
-  0x00000de8 79635f67 61746550 36666c6f 61743200 yc_gateP6float2.
-  0x00000df8 5f5a3232 746f6666 5f676174 655f7461 _Z22toff_gate_ta
-  0x00000e08 72676574 5f736d61 6c6c5036 666c6f61 rget_smallP6floa
-  0x00000e18 7432005f 5a323074 6f66665f 67617465 t2._Z20toff_gate
-  0x00000e28 5f746172 6765745f 6d696450 36666c6f _target_midP6flo
-  0x00000e38 61743200 5f5a3230 746f6666 5f676174 at2._Z20toff_gat
-  0x00000e48 655f7461 72676574 5f626967 5036666c e_target_bigP6fl
-  0x00000e58 6f617432 005f5a32 31667265 645f6761 oat2._Z21fred_ga
-  0x00000e68 74655f63 6f6e7472 6f6c5f62 69675036 te_control_bigP6
-  0x00000e78 666c6f61 7432005f 5a323166 7265645f float2._Z21fred_
-  0x00000e88 67617465 5f636f6e 74726f6c 5f6d6964 gate_control_mid
-  0x00000e98 5036666c 6f617432 005f5a32 33667265 P6float2._Z23fre
-  0x00000ea8 645f6761 74655f63 6f6e7472 6f6c5f73 d_gate_control_s
-  0x00000eb8 6d616c6c 5036666c 6f617432 005f5a31 mallP6float2._Z1
-  0x00000ec8 31696465 6e746974 794d6174 5036666c 1identityMatP6fl
-  0x00000ed8 6f617432 69005f5a 32306765 6e657261 oat2i._Z20genera
-  0x00000ee8 74655f62 696e6172 795f6461 74616600 te_binary_dataf.
-  0x00000ef8 74696d65 00737261 6e64005f 5a376765 time.srand._Z7ge
-  0x00000f08 7470726f 62503666 6c6f6174 3250666d tprobP6float2Pfm
-  0x00000f18 005f5a34 68617368 504b6300 5f5a3969 ._Z4hashPKc._Z9i
-  0x00000f28 73496e41 72726179 50504b63 50636900 sInArrayPPKcPci.
-  0x00000f38 73747263 6d70005f 5a313467 65744172 strcmp._Z14getAr
-  0x00000f48 7261794c 656e6774 68506900 5f5a3133 rayLengthPi._Z13
-  0x00000f58 6e6f726d 616c697a 6174696f 6e503666 normalizationP6f
-  0x00000f68 6c6f6174 32690065 78656375 74655f63 loat2i.execute_c
-  0x00000f78 69726375 69740073 696e676c 65476174 ircuit.singleGat
-  0x00000f88 65416374 696f6e00 646f7562 6c654761 eAction.doubleGa
-  0x00000f98 74654163 74696f6e 00747269 706c6547 teAction.tripleG
-  0x00000fa8 61746541 6374696f 6e005f5a 35315f5f ateAction._Z51__
-  0x00000fb8 64657669 63655f73 7475625f 5f5a3139 device_stub__Z19
-  0x00000fc8 61637469 6f6e4f6e 53696e67 6c655175 actionOnSingleQu
-  0x00000fd8 62697450 36666c6f 61743253 305f6d50 bitP6float2S0_mP
-  0x00000fe8 6d503666 6c6f6174 3253305f 6d506d00 mP6float2S0_mPm.
-  0x00000ff8 5f5f6375 6461506f 7043616c 6c436f6e __cudaPopCallCon
-  0x00001008 66696775 72617469 6f6e005f 5a313961 figuration._Z19a
-  0x00001018 6374696f 6e4f6e53 696e676c 65517562 ctionOnSingleQub
-  0x00001028 69745036 666c6f61 74325330 5f6d506d itP6float2S0_mPm
-  0x00001038 00637564 614c6175 6e63684b 65726e65 .cudaLaunchKerne
-  0x00001048 6c006375 64615365 74446576 69636500 l.cudaSetDevice.
-  0x00001058 6d616c6c 6f630063 7564614d 616c6c6f malloc.cudaMallo
-  0x00001068 63006375 64614d65 6d637079 005f5f63 c.cudaMemcpy.__c
-  0x00001078 75646150 75736843 616c6c43 6f6e6669 udaPushCallConfi
-  0x00001088 67757261 74696f6e 00637564 61446576 guration.cudaDev
-  0x00001098 69636553 796e6368 726f6e69 7a650063 iceSynchronize.c
-  0x000010a8 75646146 72656500 66726565 005f5a35 udaFree.free._Z5
-  0x000010b8 315f5f64 65766963 655f7374 75625f5f 1__device_stub__
-  0x000010c8 5a313961 6374696f 6e4f6e44 6f75626c Z19actionOnDoubl
-  0x000010d8 65517562 69745036 666c6f61 74325330 eQubitP6float2S0
-  0x000010e8 5f6d506d 5036666c 6f617432 53305f6d _mPmP6float2S0_m
-  0x000010f8 506d005f 5a313961 6374696f 6e4f6e44 Pm._Z19actionOnD
-  0x00001108 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
-  0x00001118 74325330 5f6d506d 0071736f 72740070 t2S0_mPm.qsort.p
-  0x00001128 75747300 5f5a3530 5f5f6465 76696365 uts._Z50__device
-  0x00001138 5f737475 625f5f5a 31386163 74696f6e _stub__Z18action
-  0x00001148 4f6e5472 69706c65 47617465 5036666c OnTripleGateP6fl
-  0x00001158 6f617432 53305f6d 506d5036 666c6f61 oat2S0_mPmP6floa
-  0x00001168 74325330 5f6d506d 005f5a31 38616374 t2S0_mPm._Z18act
-  0x00001178 696f6e4f 6e547269 706c6547 61746550 ionOnTripleGateP
-  0x00001188 36666c6f 61743253 305f6d50 6d005f5f 6float2S0_mPm.__
-  0x00001198 63756461 52656769 73746572 46617442 cudaRegisterFatB
-  0x000011a8 696e6172 79005f5f 63756461 52656769 inary.__cudaRegi
-  0x000011b8 73746572 46756e63 74696f6e 005f5f63 sterFunction.__c
-  0x000011c8 75646152 65676973 74657246 61744269 udaRegisterFatBi
-  0x000011d8 6e617279 456e6400 6c696263 75646172 naryEnd.libcudar
-  0x000011e8 742e736f 2e313200 6c696272 742e736f t.so.12.librt.so
-  0x000011f8 2e31006c 69627074 68726561 642e736f .1.libpthread.so
-  0x00001208 2e30006c 6962646c 2e736f2e 32006c69 .0.libdl.so.2.li
-  0x00001218 62737464 632b2b2e 736f2e36 006c6962 bstdc++.so.6.lib
-  0x00001228 6d2e736f 2e36006c 69626763 635f732e m.so.6.libgcc_s.
-  0x00001238 736f2e31 006c6962 632e736f 2e36005f so.1.libc.so.6._
-  0x00001248 5f637861 5f617465 78697400 5f656461 _cxa_atexit._eda
-  0x00001258 7461005f 5f627373 5f737461 7274005f ta.__bss_start._
-  0x00001268 656e6400 474c4942 435f322e 322e3500 end.GLIBC_2.2.5.
+  0x00000b80 005f5f67 6d6f6e5f 73746172 745f5f00 .__gmon_start__.
+  0x00000b90 5f49544d 5f646572 65676973 74657254 _ITM_deregisterT
+  0x00000ba0 4d436c6f 6e655461 626c6500 5f49544d MCloneTable._ITM
+  0x00000bb0 5f726567 69737465 72544d43 6c6f6e65 _registerTMClone
+  0x00000bc0 5461626c 65005f5f 6378615f 66696e61 Table.__cxa_fina
+  0x00000bd0 6c697a65 005f5a37 636f6d70 61726550 lize._Z7compareP
+  0x00000be0 4b765330 5f005f5f 63756461 556e7265 KvS0_.__cudaUnre
+  0x00000bf0 67697374 65724661 7442696e 61727900 gisterFatBinary.
+  0x00000c00 5f5a3678 5f676174 65503666 6c6f6174 _Z6x_gateP6float
+  0x00000c10 32005f5a 36795f67 61746550 36666c6f 2._Z6y_gateP6flo
+  0x00000c20 61743200 5f5a367a 5f676174 65503666 at2._Z6z_gateP6f
+  0x00000c30 6c6f6174 32005f5a 36735f67 61746550 loat2._Z6s_gateP
+  0x00000c40 36666c6f 61743200 5f5a3873 64675f67 6float2._Z8sdg_g
+  0x00000c50 61746550 36666c6f 61743200 5f5a3674 ateP6float2._Z6t
+  0x00000c60 5f676174 65503666 6c6f6174 32005f5a _gateP6float2._Z
+  0x00000c70 38746467 5f676174 65503666 6c6f6174 8tdg_gateP6float
+  0x00000c80 32005f5a 36685f67 61746550 36666c6f 2._Z6h_gateP6flo
+  0x00000c90 61743200 5f5a3772 785f6761 74655036 at2._Z7rx_gateP6
+  0x00000ca0 666c6f61 74326600 73696e63 6f736600 float2f.sincosf.
+  0x00000cb0 5f5a3772 795f6761 74655036 666c6f61 _Z7ry_gateP6floa
+  0x00000cc0 74326600 5f5a3772 7a5f6761 74655036 t2f._Z7rz_gateP6
+  0x00000cd0 666c6f61 74326600 5f5a3131 64616d70 float2f._Z11damp
+  0x00000ce0 5f695f67 61746550 36666c6f 61743266 _i_gateP6float2f
+  0x00000cf0 00737172 7466005f 5a377064 5f676174 .sqrtf._Z7pd_gat
+  0x00000d00 65503666 6c6f6174 3266005f 5a376164 eP6float2f._Z7ad
+  0x00000d10 5f676174 65503666 6c6f6174 3266005f _gateP6float2f._
+  0x00000d20 5a397377 61705f67 61746550 36666c6f Z9swap_gateP6flo
+  0x00000d30 61743200 5f5a3130 69737761 705f6761 at2._Z10iswap_ga
+  0x00000d40 74655036 666c6f61 7432005f 5a313163 teP6float2._Z11c
+  0x00000d50 70686173 655f6761 74655036 666c6f61 phase_gateP6floa
+  0x00000d60 74326600 5f5a3231 636e6f74 5f676174 t2f._Z21cnot_gat
+  0x00000d70 655f636f 6e74726f 6c5f6269 67503666 e_control_bigP6f
+  0x00000d80 6c6f6174 32005f5a 3233636e 6f745f67 loat2._Z23cnot_g
+  0x00000d90 6174655f 636f6e74 726f6c5f 736d616c ate_control_smal
+  0x00000da0 6c503666 6c6f6174 32005f5a 37637a5f lP6float2._Z7cz_
+  0x00000db0 67617465 5036666c 6f617432 005f5a38 gateP6float2._Z8
+  0x00000dc0 7278785f 67617465 5036666c 6f617432 rxx_gateP6float2
+  0x00000dd0 66005f5a 38727979 5f676174 65503666 f._Z8ryy_gateP6f
+  0x00000de0 6c6f6174 3266005f 5a38727a 7a5f6761 loat2f._Z8rzz_ga
+  0x00000df0 74655036 666c6f61 74326600 5f5a3873 teP6float2f._Z8s
+  0x00000e00 79635f67 61746550 36666c6f 61743200 yc_gateP6float2.
+  0x00000e10 5f5a3232 746f6666 5f676174 655f7461 _Z22toff_gate_ta
+  0x00000e20 72676574 5f736d61 6c6c5036 666c6f61 rget_smallP6floa
+  0x00000e30 7432005f 5a323074 6f66665f 67617465 t2._Z20toff_gate
+  0x00000e40 5f746172 6765745f 6d696450 36666c6f _target_midP6flo
+  0x00000e50 61743200 5f5a3230 746f6666 5f676174 at2._Z20toff_gat
+  0x00000e60 655f7461 72676574 5f626967 5036666c e_target_bigP6fl
+  0x00000e70 6f617432 005f5a32 31667265 645f6761 oat2._Z21fred_ga
+  0x00000e80 74655f63 6f6e7472 6f6c5f62 69675036 te_control_bigP6
+  0x00000e90 666c6f61 7432005f 5a323166 7265645f float2._Z21fred_
+  0x00000ea0 67617465 5f636f6e 74726f6c 5f6d6964 gate_control_mid
+  0x00000eb0 5036666c 6f617432 005f5a32 33667265 P6float2._Z23fre
+  0x00000ec0 645f6761 74655f63 6f6e7472 6f6c5f73 d_gate_control_s
+  0x00000ed0 6d616c6c 5036666c 6f617432 005f5a31 mallP6float2._Z1
+  0x00000ee0 31696465 6e746974 794d6174 5036666c 1identityMatP6fl
+  0x00000ef0 6f617432 69005f5a 32306765 6e657261 oat2i._Z20genera
+  0x00000f00 74655f62 696e6172 795f6461 74616600 te_binary_dataf.
+  0x00000f10 74696d65 00737261 6e64005f 5a376765 time.srand._Z7ge
+  0x00000f20 7470726f 62503666 6c6f6174 3250666d tprobP6float2Pfm
+  0x00000f30 005f5a34 68617368 504b6300 5f5a3969 ._Z4hashPKc._Z9i
+  0x00000f40 73496e41 72726179 50504b63 50636900 sInArrayPPKcPci.
+  0x00000f50 73747263 6d70005f 5a313467 65744172 strcmp._Z14getAr
+  0x00000f60 7261794c 656e6774 68506900 5f5a3133 rayLengthPi._Z13
+  0x00000f70 6e6f726d 616c697a 6174696f 6e503666 normalizationP6f
+  0x00000f80 6c6f6174 32690065 78656375 74655f63 loat2i.execute_c
+  0x00000f90 69726375 69740073 696e676c 65476174 ircuit.singleGat
+  0x00000fa0 65416374 696f6e00 646f7562 6c654761 eAction.doubleGa
+  0x00000fb0 74654163 74696f6e 00747269 706c6547 teAction.tripleG
+  0x00000fc0 61746541 6374696f 6e005f5a 35315f5f ateAction._Z51__
+  0x00000fd0 64657669 63655f73 7475625f 5f5a3139 device_stub__Z19
+  0x00000fe0 61637469 6f6e4f6e 53696e67 6c655175 actionOnSingleQu
+  0x00000ff0 62697450 36666c6f 61743253 305f6d50 bitP6float2S0_mP
+  0x00001000 6d503666 6c6f6174 3253305f 6d506d00 mP6float2S0_mPm.
+  0x00001010 5f5f6375 6461506f 7043616c 6c436f6e __cudaPopCallCon
+  0x00001020 66696775 72617469 6f6e005f 5a313961 figuration._Z19a
+  0x00001030 6374696f 6e4f6e53 696e676c 65517562 ctionOnSingleQub
+  0x00001040 69745036 666c6f61 74325330 5f6d506d itP6float2S0_mPm
+  0x00001050 00637564 614c6175 6e63684b 65726e65 .cudaLaunchKerne
+  0x00001060 6c006375 64615365 74446576 69636500 l.cudaSetDevice.
+  0x00001070 6d616c6c 6f630063 7564614d 616c6c6f malloc.cudaMallo
+  0x00001080 63006375 64614d65 6d637079 005f5f63 c.cudaMemcpy.__c
+  0x00001090 75646150 75736843 616c6c43 6f6e6669 udaPushCallConfi
+  0x000010a0 67757261 74696f6e 00637564 61446576 guration.cudaDev
+  0x000010b0 69636553 796e6368 726f6e69 7a650063 iceSynchronize.c
+  0x000010c0 75646146 72656500 66726565 005f5a35 udaFree.free._Z5
+  0x000010d0 315f5f64 65766963 655f7374 75625f5f 1__device_stub__
+  0x000010e0 5a313961 6374696f 6e4f6e44 6f75626c Z19actionOnDoubl
+  0x000010f0 65517562 69745036 666c6f61 74325330 eQubitP6float2S0
+  0x00001100 5f6d506d 5036666c 6f617432 53305f6d _mPmP6float2S0_m
+  0x00001110 506d005f 5a313961 6374696f 6e4f6e44 Pm._Z19actionOnD
+  0x00001120 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
+  0x00001130 74325330 5f6d506d 00707269 6e746600 t2S0_mPm.printf.
+  0x00001140 71736f72 74007075 7473005f 5a35305f qsort.puts._Z50_
+  0x00001150 5f646576 6963655f 73747562 5f5f5a31 _device_stub__Z1
+  0x00001160 38616374 696f6e4f 6e547269 706c6547 8actionOnTripleG
+  0x00001170 61746550 36666c6f 61743253 305f6d50 ateP6float2S0_mP
+  0x00001180 6d503666 6c6f6174 3253305f 6d506d00 mP6float2S0_mPm.
+  0x00001190 5f5a3138 61637469 6f6e4f6e 54726970 _Z18actionOnTrip
+  0x000011a0 6c654761 74655036 666c6f61 74325330 leGateP6float2S0
+  0x000011b0 5f6d506d 005f5f63 75646152 65676973 _mPm.__cudaRegis
+  0x000011c0 74657246 61744269 6e617279 005f5f63 terFatBinary.__c
+  0x000011d0 75646152 65676973 74657246 756e6374 udaRegisterFunct
+  0x000011e0 696f6e00 5f5f6375 64615265 67697374 ion.__cudaRegist
+  0x000011f0 65724661 7442696e 61727945 6e64006c erFatBinaryEnd.l
+  0x00001200 69626375 64617274 2e736f2e 3132006c ibcudart.so.12.l
+  0x00001210 69627274 2e736f2e 31006c69 62707468 ibrt.so.1.libpth
+  0x00001220 72656164 2e736f2e 30006c69 62646c2e read.so.0.libdl.
+  0x00001230 736f2e32 006c6962 73746463 2b2b2e73 so.2.libstdc++.s
+  0x00001240 6f2e3600 6c69626d 2e736f2e 36006c69 o.6.libm.so.6.li
+  0x00001250 62676363 5f732e73 6f2e3100 6c696263 bgcc_s.so.1.libc
+  0x00001260 2e736f2e 36005f5f 6378615f 61746578 .so.6.__cxa_atex
+  0x00001270 6974005f 65646174 61005f5f 6273735f it._edata.__bss_
+  0x00001280 73746172 74005f65 6e640047 4c494243 start._end.GLIBC
+  0x00001290 5f322e32 2e3500                     _2.2.5.
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.init {}

```diff
@@ -1,21 +1,21 @@
 
 
 
 Disassembly of section .init:
 
-0000000000001b10 <_init>:
+0000000000001b50 <_init>:
 _init():
 /opt/glibc-2.31/csu/../sysdeps/x86_64/crti.S:66
 	sub    $0x8,%rsp
 /opt/glibc-2.31/csu/../sysdeps/x86_64/crti.S:68
-	mov    0x20a4d5(%rip),%rax        
+	mov    0x20a495(%rip),%rax        
 /opt/glibc-2.31/csu/../sysdeps/x86_64/crti.S:69
 	test   %rax,%rax
 /opt/glibc-2.31/csu/../sysdeps/x86_64/crti.S:70
-	je     1b22 <_init+0x12>
+	je     1b62 <_init+0x12>
 /opt/glibc-2.31/csu/../sysdeps/x86_64/crti.S:71
 	call   *%rax
 /opt/glibc-2.31/csu/../sysdeps/x86_64/crtn.S:40
 	add    $0x8,%rsp
 /opt/glibc-2.31/csu/../sysdeps/x86_64/crtn.S:41
 	ret
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt {}

```diff
@@ -1,334 +1,339 @@
 
 
 
 Disassembly of section .plt:
 
-0000000000001b30 <.plt>:
-	push   0x20a4d2(%rip)        
-	jmp    *0x20a4d4(%rip)        
+0000000000001b70 <.plt>:
+	push   0x20a492(%rip)        
+	jmp    *0x20a494(%rip)        
 	nopl   0x0(%rax)
 
-0000000000001b40 <cphase_gate(float2*, float)@plt>:
-	jmp    *0x20a4d2(%rip)        
+0000000000001b80 <cphase_gate(float2*, float)@plt>:
+	jmp    *0x20a492(%rip)        
 	push   $0x0
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001b50 <ad_gate(float2*, float)@plt>:
-	jmp    *0x20a4ca(%rip)        
+0000000000001b90 <ad_gate(float2*, float)@plt>:
+	jmp    *0x20a48a(%rip)        
 	push   $0x1
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001b60 <cudaMalloc@plt>:
-	jmp    *0x20a4c2(%rip)        
+0000000000001ba0 <printf@plt>:
+	jmp    *0x20a482(%rip)        
 	push   $0x2
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001b70 <hash(char const*)@plt>:
-	jmp    *0x20a4ba(%rip)        
+0000000000001bb0 <cudaMalloc@plt>:
+	jmp    *0x20a47a(%rip)        
 	push   $0x3
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001b80 <pd_gate(float2*, float)@plt>:
-	jmp    *0x20a4b2(%rip)        
+0000000000001bc0 <hash(char const*)@plt>:
+	jmp    *0x20a472(%rip)        
 	push   $0x4
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001b90 <__device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>:
-	jmp    *0x20a4aa(%rip)        
+0000000000001bd0 <pd_gate(float2*, float)@plt>:
+	jmp    *0x20a46a(%rip)        
 	push   $0x5
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001ba0 <y_gate(float2*)@plt>:
-	jmp    *0x20a4a2(%rip)        
+0000000000001be0 <__device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>:
+	jmp    *0x20a462(%rip)        
 	push   $0x6
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001bb0 <cudaLaunchKernel@plt>:
-	jmp    *0x20a49a(%rip)        
+0000000000001bf0 <y_gate(float2*)@plt>:
+	jmp    *0x20a45a(%rip)        
 	push   $0x7
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001bc0 <toff_gate_target_small(float2*)@plt>:
-	jmp    *0x20a492(%rip)        
+0000000000001c00 <cudaLaunchKernel@plt>:
+	jmp    *0x20a452(%rip)        
 	push   $0x8
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001bd0 <rand@plt>:
-	jmp    *0x20a48a(%rip)        
+0000000000001c10 <toff_gate_target_small(float2*)@plt>:
+	jmp    *0x20a44a(%rip)        
 	push   $0x9
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001be0 <fred_gate_control_small(float2*)@plt>:
-	jmp    *0x20a482(%rip)        
+0000000000001c20 <rand@plt>:
+	jmp    *0x20a442(%rip)        
 	push   $0xa
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001bf0 <__cudaUnregisterFatBinary@plt>:
-	jmp    *0x20a47a(%rip)        
+0000000000001c30 <fred_gate_control_small(float2*)@plt>:
+	jmp    *0x20a43a(%rip)        
 	push   $0xb
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001c00 <fred_gate_control_mid(float2*)@plt>:
-	jmp    *0x20a472(%rip)        
+0000000000001c40 <__cudaUnregisterFatBinary@plt>:
+	jmp    *0x20a432(%rip)        
 	push   $0xc
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001c10 <cnot_gate_control_small(float2*)@plt>:
-	jmp    *0x20a46a(%rip)        
+0000000000001c50 <fred_gate_control_mid(float2*)@plt>:
+	jmp    *0x20a42a(%rip)        
 	push   $0xd
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001c20 <ry_gate(float2*, float)@plt>:
-	jmp    *0x20a462(%rip)        
+0000000000001c60 <cnot_gate_control_small(float2*)@plt>:
+	jmp    *0x20a422(%rip)        
 	push   $0xe
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001c30 <sincosf@plt>:
-	jmp    *0x20a45a(%rip)        
+0000000000001c70 <ry_gate(float2*, float)@plt>:
+	jmp    *0x20a41a(%rip)        
 	push   $0xf
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001c40 <__cxa_finalize@plt>:
-	jmp    *0x20a452(%rip)        
+0000000000001c80 <sincosf@plt>:
+	jmp    *0x20a412(%rip)        
 	push   $0x10
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001c50 <fred_gate_control_big(float2*)@plt>:
-	jmp    *0x20a44a(%rip)        
+0000000000001c90 <__cxa_finalize@plt>:
+	jmp    *0x20a40a(%rip)        
 	push   $0x11
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001c60 <syc_gate(float2*)@plt>:
-	jmp    *0x20a442(%rip)        
+0000000000001ca0 <fred_gate_control_big(float2*)@plt>:
+	jmp    *0x20a402(%rip)        
 	push   $0x12
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001c70 <rxx_gate(float2*, float)@plt>:
-	jmp    *0x20a43a(%rip)        
+0000000000001cb0 <syc_gate(float2*)@plt>:
+	jmp    *0x20a3fa(%rip)        
 	push   $0x13
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001c80 <toff_gate_target_mid(float2*)@plt>:
-	jmp    *0x20a432(%rip)        
+0000000000001cc0 <rxx_gate(float2*, float)@plt>:
+	jmp    *0x20a3f2(%rip)        
 	push   $0x14
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001c90 <rzz_gate(float2*, float)@plt>:
-	jmp    *0x20a42a(%rip)        
+0000000000001cd0 <toff_gate_target_mid(float2*)@plt>:
+	jmp    *0x20a3ea(%rip)        
 	push   $0x15
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001ca0 <isInArray(char const**, char*, int)@plt>:
-	jmp    *0x20a422(%rip)        
+0000000000001ce0 <rzz_gate(float2*, float)@plt>:
+	jmp    *0x20a3e2(%rip)        
 	push   $0x16
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001cb0 <cnot_gate_control_big(float2*)@plt>:
-	jmp    *0x20a41a(%rip)        
+0000000000001cf0 <isInArray(char const**, char*, int)@plt>:
+	jmp    *0x20a3da(%rip)        
 	push   $0x17
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001cc0 <x_gate(float2*)@plt>:
-	jmp    *0x20a412(%rip)        
+0000000000001d00 <cnot_gate_control_big(float2*)@plt>:
+	jmp    *0x20a3d2(%rip)        
 	push   $0x18
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001cd0 <s_gate(float2*)@plt>:
-	jmp    *0x20a40a(%rip)        
+0000000000001d10 <x_gate(float2*)@plt>:
+	jmp    *0x20a3ca(%rip)        
 	push   $0x19
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001ce0 <damp_i_gate(float2*, float)@plt>:
-	jmp    *0x20a402(%rip)        
+0000000000001d20 <s_gate(float2*)@plt>:
+	jmp    *0x20a3c2(%rip)        
 	push   $0x1a
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001cf0 <iswap_gate(float2*)@plt>:
-	jmp    *0x20a3fa(%rip)        
+0000000000001d30 <damp_i_gate(float2*, float)@plt>:
+	jmp    *0x20a3ba(%rip)        
 	push   $0x1b
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001d00 <__cxa_atexit@plt>:
-	jmp    *0x20a3f2(%rip)        
+0000000000001d40 <iswap_gate(float2*)@plt>:
+	jmp    *0x20a3b2(%rip)        
 	push   $0x1c
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001d10 <__cudaRegisterFatBinary@plt>:
-	jmp    *0x20a3ea(%rip)        
+0000000000001d50 <__cxa_atexit@plt>:
+	jmp    *0x20a3aa(%rip)        
 	push   $0x1d
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001d20 <time@plt>:
-	jmp    *0x20a3e2(%rip)        
+0000000000001d60 <__cudaRegisterFatBinary@plt>:
+	jmp    *0x20a3a2(%rip)        
 	push   $0x1e
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001d30 <srand@plt>:
-	jmp    *0x20a3da(%rip)        
+0000000000001d70 <time@plt>:
+	jmp    *0x20a39a(%rip)        
 	push   $0x1f
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001d40 <t_gate(float2*)@plt>:
-	jmp    *0x20a3d2(%rip)        
+0000000000001d80 <srand@plt>:
+	jmp    *0x20a392(%rip)        
 	push   $0x20
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001d50 <normalization(float2*, int)@plt>:
-	jmp    *0x20a3ca(%rip)        
+0000000000001d90 <t_gate(float2*)@plt>:
+	jmp    *0x20a38a(%rip)        
 	push   $0x21
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001d60 <z_gate(float2*)@plt>:
-	jmp    *0x20a3c2(%rip)        
+0000000000001da0 <normalization(float2*, int)@plt>:
+	jmp    *0x20a382(%rip)        
 	push   $0x22
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001d70 <actionOnDoubleQubit(float2*, float2*, unsigned long, unsigned long*)@plt>:
-	jmp    *0x20a3ba(%rip)        
+0000000000001db0 <z_gate(float2*)@plt>:
+	jmp    *0x20a37a(%rip)        
 	push   $0x23
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001d80 <__device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>:
-	jmp    *0x20a3b2(%rip)        
+0000000000001dc0 <actionOnDoubleQubit(float2*, float2*, unsigned long, unsigned long*)@plt>:
+	jmp    *0x20a372(%rip)        
 	push   $0x24
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001d90 <free@plt>:
-	jmp    *0x20a3aa(%rip)        
+0000000000001dd0 <__device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>:
+	jmp    *0x20a36a(%rip)        
 	push   $0x25
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001da0 <cudaMemcpy@plt>:
-	jmp    *0x20a3a2(%rip)        
+0000000000001de0 <free@plt>:
+	jmp    *0x20a362(%rip)        
 	push   $0x26
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001db0 <exit@plt>:
-	jmp    *0x20a39a(%rip)        
+0000000000001df0 <cudaMemcpy@plt>:
+	jmp    *0x20a35a(%rip)        
 	push   $0x27
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001dc0 <tdg_gate(float2*)@plt>:
-	jmp    *0x20a392(%rip)        
+0000000000001e00 <exit@plt>:
+	jmp    *0x20a352(%rip)        
 	push   $0x28
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001dd0 <cz_gate(float2*)@plt>:
-	jmp    *0x20a38a(%rip)        
+0000000000001e10 <tdg_gate(float2*)@plt>:
+	jmp    *0x20a34a(%rip)        
 	push   $0x29
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001de0 <actionOnTripleGate(float2*, float2*, unsigned long, unsigned long*)@plt>:
-	jmp    *0x20a382(%rip)        
+0000000000001e20 <cz_gate(float2*)@plt>:
+	jmp    *0x20a342(%rip)        
 	push   $0x2a
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001df0 <malloc@plt>:
-	jmp    *0x20a37a(%rip)        
+0000000000001e30 <actionOnTripleGate(float2*, float2*, unsigned long, unsigned long*)@plt>:
+	jmp    *0x20a33a(%rip)        
 	push   $0x2b
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001e00 <__device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>:
-	jmp    *0x20a372(%rip)        
+0000000000001e40 <malloc@plt>:
+	jmp    *0x20a332(%rip)        
 	push   $0x2c
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001e10 <getArrayLength(int*)@plt>:
-	jmp    *0x20a36a(%rip)        
+0000000000001e50 <__device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>:
+	jmp    *0x20a32a(%rip)        
 	push   $0x2d
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001e20 <sdg_gate(float2*)@plt>:
-	jmp    *0x20a362(%rip)        
+0000000000001e60 <getArrayLength(int*)@plt>:
+	jmp    *0x20a322(%rip)        
 	push   $0x2e
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001e30 <strcmp@plt>:
-	jmp    *0x20a35a(%rip)        
+0000000000001e70 <sdg_gate(float2*)@plt>:
+	jmp    *0x20a31a(%rip)        
 	push   $0x2f
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001e40 <__cudaRegisterFunction@plt>:
-	jmp    *0x20a352(%rip)        
+0000000000001e80 <strcmp@plt>:
+	jmp    *0x20a312(%rip)        
 	push   $0x30
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001e50 <cudaFree@plt>:
-	jmp    *0x20a34a(%rip)        
+0000000000001e90 <__cudaRegisterFunction@plt>:
+	jmp    *0x20a30a(%rip)        
 	push   $0x31
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001e60 <toff_gate_target_big(float2*)@plt>:
-	jmp    *0x20a342(%rip)        
+0000000000001ea0 <cudaFree@plt>:
+	jmp    *0x20a302(%rip)        
 	push   $0x32
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001e70 <ryy_gate(float2*, float)@plt>:
-	jmp    *0x20a33a(%rip)        
+0000000000001eb0 <toff_gate_target_big(float2*)@plt>:
+	jmp    *0x20a2fa(%rip)        
 	push   $0x33
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001e80 <puts@plt>:
-	jmp    *0x20a332(%rip)        
+0000000000001ec0 <ryy_gate(float2*, float)@plt>:
+	jmp    *0x20a2f2(%rip)        
 	push   $0x34
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001e90 <actionOnSingleQubit(float2*, float2*, unsigned long, unsigned long*)@plt>:
-	jmp    *0x20a32a(%rip)        
+0000000000001ed0 <puts@plt>:
+	jmp    *0x20a2ea(%rip)        
 	push   $0x35
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001ea0 <__cudaPopCallConfiguration@plt>:
-	jmp    *0x20a322(%rip)        
+0000000000001ee0 <actionOnSingleQubit(float2*, float2*, unsigned long, unsigned long*)@plt>:
+	jmp    *0x20a2e2(%rip)        
 	push   $0x36
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001eb0 <cudaDeviceSynchronize@plt>:
-	jmp    *0x20a31a(%rip)        
+0000000000001ef0 <__cudaPopCallConfiguration@plt>:
+	jmp    *0x20a2da(%rip)        
 	push   $0x37
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001ec0 <rz_gate(float2*, float)@plt>:
-	jmp    *0x20a312(%rip)        
+0000000000001f00 <cudaDeviceSynchronize@plt>:
+	jmp    *0x20a2d2(%rip)        
 	push   $0x38
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001ed0 <__cudaPushCallConfiguration@plt>:
-	jmp    *0x20a30a(%rip)        
+0000000000001f10 <rz_gate(float2*, float)@plt>:
+	jmp    *0x20a2ca(%rip)        
 	push   $0x39
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001ee0 <h_gate(float2*)@plt>:
-	jmp    *0x20a302(%rip)        
+0000000000001f20 <__cudaPushCallConfiguration@plt>:
+	jmp    *0x20a2c2(%rip)        
 	push   $0x3a
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001ef0 <sqrtf@plt>:
-	jmp    *0x20a2fa(%rip)        
+0000000000001f30 <h_gate(float2*)@plt>:
+	jmp    *0x20a2ba(%rip)        
 	push   $0x3b
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001f00 <__cudaRegisterFatBinaryEnd@plt>:
-	jmp    *0x20a2f2(%rip)        
+0000000000001f40 <sqrtf@plt>:
+	jmp    *0x20a2b2(%rip)        
 	push   $0x3c
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001f10 <swap_gate(float2*)@plt>:
-	jmp    *0x20a2ea(%rip)        
+0000000000001f50 <__cudaRegisterFatBinaryEnd@plt>:
+	jmp    *0x20a2aa(%rip)        
 	push   $0x3d
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001f20 <rx_gate(float2*, float)@plt>:
-	jmp    *0x20a2e2(%rip)        
+0000000000001f60 <swap_gate(float2*)@plt>:
+	jmp    *0x20a2a2(%rip)        
 	push   $0x3e
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001f30 <qsort@plt>:
-	jmp    *0x20a2da(%rip)        
+0000000000001f70 <rx_gate(float2*, float)@plt>:
+	jmp    *0x20a29a(%rip)        
 	push   $0x3f
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
 
-0000000000001f40 <cudaSetDevice@plt>:
-	jmp    *0x20a2d2(%rip)        
+0000000000001f80 <qsort@plt>:
+	jmp    *0x20a292(%rip)        
 	push   $0x40
-	jmp    1b30 <.plt>
+	jmp    1b70 <.plt>
+
+0000000000001f90 <cudaSetDevice@plt>:
+	jmp    *0x20a28a(%rip)        
+	push   $0x41
+	jmp    1b70 <.plt>
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -1,425 +1,425 @@
 
 
 
 Disassembly of section .text:
 
-0000000000001f50 <__sti____cudaRegisterAll()>:
+0000000000001fa0 <__sti____cudaRegisterAll()>:
 __sti____cudaRegisterAll():
 	push   %rbp
-	lea    0x20a2d0(%rip),%rdi        
-	call   1d10 <__cudaRegisterFatBinary@plt>
+	lea    0x20a288(%rip),%rdi        
+	call   1d60 <__cudaRegisterFatBinary@plt>
 	push   $0x0
 	xor    %r9d,%r9d
 	mov    $0xffffffff,%r8d
 	push   $0x0
-	lea    0x2ba7(%rip),%rcx        
+	lea    0x2be7(%rip),%rcx        
 	mov    %rax,%rdi
 	mov    %rax,%rbp
 	push   $0x0
-	mov    0x20a048(%rip),%rsi        
+	mov    0x209ff8(%rip),%rsi        
 	mov    %rcx,%rdx
 	push   $0x0
-	mov    %rax,0x20a2bc(%rip)        
-	call   1e40 <__cudaRegisterFunction@plt>
+	mov    %rax,0x20a274(%rip)        
+	call   1e90 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
 	mov    %rbp,%rdi
 	xor    %r9d,%r9d
 	push   $0x0
-	lea    0x2b9c(%rip),%rcx        
-	mov    0x20a015(%rip),%rsi        
+	lea    0x2bdc(%rip),%rcx        
+	mov    0x209fc5(%rip),%rsi        
 	mov    $0xffffffff,%r8d
 	push   $0x0
 	mov    %rcx,%rdx
 	push   $0x0
 	push   $0x0
-	call   1e40 <__cudaRegisterFunction@plt>
+	call   1e90 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
 	mov    %rbp,%rdi
 	xor    %r9d,%r9d
 	push   $0x0
-	lea    0x2b96(%rip),%rcx        
-	mov    0x209fff(%rip),%rsi        
+	lea    0x2bd6(%rip),%rcx        
+	mov    0x209faf(%rip),%rsi        
 	mov    $0xffffffff,%r8d
 	push   $0x0
 	mov    %rcx,%rdx
 	push   $0x0
 	push   $0x0
-	call   1e40 <__cudaRegisterFunction@plt>
-	mov    0x20a254(%rip),%rdi        
+	call   1e90 <__cudaRegisterFunction@plt>
+	mov    0x20a20c(%rip),%rdi        
 	add    $0x20,%rsp
-	call   1f00 <__cudaRegisterFatBinaryEnd@plt>
+	call   1f50 <__cudaRegisterFatBinaryEnd@plt>
 	lea    0xdc(%rip),%rdi        
 	pop    %rbp
-	jmp    49e0 <atexit>
+	jmp    4a50 <atexit>
 	nopw   0x0(%rax,%rax,1)
 
-0000000000002010 <deregister_tm_clones>:
+0000000000002060 <deregister_tm_clones>:
 deregister_tm_clones():
-	lea    0x20a211(%rip),%rdi        
-	lea    0x20a20a(%rip),%rax        
+	lea    0x20a1c9(%rip),%rdi        
+	lea    0x20a1c2(%rip),%rax        
 	cmp    %rdi,%rax
-	je     2038 <deregister_tm_clones+0x28>
-	mov    0x209fb6(%rip),%rax        
+	je     2088 <deregister_tm_clones+0x28>
+	mov    0x209f66(%rip),%rax        
 	test   %rax,%rax
-	je     2038 <deregister_tm_clones+0x28>
+	je     2088 <deregister_tm_clones+0x28>
 	jmp    *%rax
 	nopl   0x0(%rax)
 	ret
 	nopl   0x0(%rax)
 
-0000000000002040 <register_tm_clones>:
+0000000000002090 <register_tm_clones>:
 register_tm_clones():
-	lea    0x20a1e1(%rip),%rdi        
-	lea    0x20a1da(%rip),%rsi        
+	lea    0x20a199(%rip),%rdi        
+	lea    0x20a192(%rip),%rsi        
 	sub    %rdi,%rsi
 	mov    %rsi,%rax
 	shr    $0x3f,%rsi
 	sar    $0x3,%rax
 	add    %rax,%rsi
 	sar    $1,%rsi
-	je     2078 <register_tm_clones+0x38>
-	mov    0x209f8d(%rip),%rax        
+	je     20c8 <register_tm_clones+0x38>
+	mov    0x209f3d(%rip),%rax        
 	test   %rax,%rax
-	je     2078 <register_tm_clones+0x38>
+	je     20c8 <register_tm_clones+0x38>
 	jmp    *%rax
 	nopw   0x0(%rax,%rax,1)
 	ret
 	nopl   0x0(%rax)
 
-0000000000002080 <__do_global_dtors_aux>:
+00000000000020d0 <__do_global_dtors_aux>:
 __do_global_dtors_aux():
-	cmpb   $0x0,0x20a1b9(%rip)        
-	jne    20b8 <__do_global_dtors_aux+0x38>
+	cmpb   $0x0,0x20a171(%rip)        
+	jne    2108 <__do_global_dtors_aux+0x38>
 	push   %rbp
-	cmpq   $0x0,0x209f1e(%rip)        
+	cmpq   $0x0,0x209ece(%rip)        
 	mov    %rsp,%rbp
-	je     20a3 <__do_global_dtors_aux+0x23>
-	mov    0x20a182(%rip),%rdi        
-	call   1c40 <__cxa_finalize@plt>
-	call   2010 <deregister_tm_clones>
-	movb   $0x1,0x20a191(%rip)        
+	je     20f3 <__do_global_dtors_aux+0x23>
+	mov    0x20a13a(%rip),%rdi        
+	call   1c90 <__cxa_finalize@plt>
+	call   2060 <deregister_tm_clones>
+	movb   $0x1,0x20a149(%rip)        
 	pop    %rbp
 	ret
 	nopl   0x0(%rax)
 	ret
 	nopl   0x0(%rax)
 
-00000000000020c0 <frame_dummy>:
+0000000000002110 <frame_dummy>:
 frame_dummy():
-	jmp    2040 <register_tm_clones>
+	jmp    2090 <register_tm_clones>
 	cs nopw 0x0(%rax,%rax,1)
 	nop
 
-00000000000020d0 <compare(void const*, void const*)>:
+0000000000002120 <compare(void const*, void const*)>:
 compare(void const*, void const*):
 	mov    (%rdi),%eax
 	sub    (%rsi),%eax
 	ret
 	nop
 	cs nopw 0x0(%rax,%rax,1)
 
-00000000000020e0 <__cudaUnregisterBinaryUtil()>:
+0000000000002130 <__cudaUnregisterBinaryUtil()>:
 __cudaUnregisterBinaryUtil():
-	mov    0x20a161(%rip),%rdi        
-	jmp    1bf0 <__cudaUnregisterFatBinary@plt>
+	mov    0x20a119(%rip),%rdi        
+	jmp    1c40 <__cudaUnregisterFatBinary@plt>
 	nopl   0x0(%rax)
 
-00000000000020f0 <x_gate(float2*)>:
+0000000000002140 <x_gate(float2*)>:
 x_gate(float2*):
-	movaps 0x2a99(%rip),%xmm0        
+	movaps 0x2ad9(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movss  0x2a9e(%rip),%xmm0        
+	movss  0x2ade(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	nopw   0x0(%rax,%rax,1)
 
-0000000000002110 <y_gate(float2*)>:
+0000000000002160 <y_gate(float2*)>:
 y_gate(float2*):
-	movaps 0x2a99(%rip),%xmm0        
+	movaps 0x2ad9(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movaps 0x2a9f(%rip),%xmm0        
+	movaps 0x2adf(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000002130 <z_gate(float2*)>:
+0000000000002180 <z_gate(float2*)>:
 z_gate(float2*):
-	movss  0x2a68(%rip),%xmm0        
+	movss  0x2aa8(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movaps 0x2a8e(%rip),%xmm0        
+	movaps 0x2ace(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	nopw   0x0(%rax,%rax,1)
 
-0000000000002150 <s_gate(float2*)>:
+00000000000021a0 <s_gate(float2*)>:
 s_gate(float2*):
-	movss  0x2a48(%rip),%xmm0        
+	movss  0x2a88(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movaps 0x2a7e(%rip),%xmm0        
+	movaps 0x2abe(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	nopw   0x0(%rax,%rax,1)
 
-0000000000002170 <sdg_gate(float2*)>:
+00000000000021c0 <sdg_gate(float2*)>:
 sdg_gate(float2*):
-	movss  0x2a28(%rip),%xmm0        
+	movss  0x2a68(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movaps 0x2a2e(%rip),%xmm0        
+	movaps 0x2a6e(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	nopw   0x0(%rax,%rax,1)
 
-0000000000002190 <t_gate(float2*)>:
+00000000000021e0 <t_gate(float2*)>:
 t_gate(float2*):
-	movss  0x2a08(%rip),%xmm0        
+	movss  0x2a48(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movaps 0x2a4e(%rip),%xmm0        
+	movaps 0x2a8e(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	nopw   0x0(%rax,%rax,1)
 
-00000000000021b0 <tdg_gate(float2*)>:
+0000000000002200 <tdg_gate(float2*)>:
 tdg_gate(float2*):
-	movss  0x29e8(%rip),%xmm0        
+	movss  0x2a28(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movaps 0x2a3e(%rip),%xmm0        
+	movaps 0x2a7e(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	nopw   0x0(%rax,%rax,1)
 
-00000000000021d0 <h_gate(float2*)>:
+0000000000002220 <h_gate(float2*)>:
 h_gate(float2*):
-	movaps 0x2a39(%rip),%xmm0        
+	movaps 0x2a79(%rip),%xmm0        
 	movups %xmm0,(%rdi)
-	movaps 0x2a3f(%rip),%xmm0        
+	movaps 0x2a7f(%rip),%xmm0        
 	movups %xmm0,0x10(%rdi)
 	ret
 	cs nopw 0x0(%rax,%rax,1)
 
-00000000000021f0 <rx_gate(float2*, float)>:
+0000000000002240 <rx_gate(float2*, float)>:
 rx_gate(float2*, float):
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
-	mulss  0x2ae0(%rip),%xmm0        
+	mulss  0x2b20(%rip),%xmm0        
 	lea    0xc(%rsp),%rdi
 	lea    0x8(%rsp),%rsi
-	call   1c30 <sincosf@plt>
+	call   1c80 <sincosf@plt>
 	movss  0x8(%rsp),%xmm1
 	movss  0xc(%rsp),%xmm0
 	movq   $0x0,0x4(%rbx)
-	xorps  0x2a06(%rip),%xmm0        
+	xorps  0x2a46(%rip),%xmm0        
 	movl   $0x0,0x10(%rbx)
 	movl   $0x0,0x1c(%rbx)
 	movss  %xmm1,(%rbx)
 	movss  %xmm0,0xc(%rbx)
 	movss  %xmm0,0x14(%rbx)
 	movss  %xmm1,0x18(%rbx)
 	add    $0x10,%rsp
 	pop    %rbx
 	ret
 	nopl   0x0(%rax,%rax,1)
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000002260 <ry_gate(float2*, float)>:
+00000000000022b0 <ry_gate(float2*, float)>:
 ry_gate(float2*, float):
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
-	mulss  0x2a70(%rip),%xmm0        
+	mulss  0x2ab0(%rip),%xmm0        
 	lea    0xc(%rsp),%rdi
 	lea    0x8(%rsp),%rsi
-	call   1c30 <sincosf@plt>
+	call   1c80 <sincosf@plt>
 	movss  0xc(%rsp),%xmm1
 	movss  0x8(%rsp),%xmm0
 	movl   $0x0,0x4(%rbx)
 	movl   $0x0,0xc(%rbx)
 	movaps %xmm1,%xmm2
-	xorps  0x298d(%rip),%xmm2        
+	xorps  0x29cd(%rip),%xmm2        
 	movl   $0x0,0x14(%rbx)
 	movl   $0x0,0x1c(%rbx)
 	movss  %xmm0,(%rbx)
 	movss  %xmm2,0x8(%rbx)
 	movss  %xmm1,0x10(%rbx)
 	movss  %xmm0,0x18(%rbx)
 	add    $0x10,%rsp
 	pop    %rbx
 	ret
 	nopw   0x0(%rax,%rax,1)
 
-00000000000022d0 <rz_gate(float2*, float)>:
+0000000000002320 <rz_gate(float2*, float)>:
 rz_gate(float2*, float):
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
-	mulss  0x2a00(%rip),%xmm0        
+	mulss  0x2a40(%rip),%xmm0        
 	lea    0xc(%rsp),%rdi
 	lea    0x8(%rsp),%rsi
-	call   1c30 <sincosf@plt>
+	call   1c80 <sincosf@plt>
 	movss  0xc(%rsp),%xmm0
 	movss  0x8(%rsp),%xmm1
 	movq   $0x0,0x8(%rbx)
 	movq   $0x0,0x10(%rbx)
 	movaps %xmm0,%xmm2
-	xorps  0x291b(%rip),%xmm2        
+	xorps  0x295b(%rip),%xmm2        
 	movss  %xmm1,(%rbx)
 	movss  %xmm1,0x18(%rbx)
 	movss  %xmm2,0x4(%rbx)
 	movss  %xmm0,0x1c(%rbx)
 	add    $0x10,%rsp
 	pop    %rbx
 	ret
 	xchg   %ax,%ax
 
-0000000000002330 <damp_i_gate(float2*, float)>:
+0000000000002380 <damp_i_gate(float2*, float)>:
 damp_i_gate(float2*, float):
 	pxor   %xmm3,%xmm3
 	comiss %xmm3,%xmm0
-	jbe    2346 <damp_i_gate(float2*, float)+0x16>
-	movss  0x29a3(%rip),%xmm1        
+	jbe    2396 <damp_i_gate(float2*, float)+0x16>
+	movss  0x29e3(%rip),%xmm1        
 	comiss %xmm0,%xmm1
-	ja     2350 <damp_i_gate(float2*, float)+0x20>
+	ja     23a0 <damp_i_gate(float2*, float)+0x20>
 	ret
 	nopw   0x0(%rax,%rax,1)
 	subss  %xmm0,%xmm1
-	movss  0x2844(%rip),%xmm2        
+	movss  0x2884(%rip),%xmm2        
 	movq   $0x0,0x10(%rdi)
 	movups %xmm2,(%rdi)
 	ucomiss %xmm1,%xmm3
 	movaps %xmm1,%xmm2
 	sqrtss %xmm2,%xmm2
-	ja     2380 <damp_i_gate(float2*, float)+0x50>
+	ja     23d0 <damp_i_gate(float2*, float)+0x50>
 	movl   $0x0,0x1c(%rdi)
 	movss  %xmm2,0x18(%rdi)
 	ret
 	sub    $0x18,%rsp
 	movaps %xmm1,%xmm0
 	mov    %rdi,0x8(%rsp)
 	movss  %xmm2,0x4(%rsp)
-	call   1ef0 <sqrtf@plt>
+	call   1f40 <sqrtf@plt>
 	mov    0x8(%rsp),%rdi
 	movss  0x4(%rsp),%xmm2
 	movl   $0x0,0x1c(%rdi)
 	movss  %xmm2,0x18(%rdi)
 	add    $0x18,%rsp
 	ret
 	nopl   (%rax)
 	cs nopw 0x0(%rax,%rax,1)
 
-00000000000023c0 <pd_gate(float2*, float)>:
+0000000000002410 <pd_gate(float2*, float)>:
 pd_gate(float2*, float):
 	pxor   %xmm2,%xmm2
 	comiss %xmm2,%xmm0
-	jbe    23d6 <pd_gate(float2*, float)+0x16>
-	movss  0x2913(%rip),%xmm1        
+	jbe    2426 <pd_gate(float2*, float)+0x16>
+	movss  0x2953(%rip),%xmm1        
 	comiss %xmm0,%xmm1
-	ja     23e0 <pd_gate(float2*, float)+0x20>
+	ja     2430 <pd_gate(float2*, float)+0x20>
 	ret
 	nopw   0x0(%rax,%rax,1)
 	ucomiss %xmm0,%xmm2
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x10(%rdi)
 	movups %xmm1,(%rdi)
 	movaps %xmm0,%xmm1
 	sqrtss %xmm1,%xmm1
-	ja     2408 <pd_gate(float2*, float)+0x48>
+	ja     2458 <pd_gate(float2*, float)+0x48>
 	movl   $0x0,0x1c(%rdi)
 	movss  %xmm1,0x18(%rdi)
 	ret
 	sub    $0x18,%rsp
 	mov    %rdi,0x8(%rsp)
 	movss  %xmm1,0x4(%rsp)
-	call   1ef0 <sqrtf@plt>
+	call   1f40 <sqrtf@plt>
 	mov    0x8(%rsp),%rdi
 	movss  0x4(%rsp),%xmm1
 	movl   $0x0,0x1c(%rdi)
 	movss  %xmm1,0x18(%rdi)
 	add    $0x18,%rsp
 	ret
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002440 <ad_gate(float2*, float)>:
+0000000000002490 <ad_gate(float2*, float)>:
 ad_gate(float2*, float):
 	pxor   %xmm2,%xmm2
 	comiss %xmm2,%xmm0
-	jbe    2456 <ad_gate(float2*, float)+0x16>
-	movss  0x2893(%rip),%xmm1        
+	jbe    24a6 <ad_gate(float2*, float)+0x16>
+	movss  0x28d3(%rip),%xmm1        
 	comiss %xmm0,%xmm1
-	ja     2460 <ad_gate(float2*, float)+0x20>
+	ja     24b0 <ad_gate(float2*, float)+0x20>
 	ret
 	nopw   0x0(%rax,%rax,1)
 	sub    $0x18,%rsp
 	ucomiss %xmm0,%xmm2
 	movaps %xmm0,%xmm1
 	movq   $0x0,(%rdi)
 	sqrtss %xmm1,%xmm1
-	ja     2498 <ad_gate(float2*, float)+0x58>
+	ja     24e8 <ad_gate(float2*, float)+0x58>
 	movl   $0x0,0xc(%rdi)
 	movq   $0x0,0x10(%rdi)
 	movq   $0x0,0x18(%rdi)
 	movss  %xmm1,0x8(%rdi)
 	add    $0x18,%rsp
 	ret
 	mov    %rdi,0x8(%rsp)
 	movss  %xmm1,0x4(%rsp)
-	call   1ef0 <sqrtf@plt>
+	call   1f40 <sqrtf@plt>
 	mov    0x8(%rsp),%rdi
 	movss  0x4(%rsp),%xmm1
-	jmp    2477 <ad_gate(float2*, float)+0x37>
+	jmp    24c7 <ad_gate(float2*, float)+0x37>
 	nop
 	cs nopw 0x0(%rax,%rax,1)
 
-00000000000024c0 <swap_gate(float2*)>:
+0000000000002510 <swap_gate(float2*)>:
 swap_gate(float2*):
-	movss  0x26d8(%rip),%xmm1        
+	movss  0x2718(%rip),%xmm1        
 	pxor   %xmm0,%xmm0
 	movups %xmm1,(%rdi)
 	movups %xmm1,0x30(%rdi)
-	movaps 0x26b6(%rip),%xmm1        
+	movaps 0x26f6(%rip),%xmm1        
 	movups %xmm0,0x10(%rdi)
 	movups %xmm0,0x20(%rdi)
 	movups %xmm1,0x40(%rdi)
 	movups %xmm0,0x50(%rdi)
 	movups %xmm0,0x60(%rdi)
 	movups %xmm1,0x70(%rdi)
 	ret
 	nopl   (%rax)
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000002500 <iswap_gate(float2*)>:
+0000000000002550 <iswap_gate(float2*)>:
 iswap_gate(float2*):
-	movaps 0x26b9(%rip),%xmm1        
-	movss  0x2691(%rip),%xmm0        
+	movaps 0x26f9(%rip),%xmm1        
+	movss  0x26d1(%rip),%xmm0        
 	movups %xmm0,(%rdi)
 	pxor   %xmm0,%xmm0
 	movups %xmm0,0x10(%rdi)
 	movups %xmm0,0x20(%rdi)
 	movups %xmm1,0x30(%rdi)
-	movaps 0x26b7(%rip),%xmm1        
+	movaps 0x26f7(%rip),%xmm1        
 	movups %xmm0,0x50(%rdi)
 	movups %xmm0,0x60(%rdi)
-	movaps 0x2658(%rip),%xmm0        
+	movaps 0x2698(%rip),%xmm0        
 	movups %xmm1,0x40(%rdi)
 	movups %xmm0,0x70(%rdi)
 	ret
 	nopl   0x0(%rax,%rax,1)
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000002550 <cphase_gate(float2*, float)>:
+00000000000025a0 <cphase_gate(float2*, float)>:
 cphase_gate(float2*, float):
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
 	lea    0xc(%rsp),%rdi
 	lea    0x8(%rsp),%rsi
-	call   1c30 <sincosf@plt>
+	call   1c80 <sincosf@plt>
 	pxor   %xmm0,%xmm0
-	movaps 0x261e(%rip),%xmm2        
-	movss  0x2626(%rip),%xmm1        
+	movaps 0x265e(%rip),%xmm2        
+	movss  0x2666(%rip),%xmm1        
 	movups %xmm0,0x10(%rbx)
 	movups %xmm0,0x30(%rbx)
 	movups %xmm0,0x40(%rbx)
 	movups %xmm0,0x60(%rbx)
 	movss  0x8(%rsp),%xmm0
 	movq   $0x0,0x70(%rbx)
 	movss  %xmm0,0x78(%rbx)
@@ -429,78 +429,78 @@
 	movups %xmm1,0x50(%rbx)
 	movss  %xmm0,0x7c(%rbx)
 	add    $0x10,%rsp
 	pop    %rbx
 	ret
 	nopl   0x0(%rax)
 
-00000000000025c0 <cnot_gate_control_big(float2*)>:
+0000000000002610 <cnot_gate_control_big(float2*)>:
 cnot_gate_control_big(float2*):
-	movaps 0x25c9(%rip),%xmm2        
+	movaps 0x2609(%rip),%xmm2        
 	pxor   %xmm0,%xmm0
-	movss  0x25cd(%rip),%xmm1        
+	movss  0x260d(%rip),%xmm1        
 	movups %xmm1,(%rdi)
 	movups %xmm0,0x10(%rdi)
 	movups %xmm2,0x20(%rdi)
 	movups %xmm0,0x30(%rdi)
 	movups %xmm0,0x40(%rdi)
 	movups %xmm2,0x50(%rdi)
 	movups %xmm0,0x60(%rdi)
 	movups %xmm1,0x70(%rdi)
 	ret
 	nopl   (%rax)
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000002600 <cnot_gate_control_small(float2*)>:
+0000000000002650 <cnot_gate_control_small(float2*)>:
 cnot_gate_control_small(float2*):
-	movaps 0x2589(%rip),%xmm1        
+	movaps 0x25c9(%rip),%xmm1        
 	pxor   %xmm0,%xmm0
-	movss  0x258d(%rip),%xmm2        
+	movss  0x25cd(%rip),%xmm2        
 	movups %xmm2,(%rdi)
 	movups %xmm0,0x10(%rdi)
 	movups %xmm0,0x20(%rdi)
 	movups %xmm1,0x30(%rdi)
 	movups %xmm0,0x40(%rdi)
 	movups %xmm2,0x50(%rdi)
 	movups %xmm1,0x60(%rdi)
 	movups %xmm0,0x70(%rdi)
 	ret
 	nopl   (%rax)
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000002640 <cz_gate(float2*)>:
+0000000000002690 <cz_gate(float2*)>:
 cz_gate(float2*):
 	pxor   %xmm0,%xmm0
-	movaps 0x2545(%rip),%xmm2        
-	movss  0x254d(%rip),%xmm1        
+	movaps 0x2585(%rip),%xmm2        
+	movss  0x258d(%rip),%xmm1        
 	movups %xmm0,0x10(%rdi)
 	movups %xmm0,0x30(%rdi)
 	movups %xmm0,0x40(%rdi)
 	movups %xmm0,0x60(%rdi)
-	movaps 0x2566(%rip),%xmm0        
+	movaps 0x25a6(%rip),%xmm0        
 	movups %xmm1,(%rdi)
 	movups %xmm2,0x20(%rdi)
 	movups %xmm1,0x50(%rdi)
 	movups %xmm0,0x70(%rdi)
 	ret
 	nopw   0x0(%rax,%rax,1)
 
-0000000000002680 <rxx_gate(float2*, float)>:
+00000000000026d0 <rxx_gate(float2*, float)>:
 rxx_gate(float2*, float):
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
-	mulss  0x2650(%rip),%xmm0        
+	mulss  0x2690(%rip),%xmm0        
 	lea    0xc(%rsp),%rdi
 	lea    0x8(%rsp),%rsi
-	call   1c30 <sincosf@plt>
+	call   1c80 <sincosf@plt>
 	movss  0x8(%rsp),%xmm1
 	movss  0xc(%rsp),%xmm0
 	movq   $0x0,0x4(%rbx)
-	xorps  0x2576(%rip),%xmm0        
+	xorps  0x25b6(%rip),%xmm0        
 	movq   $0x0,0xc(%rbx)
 	movq   $0x0,0x14(%rbx)
 	movq   $0x0,0x20(%rbx)
 	movq   $0x0,0x2c(%rbx)
 	movq   $0x0,0x38(%rbx)
 	movq   $0x0,0x40(%rbx)
 	movl   $0x0,0x48(%rbx)
@@ -519,29 +519,29 @@
 	movss  %xmm1,0x78(%rbx)
 	add    $0x10,%rsp
 	pop    %rbx
 	ret
 	nop
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000002750 <ryy_gate(float2*, float)>:
+00000000000027a0 <ryy_gate(float2*, float)>:
 ryy_gate(float2*, float):
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
-	mulss  0x2580(%rip),%xmm0        
+	mulss  0x25c0(%rip),%xmm0        
 	lea    0xc(%rsp),%rdi
 	lea    0x8(%rsp),%rsi
-	call   1c30 <sincosf@plt>
+	call   1c80 <sincosf@plt>
 	movss  0xc(%rsp),%xmm1
 	movss  0x8(%rsp),%xmm0
 	movq   $0x0,0x4(%rbx)
 	movq   $0x0,0xc(%rbx)
 	movaps %xmm1,%xmm2
-	xorps  0x249b(%rip),%xmm2        
+	xorps  0x24db(%rip),%xmm2        
 	movq   $0x0,0x14(%rbx)
 	movq   $0x0,0x20(%rbx)
 	movq   $0x0,0x2c(%rbx)
 	movq   $0x0,0x38(%rbx)
 	movq   $0x0,0x40(%rbx)
 	movl   $0x0,0x48(%rbx)
 	movq   $0x0,0x54(%rbx)
@@ -558,29 +558,29 @@
 	movss  %xmm1,0x64(%rbx)
 	movss  %xmm0,0x78(%rbx)
 	add    $0x10,%rsp
 	pop    %rbx
 	ret
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002820 <rzz_gate(float2*, float)>:
+0000000000002870 <rzz_gate(float2*, float)>:
 rzz_gate(float2*, float):
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
-	mulss  0x24b0(%rip),%xmm0        
+	mulss  0x24f0(%rip),%xmm0        
 	lea    0xc(%rsp),%rdi
 	lea    0x8(%rsp),%rsi
-	call   1c30 <sincosf@plt>
+	call   1c80 <sincosf@plt>
 	movss  0xc(%rsp),%xmm1
 	movss  0x8(%rsp),%xmm0
 	movq   $0x0,0x8(%rbx)
 	movq   $0x0,0x10(%rbx)
 	movaps %xmm1,%xmm2
-	xorps  0x23cb(%rip),%xmm2        
+	xorps  0x240b(%rip),%xmm2        
 	movq   $0x0,0x18(%rbx)
 	movq   $0x0,0x20(%rbx)
 	movq   $0x0,0x30(%rbx)
 	movq   $0x0,0x38(%rbx)
 	movq   $0x0,0x40(%rbx)
 	movq   $0x0,0x48(%rbx)
 	movq   $0x0,0x58(%rbx)
@@ -597,74 +597,74 @@
 	movss  %xmm2,0x7c(%rbx)
 	add    $0x10,%rsp
 	pop    %rbx
 	ret
 	nopl   0x0(%rax)
 	cs nopw 0x0(%rax,%rax,1)
 
-00000000000028f0 <syc_gate(float2*)>:
+0000000000002940 <syc_gate(float2*)>:
 syc_gate(float2*):
-	movaps 0x2349(%rip),%xmm1        
-	movss  0x22a1(%rip),%xmm0        
+	movaps 0x2389(%rip),%xmm1        
+	movss  0x22e1(%rip),%xmm0        
 	movups %xmm0,(%rdi)
 	pxor   %xmm0,%xmm0
 	movups %xmm0,0x10(%rdi)
 	movups %xmm0,0x20(%rdi)
 	movups %xmm1,0x30(%rdi)
-	movaps 0x2297(%rip),%xmm1        
+	movaps 0x22d7(%rip),%xmm1        
 	movups %xmm0,0x50(%rdi)
 	movups %xmm0,0x60(%rdi)
-	movaps 0x2328(%rip),%xmm0        
+	movaps 0x2368(%rip),%xmm0        
 	movups %xmm1,0x40(%rdi)
 	movups %xmm0,0x70(%rdi)
 	ret
 	nopl   0x0(%rax,%rax,1)
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000002940 <toff_gate_target_small(float2*)>:
+0000000000002990 <toff_gate_target_small(float2*)>:
 toff_gate_target_small(float2*):
-	movss  0x239c(%rip),%xmm0        
+	movss  0x23dc(%rip),%xmm0        
 	xor    %eax,%eax
-	jmp    2961 <toff_gate_target_small(float2*)+0x21>
+	jmp    29b1 <toff_gate_target_small(float2*)+0x21>
 	nopl   0x0(%rax)
 	movss  %xmm0,(%rdi,%rax,8)
 	movl   $0x0,0x4(%rdi,%rax,8)
 	add    $0x1,%rax
 	cmp    $0x2f,%rax
-	ja     2980 <toff_gate_target_small(float2*)+0x40>
+	ja     29d0 <toff_gate_target_small(float2*)+0x40>
 	imul   $0x38e38e39,%eax,%edx
 	cmp    $0x1c71c71c,%edx
-	jbe    2950 <toff_gate_target_small(float2*)+0x10>
+	jbe    29a0 <toff_gate_target_small(float2*)+0x10>
 	movl   $0x0,(%rdi,%rax,8)
-	jmp    2955 <toff_gate_target_small(float2*)+0x15>
+	jmp    29a5 <toff_gate_target_small(float2*)+0x15>
 	xchg   %ax,%ax
 	movl   $0x0,(%rdi,%rax,8)
 	movl   $0x0,0x4(%rdi,%rax,8)
 	cmp    $0x3f,%eax
-	jne    295d <toff_gate_target_small(float2*)+0x1d>
+	jne    29ad <toff_gate_target_small(float2*)+0x1d>
 	movss  %xmm0,0x1b8(%rdi)
 	movss  %xmm0,0x1f0(%rdi)
 	ret
 	nop
 	cs nopw 0x0(%rax,%rax,1)
 
-00000000000029b0 <toff_gate_target_mid(float2*)>:
+0000000000002a00 <toff_gate_target_mid(float2*)>:
 toff_gate_target_mid(float2*):
-	movdqa 0x22e8(%rip),%xmm4        
+	movdqa 0x2328(%rip),%xmm4        
 	pxor   %xmm3,%xmm3
 	mov    %rdi,%rax
-	movdqa 0x2299(%rip),%xmm5        
+	movdqa 0x22d9(%rip),%xmm5        
 	movdqa %xmm3,%xmm7
 	lea    0x1e0(%rdi),%rdx
-	movdqa 0x2295(%rip),%xmm11        
-	movdqa 0x229c(%rip),%xmm10        
+	movdqa 0x22d5(%rip),%xmm11        
+	movdqa 0x22dc(%rip),%xmm10        
 	pcmpgtd %xmm4,%xmm7
-	movaps 0x22c0(%rip),%xmm8        
+	movaps 0x2300(%rip),%xmm8        
 	pxor   %xmm6,%xmm6
-	movdqa 0x2293(%rip),%xmm9        
+	movdqa 0x22d3(%rip),%xmm9        
 	nopl   (%rax)
 	movdqa %xmm5,%xmm0
 	movdqa %xmm3,%xmm12
 	movdqa %xmm7,%xmm13
 	movups 0x10(%rax),%xmm15
 	movdqa %xmm0,%xmm2
 	movdqa %xmm0,%xmm1
@@ -717,38 +717,38 @@
 	movaps %xmm2,%xmm0
 	movaps %xmm2,%xmm1
 	unpcklps %xmm6,%xmm1
 	unpckhps %xmm6,%xmm0
 	movups %xmm1,-0x20(%rax)
 	movups %xmm0,-0x10(%rax)
 	cmp    %rdx,%rax
-	jne    2a00 <toff_gate_target_mid(float2*)+0x50>
+	jne    2a50 <toff_gate_target_mid(float2*)+0x50>
 	movl   $0x3f800000,0x1a8(%rdi)
 	movq   $0x0,0x1e0(%rdi)
 	movq   $0x3f800000,0x1e8(%rdi)
 	movq   $0x0,0x1f0(%rdi)
 	movq   $0x0,0x1f8(%rdi)
 	ret
 	nopl   0x0(%rax)
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000002b50 <toff_gate_target_big(float2*)>:
+0000000000002ba0 <toff_gate_target_big(float2*)>:
 toff_gate_target_big(float2*):
-	movdqa 0x2148(%rip),%xmm4        
+	movdqa 0x2188(%rip),%xmm4        
 	pxor   %xmm3,%xmm3
 	mov    %rdi,%rax
-	movdqa 0x20f9(%rip),%xmm5        
+	movdqa 0x2139(%rip),%xmm5        
 	movdqa %xmm3,%xmm7
 	lea    0x1e0(%rdi),%rdx
-	movdqa 0x20f5(%rip),%xmm11        
-	movdqa 0x213c(%rip),%xmm10        
+	movdqa 0x2135(%rip),%xmm11        
+	movdqa 0x217c(%rip),%xmm10        
 	pcmpgtd %xmm4,%xmm7
-	movaps 0x2120(%rip),%xmm8        
+	movaps 0x2160(%rip),%xmm8        
 	pxor   %xmm6,%xmm6
-	movdqa 0x20f3(%rip),%xmm9        
+	movdqa 0x2133(%rip),%xmm9        
 	nopl   (%rax)
 	movdqa %xmm5,%xmm0
 	movdqa %xmm3,%xmm12
 	movdqa %xmm7,%xmm13
 	movups 0x10(%rax),%xmm15
 	movdqa %xmm0,%xmm2
 	movdqa %xmm0,%xmm1
@@ -801,38 +801,38 @@
 	movaps %xmm2,%xmm0
 	movaps %xmm2,%xmm1
 	unpcklps %xmm6,%xmm1
 	unpckhps %xmm6,%xmm0
 	movups %xmm1,-0x20(%rax)
 	movups %xmm0,-0x10(%rax)
 	cmp    %rdx,%rax
-	jne    2ba0 <toff_gate_target_big(float2*)+0x50>
-	movss  0x2031(%rip),%xmm0        
+	jne    2bf0 <toff_gate_target_big(float2*)+0x50>
+	movss  0x2071(%rip),%xmm0        
 	movq   $0x0,0x1e0(%rdi)
 	movq   $0x0,0x1e8(%rdi)
 	movq   $0x0,0x1f0(%rdi)
 	movq   $0x0,0x1f8(%rdi)
 	movss  %xmm0,0xf8(%rdi)
 	movss  %xmm0,0x1d8(%rdi)
 	ret
 
-0000000000002cf0 <fred_gate_control_big(float2*)>:
+0000000000002d40 <fred_gate_control_big(float2*)>:
 fred_gate_control_big(float2*):
-	movdqa 0x1fa8(%rip),%xmm4        
+	movdqa 0x1fe8(%rip),%xmm4        
 	pxor   %xmm3,%xmm3
 	mov    %rdi,%rax
-	movdqa 0x1f59(%rip),%xmm5        
+	movdqa 0x1f99(%rip),%xmm5        
 	movdqa %xmm3,%xmm7
 	lea    0x1e0(%rdi),%rdx
-	movdqa 0x1f55(%rip),%xmm11        
-	movdqa 0x1f5c(%rip),%xmm10        
+	movdqa 0x1f95(%rip),%xmm11        
+	movdqa 0x1f9c(%rip),%xmm10        
 	pcmpgtd %xmm4,%xmm7
-	movaps 0x1f80(%rip),%xmm8        
+	movaps 0x1fc0(%rip),%xmm8        
 	pxor   %xmm6,%xmm6
-	movdqa 0x1f93(%rip),%xmm9        
+	movdqa 0x1fd3(%rip),%xmm9        
 	nopl   (%rax)
 	movdqa %xmm5,%xmm0
 	movdqa %xmm3,%xmm12
 	movdqa %xmm7,%xmm13
 	movups 0x10(%rax),%xmm15
 	movdqa %xmm0,%xmm2
 	movdqa %xmm0,%xmm1
@@ -885,38 +885,38 @@
 	movaps %xmm2,%xmm0
 	movaps %xmm2,%xmm1
 	unpcklps %xmm6,%xmm1
 	unpckhps %xmm6,%xmm0
 	movups %xmm1,-0x20(%rax)
 	movups %xmm0,-0x10(%rax)
 	cmp    %rdx,%rax
-	jne    2d40 <fred_gate_control_big(float2*)+0x50>
-	movss  0x1e91(%rip),%xmm0        
+	jne    2d90 <fred_gate_control_big(float2*)+0x50>
+	movss  0x1ed1(%rip),%xmm0        
 	movq   $0x0,0x1e0(%rdi)
 	movq   $0x0,0x1e8(%rdi)
 	movq   $0x0,0x1f0(%rdi)
 	movq   $0x3f800000,0x1f8(%rdi)
 	movss  %xmm0,0x170(%rdi)
 	movss  %xmm0,0x1a8(%rdi)
 	ret
 
-0000000000002e90 <fred_gate_control_mid(float2*)>:
+0000000000002ee0 <fred_gate_control_mid(float2*)>:
 fred_gate_control_mid(float2*):
-	movdqa 0x1e08(%rip),%xmm4        
+	movdqa 0x1e48(%rip),%xmm4        
 	pxor   %xmm3,%xmm3
 	mov    %rdi,%rax
-	movdqa 0x1db9(%rip),%xmm5        
+	movdqa 0x1df9(%rip),%xmm5        
 	movdqa %xmm3,%xmm7
 	lea    0x1e0(%rdi),%rdx
-	movdqa 0x1db5(%rip),%xmm11        
-	movdqa 0x1dfc(%rip),%xmm10        
+	movdqa 0x1df5(%rip),%xmm11        
+	movdqa 0x1e3c(%rip),%xmm10        
 	pcmpgtd %xmm4,%xmm7
-	movaps 0x1de0(%rip),%xmm8        
+	movaps 0x1e20(%rip),%xmm8        
 	pxor   %xmm6,%xmm6
-	movdqa 0x1df3(%rip),%xmm9        
+	movdqa 0x1e33(%rip),%xmm9        
 	nopl   (%rax)
 	movdqa %xmm5,%xmm0
 	movdqa %xmm3,%xmm12
 	movdqa %xmm7,%xmm13
 	movups 0x10(%rax),%xmm15
 	movdqa %xmm0,%xmm2
 	movdqa %xmm0,%xmm1
@@ -969,38 +969,38 @@
 	movaps %xmm2,%xmm0
 	movaps %xmm2,%xmm1
 	unpcklps %xmm6,%xmm1
 	unpckhps %xmm6,%xmm0
 	movups %xmm1,-0x20(%rax)
 	movups %xmm0,-0x10(%rax)
 	cmp    %rdx,%rax
-	jne    2ee0 <fred_gate_control_mid(float2*)+0x50>
-	movss  0x1cf1(%rip),%xmm0        
+	jne    2f30 <fred_gate_control_mid(float2*)+0x50>
+	movss  0x1d31(%rip),%xmm0        
 	movq   $0x0,0x1e0(%rdi)
 	movq   $0x0,0x1e8(%rdi)
 	movq   $0x0,0x1f0(%rdi)
 	movq   $0x3f800000,0x1f8(%rdi)
 	movss  %xmm0,0xf0(%rdi)
 	movss  %xmm0,0x198(%rdi)
 	ret
 
-0000000000003030 <fred_gate_control_small(float2*)>:
+0000000000003080 <fred_gate_control_small(float2*)>:
 fred_gate_control_small(float2*):
-	movdqa 0x1c68(%rip),%xmm4        
+	movdqa 0x1ca8(%rip),%xmm4        
 	pxor   %xmm3,%xmm3
 	mov    %rdi,%rax
-	movdqa 0x1c19(%rip),%xmm5        
+	movdqa 0x1c59(%rip),%xmm5        
 	movdqa %xmm3,%xmm7
 	lea    0x1e0(%rdi),%rdx
-	movdqa 0x1c15(%rip),%xmm11        
-	movdqa 0x1c5c(%rip),%xmm10        
+	movdqa 0x1c55(%rip),%xmm11        
+	movdqa 0x1c9c(%rip),%xmm10        
 	pcmpgtd %xmm4,%xmm7
-	movaps 0x1c40(%rip),%xmm8        
+	movaps 0x1c80(%rip),%xmm8        
 	pxor   %xmm6,%xmm6
-	movdqa 0x1c03(%rip),%xmm9        
+	movdqa 0x1c43(%rip),%xmm9        
 	nopl   (%rax)
 	movdqa %xmm5,%xmm0
 	movdqa %xmm3,%xmm12
 	movdqa %xmm7,%xmm13
 	movups 0x10(%rax),%xmm15
 	movdqa %xmm0,%xmm2
 	movdqa %xmm0,%xmm1
@@ -1053,95 +1053,95 @@
 	movaps %xmm2,%xmm0
 	movaps %xmm2,%xmm1
 	unpcklps %xmm6,%xmm1
 	unpckhps %xmm6,%xmm0
 	movups %xmm1,-0x20(%rax)
 	movups %xmm0,-0x10(%rax)
 	cmp    %rdx,%rax
-	jne    3080 <fred_gate_control_small(float2*)+0x50>
-	movss  0x1b51(%rip),%xmm0        
+	jne    30d0 <fred_gate_control_small(float2*)+0x50>
+	movss  0x1b91(%rip),%xmm0        
 	movq   $0x0,0x1e0(%rdi)
 	movq   $0x0,0x1e8(%rdi)
 	movq   $0x0,0x1f0(%rdi)
 	movq   $0x3f800000,0x1f8(%rdi)
 	movss  %xmm0,0xe8(%rdi)
 	movss  %xmm0,0x158(%rdi)
 	ret
 
-00000000000031d0 <identityMat(float2*, int)>:
+0000000000003220 <identityMat(float2*, int)>:
 identityMat(float2*, int):
 	lea    (%rsi,%rsi,1),%ecx
 	mov    %esi,%eax
 	mov    $0x1,%esi
-	movss  0x1b02(%rip),%xmm0        
+	movss  0x1b42(%rip),%xmm0        
 	mov    %esi,%edx
 	shl    %cl,%edx
 	lea    0x1(%rax),%ecx
 	shl    %cl,%esi
 	lea    -0x1(%rdx),%r8d
 	xor    %ecx,%ecx
 	test   %edx,%edx
-	jg     3219 <identityMat(float2*, int)+0x49>
-	jmp    323a <identityMat(float2*, int)+0x6a>
+	jg     3269 <identityMat(float2*, int)+0x49>
+	jmp    328a <identityMat(float2*, int)+0x6a>
 	nopw   0x0(%rax,%rax,1)
 	movl   $0x0,0x4(%rdi,%rcx,8)
 	lea    0x1(%rcx),%rax
 	movss  %xmm0,(%rdi,%rcx,8)
 	cmp    %r8,%rcx
-	je     323a <identityMat(float2*, int)+0x6a>
+	je     328a <identityMat(float2*, int)+0x6a>
 	mov    %rax,%rcx
 	mov    %ecx,%eax
 	cltd
 	idiv   %esi
 	test   %edx,%edx
-	je     3200 <identityMat(float2*, int)+0x30>
+	je     3250 <identityMat(float2*, int)+0x30>
 	movl   $0x0,(%rdi,%rcx,8)
 	lea    0x1(%rcx),%rax
 	movl   $0x0,0x4(%rdi,%rcx,8)
 	cmp    %r8,%rcx
-	jne    3216 <identityMat(float2*, int)+0x46>
+	jne    3266 <identityMat(float2*, int)+0x46>
 	ret
 	nopl   0x0(%rax,%rax,1)
 
-0000000000003240 <generate_binary_data(float)>:
+0000000000003290 <generate_binary_data(float)>:
 generate_binary_data(float):
 	sub    $0x18,%rsp
 	xor    %edi,%edi
 	movss  %xmm0,0xc(%rsp)
-	call   1d20 <time@plt>
+	call   1d70 <time@plt>
 	mov    %rax,%rdi
-	call   1d30 <srand@plt>
-	call   1bd0 <rand@plt>
+	call   1d80 <srand@plt>
+	call   1c20 <rand@plt>
 	pxor   %xmm1,%xmm1
 	movss  0xc(%rsp),%xmm0
 	cvtsi2ss %eax,%xmm1
-	mulss  0x1a74(%rip),%xmm1        
+	mulss  0x1ab4(%rip),%xmm1        
 	xor    %eax,%eax
 	comiss %xmm1,%xmm0
 	seta   %al
 	add    $0x18,%rsp
 	ret
 	nopl   0x0(%rax,%rax,1)
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000003290 <getprob(float2*, float*, unsigned long)>:
+00000000000032e0 <getprob(float2*, float*, unsigned long)>:
 getprob(float2*, float*, unsigned long):
 	test   %rdx,%rdx
-	je     33ad <getprob(float2*, float*, unsigned long)+0x11d>
+	je     33fd <getprob(float2*, float*, unsigned long)+0x11d>
 	lea    (%rsi,%rdx,4),%rax
 	cmp    %rax,%rdi
 	lea    (%rdi,%rdx,8),%rax
 	setae  %cl
 	cmp    %rax,%rsi
 	setae  %al
 	or     %al,%cl
-	je     3380 <getprob(float2*, float*, unsigned long)+0xf0>
+	je     33d0 <getprob(float2*, float*, unsigned long)+0xf0>
 	lea    -0x1(%rdx),%rax
 	cmp    $0x2,%rax
-	jbe    3380 <getprob(float2*, float*, unsigned long)+0xf0>
+	jbe    33d0 <getprob(float2*, float*, unsigned long)+0xf0>
 	mov    %rdx,%rcx
 	xor    %eax,%eax
 	shr    $0x2,%rcx
 	shl    $0x4,%rcx
 	movups (%rdi,%rax,2),%xmm0
 	movups 0x10(%rdi,%rax,2),%xmm2
 	movaps %xmm0,%xmm1
@@ -1149,41 +1149,41 @@
 	shufps $0x88,%xmm2,%xmm1
 	mulps  %xmm0,%xmm0
 	mulps  %xmm1,%xmm1
 	addps  %xmm1,%xmm0
 	movups %xmm0,(%rsi,%rax,1)
 	add    $0x10,%rax
 	cmp    %rcx,%rax
-	jne    32d0 <getprob(float2*, float*, unsigned long)+0x40>
+	jne    3320 <getprob(float2*, float*, unsigned long)+0x40>
 	mov    %rdx,%rax
 	and    $0xfffffffffffffffc,%rax
 	test   $0x3,%dl
-	je     33ad <getprob(float2*, float*, unsigned long)+0x11d>
+	je     33fd <getprob(float2*, float*, unsigned long)+0x11d>
 	lea    (%rdi,%rax,8),%rcx
 	movss  (%rcx),%xmm0
 	movss  0x4(%rcx),%xmm1
 	lea    0x1(%rax),%ecx
 	movslq %ecx,%rcx
 	mulss  %xmm0,%xmm0
 	mulss  %xmm1,%xmm1
 	addss  %xmm1,%xmm0
 	movss  %xmm0,(%rsi,%rax,4)
 	cmp    %rcx,%rdx
-	jbe    33ad <getprob(float2*, float*, unsigned long)+0x11d>
+	jbe    33fd <getprob(float2*, float*, unsigned long)+0x11d>
 	lea    (%rdi,%rcx,8),%r8
 	add    $0x2,%eax
 	movss  (%r8),%xmm0
 	movss  0x4(%r8),%xmm1
 	cltq
 	mulss  %xmm0,%xmm0
 	mulss  %xmm1,%xmm1
 	addss  %xmm1,%xmm0
 	movss  %xmm0,(%rsi,%rcx,4)
 	cmp    %rax,%rdx
-	jbe    33ad <getprob(float2*, float*, unsigned long)+0x11d>
+	jbe    33fd <getprob(float2*, float*, unsigned long)+0x11d>
 	lea    (%rdi,%rax,8),%rdx
 	movss  (%rdx),%xmm0
 	movss  0x4(%rdx),%xmm1
 	mulss  %xmm0,%xmm0
 	mulss  %xmm1,%xmm1
 	addss  %xmm1,%xmm0
 	movss  %xmm0,(%rsi,%rax,4)
@@ -1195,57 +1195,57 @@
 	movss  0x4(%rdi,%rax,8),%xmm0
 	mulss  %xmm1,%xmm1
 	mulss  %xmm0,%xmm0
 	addss  %xmm1,%xmm0
 	movss  %xmm0,(%rsi,%rax,4)
 	add    $0x1,%rax
 	cmp    %rax,%rdx
-	jne    3388 <getprob(float2*, float*, unsigned long)+0xf8>
+	jne    33d8 <getprob(float2*, float*, unsigned long)+0xf8>
 	ret
 	xchg   %ax,%ax
 
-00000000000033b0 <hash(char const*)>:
+0000000000003400 <hash(char const*)>:
 hash(char const*):
 	movsbl (%rdi),%eax
 	lea    0x1(%rdi),%rdx
 	mov    $0x1,%r8d
 	test   %al,%al
-	je     33db <hash(char const*)+0x2b>
+	je     342b <hash(char const*)+0x2b>
 	nopl   0x0(%rax)
 	lea    (%rax,%r8,2),%eax
 	add    $0x1,%rdx
 	add    %eax,%r8d
 	movsbl -0x1(%rdx),%eax
 	test   %al,%al
-	jne    33c8 <hash(char const*)+0x18>
+	jne    3418 <hash(char const*)+0x18>
 	mov    %r8d,%eax
 	ret
 	nop
 
-00000000000033e0 <isInArray(char const**, char*, int)>:
+0000000000003430 <isInArray(char const**, char*, int)>:
 isInArray(char const**, char*, int):
 	test   %edx,%edx
-	jle    342f <isInArray(char const**, char*, int)+0x4f>
+	jle    347f <isInArray(char const**, char*, int)+0x4f>
 	lea    -0x1(%rdx),%eax
 	push   %r12
 	lea    0x8(%rdi,%rax,8),%r12
 	push   %rbp
 	mov    %rsi,%rbp
 	push   %rbx
 	mov    %rdi,%rbx
-	jmp    3409 <isInArray(char const**, char*, int)+0x29>
+	jmp    3459 <isInArray(char const**, char*, int)+0x29>
 	nopl   0x0(%rax,%rax,1)
 	add    $0x8,%rbx
 	cmp    %r12,%rbx
-	je     3428 <isInArray(char const**, char*, int)+0x48>
+	je     3478 <isInArray(char const**, char*, int)+0x48>
 	mov    (%rbx),%rdi
 	mov    %rbp,%rsi
-	call   1e30 <strcmp@plt>
+	call   1e80 <strcmp@plt>
 	test   %eax,%eax
-	jne    3400 <isInArray(char const**, char*, int)+0x20>
+	jne    3450 <isInArray(char const**, char*, int)+0x20>
 	pop    %rbx
 	mov    $0x1,%eax
 	pop    %rbp
 	pop    %r12
 	ret
 	nopw   0x0(%rax,%rax,1)
 	pop    %rbx
@@ -1254,40 +1254,40 @@
 	pop    %r12
 	ret
 	xor    %eax,%eax
 	ret
 	nopl   0x0(%rax)
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000003440 <getArrayLength(int*)>:
+0000000000003490 <getArrayLength(int*)>:
 getArrayLength(int*):
 	xor    %eax,%eax
 	cmpl   $0xffffffff,(%rdi)
-	je     3460 <getArrayLength(int*)+0x20>
+	je     34b0 <getArrayLength(int*)+0x20>
 	nopw   0x0(%rax,%rax,1)
 	add    $0x4,%rdi
 	add    $0x1,%eax
 	cmpl   $0xffffffff,(%rdi)
-	jne    3450 <getArrayLength(int*)+0x10>
+	jne    34a0 <getArrayLength(int*)+0x10>
 	ret
 	nopl   (%rax)
 	ret
 	nopl   0x0(%rax,%rax,1)
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000003470 <normalization(float2*, int)>:
+00000000000034c0 <normalization(float2*, int)>:
 normalization(float2*, int):
 	mov    %esi,%ecx
 	mov    $0x1,%esi
 	shl    %cl,%esi
 	test   %esi,%esi
-	jle    35e0 <normalization(float2*, int)+0x170>
+	jle    3630 <normalization(float2*, int)+0x170>
 	lea    -0x1(%rsi),%r8d
 	cmp    $0x2,%r8d
-	jbe    3663 <normalization(float2*, int)+0x1f3>
+	jbe    36b3 <normalization(float2*, int)+0x1f3>
 	mov    %esi,%edx
 	mov    %rdi,%rax
 	pxor   %xmm3,%xmm3
 	shr    $0x2,%edx
 	shl    $0x5,%rdx
 	add    %rdi,%rdx
 	nopw   0x0(%rax,%rax,1)
@@ -1308,266 +1308,266 @@
 	movaps %xmm0,%xmm2
 	unpckhps %xmm0,%xmm2
 	shufps $0xff,%xmm0,%xmm0
 	addss  %xmm2,%xmm1
 	movaps %xmm1,%xmm3
 	addss  %xmm0,%xmm3
 	cmp    %rdx,%rax
-	jne    34a8 <normalization(float2*, int)+0x38>
+	jne    34f8 <normalization(float2*, int)+0x38>
 	mov    %esi,%eax
 	and    $0xfffffffc,%eax
 	test   $0x3,%sil
-	je     356f <normalization(float2*, int)+0xff>
+	je     35bf <normalization(float2*, int)+0xff>
 	movslq %eax,%rdx
 	lea    (%rdi,%rdx,8),%rdx
 	movss  (%rdx),%xmm0
 	movss  0x4(%rdx),%xmm1
 	lea    0x1(%rax),%edx
 	mulss  %xmm0,%xmm0
 	mulss  %xmm1,%xmm1
 	addss  %xmm1,%xmm0
 	addss  %xmm0,%xmm3
 	cmp    %esi,%edx
-	jge    3640 <normalization(float2*, int)+0x1d0>
+	jge    3690 <normalization(float2*, int)+0x1d0>
 	movslq %edx,%rdx
 	add    $0x2,%eax
 	lea    (%rdi,%rdx,8),%rdx
 	movss  (%rdx),%xmm1
 	movss  0x4(%rdx),%xmm0
 	mulss  %xmm1,%xmm1
 	mulss  %xmm0,%xmm0
 	addss  %xmm1,%xmm0
 	addss  %xmm0,%xmm3
 	cmp    %eax,%esi
-	jle    356f <normalization(float2*, int)+0xff>
+	jle    35bf <normalization(float2*, int)+0xff>
 	cltq
 	lea    (%rdi,%rax,8),%rax
 	movss  (%rax),%xmm0
 	movss  0x4(%rax),%xmm1
 	mulss  %xmm0,%xmm0
 	mulss  %xmm1,%xmm1
 	addss  %xmm1,%xmm0
 	addss  %xmm0,%xmm3
-	movsd  0x1779(%rip),%xmm1        
+	movsd  0x17b9(%rip),%xmm1        
 	pxor   %xmm0,%xmm0
 	cvtss2sd %xmm3,%xmm0
 	comisd %xmm0,%xmm1
-	ja     35e8 <normalization(float2*, int)+0x178>
+	ja     3638 <normalization(float2*, int)+0x178>
 	mov    %esi,%edx
 	movaps %xmm3,%xmm1
 	mov    %rdi,%rax
 	shr    $1,%edx
 	shufps $0x0,%xmm1,%xmm1
 	shl    $0x4,%rdx
 	add    %rdi,%rdx
 	nopw   0x0(%rax,%rax,1)
 	movups (%rax),%xmm0
 	add    $0x10,%rax
 	divps  %xmm1,%xmm0
 	movups %xmm0,-0x10(%rax)
 	cmp    %rdx,%rax
-	jne    35a0 <normalization(float2*, int)+0x130>
+	jne    35f0 <normalization(float2*, int)+0x130>
 	mov    %esi,%ecx
 	and    $0xfffffffe,%ecx
 	and    $0x1,%esi
-	je     35e0 <normalization(float2*, int)+0x170>
+	je     3630 <normalization(float2*, int)+0x170>
 	movslq %ecx,%rcx
 	lea    (%rdi,%rcx,8),%rax
 	movss  (%rax),%xmm0
 	divss  %xmm3,%xmm0
 	movss  %xmm0,(%rax)
 	movss  0x4(%rax),%xmm0
 	divss  %xmm3,%xmm0
 	movss  %xmm0,0x4(%rax)
 	ret
 	nop
 	ret
 	nopl   0x0(%rax)
-	movss  0x16f4(%rip),%xmm0        
+	movss  0x1734(%rip),%xmm0        
 	mov    %r8d,%ecx
 	xor    %eax,%eax
-	jmp    3613 <normalization(float2*, int)+0x1a3>
+	jmp    3663 <normalization(float2*, int)+0x1a3>
 	nopw   0x0(%rax,%rax,1)
 	movl   $0x0,(%rdi,%rax,8)
 	lea    0x1(%rax),%rdx
 	cmp    %rcx,%rax
-	je     3625 <normalization(float2*, int)+0x1b5>
+	je     3675 <normalization(float2*, int)+0x1b5>
 	mov    %rdx,%rax
 	test   %rax,%rax
-	jne    3600 <normalization(float2*, int)+0x190>
+	jne    3650 <normalization(float2*, int)+0x190>
 	movss  %xmm0,(%rdi)
 	lea    0x1(%rax),%rdx
 	cmp    %rcx,%rax
-	jne    3610 <normalization(float2*, int)+0x1a0>
+	jne    3660 <normalization(float2*, int)+0x1a0>
 	lea    0x4(%rdi),%rdx
 	lea    0xc(%rdi,%rax,8),%rax
 	xchg   %ax,%ax
 	movl   $0x0,(%rdx)
 	add    $0x8,%rdx
 	cmp    %rax,%rdx
-	jne    3630 <normalization(float2*, int)+0x1c0>
+	jne    3680 <normalization(float2*, int)+0x1c0>
 	ret
-	movsd  0x16a8(%rip),%xmm1        
+	movsd  0x16e8(%rip),%xmm1        
 	pxor   %xmm0,%xmm0
 	cvtss2sd %xmm3,%xmm0
 	comisd %xmm0,%xmm1
-	ja     35e8 <normalization(float2*, int)+0x178>
+	ja     3638 <normalization(float2*, int)+0x178>
 	test   %ecx,%ecx
-	je     35bd <normalization(float2*, int)+0x14d>
-	jmp    3585 <normalization(float2*, int)+0x115>
+	je     360d <normalization(float2*, int)+0x14d>
+	jmp    35d5 <normalization(float2*, int)+0x115>
 	xor    %eax,%eax
 	pxor   %xmm3,%xmm3
-	jmp    34fe <normalization(float2*, int)+0x8e>
+	jmp    354e <normalization(float2*, int)+0x8e>
 	xchg   %ax,%ax
 
-0000000000003670 <execute_circuit>:
+00000000000036c0 <execute_circuit>:
 execute_circuit():
 	push   %r15
-	lea    0x1399(%rip),%rax        
+	lea    0x13b9(%rip),%rax        
 	mov    %rsi,%r9
-	lea    0x13c9(%rip),%rsi        
+	lea    0x13df(%rip),%rsi        
 	push   %r14
 	movq   %rax,%xmm1
 	movq   %rsi,%xmm0
-	lea    0x136a(%rip),%rax        
+	lea    0x138a(%rip),%rax        
 	push   %r13
 	punpcklqdq %xmm1,%xmm0
 	movq   %rax,%xmm2
-	lea    0x135a(%rip),%rsi        
+	lea    0x137a(%rip),%rsi        
 	push   %r12
-	lea    0x1355(%rip),%rax        
+	lea    0x1375(%rip),%rax        
 	mov    %ecx,%r12d
-	lea    0x1359(%rip),%rcx        
+	lea    0x1379(%rip),%rcx        
 	push   %rbp
 	mov    %rdi,%rbp
-	lea    0x1368(%rip),%rdi        
+	lea    0x1388(%rip),%rdi        
 	movq   %rax,%xmm3
 	push   %rbx
-	lea    0x1339(%rip),%rax        
+	lea    0x1359(%rip),%rax        
 	movq   %rax,%xmm4
-	lea    0x1332(%rip),%rax        
+	lea    0x1352(%rip),%rax        
 	movq   %rax,%xmm5
-	lea    0x132c(%rip),%rax        
+	lea    0x134c(%rip),%rax        
 	sub    $0xe8,%rsp
 	movq   %rax,%xmm6
-	lea    0x1323(%rip),%rax        
+	lea    0x1343(%rip),%rax        
 	movaps %xmm0,0x70(%rsp)
 	movq   %rdi,%xmm0
 	movq   %rax,%xmm7
-	lea    0x12f4(%rip),%rdi        
+	lea    0x1314(%rip),%rdi        
 	punpcklqdq %xmm2,%xmm0
-	lea    0x1305(%rip),%rax        
+	lea    0x1325(%rip),%rax        
 	movaps %xmm0,0x80(%rsp)
 	movq   %rsi,%xmm0
-	lea    0x12db(%rip),%rsi        
+	lea    0x12fb(%rip),%rsi        
 	movq   %rax,%xmm1
 	punpcklqdq %xmm3,%xmm0
-	lea    0x1308(%rip),%rax        
+	lea    0x131e(%rip),%rax        
 	movaps %xmm0,0x90(%rsp)
 	movq   %rdi,%xmm0
-	lea    0x12c7(%rip),%rdi        
+	lea    0x12e7(%rip),%rdi        
 	movq   %rax,%xmm2
 	punpcklqdq %xmm4,%xmm0
-	lea    0x12c9(%rip),%rax        
+	lea    0x12e9(%rip),%rax        
 	movaps %xmm0,0xa0(%rsp)
 	movq   %rsi,%xmm0
-	lea    0x12ca(%rip),%rsi        
+	lea    0x12ea(%rip),%rsi        
 	movq   %rax,%xmm3
 	punpcklqdq %xmm5,%xmm0
-	lea    0x12ad(%rip),%rax        
+	lea    0x12cd(%rip),%rax        
 	movaps %xmm0,0xb0(%rsp)
 	movq   %rcx,%xmm0
-	lea    0x128b(%rip),%rcx        
+	lea    0x12ab(%rip),%rcx        
 	movq   %rax,%xmm4
 	punpcklqdq %xmm6,%xmm0
-	lea    0x128d(%rip),%rax        
+	lea    0x12ad(%rip),%rax        
 	movaps %xmm0,0xc0(%rsp)
 	movq   %rdi,%xmm0
-	lea    0x126a(%rip),%rdi        
+	lea    0x128a(%rip),%rdi        
 	punpcklqdq %xmm7,%xmm0
 	mov    %rax,0x60(%rsp)
-	lea    0x1271(%rip),%rax        
+	lea    0x1291(%rip),%rax        
 	movaps %xmm0,0xd0(%rsp)
 	movq   %rsi,%xmm0
-	lea    0x124d(%rip),%rsi        
+	lea    0x126d(%rip),%rsi        
 	movq   %rax,%xmm5
 	punpcklqdq %xmm1,%xmm0
 	movaps %xmm0,0x20(%rsp)
 	movq   %rcx,%xmm0
-	lea    0x123f(%rip),%rcx        
+	lea    0x125f(%rip),%rcx        
 	punpcklqdq %xmm2,%xmm0
 	movaps %xmm0,0x30(%rsp)
 	movq   %rdi,%xmm0
 	punpcklqdq %xmm3,%xmm0
 	movaps %xmm0,0x40(%rsp)
 	movq   %rsi,%xmm0
 	punpcklqdq %xmm4,%xmm0
 	movaps %xmm0,0x50(%rsp)
 	movq   %rcx,%xmm0
 	punpcklqdq %xmm5,%xmm0
 	movaps %xmm0,0x10(%rsp)
 	test   %edx,%edx
-	jle    38c8 <execute_circuit+0x258>
+	jle    3918 <execute_circuit+0x258>
 	lea    -0x1(%rdx),%eax
 	mov    %r8d,%r13d
 	lea    0x70(%rsp),%r14
 	mov    %r9,%r15
 	lea    (%rax,%rax,2),%rax
 	lea    0x18(%r9,%rax,8),%rax
 	mov    %rax,(%rsp)
 	lea    0x20(%rsp),%rax
 	mov    %rax,0x8(%rsp)
-	jmp    3891 <execute_circuit+0x221>
+	jmp    38e1 <execute_circuit+0x221>
 	nopl   0x0(%rax,%rax,1)
-	mov    0x208761(%rip),%rbx        
+	mov    0x208711(%rip),%rbx        
 	movss  0x10(%r15),%xmm0
 	mov    0x8(%r15),%rcx
 	mov    %r13d,%r8d
 	mov    %r12d,%edx
 	mov    (%r15),%rdi
 	mov    %rbp,%rsi
 	add    $0x18,%r15
 	call   *%rbx
 	cmp    %r15,(%rsp)
-	je     38c8 <execute_circuit+0x258>
+	je     3918 <execute_circuit+0x258>
 	mov    (%r15),%rsi
 	mov    $0xe,%edx
 	mov    %r14,%rdi
-	call   1ca0 <isInArray(char const**, char*, int)@plt>
+	call   1cf0 <isInArray(char const**, char*, int)@plt>
 	test   %al,%al
-	jne    3868 <execute_circuit+0x1f8>
+	jne    38b8 <execute_circuit+0x1f8>
 	mov    (%r15),%rsi
 	mov    0x8(%rsp),%rdi
 	mov    $0x9,%edx
-	call   1ca0 <isInArray(char const**, char*, int)@plt>
+	call   1cf0 <isInArray(char const**, char*, int)@plt>
 	test   %al,%al
-	je     38e0 <execute_circuit+0x270>
-	mov    0x2086f6(%rip),%rbx        
-	jmp    386f <execute_circuit+0x1ff>
+	je     3930 <execute_circuit+0x270>
+	mov    0x2086a6(%rip),%rbx        
+	jmp    38bf <execute_circuit+0x1ff>
 	nopl   0x0(%rax)
 	add    $0xe8,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	nopw   0x0(%rax,%rax,1)
 	mov    (%r15),%rsi
 	lea    0x10(%rsp),%rdi
 	mov    $0x2,%edx
-	call   1ca0 <isInArray(char const**, char*, int)@plt>
+	call   1cf0 <isInArray(char const**, char*, int)@plt>
 	test   %al,%al
-	je     386f <execute_circuit+0x1ff>
-	mov    0x2086e7(%rip),%rbx        
-	jmp    386f <execute_circuit+0x1ff>
+	je     38bf <execute_circuit+0x1ff>
+	mov    0x208697(%rip),%rbx        
+	jmp    38bf <execute_circuit+0x1ff>
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000003910 <__device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)>:
+0000000000003960 <__device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)>:
 __device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*):
 	sub    $0x88,%rsp
 	lea    0x18(%rsp),%rax
 	mov    %rdi,0x18(%rsp)
 	lea    0x30(%rsp),%rdi
 	movq   %rax,%xmm0
 	lea    0x10(%rsp),%rax
@@ -1587,140 +1587,140 @@
 	movl   $0x1,0x38(%rsp)
 	movabs $0x100000001,%rax
 	punpcklqdq %xmm2,%xmm0
 	mov    %rax,0x30(%rsp)
 	mov    %rax,0x3c(%rsp)
 	movl   $0x1,0x44(%rsp)
 	movaps %xmm0,0x70(%rsp)
-	call   1ea0 <__cudaPopCallConfiguration@plt>
+	call   1ef0 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
-	jne    39d1 <__device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xc1>
+	jne    3a21 <__device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xc1>
 	push   0x28(%rsp)
-	mov    0x20862a(%rip),%rdi        
+	mov    0x2085da(%rip),%rdi        
 	push   0x28(%rsp)
 	mov    0x4c(%rsp),%rcx
 	mov    0x54(%rsp),%r8d
 	mov    0x40(%rsp),%rsi
 	mov    0x48(%rsp),%edx
 	lea    0x70(%rsp),%r9
-	call   1bb0 <cudaLaunchKernel@plt>
+	call   1c00 <cudaLaunchKernel@plt>
 	pop    %rax
 	pop    %rdx
 	add    $0x88,%rsp
 	ret
 	nopl   0x0(%rax)
 
-00000000000039e0 <actionOnSingleQubit(float2*, float2*, unsigned long, unsigned long*)>:
+0000000000003a30 <actionOnSingleQubit(float2*, float2*, unsigned long, unsigned long*)>:
 actionOnSingleQubit(float2*, float2*, unsigned long, unsigned long*):
-	jmp    1e00 <__device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>
+	jmp    1e50 <__device_stub__Z19actionOnSingleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>
 	nop
 	cs nopw 0x0(%rax,%rax,1)
 
-00000000000039f0 <singleGateAction>:
+0000000000003a40 <singleGateAction>:
 singleGateAction():
 	push   %r15
-	lea    0x1019(%rip),%rax        
+	lea    0x1039(%rip),%rax        
 	push   %r14
 	movq   %rax,%xmm1
-	lea    0xff9(%rip),%rax        
+	lea    0x1019(%rip),%rax        
 	mov    %rdi,%r14
 	push   %r13
 	movq   %rax,%xmm2
 	mov    %rsi,%r13
 	mov    %rcx,%rdi
 	push   %r12
-	lea    0xfe6(%rip),%rax        
-	lea    0xff7(%rip),%rsi        
+	lea    0x1006(%rip),%rax        
+	lea    0x1017(%rip),%rsi        
 	push   %rbp
 	movq   %rax,%xmm3
-	lea    0xfd8(%rip),%rax        
+	lea    0xff8(%rip),%rax        
 	mov    %r8d,%ebp
 	push   %rbx
-	lea    0x100d(%rip),%rbx        
+	lea    0x1023(%rip),%rbx        
 	movq   %rax,%xmm4
-	lea    0xfc6(%rip),%rax        
+	lea    0xfe6(%rip),%rax        
 	movq   %rax,%xmm5
-	lea    0xfc0(%rip),%rax        
+	lea    0xfe0(%rip),%rax        
 	movq   %rax,%xmm6
-	lea    0xfbe(%rip),%rax        
+	lea    0xfde(%rip),%rax        
 	sub    $0xc8,%rsp
 	movq   %rax,%xmm7
 	movss  %xmm0,0x1c(%rsp)
 	movq   %rbx,%xmm0
-	lea    0xfad(%rip),%rbx        
+	lea    0xfcd(%rip),%rbx        
 	punpcklqdq %xmm1,%xmm0
 	mov    %edx,0x4(%rsp)
-	lea    0xf7e(%rip),%rdx        
+	lea    0xf9e(%rip),%rdx        
 	movaps %xmm0,0x50(%rsp)
 	movq   %rbx,%xmm0
-	lea    0xf61(%rip),%rbx        
+	lea    0xf81(%rip),%rbx        
 	punpcklqdq %xmm2,%xmm0
 	mov    %rcx,0x10(%rsp)
 	movaps %xmm0,0x60(%rsp)
 	movq   %rbx,%xmm0
-	lea    0xf4d(%rip),%rbx        
+	lea    0xf6d(%rip),%rbx        
 	punpcklqdq %xmm3,%xmm0
 	movaps %xmm0,0x70(%rsp)
 	movq   %rbx,%xmm0
-	lea    0xf44(%rip),%rbx        
+	lea    0xf64(%rip),%rbx        
 	punpcklqdq %xmm4,%xmm0
 	movaps %xmm0,0x80(%rsp)
 	movq   %rdx,%xmm0
 	punpcklqdq %xmm5,%xmm0
 	movaps %xmm0,0x90(%rsp)
 	movq   %rbx,%xmm0
 	punpcklqdq %xmm6,%xmm0
 	movaps %xmm0,0xa0(%rsp)
 	movq   %rsi,%xmm0
 	punpcklqdq %xmm7,%xmm0
 	movaps %xmm0,0xb0(%rsp)
-	call   1e10 <getArrayLength(int*)@plt>
+	call   1e60 <getArrayLength(int*)@plt>
 	cmp    $0x1,%eax
-	jne    3f0b <singleGateAction+0x51b>
+	jne    3f5b <singleGateAction+0x51b>
 	mov    %ebp,%edi
 	mov    %eax,%ebx
-	call   1f40 <cudaSetDevice@plt>
+	call   1f90 <cudaSetDevice@plt>
 	mov    $0x20,%edi
-	call   1df0 <malloc@plt>
+	call   1e40 <malloc@plt>
 	mov    $0x8,%edi
 	mov    %rax,%r12
-	call   1df0 <malloc@plt>
+	call   1e40 <malloc@plt>
 	movzbl 0x4(%rsp),%ecx
 	lea    0x20(%rsp),%rdi
 	mov    $0x20,%esi
 	movq   $0x0,0x20(%rsp)
 	mov    %rax,%rbp
 	mov    %ebx,%eax
 	movq   $0x0,0x28(%rsp)
 	shl    %cl,%eax
 	movq   $0x0,0x30(%rsp)
 	cltq
 	lea    0x0(,%rax,8),%r15
 	mov    %rax,0x8(%rsp)
-	call   1b60 <cudaMalloc@plt>
+	call   1bb0 <cudaMalloc@plt>
 	lea    0x28(%rsp),%rdi
 	mov    %r15,%rsi
-	call   1b60 <cudaMalloc@plt>
+	call   1bb0 <cudaMalloc@plt>
 	lea    0x30(%rsp),%rdi
 	mov    $0x8,%esi
-	call   1b60 <cudaMalloc@plt>
+	call   1bb0 <cudaMalloc@plt>
 	mov    0x28(%rsp),%rdi
 	mov    %r15,%rdx
 	mov    %r13,%rsi
 	mov    $0x1,%ecx
-	call   1da0 <cudaMemcpy@plt>
+	call   1df0 <cudaMemcpy@plt>
 	mov    %r14,%rdi
-	call   1b70 <hash(char const*)@plt>
+	call   1bc0 <hash(char const*)@plt>
 	lea    0x50(%rsp),%rdi
 	mov    $0xe,%edx
 	mov    %r14,%rsi
 	mov    %eax,0x18(%rsp)
-	call   1ca0 <isInArray(char const**, char*, int)@plt>
+	call   1cf0 <isInArray(char const**, char*, int)@plt>
 	test   %al,%al
-	je     3f15 <singleGateAction+0x525>
+	je     3f65 <singleGateAction+0x525>
 	mov    0x10(%rsp),%rsi
 	mov    0x8(%rsp),%rdx
 	mov    0x30(%rsp),%rdi
 	mov    (%rsi),%ecx
 	mov    %ebx,%esi
 	shl    %cl,%esi
 	add    $0x1,%ecx
@@ -1737,191 +1737,191 @@
 	mov    %rcx,0x48(%rsp)
 	mov    $0x1,%ecx
 	div    %rsi
 	mov    $0x8,%edx
 	mov    %rbp,%rsi
 	add    $0x1,%eax
 	mov    %eax,0x44(%rsp)
-	call   1da0 <cudaMemcpy@plt>
+	call   1df0 <cudaMemcpy@plt>
 	mov    0x18(%rsp),%r8d
 	cmp    $0x1bd,%r8d
-	je     3ef8 <singleGateAction+0x508>
-	ja     3dd0 <singleGateAction+0x3e0>
+	je     3f48 <singleGateAction+0x508>
+	ja     3e20 <singleGateAction+0x3e0>
 	cmp    $0x7d,%r8d
-	ja     3d48 <singleGateAction+0x358>
+	ja     3d98 <singleGateAction+0x358>
 	cmp    $0x6a,%r8d
-	jbe    3ca8 <singleGateAction+0x2b8>
+	jbe    3cf8 <singleGateAction+0x2b8>
 	sub    $0x6b,%r8d
 	cmp    $0x12,%r8d
-	ja     3ca8 <singleGateAction+0x2b8>
-	lea    0xde0(%rip),%rdx        
+	ja     3cf8 <singleGateAction+0x2b8>
+	lea    0xe10(%rip),%rdx        
 	movslq (%rdx,%r8,4),%rax
 	add    %rdx,%rax
 	jmp    *%rax
 	nopl   0x0(%rax)
 	cmp    $0x1d8,%r8d
-	je     3ee0 <singleGateAction+0x4f0>
+	je     3f30 <singleGateAction+0x4f0>
 	cmp    $0x1d9,%r8d
-	jne    3e10 <singleGateAction+0x420>
+	jne    3e60 <singleGateAction+0x420>
 	movss  0x1c(%rsp),%xmm0
 	mov    %r12,%rdi
-	call   1ec0 <rz_gate(float2*, float)@plt>
+	call   1f10 <rz_gate(float2*, float)@plt>
 	mov    0x20(%rsp),%rdi
 	mov    $0x1,%ecx
 	mov    $0x20,%edx
 	mov    %r12,%rsi
-	call   1da0 <cudaMemcpy@plt>
+	call   1df0 <cudaMemcpy@plt>
 	mov    %ebx,0x38(%rsp)
 	mov    0x40(%rsp),%ecx
 	xor    %r9d,%r9d
 	mov    0x38(%rsp),%rdx
 	mov    0x44(%rsp),%rdi
 	xor    %r8d,%r8d
 	mov    0x4c(%rsp),%esi
-	call   1ed0 <__cudaPushCallConfiguration@plt>
+	call   1f20 <__cudaPushCallConfiguration@plt>
 	test   %eax,%eax
-	je     3e30 <singleGateAction+0x440>
-	call   1eb0 <cudaDeviceSynchronize@plt>
+	je     3e80 <singleGateAction+0x440>
+	call   1f00 <cudaDeviceSynchronize@plt>
 	mov    0x28(%rsp),%rsi
 	mov    %r15,%rdx
 	mov    %r13,%rdi
 	mov    $0x2,%ecx
-	call   1da0 <cudaMemcpy@plt>
+	call   1df0 <cudaMemcpy@plt>
 	mov    0x20(%rsp),%rdi
-	call   1e50 <cudaFree@plt>
+	call   1ea0 <cudaFree@plt>
 	mov    0x28(%rsp),%rdi
-	call   1e50 <cudaFree@plt>
+	call   1ea0 <cudaFree@plt>
 	mov    0x30(%rsp),%rdi
-	call   1e50 <cudaFree@plt>
+	call   1ea0 <cudaFree@plt>
 	mov    %r12,%rdi
-	call   1d90 <free@plt>
+	call   1de0 <free@plt>
 	add    $0xc8,%rsp
 	mov    %rbp,%rdi
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
-	jmp    1d90 <free@plt>
+	jmp    1de0 <free@plt>
 	nopl   0x0(%rax)
 	cmp    $0x190,%r8d
-	jne    3ca8 <singleGateAction+0x2b8>
+	jne    3cf8 <singleGateAction+0x2b8>
 	movss  0x1c(%rsp),%xmm0
 	mov    %r12,%rdi
-	call   1b50 <ad_gate(float2*, float)@plt>
+	call   1b90 <ad_gate(float2*, float)@plt>
 	mov    0x20(%rsp),%rdi
 	mov    $0x1,%ecx
 	mov    $0x20,%edx
 	mov    %r12,%rsi
-	call   1da0 <cudaMemcpy@plt>
+	call   1df0 <cudaMemcpy@plt>
 	mov    %ebx,0x38(%rsp)
 	mov    0x40(%rsp),%ecx
 	xor    %r9d,%r9d
 	mov    0x38(%rsp),%rdx
 	mov    0x44(%rsp),%rdi
 	xor    %r8d,%r8d
 	mov    0x4c(%rsp),%esi
-	call   1ed0 <__cudaPushCallConfiguration@plt>
+	call   1f20 <__cudaPushCallConfiguration@plt>
 	test   %eax,%eax
-	je     3ea0 <singleGateAction+0x4b0>
-	call   1eb0 <cudaDeviceSynchronize@plt>
+	je     3ef0 <singleGateAction+0x4b0>
+	call   1f00 <cudaDeviceSynchronize@plt>
 	mov    0x28(%rsp),%rsi
 	mov    %r13,%rdi
 	mov    %r15,%rdx
 	mov    $0x2,%ecx
-	call   1da0 <cudaMemcpy@plt>
+	call   1df0 <cudaMemcpy@plt>
 	mov    0x4(%rsp),%esi
 	mov    %r13,%rdi
-	call   1d50 <normalization(float2*, int)@plt>
-	jmp    3d02 <singleGateAction+0x312>
+	call   1da0 <normalization(float2*, int)@plt>
+	jmp    3d52 <singleGateAction+0x312>
 	xchg   %ax,%ax
 	cmp    $0x5b9,%r8d
-	je     3ec0 <singleGateAction+0x4d0>
-	jbe    3c80 <singleGateAction+0x290>
+	je     3f10 <singleGateAction+0x4d0>
+	jbe    3cd0 <singleGateAction+0x290>
 	cmp    $0x5c2,%r8d
-	je     3ed0 <singleGateAction+0x4e0>
+	je     3f20 <singleGateAction+0x4e0>
 	cmp    $0x914b,%r8d
-	jne    3ca8 <singleGateAction+0x2b8>
+	jne    3cf8 <singleGateAction+0x2b8>
 	movss  0x1c(%rsp),%xmm0
 	mov    %r12,%rdi
-	call   1ce0 <damp_i_gate(float2*, float)@plt>
-	jmp    3d63 <singleGateAction+0x373>
+	call   1d30 <damp_i_gate(float2*, float)@plt>
+	jmp    3db3 <singleGateAction+0x373>
 	cmp    $0x1d7,%r8d
-	jne    3ca8 <singleGateAction+0x2b8>
+	jne    3cf8 <singleGateAction+0x2b8>
 	movss  0x1c(%rsp),%xmm0
 	mov    %r12,%rdi
-	call   1f20 <rx_gate(float2*, float)@plt>
-	jmp    3ca8 <singleGateAction+0x2b8>
+	call   1f70 <rx_gate(float2*, float)@plt>
+	jmp    3cf8 <singleGateAction+0x2b8>
 	mov    0x30(%rsp),%rcx
 	mov    0x8(%rsp),%rdx
 	mov    0x20(%rsp),%rsi
 	mov    0x28(%rsp),%rdi
-	call   1e90 <actionOnSingleQubit(float2*, float2*, unsigned long, unsigned long*)@plt>
-	jmp    3ce8 <singleGateAction+0x2f8>
+	call   1ee0 <actionOnSingleQubit(float2*, float2*, unsigned long, unsigned long*)@plt>
+	jmp    3d38 <singleGateAction+0x2f8>
 	mov    %r12,%rdi
-	call   1d60 <z_gate(float2*)@plt>
-	jmp    3ca8 <singleGateAction+0x2b8>
+	call   1db0 <z_gate(float2*)@plt>
+	jmp    3cf8 <singleGateAction+0x2b8>
 	mov    %r12,%rdi
-	call   1ee0 <h_gate(float2*)@plt>
-	jmp    3ca8 <singleGateAction+0x2b8>
+	call   1f30 <h_gate(float2*)@plt>
+	jmp    3cf8 <singleGateAction+0x2b8>
 	mov    %r12,%rdi
-	call   1cd0 <s_gate(float2*)@plt>
-	jmp    3ca8 <singleGateAction+0x2b8>
+	call   1d20 <s_gate(float2*)@plt>
+	jmp    3cf8 <singleGateAction+0x2b8>
 	mov    %r12,%rdi
-	call   1d40 <t_gate(float2*)@plt>
-	jmp    3ca8 <singleGateAction+0x2b8>
+	call   1d90 <t_gate(float2*)@plt>
+	jmp    3cf8 <singleGateAction+0x2b8>
 	mov    %r12,%rdi
-	call   1cc0 <x_gate(float2*)@plt>
-	jmp    3ca8 <singleGateAction+0x2b8>
+	call   1d10 <x_gate(float2*)@plt>
+	jmp    3cf8 <singleGateAction+0x2b8>
 	mov    %r12,%rdi
-	call   1ba0 <y_gate(float2*)@plt>
-	jmp    3ca8 <singleGateAction+0x2b8>
+	call   1bf0 <y_gate(float2*)@plt>
+	jmp    3cf8 <singleGateAction+0x2b8>
 	nopl   0x0(%rax)
 	mov    0x30(%rsp),%rcx
 	mov    0x8(%rsp),%rdx
 	mov    0x20(%rsp),%rsi
 	mov    0x28(%rsp),%rdi
-	call   1e90 <actionOnSingleQubit(float2*, float2*, unsigned long, unsigned long*)@plt>
-	jmp    3da3 <singleGateAction+0x3b3>
+	call   1ee0 <actionOnSingleQubit(float2*, float2*, unsigned long, unsigned long*)@plt>
+	jmp    3df3 <singleGateAction+0x3b3>
 	xchg   %ax,%ax
 	mov    %r12,%rdi
-	call   1e20 <sdg_gate(float2*)@plt>
-	jmp    3ca8 <singleGateAction+0x2b8>
+	call   1e70 <sdg_gate(float2*)@plt>
+	jmp    3cf8 <singleGateAction+0x2b8>
 	nopl   (%rax)
 	mov    %r12,%rdi
-	call   1dc0 <tdg_gate(float2*)@plt>
-	jmp    3ca8 <singleGateAction+0x2b8>
+	call   1e10 <tdg_gate(float2*)@plt>
+	jmp    3cf8 <singleGateAction+0x2b8>
 	nopl   (%rax)
 	movss  0x1c(%rsp),%xmm0
 	mov    %r12,%rdi
-	call   1c20 <ry_gate(float2*, float)@plt>
-	jmp    3ca8 <singleGateAction+0x2b8>
+	call   1c70 <ry_gate(float2*, float)@plt>
+	jmp    3cf8 <singleGateAction+0x2b8>
 	nopl   0x0(%rax,%rax,1)
 	movss  0x1c(%rsp),%xmm0
 	mov    %r12,%rdi
-	call   1b80 <pd_gate(float2*, float)@plt>
-	jmp    3d63 <singleGateAction+0x373>
+	call   1bd0 <pd_gate(float2*, float)@plt>
+	jmp    3db3 <singleGateAction+0x373>
 	mov    $0x1,%edi
-	call   1db0 <exit@plt>
+	call   1e00 <exit@plt>
 	mov    0x20(%rsp),%rdi
-	call   1e50 <cudaFree@plt>
+	call   1ea0 <cudaFree@plt>
 	mov    0x28(%rsp),%rdi
-	call   1e50 <cudaFree@plt>
+	call   1ea0 <cudaFree@plt>
 	mov    0x30(%rsp),%rdi
-	call   1e50 <cudaFree@plt>
+	call   1ea0 <cudaFree@plt>
 	mov    %r12,%rdi
-	call   1d90 <free@plt>
+	call   1de0 <free@plt>
 	mov    %rbp,%rdi
-	call   1d90 <free@plt>
+	call   1de0 <free@plt>
 	mov    $0x3,%edi
-	call   1db0 <exit@plt>
+	call   1e00 <exit@plt>
 	nopl   (%rax)
 
-0000000000003f50 <__device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)>:
+0000000000003fa0 <__device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)>:
 __device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*):
 	sub    $0x88,%rsp
 	lea    0x18(%rsp),%rax
 	mov    %rdi,0x18(%rsp)
 	lea    0x30(%rsp),%rdi
 	movq   %rax,%xmm0
 	lea    0x10(%rsp),%rax
@@ -1941,149 +1941,154 @@
 	movl   $0x1,0x38(%rsp)
 	movabs $0x100000001,%rax
 	punpcklqdq %xmm2,%xmm0
 	mov    %rax,0x30(%rsp)
 	mov    %rax,0x3c(%rsp)
 	movl   $0x1,0x44(%rsp)
 	movaps %xmm0,0x70(%rsp)
-	call   1ea0 <__cudaPopCallConfiguration@plt>
+	call   1ef0 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
-	jne    4011 <__device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xc1>
+	jne    4061 <__device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xc1>
 	push   0x28(%rsp)
-	mov    0x207fd2(%rip),%rdi        
+	mov    0x207f82(%rip),%rdi        
 	push   0x28(%rsp)
 	mov    0x4c(%rsp),%rcx
 	mov    0x54(%rsp),%r8d
 	mov    0x40(%rsp),%rsi
 	mov    0x48(%rsp),%edx
 	lea    0x70(%rsp),%r9
-	call   1bb0 <cudaLaunchKernel@plt>
+	call   1c00 <cudaLaunchKernel@plt>
 	pop    %rax
 	pop    %rdx
 	add    $0x88,%rsp
 	ret
 	nopl   0x0(%rax)
 
-0000000000004020 <actionOnDoubleQubit(float2*, float2*, unsigned long, unsigned long*)>:
+0000000000004070 <actionOnDoubleQubit(float2*, float2*, unsigned long, unsigned long*)>:
 actionOnDoubleQubit(float2*, float2*, unsigned long, unsigned long*):
-	jmp    1d80 <__device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>
+	jmp    1dd0 <__device_stub__Z19actionOnDoubleQubitP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>
 	nop
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000004030 <doubleGateAction>:
+0000000000004080 <doubleGateAction>:
 doubleGateAction():
 	push   %r15
-	lea    0x9eb(%rip),%rax        
+	lea    0xa0b(%rip),%rax        
 	push   %r14
 	movq   %rax,%xmm1
-	lea    0xa04(%rip),%rax        
+	lea    0xa1a(%rip),%rax        
 	mov    %rdi,%r14
 	push   %r13
 	mov    %edx,%r13d
-	lea    0x9ef(%rip),%rdx        
+	lea    0xa0f(%rip),%rdx        
 	mov    %rcx,%rdi
 	push   %r12
 	movq   %rax,%xmm2
-	lea    0x9c9(%rip),%rax        
+	lea    0x9e9(%rip),%rax        
+	mov    %r8d,%r12d
 	push   %rbp
 	movq   %rax,%xmm3
-	lea    0x9c4(%rip),%rax        
-	mov    %r8d,%ebp
+	lea    0x9e1(%rip),%rax        
 	push   %rbx
 	movq   %rax,%xmm4
-	lea    0x9b8(%rip),%rax        
+	lea    0x9d8(%rip),%rax        
 	mov    %rcx,%rbx
 	sub    $0xa8,%rsp
 	movss  %xmm0,0x14(%rsp)
 	movq   %rdx,%xmm0
-	lea    0x98d(%rip),%rdx        
+	lea    0x9aa(%rip),%rdx        
 	punpcklqdq %xmm1,%xmm0
 	mov    %rsi,(%rsp)
-	lea    0x97b(%rip),%rsi        
+	lea    0x99e(%rip),%rsi        
 	movaps %xmm0,0x50(%rsp)
-	movq   %rsi,%xmm0
-	lea    0x974(%rip),%rsi        
+	movq   %rdx,%xmm0
+	lea    0x994(%rip),%rdx        
 	punpcklqdq %xmm2,%xmm0
 	mov    %rax,0x90(%rsp)
 	movaps %xmm0,0x60(%rsp)
-	movq   %rdx,%xmm0
+	movq   %rsi,%xmm0
 	punpcklqdq %xmm3,%xmm0
 	movaps %xmm0,0x70(%rsp)
-	movq   %rsi,%xmm0
+	movq   %rdx,%xmm0
 	punpcklqdq %xmm4,%xmm0
 	movaps %xmm0,0x80(%rsp)
-	call   1e10 <getArrayLength(int*)@plt>
-	cmp    $0x2,%eax
-	jne    4472 <doubleGateAction+0x442>
+	call   1e60 <getArrayLength(int*)@plt>
+	lea    0x96e(%rip),%rdi        
+	mov    %eax,%ebp
+	mov    %eax,%esi
+	xor    %eax,%eax
+	call   1ba0 <printf@plt>
+	cmp    $0x2,%ebp
+	jne    44e2 <doubleGateAction+0x462>
 	mov    0x4(%rbx),%eax
 	cmp    %eax,(%rbx)
-	je     44c0 <doubleGateAction+0x490>
-	mov    %ebp,%edi
-	call   1f40 <cudaSetDevice@plt>
+	je     4535 <doubleGateAction+0x4b5>
+	mov    %r12d,%edi
+	call   1f90 <cudaSetDevice@plt>
 	mov    $0x80,%edi
-	call   1df0 <malloc@plt>
+	call   1e40 <malloc@plt>
 	mov    $0x10,%edi
 	mov    %rax,%r12
-	call   1df0 <malloc@plt>
+	call   1e40 <malloc@plt>
 	mov    $0x1,%r10d
 	mov    %r13d,%ecx
 	lea    0x20(%rsp),%rdi
 	mov    %rax,%rbp
 	mov    %r10d,%eax
 	mov    $0x80,%esi
 	movq   $0x0,0x20(%rsp)
 	movq   $0x0,0x28(%rsp)
 	shl    %cl,%eax
 	movq   $0x0,0x30(%rsp)
 	cltq
 	lea    0x0(,%rax,8),%r15
 	mov    %rax,0x8(%rsp)
-	call   1b60 <cudaMalloc@plt>
+	call   1bb0 <cudaMalloc@plt>
 	lea    0x28(%rsp),%rdi
 	mov    %r15,%rsi
-	call   1b60 <cudaMalloc@plt>
+	call   1bb0 <cudaMalloc@plt>
 	lea    0x30(%rsp),%rdi
 	mov    $0x10,%esi
-	call   1b60 <cudaMalloc@plt>
+	call   1bb0 <cudaMalloc@plt>
 	mov    (%rsp),%rsi
 	mov    0x28(%rsp),%rdi
 	mov    %r15,%rdx
 	mov    $0x1,%ecx
-	call   1da0 <cudaMemcpy@plt>
+	call   1df0 <cudaMemcpy@plt>
 	mov    %r14,%rdi
-	call   1b70 <hash(char const*)@plt>
-	mov    (%rbx),%ecx
-	mov    0x4(%rbx),%esi
+	call   1bc0 <hash(char const*)@plt>
+	mov    0x4(%rbx),%ecx
+	mov    (%rbx),%esi
 	mov    $0x4,%edx
 	mov    %rbx,%rdi
 	mov    %eax,%r13d
-	mov    %ecx,0x18(%rsp)
-	mov    0x207de2(%rip),%rcx        
-	mov    %esi,0x1c(%rsp)
+	mov    %ecx,0x1c(%rsp)
+	mov    0x207d7f(%rip),%rcx        
+	mov    %esi,0x18(%rsp)
 	mov    $0x2,%esi
-	call   1f30 <qsort@plt>
+	call   1f80 <qsort@plt>
 	lea    0x50(%rsp),%rdi
 	mov    $0x9,%edx
 	mov    %r14,%rsi
-	call   1ca0 <isInArray(char const**, char*, int)@plt>
+	call   1cf0 <isInArray(char const**, char*, int)@plt>
 	test   %al,%al
-	je     4488 <doubleGateAction+0x458>
+	je     44fd <doubleGateAction+0x47d>
 	mov    (%rbx),%edx
 	mov    $0x1,%r10d
 	mov    0x30(%rsp),%rdi
 	mov    %r10d,%esi
 	mov    %edx,%ecx
 	shl    %cl,%esi
-	movslq %esi,%rcx
-	movq   %rcx,%xmm0
 	mov    0x4(%rbx),%ecx
 	mov    %r10d,%ebx
+	movslq %esi,%rsi
 	shl    %cl,%ebx
 	lea    0x1(%rdx),%ecx
 	mov    0x8(%rsp),%rdx
+	movq   %rsi,%xmm0
 	movslq %ebx,%rax
 	mov    %r10d,%ebx
 	shl    %cl,%ebx
 	movq   %rax,%xmm5
 	movabs $0x100000001,%rcx
 	movslq %ebx,%rax
 	mov    %ebx,%esi
@@ -2096,149 +2101,151 @@
 	xor    %edx,%edx
 	movups %xmm0,0x0(%rbp)
 	div    %rsi
 	mov    $0x10,%edx
 	mov    %rbp,%rsi
 	add    $0x1,%eax
 	mov    %eax,0x44(%rsp)
-	call   1da0 <cudaMemcpy@plt>
+	call   1df0 <cudaMemcpy@plt>
 	cmp    $0x5fd,%r13d
-	je     4440 <doubleGateAction+0x410>
-	jbe    4348 <doubleGateAction+0x318>
+	je     44b0 <doubleGateAction+0x430>
+	jbe    43b0 <doubleGateAction+0x330>
 	cmp    $0x1234,%r13d
-	je     4430 <doubleGateAction+0x400>
-	jbe    4378 <doubleGateAction+0x348>
+	je     44a0 <doubleGateAction+0x420>
+	jbe    43e0 <doubleGateAction+0x360>
 	cmp    $0x340f,%r13d
-	jne    42a8 <doubleGateAction+0x278>
+	jne    4310 <doubleGateAction+0x290>
 	mov    %r12,%rdi
-	call   1cf0 <iswap_gate(float2*)@plt>
-	nopl   0x0(%rax,%rax,1)
+	call   1d40 <iswap_gate(float2*)@plt>
+	cs nopw 0x0(%rax,%rax,1)
 	mov    0x20(%rsp),%rdi
 	mov    $0x1,%ecx
 	mov    $0x80,%edx
 	mov    %r12,%rsi
-	call   1da0 <cudaMemcpy@plt>
+	call   1df0 <cudaMemcpy@plt>
 	mov    %ebx,0x38(%rsp)
 	mov    0x40(%rsp),%ecx
 	xor    %r9d,%r9d
 	mov    0x38(%rsp),%rdx
 	mov    0x44(%rsp),%rdi
 	xor    %r8d,%r8d
 	mov    0x4c(%rsp),%esi
-	call   1ed0 <__cudaPushCallConfiguration@plt>
+	call   1f20 <__cudaPushCallConfiguration@plt>
 	test   %eax,%eax
-	je     43e0 <doubleGateAction+0x3b0>
-	call   1eb0 <cudaDeviceSynchronize@plt>
+	je     4448 <doubleGateAction+0x3c8>
+	call   1f00 <cudaDeviceSynchronize@plt>
 	mov    0x28(%rsp),%rsi
 	mov    (%rsp),%rdi
 	mov    %r15,%rdx
 	mov    $0x2,%ecx
-	call   1da0 <cudaMemcpy@plt>
+	call   1df0 <cudaMemcpy@plt>
 	mov    0x20(%rsp),%rdi
-	call   1e50 <cudaFree@plt>
+	call   1ea0 <cudaFree@plt>
 	mov    0x28(%rsp),%rdi
-	call   1e50 <cudaFree@plt>
+	call   1ea0 <cudaFree@plt>
 	mov    0x30(%rsp),%rdi
-	call   1e50 <cudaFree@plt>
+	call   1ea0 <cudaFree@plt>
 	mov    %r12,%rdi
-	call   1d90 <free@plt>
+	call   1de0 <free@plt>
 	add    $0xa8,%rsp
 	mov    %rbp,%rdi
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
-	jmp    1d90 <free@plt>
+	jmp    1de0 <free@plt>
 	nopw   0x0(%rax,%rax,1)
 	cmp    $0x1ac,%r13d
-	je     4458 <doubleGateAction+0x428>
-	jbe    43a8 <doubleGateAction+0x378>
+	je     44c8 <doubleGateAction+0x448>
+	jbe    4410 <doubleGateAction+0x390>
 	cmp    $0x5f4,%r13d
-	jne    42a8 <doubleGateAction+0x278>
+	jne    4310 <doubleGateAction+0x290>
 	mov    %r12,%rdi
-	call   1c60 <syc_gate(float2*)@plt>
-	jmp    42a8 <doubleGateAction+0x278>
+	call   1cb0 <syc_gate(float2*)@plt>
+	jmp    4310 <doubleGateAction+0x290>
 	nopl   0x0(%rax)
 	cmp    $0x601,%r13d
-	je     4418 <doubleGateAction+0x3e8>
+	je     4488 <doubleGateAction+0x408>
 	cmp    $0x605,%r13d
-	jne    42a8 <doubleGateAction+0x278>
+	jne    4310 <doubleGateAction+0x290>
 	movss  0x14(%rsp),%xmm0
 	mov    %r12,%rdi
-	call   1c90 <rzz_gate(float2*, float)@plt>
-	jmp    42a8 <doubleGateAction+0x278>
+	call   1ce0 <rzz_gate(float2*, float)@plt>
+	jmp    4310 <doubleGateAction+0x290>
 	nopl   (%rax)
 	cmp    $0x1a2,%r13d
-	je     4400 <doubleGateAction+0x3d0>
+	je     4470 <doubleGateAction+0x3f0>
 	cmp    $0x1aa,%r13d
-	jne    42a8 <doubleGateAction+0x278>
+	jne    4310 <doubleGateAction+0x290>
 	mov    0x1c(%rsp),%edx
 	mov    %r12,%rdi
 	cmp    %edx,0x18(%rsp)
-	jle    4468 <doubleGateAction+0x438>
-	call   1cb0 <cnot_gate_control_big(float2*)@plt>
-	jmp    42a8 <doubleGateAction+0x278>
+	jle    44d8 <doubleGateAction+0x458>
+	call   1d00 <cnot_gate_control_big(float2*)@plt>
+	jmp    4310 <doubleGateAction+0x290>
 	nopl   0x0(%rax)
 	mov    0x30(%rsp),%rcx
 	mov    0x8(%rsp),%rdx
 	mov    0x20(%rsp),%rsi
 	mov    0x28(%rsp),%rdi
-	call   1d70 <actionOnDoubleQubit(float2*, float2*, unsigned long, unsigned long*)@plt>
-	jmp    42e8 <doubleGateAction+0x2b8>
-	xchg   %ax,%ax
+	call   1dc0 <actionOnDoubleQubit(float2*, float2*, unsigned long, unsigned long*)@plt>
+	jmp    4350 <doubleGateAction+0x2d0>
+	cs nopw 0x0(%rax,%rax,1)
 	movss  0x14(%rsp),%xmm0
 	mov    %r12,%rdi
-	call   1b40 <cphase_gate(float2*, float)@plt>
-	jmp    42a8 <doubleGateAction+0x278>
+	call   1b80 <cphase_gate(float2*, float)@plt>
+	jmp    4310 <doubleGateAction+0x290>
 	nopl   0x0(%rax,%rax,1)
 	movss  0x14(%rsp),%xmm0
 	mov    %r12,%rdi
-	call   1e70 <ryy_gate(float2*, float)@plt>
-	jmp    42a8 <doubleGateAction+0x278>
+	call   1ec0 <ryy_gate(float2*, float)@plt>
+	jmp    4310 <doubleGateAction+0x290>
 	nopl   0x0(%rax,%rax,1)
 	mov    %r12,%rdi
-	call   1f10 <swap_gate(float2*)@plt>
-	jmp    42a8 <doubleGateAction+0x278>
+	call   1f60 <swap_gate(float2*)@plt>
+	jmp    4310 <doubleGateAction+0x290>
 	nopl   (%rax)
 	movss  0x14(%rsp),%xmm0
 	mov    %r12,%rdi
-	call   1c70 <rxx_gate(float2*, float)@plt>
-	jmp    42a8 <doubleGateAction+0x278>
+	call   1cc0 <rxx_gate(float2*, float)@plt>
+	jmp    4310 <doubleGateAction+0x290>
 	nopl   0x0(%rax,%rax,1)
 	mov    %r12,%rdi
-	call   1dd0 <cz_gate(float2*)@plt>
-	jmp    42a8 <doubleGateAction+0x278>
+	call   1e20 <cz_gate(float2*)@plt>
+	jmp    4310 <doubleGateAction+0x290>
 	nopl   (%rax)
-	call   1c10 <cnot_gate_control_small(float2*)@plt>
-	jmp    42a8 <doubleGateAction+0x278>
-	lea    0x627(%rip),%rdi        
-	call   1e80 <puts@plt>
+	call   1c60 <cnot_gate_control_small(float2*)@plt>
+	jmp    4310 <doubleGateAction+0x290>
+	lea    0x637(%rip),%rdi        
+	mov    %r14,%rsi
+	xor    %eax,%eax
+	call   1ba0 <printf@plt>
 	mov    $0x1,%edi
-	call   1db0 <exit@plt>
+	call   1e00 <exit@plt>
 	mov    0x20(%rsp),%rdi
-	call   1e50 <cudaFree@plt>
+	call   1ea0 <cudaFree@plt>
 	mov    0x28(%rsp),%rdi
-	call   1e50 <cudaFree@plt>
+	call   1ea0 <cudaFree@plt>
 	mov    0x30(%rsp),%rdi
-	call   1e50 <cudaFree@plt>
+	call   1ea0 <cudaFree@plt>
 	mov    %r12,%rdi
-	call   1d90 <free@plt>
+	call   1de0 <free@plt>
 	mov    %rbp,%rdi
-	call   1d90 <free@plt>
+	call   1de0 <free@plt>
 	mov    $0x3,%edi
-	call   1db0 <exit@plt>
-	lea    0x601(%rip),%rdi        
-	call   1e80 <puts@plt>
+	call   1e00 <exit@plt>
+	lea    0x61c(%rip),%rdi        
+	call   1ed0 <puts@plt>
 	mov    $0x2,%edi
-	call   1db0 <exit@plt>
-	cs nopw 0x0(%rax,%rax,1)
+	call   1e00 <exit@plt>
+	nopl   0x0(%rax,%rax,1)
 
-00000000000044e0 <__device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)>:
+0000000000004550 <__device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)>:
 __device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*):
 	sub    $0x88,%rsp
 	lea    0x18(%rsp),%rax
 	mov    %rdi,0x18(%rsp)
 	lea    0x30(%rsp),%rdi
 	movq   %rax,%xmm0
 	lea    0x10(%rsp),%rax
@@ -2258,39 +2265,39 @@
 	movl   $0x1,0x38(%rsp)
 	movabs $0x100000001,%rax
 	punpcklqdq %xmm2,%xmm0
 	mov    %rax,0x30(%rsp)
 	mov    %rax,0x3c(%rsp)
 	movl   $0x1,0x44(%rsp)
 	movaps %xmm0,0x70(%rsp)
-	call   1ea0 <__cudaPopCallConfiguration@plt>
+	call   1ef0 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
-	jne    45a1 <__device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xc1>
+	jne    4611 <__device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)+0xc1>
 	push   0x28(%rsp)
-	mov    0x207a4a(%rip),%rdi        
+	mov    0x2079da(%rip),%rdi        
 	push   0x28(%rsp)
 	mov    0x4c(%rsp),%rcx
 	mov    0x54(%rsp),%r8d
 	mov    0x40(%rsp),%rsi
 	mov    0x48(%rsp),%edx
 	lea    0x70(%rsp),%r9
-	call   1bb0 <cudaLaunchKernel@plt>
+	call   1c00 <cudaLaunchKernel@plt>
 	pop    %rax
 	pop    %rdx
 	add    $0x88,%rsp
 	ret
 	nopl   0x0(%rax)
 
-00000000000045b0 <actionOnTripleGate(float2*, float2*, unsigned long, unsigned long*)>:
+0000000000004620 <actionOnTripleGate(float2*, float2*, unsigned long, unsigned long*)>:
 actionOnTripleGate(float2*, float2*, unsigned long, unsigned long*):
-	jmp    1b90 <__device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>
+	jmp    1be0 <__device_stub__Z18actionOnTripleGateP6float2S0_mPm(float2*, float2*, unsigned long, unsigned long*)@plt>
 	nop
 	cs nopw 0x0(%rax,%rax,1)
 
-00000000000045c0 <tripleGateAction>:
+0000000000004630 <tripleGateAction>:
 tripleGateAction():
 	push   %r15
 	lea    0x47b(%rip),%rax        
 	push   %r14
 	movq   %rax,%xmm1
 	mov    %rdi,%r14
 	mov    %rcx,%rdi
@@ -2299,81 +2306,81 @@
 	push   %r12
 	push   %rbp
 	mov    %r8d,%ebp
 	push   %rbx
 	mov    %rcx,%rbx
 	sub    $0x68,%rsp
 	mov    %rsi,0x8(%rsp)
-	lea    0x455(%rip),%rsi        
+	lea    0x44b(%rip),%rsi        
 	movq   %rsi,%xmm0
 	punpcklqdq %xmm1,%xmm0
 	movaps %xmm0,0x50(%rsp)
-	call   1e10 <getArrayLength(int*)@plt>
+	call   1e60 <getArrayLength(int*)@plt>
 	cmp    $0x3,%eax
-	jne    498b <tripleGateAction+0x3cb>
+	jne    49fb <tripleGateAction+0x3cb>
 	mov    (%rbx),%ecx
 	mov    0x4(%rbx),%eax
 	cmp    %eax,%ecx
-	je     4975 <tripleGateAction+0x3b5>
+	je     49e5 <tripleGateAction+0x3b5>
 	mov    0x8(%rbx),%edx
 	cmp    %edx,%eax
-	je     4975 <tripleGateAction+0x3b5>
+	je     49e5 <tripleGateAction+0x3b5>
 	cmp    %edx,%ecx
-	je     4975 <tripleGateAction+0x3b5>
+	je     49e5 <tripleGateAction+0x3b5>
 	mov    %ebp,%edi
-	call   1f40 <cudaSetDevice@plt>
+	call   1f90 <cudaSetDevice@plt>
 	mov    $0x200,%edi
-	call   1df0 <malloc@plt>
+	call   1e40 <malloc@plt>
 	mov    $0x18,%edi
 	mov    %rax,%r12
-	call   1df0 <malloc@plt>
+	call   1e40 <malloc@plt>
 	mov    $0x1,%r8d
 	mov    %r13d,%ecx
 	lea    0x20(%rsp),%rdi
 	mov    %rax,%rbp
 	mov    %r8d,%eax
 	mov    $0x200,%esi
 	movq   $0x0,0x20(%rsp)
 	movq   $0x0,0x28(%rsp)
 	shl    %cl,%eax
 	movq   $0x0,0x30(%rsp)
 	movslq %eax,%r13
-	call   1b60 <cudaMalloc@plt>
+	call   1bb0 <cudaMalloc@plt>
 	lea    0x0(,%r13,8),%r15
 	lea    0x28(%rsp),%rdi
 	mov    %r15,%rsi
-	call   1b60 <cudaMalloc@plt>
+	call   1bb0 <cudaMalloc@plt>
 	lea    0x30(%rsp),%rdi
 	mov    $0x18,%esi
-	call   1b60 <cudaMalloc@plt>
+	call   1bb0 <cudaMalloc@plt>
 	mov    0x8(%rsp),%rsi
 	mov    0x28(%rsp),%rdi
 	mov    %r15,%rdx
 	mov    $0x1,%ecx
-	call   1da0 <cudaMemcpy@plt>
+	call   1df0 <cudaMemcpy@plt>
 	mov    %r14,%rdi
-	call   1b70 <hash(char const*)@plt>
+	call   1bc0 <hash(char const*)@plt>
 	mov    (%rbx),%esi
 	mov    $0x4,%edx
 	mov    %rbx,%rdi
-	mov    0x2078c7(%rip),%rcx        
+	mov    0x207857(%rip),%rcx        
 	mov    %eax,0x1c(%rsp)
 	mov    %esi,0x10(%rsp)
 	mov    0x4(%rbx),%esi
 	mov    %esi,0x18(%rsp)
 	mov    0x8(%rbx),%esi
 	mov    %esi,0x14(%rsp)
 	mov    $0x3,%esi
-	call   1f30 <qsort@plt>
+	call   1f80 <qsort@plt>
 	lea    0x50(%rsp),%rdi
 	mov    $0x2,%edx
 	mov    %r14,%rsi
-	call   1ca0 <isInArray(char const**, char*, int)@plt>
+	call   1cf0 <isInArray(char const**, char*, int)@plt>
 	test   %al,%al
-	je     49a1 <tripleGateAction+0x3e1>
+	je     4a11 <tripleGateAction+0x3e1>
 	mov    (%rbx),%eax
 	mov    $0x1,%r8d
 	mov    %r13,%rsi
 	mov    0x30(%rsp),%rdi
 	mov    %r8d,%edx
 	mov    %eax,%ecx
 	shl    %cl,%edx
@@ -2402,155 +2409,155 @@
 	mov    %rcx,0x48(%rsp)
 	mov    $0x1,%ecx
 	div    %rsi
 	mov    $0x18,%edx
 	mov    %rbp,%rsi
 	add    $0x1,%eax
 	mov    %eax,0x44(%rsp)
-	call   1da0 <cudaMemcpy@plt>
+	call   1df0 <cudaMemcpy@plt>
 	mov    0x1c(%rsp),%eax
 	cmp    $0x537,%eax
-	je     48b8 <tripleGateAction+0x2f8>
+	je     4928 <tripleGateAction+0x2f8>
 	cmp    $0x3229,%eax
-	je     4850 <tripleGateAction+0x290>
+	je     48c0 <tripleGateAction+0x290>
 	mov    0x20(%rsp),%rdi
 	mov    $0x1,%ecx
 	mov    $0x200,%edx
 	mov    %r12,%rsi
-	call   1da0 <cudaMemcpy@plt>
+	call   1df0 <cudaMemcpy@plt>
 	mov    %ebx,0x38(%rsp)
 	mov    0x40(%rsp),%ecx
 	xor    %r9d,%r9d
 	mov    0x38(%rsp),%rdx
 	mov    0x44(%rsp),%rdi
 	xor    %r8d,%r8d
 	mov    0x4c(%rsp),%esi
-	call   1ed0 <__cudaPushCallConfiguration@plt>
+	call   1f20 <__cudaPushCallConfiguration@plt>
 	test   %eax,%eax
-	je     4918 <tripleGateAction+0x358>
-	call   1eb0 <cudaDeviceSynchronize@plt>
+	je     4988 <tripleGateAction+0x358>
+	call   1f00 <cudaDeviceSynchronize@plt>
 	mov    0x28(%rsp),%rsi
 	mov    0x8(%rsp),%rdi
 	mov    %r15,%rdx
 	mov    $0x2,%ecx
-	call   1da0 <cudaMemcpy@plt>
+	call   1df0 <cudaMemcpy@plt>
 	mov    0x20(%rsp),%rdi
-	call   1e50 <cudaFree@plt>
+	call   1ea0 <cudaFree@plt>
 	mov    0x28(%rsp),%rdi
-	call   1e50 <cudaFree@plt>
+	call   1ea0 <cudaFree@plt>
 	mov    0x30(%rsp),%rdi
-	call   1e50 <cudaFree@plt>
+	call   1ea0 <cudaFree@plt>
 	mov    %r12,%rdi
-	call   1d90 <free@plt>
+	call   1de0 <free@plt>
 	add    $0x68,%rsp
 	mov    %rbp,%rdi
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
-	jmp    1d90 <free@plt>
+	jmp    1de0 <free@plt>
 	xchg   %ax,%ax
 	mov    0x18(%rsp),%ecx
 	mov    0x14(%rsp),%eax
 	cmp    %eax,%ecx
 	cmovle %ecx,%eax
 	cmp    0x10(%rsp),%eax
-	jg     4968 <tripleGateAction+0x3a8>
+	jg     49d8 <tripleGateAction+0x3a8>
 	mov    0x14(%rsp),%eax
 	cmp    %eax,%ecx
 	cmovge %ecx,%eax
 	cmp    0x10(%rsp),%eax
-	jl     4948 <tripleGateAction+0x388>
+	jl     49b8 <tripleGateAction+0x388>
 	mov    0x10(%rsp),%eax
 	mov    0x14(%rsp),%edi
 	cmp    %edi,%eax
-	jge    488a <tripleGateAction+0x2ca>
+	jge    48fa <tripleGateAction+0x2ca>
 	cmp    %ecx,%eax
-	jg     48a6 <tripleGateAction+0x2e6>
+	jg     4916 <tripleGateAction+0x2e6>
 	mov    0x10(%rsp),%eax
 	mov    0x18(%rsp),%esi
 	cmp    %esi,%eax
-	jge    47b6 <tripleGateAction+0x1f6>
+	jge    4826 <tripleGateAction+0x1f6>
 	mov    0x14(%rsp),%edi
 	cmp    %edi,%eax
-	jle    47b6 <tripleGateAction+0x1f6>
+	jle    4826 <tripleGateAction+0x1f6>
 	mov    %r12,%rdi
-	call   1c00 <fred_gate_control_mid(float2*)@plt>
-	jmp    47b6 <tripleGateAction+0x1f6>
+	call   1c50 <fred_gate_control_mid(float2*)@plt>
+	jmp    4826 <tripleGateAction+0x1f6>
 	nopl   0x0(%rax,%rax,1)
 	mov    0x10(%rsp),%esi
 	mov    0x18(%rsp),%eax
 	cmp    %eax,%esi
 	cmovge %esi,%eax
 	cmp    0x14(%rsp),%eax
-	jl     4958 <tripleGateAction+0x398>
+	jl     49c8 <tripleGateAction+0x398>
 	mov    0x18(%rsp),%eax
 	cmp    %eax,%esi
 	cmovle %esi,%eax
 	cmp    0x14(%rsp),%eax
-	jg     4938 <tripleGateAction+0x378>
+	jg     49a8 <tripleGateAction+0x378>
 	mov    0x14(%rsp),%eax
 	cmp    %eax,0x10(%rsp)
-	jge    48ee <tripleGateAction+0x32e>
+	jge    495e <tripleGateAction+0x32e>
 	cmp    %eax,0x18(%rsp)
-	jg     4906 <tripleGateAction+0x346>
+	jg     4976 <tripleGateAction+0x346>
 	mov    0x14(%rsp),%eax
 	cmp    %eax,0x18(%rsp)
-	jge    47b6 <tripleGateAction+0x1f6>
+	jge    4826 <tripleGateAction+0x1f6>
 	cmp    %eax,0x10(%rsp)
-	jle    47b6 <tripleGateAction+0x1f6>
+	jle    4826 <tripleGateAction+0x1f6>
 	mov    %r12,%rdi
-	call   1c80 <toff_gate_target_mid(float2*)@plt>
-	jmp    47b6 <tripleGateAction+0x1f6>
+	call   1cd0 <toff_gate_target_mid(float2*)@plt>
+	jmp    4826 <tripleGateAction+0x1f6>
 	nopl   0x0(%rax,%rax,1)
 	mov    0x30(%rsp),%rcx
 	mov    0x20(%rsp),%rsi
 	mov    %r13,%rdx
 	mov    0x28(%rsp),%rdi
-	call   1de0 <actionOnTripleGate(float2*, float2*, unsigned long, unsigned long*)@plt>
-	jmp    47f6 <tripleGateAction+0x236>
+	call   1e30 <actionOnTripleGate(float2*, float2*, unsigned long, unsigned long*)@plt>
+	jmp    4866 <tripleGateAction+0x236>
 	nopl   0x0(%rax)
 	mov    %r12,%rdi
-	call   1bc0 <toff_gate_target_small(float2*)@plt>
-	jmp    47b6 <tripleGateAction+0x1f6>
+	call   1c10 <toff_gate_target_small(float2*)@plt>
+	jmp    4826 <tripleGateAction+0x1f6>
 	nopl   (%rax)
 	mov    %r12,%rdi
-	call   1c50 <fred_gate_control_big(float2*)@plt>
-	jmp    47b6 <tripleGateAction+0x1f6>
+	call   1ca0 <fred_gate_control_big(float2*)@plt>
+	jmp    4826 <tripleGateAction+0x1f6>
 	nopl   (%rax)
 	mov    %r12,%rdi
-	call   1e60 <toff_gate_target_big(float2*)@plt>
-	jmp    47b6 <tripleGateAction+0x1f6>
+	call   1eb0 <toff_gate_target_big(float2*)@plt>
+	jmp    4826 <tripleGateAction+0x1f6>
 	nopl   (%rax)
 	mov    %r12,%rdi
-	call   1be0 <fred_gate_control_small(float2*)@plt>
-	jmp    47b6 <tripleGateAction+0x1f6>
-	lea    0x14c(%rip),%rdi        
-	call   1e80 <puts@plt>
+	call   1c30 <fred_gate_control_small(float2*)@plt>
+	jmp    4826 <tripleGateAction+0x1f6>
+	lea    0x16c(%rip),%rdi        
+	call   1ed0 <puts@plt>
 	mov    $0x2,%edi
-	call   1db0 <exit@plt>
-	lea    0x15e(%rip),%rdi        
-	call   1e80 <puts@plt>
+	call   1e00 <exit@plt>
+	lea    0x17e(%rip),%rdi        
+	call   1ed0 <puts@plt>
 	mov    $0x1,%edi
-	call   1db0 <exit@plt>
+	call   1e00 <exit@plt>
 	mov    0x20(%rsp),%rdi
-	call   1e50 <cudaFree@plt>
+	call   1ea0 <cudaFree@plt>
 	mov    0x28(%rsp),%rdi
-	call   1e50 <cudaFree@plt>
+	call   1ea0 <cudaFree@plt>
 	mov    0x30(%rsp),%rdi
-	call   1e50 <cudaFree@plt>
+	call   1ea0 <cudaFree@plt>
 	mov    %r12,%rdi
-	call   1d90 <free@plt>
+	call   1de0 <free@plt>
 	mov    %rbp,%rdi
-	call   1d90 <free@plt>
+	call   1de0 <free@plt>
 	mov    $0x3,%edi
-	call   1db0 <exit@plt>
+	call   1e00 <exit@plt>
 	nopl   0x0(%rax)
 
-00000000000049e0 <atexit>:
+0000000000004a50 <atexit>:
 atexit():
 /opt/glibc-2.31/stdlib/atexit.c:46
-	mov    0x207839(%rip),%rdx        
+	mov    0x2077d1(%rip),%rdx        
 	xor    %esi,%esi
-	jmp    1d00 <__cxa_atexit@plt>
+	jmp    1d50 <__cxa_atexit@plt>
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.fini {}

```diff
@@ -1,13 +1,13 @@
 
 
 
 Disassembly of section .fini:
 
-00000000000049f0 <_fini>:
+0000000000004a60 <_fini>:
 _fini():
 /opt/glibc-2.31/csu/../sysdeps/x86_64/crti.S:84
 	sub    $0x8,%rsp
 /opt/glibc-2.31/csu/../sysdeps/x86_64/crtn.S:44
 	add    $0x8,%rsp
 /opt/glibc-2.31/csu/../sysdeps/x86_64/crtn.S:45
 	ret
```

#### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -1,51 +1,53 @@
 
 Hex dump of section '.rodata':
-  0x00004a00 73007364 67007400 74646700 68007278 s.sdg.t.tdg.h.rx
-  0x00004a10 00727900 727a0064 616d705f 49007064 .ry.rz.damp_I.pd
-  0x00004a20 00616400 69737761 70006370 00637a00 .ad.iswap.cp.cz.
-  0x00004a30 72787800 72797900 727a7a00 73796300 rxx.ryy.rzz.syc.
-  0x00004a40 63787800 63737761 70006363 78000000 cxx.cswap.ccx...
-  0x00004a50 0bf4ffff 58f2ffff 58f2ffff 58f2ffff ....X...X...X...
-  0x00004a60 58f2ffff 58f2ffff 58f2ffff 58f2ffff X...X...X...X...
-  0x00004a70 58f2ffff 58f2ffff 58f2ffff 18f4ffff X...X...X.......
-  0x00004a80 25f4ffff 58f2ffff 58f2ffff 58f2ffff %...X...X...X...
-  0x00004a90 32f4ffff 3ff4ffff fef3ffff 00000000 2...?...........
-  0x00004aa0 4d757374 20626520 68617665 2074776f Must be have two
-  0x00004ab0 20616374 696f6e20 706f7369 74696f6e  action position
-  0x00004ac0 21000000 00000000 61637469 6f6e2070 !.......action p
-  0x00004ad0 6f736974 696f6e20 6d757374 20626520 osition must be 
-  0x00004ae0 64696666 6572656e 74210000 00000000 different!......
-  0x00004af0 4d757374 20626520 68617665 20746872 Must be have thr
-  0x00004b00 65652061 6374696f 6e20706f 73697469 ee action positi
-  0x00004b10 6f6e2100 00000000 5f5a3138 61637469 on!....._Z18acti
-  0x00004b20 6f6e4f6e 54726970 6c654761 74655036 onOnTripleGateP6
-  0x00004b30 666c6f61 74325330 5f6d506d 00000000 float2S0_mPm....
-  0x00004b40 5f5a3139 61637469 6f6e4f6e 446f7562 _Z19actionOnDoub
-  0x00004b50 6c655175 62697450 36666c6f 61743253 leQubitP6float2S
-  0x00004b60 305f6d50 6d000000 5f5a3139 61637469 0_mPm..._Z19acti
-  0x00004b70 6f6e4f6e 53696e67 6c655175 62697450 onOnSingleQubitP
-  0x00004b80 36666c6f 61743253 305f6d50 6d000000 6float2S0_mPm...
-  0x00004b90 00000000 00000000 0000803f 00000000 ...........?....
-  0x00004ba0 0000803f 00000000 00000000 00000000 ...?............
-  0x00004bb0 00000000 00000000 00000000 000080bf ................
-  0x00004bc0 00000000 0000803f 00000000 00000000 .......?........
-  0x00004bd0 00000000 00000000 000080bf 00000000 ................
-  0x00004be0 00000000 00000000 00000000 0000803f ...............?
-  0x00004bf0 00000000 00000000 f304353f f304353f ..........5?..5?
-  0x00004c00 00000000 00000000 f304353f f30435bf ..........5?..5.
-  0x00004c10 f304353f 00000000 f304353f 00000000 ..5?......5?....
-  0x00004c20 f304353f 00000000 f30435bf 00000000 ..5?......5.....
-  0x00004c30 00000080 00000000 00000000 00000000 ................
-  0x00004c40 00000000 000080bf 00000000 00000000 ................
-  0x00004c50 00000000 00000000 d7b35d3f 000000bf ..........]?....
-  0x00004c60 00000000 01000000 02000000 03000000 ................
-  0x00004c70 04000000 04000000 04000000 04000000 ................
-  0x00004c80 2d000000 2d000000 2d000000 2d000000 -...-...-...-...
-  0x00004c90 3f000000 3f000000 3f000000 3f000000 ?...?...?...?...
-  0x00004ca0 398ee338 398ee338 398ee338 398ee338 9..89..89..89..8
-  0x00004cb0 0000803f 0000803f 0000803f 0000803f ...?...?...?...?
-  0x00004cc0 1b000000 1b000000 1b000000 1b000000 ................
-  0x00004cd0 36000000 36000000 36000000 36000000 6...6...6...6...
-  0x00004ce0 0000003f 0000803f 00000030 00000000 ...?...?...0....
-  0x00004cf0 8dedb5a0 f7c6b03e                   .......>
+  0x00004a70 73007364 67007400 74646700 68007278 s.sdg.t.tdg.h.rx
+  0x00004a80 00727900 727a0064 616d705f 49007064 .ry.rz.damp_I.pd
+  0x00004a90 00616400 69737761 70006370 00637a00 .ad.iswap.cp.cz.
+  0x00004aa0 72787800 72797900 727a7a00 73796300 rxx.ryy.rzz.syc.
+  0x00004ab0 63637800 63737761 7000706f 735f6172 ccx.cswap.pos_ar
+  0x00004ac0 7261795f 73697a65 203d2025 640a0000 ray_size = %d...
+  0x00004ad0 dbf3ffff 28f2ffff 28f2ffff 28f2ffff ....(...(...(...
+  0x00004ae0 28f2ffff 28f2ffff 28f2ffff 28f2ffff (...(...(...(...
+  0x00004af0 28f2ffff 28f2ffff 28f2ffff e8f3ffff (...(...(.......
+  0x00004b00 f5f3ffff 28f2ffff 28f2ffff 28f2ffff ....(...(...(...
+  0x00004b10 02f4ffff 0ff4ffff cef3ffff 00000000 ................
+  0x00004b20 4d757374 20626520 68617665 2074776f Must be have two
+  0x00004b30 20616374 696f6e20 706f7369 74696f6e  action position
+  0x00004b40 212c2067 6174654e 616d653a 2025730a !, gateName: %s.
+  0x00004b50 00000000 00000000 61637469 6f6e2070 ........action p
+  0x00004b60 6f736974 696f6e20 6d757374 20626520 osition must be 
+  0x00004b70 64696666 6572656e 74210000 00000000 different!......
+  0x00004b80 4d757374 20626520 68617665 20746872 Must be have thr
+  0x00004b90 65652061 6374696f 6e20706f 73697469 ee action positi
+  0x00004ba0 6f6e2100 00000000 5f5a3138 61637469 on!....._Z18acti
+  0x00004bb0 6f6e4f6e 54726970 6c654761 74655036 onOnTripleGateP6
+  0x00004bc0 666c6f61 74325330 5f6d506d 00000000 float2S0_mPm....
+  0x00004bd0 5f5a3139 61637469 6f6e4f6e 446f7562 _Z19actionOnDoub
+  0x00004be0 6c655175 62697450 36666c6f 61743253 leQubitP6float2S
+  0x00004bf0 305f6d50 6d000000 5f5a3139 61637469 0_mPm..._Z19acti
+  0x00004c00 6f6e4f6e 53696e67 6c655175 62697450 onOnSingleQubitP
+  0x00004c10 36666c6f 61743253 305f6d50 6d000000 6float2S0_mPm...
+  0x00004c20 00000000 00000000 0000803f 00000000 ...........?....
+  0x00004c30 0000803f 00000000 00000000 00000000 ...?............
+  0x00004c40 00000000 00000000 00000000 000080bf ................
+  0x00004c50 00000000 0000803f 00000000 00000000 .......?........
+  0x00004c60 00000000 00000000 000080bf 00000000 ................
+  0x00004c70 00000000 00000000 00000000 0000803f ...............?
+  0x00004c80 00000000 00000000 f304353f f304353f ..........5?..5?
+  0x00004c90 00000000 00000000 f304353f f30435bf ..........5?..5.
+  0x00004ca0 f304353f 00000000 f304353f 00000000 ..5?......5?....
+  0x00004cb0 f304353f 00000000 f30435bf 00000000 ..5?......5.....
+  0x00004cc0 00000080 00000000 00000000 00000000 ................
+  0x00004cd0 00000000 000080bf 00000000 00000000 ................
+  0x00004ce0 00000000 00000000 d7b35d3f 000000bf ..........]?....
+  0x00004cf0 00000000 01000000 02000000 03000000 ................
+  0x00004d00 04000000 04000000 04000000 04000000 ................
+  0x00004d10 2d000000 2d000000 2d000000 2d000000 -...-...-...-...
+  0x00004d20 3f000000 3f000000 3f000000 3f000000 ?...?...?...?...
+  0x00004d30 398ee338 398ee338 398ee338 398ee338 9..89..89..89..8
+  0x00004d40 0000803f 0000803f 0000803f 0000803f ...?...?...?...?
+  0x00004d50 1b000000 1b000000 1b000000 1b000000 ................
+  0x00004d60 36000000 36000000 36000000 36000000 6...6...6...6...
+  0x00004d70 0000003f 0000803f 00000030 00000000 ...?...?...0....
+  0x00004d80 8dedb5a0 f7c6b03e                   .......>
```

#### readelf --wide --decompress --hex-dump=.nv_fatbin {}

```diff
@@ -1,281 +1,272 @@
 
 Hex dump of section '.nv_fatbin':
-  0x00004cf8 50ed55ba 01001000 b0030000 00000000 P.U.............
-  0x00004d08 02000101 48000000 68030000 00000000 ....H...h.......
-  0x00004d18 00000000 00000000 07000100 50000000 ............P...
-  0x00004d28 00000000 00000000 11000000 00000000 ................
-  0x00004d38 00000000 00000000 00000000 00000000 ................
-  0x00004d48 00000000 00000000 7f454c46 02010133 .........ELF...3
-  0x00004d58 07000000 00000000 0200be00 7c000000 ............|...
-  0x00004d68 00000000 00000000 f8020000 00000000 ................
-  0x00004d78 78010000 00000000 50055000 40003800 x.......P.P.@.8.
-  0x00004d88 02004000 06000100 002e7368 73747274 ..@.......shstrt
-  0x00004d98 6162002e 73747274 6162002e 73796d74 ab..strtab..symt
-  0x00004da8 6162002e 73796d74 61625f73 686e6478 ab..symtab_shndx
-  0x00004db8 002e6e76 2e696e66 6f002e6e 762e6361 ..nv.info..nv.ca
-  0x00004dc8 6c6c6772 61706800 2e6e762e 70726f74 llgraph..nv.prot
-  0x00004dd8 6f747970 65002e6e 762e7265 6c2e6163 otype..nv.rel.ac
-  0x00004de8 74696f6e 00002e73 68737472 74616200 tion...shstrtab.
-  0x00004df8 2e737472 74616200 2e73796d 74616200 .strtab..symtab.
-  0x00004e08 2e73796d 7461625f 73686e64 78002e6e .symtab_shndx..n
-  0x00004e18 762e696e 666f002e 6e762e63 616c6c67 v.info..nv.callg
-  0x00004e28 72617068 002e6e76 2e70726f 746f7479 raph..nv.prototy
-  0x00004e38 7065002e 6e762e72 656c2e61 6374696f pe..nv.rel.actio
-  0x00004e48 6e000000 00000000 00000000 00000000 n...............
-  0x00004e58 00000000 00000000 00000000 00000000 ................
-  0x00004e68 32000000 03000400 00000000 00000000 2...............
-  0x00004e78 00000000 00000000 4e000000 03000500 ........N.......
-  0x00004e88 00000000 00000000 00000000 00000000 ................
-  0x00004e98 00000000 ffffffff 00000000 feffffff ................
-  0x00004ea8 00000000 fdffffff 00000000 fcffffff ................
-  0x00004eb8 73000000 00000000 00000011 25000536 s...........%..6
-  0x00004ec8 00000000 00000000 00000000 00000000 ................
-  0x00004ed8 00000000 00000000 00000000 00000000 ................
+  0x00004d88 50ed55ba 01001000 b0030000 00000000 P.U.............
+  0x00004d98 02000101 48000000 68030000 00000000 ....H...h.......
+  0x00004da8 00000000 00000000 07000100 50000000 ............P...
+  0x00004db8 00000000 00000000 11000000 00000000 ................
+  0x00004dc8 00000000 00000000 00000000 00000000 ................
+  0x00004dd8 00000000 00000000 7f454c46 02010133 .........ELF...3
+  0x00004de8 07000000 00000000 0200be00 7c000000 ............|...
+  0x00004df8 00000000 00000000 f8020000 00000000 ................
+  0x00004e08 78010000 00000000 50055000 40003800 x.......P.P.@.8.
+  0x00004e18 02004000 06000100 002e7368 73747274 ..@.......shstrt
+  0x00004e28 6162002e 73747274 6162002e 73796d74 ab..strtab..symt
+  0x00004e38 6162002e 73796d74 61625f73 686e6478 ab..symtab_shndx
+  0x00004e48 002e6e76 2e696e66 6f002e6e 762e6361 ..nv.info..nv.ca
+  0x00004e58 6c6c6772 61706800 2e6e762e 70726f74 llgraph..nv.prot
+  0x00004e68 6f747970 65002e6e 762e7265 6c2e6163 otype..nv.rel.ac
+  0x00004e78 74696f6e 00002e73 68737472 74616200 tion...shstrtab.
+  0x00004e88 2e737472 74616200 2e73796d 74616200 .strtab..symtab.
+  0x00004e98 2e73796d 7461625f 73686e64 78002e6e .symtab_shndx..n
+  0x00004ea8 762e696e 666f002e 6e762e63 616c6c67 v.info..nv.callg
+  0x00004eb8 72617068 002e6e76 2e70726f 746f7479 raph..nv.prototy
+  0x00004ec8 7065002e 6e762e72 656c2e61 6374696f pe..nv.rel.actio
+  0x00004ed8 6e000000 00000000 00000000 00000000 n...............
   0x00004ee8 00000000 00000000 00000000 00000000 ................
-  0x00004ef8 00000000 00000000 00000000 00000000 ................
-  0x00004f08 01000000 03000000 00000000 00000000 ................
-  0x00004f18 00000000 00000000 40000000 00000000 ........@.......
-  0x00004f28 5d000000 00000000 00000000 00000000 ]...............
-  0x00004f38 01000000 00000000 00000000 00000000 ................
-  0x00004f48 0b000000 03000000 00000000 00000000 ................
-  0x00004f58 00000000 00000000 9d000000 00000000 ................
-  0x00004f68 5d000000 00000000 00000000 00000000 ]...............
-  0x00004f78 01000000 00000000 00000000 00000000 ................
-  0x00004f88 13000000 02000000 00000000 00000000 ................
-  0x00004f98 00000000 00000000 00010000 00000000 ................
-  0x00004fa8 48000000 00000000 02000000 03000000 H...............
-  0x00004fb8 08000000 00000000 18000000 00000000 ................
-  0x00004fc8 32000000 01000070 00000000 00000000 2......p........
-  0x00004fd8 00000000 00000000 48010000 00000000 ........H.......
-  0x00004fe8 20000000 00000000 03000000 00000000  ...............
-  0x00004ff8 04000000 00000000 08000000 00000000 ................
-  0x00005008 4e000000 0b000070 00000000 00000000 N......p........
-  0x00005018 00000000 00000000 68010000 00000000 ........h.......
-  0x00005028 10000000 00000000 00000000 00000000 ................
-  0x00005038 08000000 00000000 08000000 00000000 ................
-  0x00005048 06000000 05000000 f8020000 00000000 ................
-  0x00005058 00000000 00000000 00000000 00000000 ................
-  0x00005068 70000000 00000000 70000000 00000000 p.......p.......
-  0x00005078 08000000 00000000 01000000 05000000 ................
-  0x00005088 f8020000 00000000 00000000 00000000 ................
-  0x00005098 00000000 00000000 70000000 00000000 ........p.......
-  0x000050a8 70000000 00000000 08000000 00000000 p...............
-  0x000050b8 50ed55ba 01001000 905c0000 00000000 P.U......\......
-  0x000050c8 02000101 48000000 a83c0000 00000000 ....H....<......
-  0x000050d8 00000000 00000000 07000100 50000000 ............P...
-  0x000050e8 00000000 00000000 11000000 00000000 ................
-  0x000050f8 00000000 00000000 00000000 00000000 ................
-  0x00005108 00000000 00000000 7f454c46 02010133 .........ELF...3
-  0x00005118 07000000 00000000 0200be00 7c000000 ............|...
-  0x00005128 00000000 00000000 003c0000 00000000 .........<......
-  0x00005138 80370000 00000000 50055000 40003800 .7......P.P.@.8.
-  0x00005148 03004000 12000100 002e7368 73747274 ..@.......shstrt
-  0x00005158 6162002e 73747274 6162002e 73796d74 ab..strtab..symt
-  0x00005168 6162002e 73796d74 61625f73 686e6478 ab..symtab_shndx
-  0x00005178 002e6e76 2e696e66 6f002e74 6578742e ..nv.info..text.
-  0x00005188 5f5a3138 61637469 6f6e4f6e 54726970 _Z18actionOnTrip
-  0x00005198 6c654761 74655036 666c6f61 74325330 leGateP6float2S0
-  0x000051a8 5f6d506d 002e6e76 2e696e66 6f2e5f5a _mPm..nv.info._Z
-  0x000051b8 31386163 74696f6e 4f6e5472 69706c65 18actionOnTriple
-  0x000051c8 47617465 5036666c 6f617432 53305f6d GateP6float2S0_m
-  0x000051d8 506d002e 6e762e73 68617265 642e5f5a Pm..nv.shared._Z
-  0x000051e8 31386163 74696f6e 4f6e5472 69706c65 18actionOnTriple
-  0x000051f8 47617465 5036666c 6f617432 53305f6d GateP6float2S0_m
-  0x00005208 506d002e 6e762e63 6f6e7374 616e7430 Pm..nv.constant0
-  0x00005218 2e5f5a31 38616374 696f6e4f 6e547269 ._Z18actionOnTri
-  0x00005228 706c6547 61746550 36666c6f 61743253 pleGateP6float2S
-  0x00005238 305f6d50 6d002e72 656c2e6e 762e636f 0_mPm..rel.nv.co
-  0x00005248 6e737461 6e74302e 5f5a3138 61637469 nstant0._Z18acti
-  0x00005258 6f6e4f6e 54726970 6c654761 74655036 onOnTripleGateP6
-  0x00005268 666c6f61 74325330 5f6d506d 002e7465 float2S0_mPm..te
-  0x00005278 78742e5f 5a313961 6374696f 6e4f6e44 xt._Z19actionOnD
-  0x00005288 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
-  0x00005298 74325330 5f6d506d 002e6e76 2e696e66 t2S0_mPm..nv.inf
-  0x000052a8 6f2e5f5a 31396163 74696f6e 4f6e446f o._Z19actionOnDo
-  0x000052b8 75626c65 51756269 74503666 6c6f6174 ubleQubitP6float
-  0x000052c8 3253305f 6d506d00 2e6e762e 73686172 2S0_mPm..nv.shar
-  0x000052d8 65642e5f 5a313961 6374696f 6e4f6e44 ed._Z19actionOnD
-  0x000052e8 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
-  0x000052f8 74325330 5f6d506d 002e6e76 2e636f6e t2S0_mPm..nv.con
-  0x00005308 7374616e 74302e5f 5a313961 6374696f stant0._Z19actio
-  0x00005318 6e4f6e44 6f75626c 65517562 69745036 nOnDoubleQubitP6
-  0x00005328 666c6f61 74325330 5f6d506d 002e7265 float2S0_mPm..re
-  0x00005338 6c2e6e76 2e636f6e 7374616e 74302e5f l.nv.constant0._
-  0x00005348 5a313961 6374696f 6e4f6e44 6f75626c Z19actionOnDoubl
-  0x00005358 65517562 69745036 666c6f61 74325330 eQubitP6float2S0
-  0x00005368 5f6d506d 002e7465 78742e5f 5a313961 _mPm..text._Z19a
-  0x00005378 6374696f 6e4f6e53 696e676c 65517562 ctionOnSingleQub
-  0x00005388 69745036 666c6f61 74325330 5f6d506d itP6float2S0_mPm
-  0x00005398 002e6e76 2e696e66 6f2e5f5a 31396163 ..nv.info._Z19ac
-  0x000053a8 74696f6e 4f6e5369 6e676c65 51756269 tionOnSingleQubi
-  0x000053b8 74503666 6c6f6174 3253305f 6d506d00 tP6float2S0_mPm.
-  0x000053c8 2e6e762e 73686172 65642e5f 5a313961 .nv.shared._Z19a
-  0x000053d8 6374696f 6e4f6e53 696e676c 65517562 ctionOnSingleQub
-  0x000053e8 69745036 666c6f61 74325330 5f6d506d itP6float2S0_mPm
-  0x000053f8 002e6e76 2e636f6e 7374616e 74302e5f ..nv.constant0._
-  0x00005408 5a313961 6374696f 6e4f6e53 696e676c Z19actionOnSingl
-  0x00005418 65517562 69745036 666c6f61 74325330 eQubitP6float2S0
-  0x00005428 5f6d506d 002e7265 6c2e6e76 2e636f6e _mPm..rel.nv.con
-  0x00005438 7374616e 74302e5f 5a313961 6374696f stant0._Z19actio
-  0x00005448 6e4f6e53 696e676c 65517562 69745036 nOnSingleQubitP6
-  0x00005458 666c6f61 74325330 5f6d506d 002e6465 float2S0_mPm..de
-  0x00005468 6275675f 6672616d 65002e72 656c2e64 bug_frame..rel.d
-  0x00005478 65627567 5f667261 6d65002e 72656c61 ebug_frame..rela
-  0x00005488 2e646562 75675f66 72616d65 002e6e76 .debug_frame..nv
-  0x00005498 2e63616c 6c677261 7068002e 6e762e70 .callgraph..nv.p
-  0x000054a8 726f746f 74797065 002e6e76 2e72656c rototype..nv.rel
-  0x000054b8 2e616374 696f6e00 002e7368 73747274 .action...shstrt
-  0x000054c8 6162002e 73747274 6162002e 73796d74 ab..strtab..symt
-  0x000054d8 6162002e 73796d74 61625f73 686e6478 ab..symtab_shndx
-  0x000054e8 002e6e76 2e696e66 6f002e74 6578742e ..nv.info..text.
-  0x000054f8 5f5a3138 61637469 6f6e4f6e 54726970 _Z18actionOnTrip
-  0x00005508 6c654761 74655036 666c6f61 74325330 leGateP6float2S0
-  0x00005518 5f6d506d 002e6e76 2e696e66 6f2e5f5a _mPm..nv.info._Z
-  0x00005528 31386163 74696f6e 4f6e5472 69706c65 18actionOnTriple
-  0x00005538 47617465 5036666c 6f617432 53305f6d GateP6float2S0_m
-  0x00005548 506d002e 6e762e73 68617265 642e5f5a Pm..nv.shared._Z
-  0x00005558 31386163 74696f6e 4f6e5472 69706c65 18actionOnTriple
-  0x00005568 47617465 5036666c 6f617432 53305f6d GateP6float2S0_m
-  0x00005578 506d002e 72656c2e 6e762e63 6f6e7374 Pm..rel.nv.const
-  0x00005588 616e7430 2e5f5a31 38616374 696f6e4f ant0._Z18actionO
-  0x00005598 6e547269 706c6547 61746550 36666c6f nTripleGateP6flo
-  0x000055a8 61743253 305f6d50 6d002e6e 762e636f at2S0_mPm..nv.co
-  0x000055b8 6e737461 6e74302e 5f5a3138 61637469 nstant0._Z18acti
-  0x000055c8 6f6e4f6e 54726970 6c654761 74655036 onOnTripleGateP6
-  0x000055d8 666c6f61 74325330 5f6d506d 002e7465 float2S0_mPm..te
-  0x000055e8 78742e5f 5a313961 6374696f 6e4f6e44 xt._Z19actionOnD
-  0x000055f8 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
-  0x00005608 74325330 5f6d506d 002e6e76 2e696e66 t2S0_mPm..nv.inf
-  0x00005618 6f2e5f5a 31396163 74696f6e 4f6e446f o._Z19actionOnDo
-  0x00005628 75626c65 51756269 74503666 6c6f6174 ubleQubitP6float
-  0x00005638 3253305f 6d506d00 2e6e762e 73686172 2S0_mPm..nv.shar
-  0x00005648 65642e5f 5a313961 6374696f 6e4f6e44 ed._Z19actionOnD
-  0x00005658 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
-  0x00005668 74325330 5f6d506d 002e7265 6c2e6e76 t2S0_mPm..rel.nv
-  0x00005678 2e636f6e 7374616e 74302e5f 5a313961 .constant0._Z19a
-  0x00005688 6374696f 6e4f6e44 6f75626c 65517562 ctionOnDoubleQub
-  0x00005698 69745036 666c6f61 74325330 5f6d506d itP6float2S0_mPm
-  0x000056a8 002e6e76 2e636f6e 7374616e 74302e5f ..nv.constant0._
-  0x000056b8 5a313961 6374696f 6e4f6e44 6f75626c Z19actionOnDoubl
-  0x000056c8 65517562 69745036 666c6f61 74325330 eQubitP6float2S0
-  0x000056d8 5f6d506d 002e7465 78742e5f 5a313961 _mPm..text._Z19a
-  0x000056e8 6374696f 6e4f6e53 696e676c 65517562 ctionOnSingleQub
-  0x000056f8 69745036 666c6f61 74325330 5f6d506d itP6float2S0_mPm
-  0x00005708 002e6e76 2e696e66 6f2e5f5a 31396163 ..nv.info._Z19ac
-  0x00005718 74696f6e 4f6e5369 6e676c65 51756269 tionOnSingleQubi
-  0x00005728 74503666 6c6f6174 3253305f 6d506d00 tP6float2S0_mPm.
-  0x00005738 2e6e762e 73686172 65642e5f 5a313961 .nv.shared._Z19a
-  0x00005748 6374696f 6e4f6e53 696e676c 65517562 ctionOnSingleQub
-  0x00005758 69745036 666c6f61 74325330 5f6d506d itP6float2S0_mPm
-  0x00005768 002e7265 6c2e6e76 2e636f6e 7374616e ..rel.nv.constan
-  0x00005778 74302e5f 5a313961 6374696f 6e4f6e53 t0._Z19actionOnS
-  0x00005788 696e676c 65517562 69745036 666c6f61 ingleQubitP6floa
-  0x00005798 74325330 5f6d506d 002e6e76 2e636f6e t2S0_mPm..nv.con
-  0x000057a8 7374616e 74302e5f 5a313961 6374696f stant0._Z19actio
-  0x000057b8 6e4f6e53 696e676c 65517562 69745036 nOnSingleQubitP6
-  0x000057c8 666c6f61 74325330 5f6d506d 002e6465 float2S0_mPm..de
-  0x000057d8 6275675f 6672616d 65002e72 656c2e64 bug_frame..rel.d
-  0x000057e8 65627567 5f667261 6d65002e 72656c61 ebug_frame..rela
-  0x000057f8 2e646562 75675f66 72616d65 002e6e76 .debug_frame..nv
-  0x00005808 2e63616c 6c677261 7068002e 6e762e70 .callgraph..nv.p
-  0x00005818 726f746f 74797065 002e6e76 2e72656c rototype..nv.rel
-  0x00005828 2e616374 696f6e00 5f5a3138 61637469 .action._Z18acti
-  0x00005838 6f6e4f6e 54726970 6c654761 74655036 onOnTripleGateP6
-  0x00005848 666c6f61 74325330 5f6d506d 005f5a31 float2S0_mPm._Z1
-  0x00005858 39616374 696f6e4f 6e446f75 626c6551 9actionOnDoubleQ
-  0x00005868 75626974 5036666c 6f617432 53305f6d ubitP6float2S0_m
-  0x00005878 506d005f 5a313961 6374696f 6e4f6e53 Pm._Z19actionOnS
-  0x00005888 696e676c 65517562 69745036 666c6f61 ingleQubitP6floa
-  0x00005898 74325330 5f6d506d 00000000 00000000 t2S0_mPm........
-  0x000058a8 00000000 00000000 00000000 00000000 ................
-  0x000058b8 00000000 00000000 32000000 03000f00 ........2.......
-  0x000058c8 00000000 00000000 00000000 00000000 ................
-  0x000058d8 f2000000 03000c00 00000000 00000000 ................
-  0x000058e8 00000000 00000000 25010000 03001000 ........%.......
-  0x000058f8 00000000 00000000 00000000 00000000 ................
-  0x00005908 e9010000 03000d00 00000000 00000000 ................
-  0x00005918 00000000 00000000 1d020000 03001100 ................
-  0x00005928 00000000 00000000 00000000 00000000 ................
-  0x00005938 e1020000 03000e00 00000000 00000000 ................
-  0x00005948 00000000 00000000 15030000 03000400 ................
+  0x00004ef8 32000000 03000400 00000000 00000000 2...............
+  0x00004f08 00000000 00000000 4e000000 03000500 ........N.......
+  0x00004f18 00000000 00000000 00000000 00000000 ................
+  0x00004f28 00000000 ffffffff 00000000 feffffff ................
+  0x00004f38 00000000 fdffffff 00000000 fcffffff ................
+  0x00004f48 73000000 00000000 00000011 25000536 s...........%..6
+  0x00004f58 00000000 00000000 00000000 00000000 ................
+  0x00004f68 00000000 00000000 00000000 00000000 ................
+  0x00004f78 00000000 00000000 00000000 00000000 ................
+  0x00004f88 00000000 00000000 00000000 00000000 ................
+  0x00004f98 01000000 03000000 00000000 00000000 ................
+  0x00004fa8 00000000 00000000 40000000 00000000 ........@.......
+  0x00004fb8 5d000000 00000000 00000000 00000000 ]...............
+  0x00004fc8 01000000 00000000 00000000 00000000 ................
+  0x00004fd8 0b000000 03000000 00000000 00000000 ................
+  0x00004fe8 00000000 00000000 9d000000 00000000 ................
+  0x00004ff8 5d000000 00000000 00000000 00000000 ]...............
+  0x00005008 01000000 00000000 00000000 00000000 ................
+  0x00005018 13000000 02000000 00000000 00000000 ................
+  0x00005028 00000000 00000000 00010000 00000000 ................
+  0x00005038 48000000 00000000 02000000 03000000 H...............
+  0x00005048 08000000 00000000 18000000 00000000 ................
+  0x00005058 32000000 01000070 00000000 00000000 2......p........
+  0x00005068 00000000 00000000 48010000 00000000 ........H.......
+  0x00005078 20000000 00000000 03000000 00000000  ...............
+  0x00005088 04000000 00000000 08000000 00000000 ................
+  0x00005098 4e000000 0b000070 00000000 00000000 N......p........
+  0x000050a8 00000000 00000000 68010000 00000000 ........h.......
+  0x000050b8 10000000 00000000 00000000 00000000 ................
+  0x000050c8 08000000 00000000 08000000 00000000 ................
+  0x000050d8 06000000 05000000 f8020000 00000000 ................
+  0x000050e8 00000000 00000000 00000000 00000000 ................
+  0x000050f8 70000000 00000000 70000000 00000000 p.......p.......
+  0x00005108 08000000 00000000 01000000 05000000 ................
+  0x00005118 f8020000 00000000 00000000 00000000 ................
+  0x00005128 00000000 00000000 70000000 00000000 ........p.......
+  0x00005138 70000000 00000000 08000000 00000000 p...............
+  0x00005148 50ed55ba 01001000 905c0000 00000000 P.U......\......
+  0x00005158 02000101 48000000 a83c0000 00000000 ....H....<......
+  0x00005168 00000000 00000000 07000100 50000000 ............P...
+  0x00005178 00000000 00000000 11000000 00000000 ................
+  0x00005188 00000000 00000000 00000000 00000000 ................
+  0x00005198 00000000 00000000 7f454c46 02010133 .........ELF...3
+  0x000051a8 07000000 00000000 0200be00 7c000000 ............|...
+  0x000051b8 00000000 00000000 003c0000 00000000 .........<......
+  0x000051c8 80370000 00000000 50055000 40003800 .7......P.P.@.8.
+  0x000051d8 03004000 12000100 002e7368 73747274 ..@.......shstrt
+  0x000051e8 6162002e 73747274 6162002e 73796d74 ab..strtab..symt
+  0x000051f8 6162002e 73796d74 61625f73 686e6478 ab..symtab_shndx
+  0x00005208 002e6e76 2e696e66 6f002e74 6578742e ..nv.info..text.
+  0x00005218 5f5a3138 61637469 6f6e4f6e 54726970 _Z18actionOnTrip
+  0x00005228 6c654761 74655036 666c6f61 74325330 leGateP6float2S0
+  0x00005238 5f6d506d 002e6e76 2e696e66 6f2e5f5a _mPm..nv.info._Z
+  0x00005248 31386163 74696f6e 4f6e5472 69706c65 18actionOnTriple
+  0x00005258 47617465 5036666c 6f617432 53305f6d GateP6float2S0_m
+  0x00005268 506d002e 6e762e73 68617265 642e5f5a Pm..nv.shared._Z
+  0x00005278 31386163 74696f6e 4f6e5472 69706c65 18actionOnTriple
+  0x00005288 47617465 5036666c 6f617432 53305f6d GateP6float2S0_m
+  0x00005298 506d002e 6e762e63 6f6e7374 616e7430 Pm..nv.constant0
+  0x000052a8 2e5f5a31 38616374 696f6e4f 6e547269 ._Z18actionOnTri
+  0x000052b8 706c6547 61746550 36666c6f 61743253 pleGateP6float2S
+  0x000052c8 305f6d50 6d002e72 656c2e6e 762e636f 0_mPm..rel.nv.co
+  0x000052d8 6e737461 6e74302e 5f5a3138 61637469 nstant0._Z18acti
+  0x000052e8 6f6e4f6e 54726970 6c654761 74655036 onOnTripleGateP6
+  0x000052f8 666c6f61 74325330 5f6d506d 002e7465 float2S0_mPm..te
+  0x00005308 78742e5f 5a313961 6374696f 6e4f6e44 xt._Z19actionOnD
+  0x00005318 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
+  0x00005328 74325330 5f6d506d 002e6e76 2e696e66 t2S0_mPm..nv.inf
+  0x00005338 6f2e5f5a 31396163 74696f6e 4f6e446f o._Z19actionOnDo
+  0x00005348 75626c65 51756269 74503666 6c6f6174 ubleQubitP6float
+  0x00005358 3253305f 6d506d00 2e6e762e 73686172 2S0_mPm..nv.shar
+  0x00005368 65642e5f 5a313961 6374696f 6e4f6e44 ed._Z19actionOnD
+  0x00005378 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
+  0x00005388 74325330 5f6d506d 002e6e76 2e636f6e t2S0_mPm..nv.con
+  0x00005398 7374616e 74302e5f 5a313961 6374696f stant0._Z19actio
+  0x000053a8 6e4f6e44 6f75626c 65517562 69745036 nOnDoubleQubitP6
+  0x000053b8 666c6f61 74325330 5f6d506d 002e7265 float2S0_mPm..re
+  0x000053c8 6c2e6e76 2e636f6e 7374616e 74302e5f l.nv.constant0._
+  0x000053d8 5a313961 6374696f 6e4f6e44 6f75626c Z19actionOnDoubl
+  0x000053e8 65517562 69745036 666c6f61 74325330 eQubitP6float2S0
+  0x000053f8 5f6d506d 002e7465 78742e5f 5a313961 _mPm..text._Z19a
+  0x00005408 6374696f 6e4f6e53 696e676c 65517562 ctionOnSingleQub
+  0x00005418 69745036 666c6f61 74325330 5f6d506d itP6float2S0_mPm
+  0x00005428 002e6e76 2e696e66 6f2e5f5a 31396163 ..nv.info._Z19ac
+  0x00005438 74696f6e 4f6e5369 6e676c65 51756269 tionOnSingleQubi
+  0x00005448 74503666 6c6f6174 3253305f 6d506d00 tP6float2S0_mPm.
+  0x00005458 2e6e762e 73686172 65642e5f 5a313961 .nv.shared._Z19a
+  0x00005468 6374696f 6e4f6e53 696e676c 65517562 ctionOnSingleQub
+  0x00005478 69745036 666c6f61 74325330 5f6d506d itP6float2S0_mPm
+  0x00005488 002e6e76 2e636f6e 7374616e 74302e5f ..nv.constant0._
+  0x00005498 5a313961 6374696f 6e4f6e53 696e676c Z19actionOnSingl
+  0x000054a8 65517562 69745036 666c6f61 74325330 eQubitP6float2S0
+  0x000054b8 5f6d506d 002e7265 6c2e6e76 2e636f6e _mPm..rel.nv.con
+  0x000054c8 7374616e 74302e5f 5a313961 6374696f stant0._Z19actio
+  0x000054d8 6e4f6e53 696e676c 65517562 69745036 nOnSingleQubitP6
+  0x000054e8 666c6f61 74325330 5f6d506d 002e6465 float2S0_mPm..de
+  0x000054f8 6275675f 6672616d 65002e72 656c2e64 bug_frame..rel.d
+  0x00005508 65627567 5f667261 6d65002e 72656c61 ebug_frame..rela
+  0x00005518 2e646562 75675f66 72616d65 002e6e76 .debug_frame..nv
+  0x00005528 2e63616c 6c677261 7068002e 6e762e70 .callgraph..nv.p
+  0x00005538 726f746f 74797065 002e6e76 2e72656c rototype..nv.rel
+  0x00005548 2e616374 696f6e00 002e7368 73747274 .action...shstrt
+  0x00005558 6162002e 73747274 6162002e 73796d74 ab..strtab..symt
+  0x00005568 6162002e 73796d74 61625f73 686e6478 ab..symtab_shndx
+  0x00005578 002e6e76 2e696e66 6f002e74 6578742e ..nv.info..text.
+  0x00005588 5f5a3138 61637469 6f6e4f6e 54726970 _Z18actionOnTrip
+  0x00005598 6c654761 74655036 666c6f61 74325330 leGateP6float2S0
+  0x000055a8 5f6d506d 002e6e76 2e696e66 6f2e5f5a _mPm..nv.info._Z
+  0x000055b8 31386163 74696f6e 4f6e5472 69706c65 18actionOnTriple
+  0x000055c8 47617465 5036666c 6f617432 53305f6d GateP6float2S0_m
+  0x000055d8 506d002e 6e762e73 68617265 642e5f5a Pm..nv.shared._Z
+  0x000055e8 31386163 74696f6e 4f6e5472 69706c65 18actionOnTriple
+  0x000055f8 47617465 5036666c 6f617432 53305f6d GateP6float2S0_m
+  0x00005608 506d002e 72656c2e 6e762e63 6f6e7374 Pm..rel.nv.const
+  0x00005618 616e7430 2e5f5a31 38616374 696f6e4f ant0._Z18actionO
+  0x00005628 6e547269 706c6547 61746550 36666c6f nTripleGateP6flo
+  0x00005638 61743253 305f6d50 6d002e6e 762e636f at2S0_mPm..nv.co
+  0x00005648 6e737461 6e74302e 5f5a3138 61637469 nstant0._Z18acti
+  0x00005658 6f6e4f6e 54726970 6c654761 74655036 onOnTripleGateP6
+  0x00005668 666c6f61 74325330 5f6d506d 002e7465 float2S0_mPm..te
+  0x00005678 78742e5f 5a313961 6374696f 6e4f6e44 xt._Z19actionOnD
+  0x00005688 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
+  0x00005698 74325330 5f6d506d 002e6e76 2e696e66 t2S0_mPm..nv.inf
+  0x000056a8 6f2e5f5a 31396163 74696f6e 4f6e446f o._Z19actionOnDo
+  0x000056b8 75626c65 51756269 74503666 6c6f6174 ubleQubitP6float
+  0x000056c8 3253305f 6d506d00 2e6e762e 73686172 2S0_mPm..nv.shar
+  0x000056d8 65642e5f 5a313961 6374696f 6e4f6e44 ed._Z19actionOnD
+  0x000056e8 6f75626c 65517562 69745036 666c6f61 oubleQubitP6floa
+  0x000056f8 74325330 5f6d506d 002e7265 6c2e6e76 t2S0_mPm..rel.nv
+  0x00005708 2e636f6e 7374616e 74302e5f 5a313961 .constant0._Z19a
+  0x00005718 6374696f 6e4f6e44 6f75626c 65517562 ctionOnDoubleQub
+  0x00005728 69745036 666c6f61 74325330 5f6d506d itP6float2S0_mPm
+  0x00005738 002e6e76 2e636f6e 7374616e 74302e5f ..nv.constant0._
+  0x00005748 5a313961 6374696f 6e4f6e44 6f75626c Z19actionOnDoubl
+  0x00005758 65517562 69745036 666c6f61 74325330 eQubitP6float2S0
+  0x00005768 5f6d506d 002e7465 78742e5f 5a313961 _mPm..text._Z19a
+  0x00005778 6374696f 6e4f6e53 696e676c 65517562 ctionOnSingleQub
+  0x00005788 69745036 666c6f61 74325330 5f6d506d itP6float2S0_mPm
+  0x00005798 002e6e76 2e696e66 6f2e5f5a 31396163 ..nv.info._Z19ac
+  0x000057a8 74696f6e 4f6e5369 6e676c65 51756269 tionOnSingleQubi
+  0x000057b8 74503666 6c6f6174 3253305f 6d506d00 tP6float2S0_mPm.
+  0x000057c8 2e6e762e 73686172 65642e5f 5a313961 .nv.shared._Z19a
+  0x000057d8 6374696f 6e4f6e53 696e676c 65517562 ctionOnSingleQub
+  0x000057e8 69745036 666c6f61 74325330 5f6d506d itP6float2S0_mPm
+  0x000057f8 002e7265 6c2e6e76 2e636f6e 7374616e ..rel.nv.constan
+  0x00005808 74302e5f 5a313961 6374696f 6e4f6e53 t0._Z19actionOnS
+  0x00005818 696e676c 65517562 69745036 666c6f61 ingleQubitP6floa
+  0x00005828 74325330 5f6d506d 002e6e76 2e636f6e t2S0_mPm..nv.con
+  0x00005838 7374616e 74302e5f 5a313961 6374696f stant0._Z19actio
+  0x00005848 6e4f6e53 696e676c 65517562 69745036 nOnSingleQubitP6
+  0x00005858 666c6f61 74325330 5f6d506d 002e6465 float2S0_mPm..de
+  0x00005868 6275675f 6672616d 65002e72 656c2e64 bug_frame..rel.d
+  0x00005878 65627567 5f667261 6d65002e 72656c61 ebug_frame..rela
+  0x00005888 2e646562 75675f66 72616d65 002e6e76 .debug_frame..nv
+  0x00005898 2e63616c 6c677261 7068002e 6e762e70 .callgraph..nv.p
+  0x000058a8 726f746f 74797065 002e6e76 2e72656c rototype..nv.rel
+  0x000058b8 2e616374 696f6e00 5f5a3138 61637469 .action._Z18acti
+  0x000058c8 6f6e4f6e 54726970 6c654761 74655036 onOnTripleGateP6
+  0x000058d8 666c6f61 74325330 5f6d506d 005f5a31 float2S0_mPm._Z1
+  0x000058e8 39616374 696f6e4f 6e446f75 626c6551 9actionOnDoubleQ
+  0x000058f8 75626974 5036666c 6f617432 53305f6d ubitP6float2S0_m
+  0x00005908 506d005f 5a313961 6374696f 6e4f6e53 Pm._Z19actionOnS
+  0x00005918 696e676c 65517562 69745036 666c6f61 ingleQubitP6floa
+  0x00005928 74325330 5f6d506d 00000000 00000000 t2S0_mPm........
+  0x00005938 00000000 00000000 00000000 00000000 ................
+  0x00005948 00000000 00000000 32000000 03000f00 ........2.......
   0x00005958 00000000 00000000 00000000 00000000 ................
-  0x00005968 45030000 03000900 00000000 00000000 E...............
-  0x00005978 00000000 00000000 61030000 03000a00 ........a.......
+  0x00005968 f2000000 03000c00 00000000 00000000 ................
+  0x00005978 00000000 00000000 25010000 03001000 ........%.......
   0x00005988 00000000 00000000 00000000 00000000 ................
-  0x00005998 70030000 12100f00 00000000 00000000 p...............
-  0x000059a8 001a0000 00000000 95030000 12101000 ................
-  0x000059b8 00000000 00000000 80080000 00000000 ................
-  0x000059c8 bb030000 12101100 00000000 00000000 ................
-  0x000059d8 00040000 00000000 ffffffff 24000000 ............$...
-  0x000059e8 00000000 ffffffff ffffffff 0300047c ...............|
-  0x000059f8 ffffffff 0f0c8180 80280008 ff818028 .........(.....(
-  0x00005a08 08818080 28000000 ffffffff 34000000 ....(.......4...
+  0x00005998 e9010000 03000d00 00000000 00000000 ................
+  0x000059a8 00000000 00000000 1d020000 03001100 ................
+  0x000059b8 00000000 00000000 00000000 00000000 ................
+  0x000059c8 e1020000 03000e00 00000000 00000000 ................
+  0x000059d8 00000000 00000000 15030000 03000400 ................
+  0x000059e8 00000000 00000000 00000000 00000000 ................
+  0x000059f8 45030000 03000900 00000000 00000000 E...............
+  0x00005a08 00000000 00000000 61030000 03000a00 ........a.......
   0x00005a18 00000000 00000000 00000000 00000000 ................
-  0x00005a28 00000000 001a0000 00000000 04040000 ................
-  0x00005a38 0004e000 00000c81 80802800 046c0500 ..........(..l..
-  0x00005a48 00000000 00000000 ffffffff 24000000 ............$...
-  0x00005a58 00000000 ffffffff ffffffff 0300047c ...............|
-  0x00005a68 ffffffff 0f0c8180 80280008 ff818028 .........(.....(
-  0x00005a78 08818080 28000000 ffffffff 34000000 ....(.......4...
-  0x00005a88 00000000 70000000 00000000 00000000 ....p...........
-  0x00005a98 00000000 80080000 00000000 04040000 ................
-  0x00005aa8 00046800 00000c81 80802800 04800100 ..h.......(.....
-  0x00005ab8 00000000 00000000 ffffffff 24000000 ............$...
-  0x00005ac8 00000000 ffffffff ffffffff 0300047c ...............|
-  0x00005ad8 ffffffff 0f0c8180 80280008 ff818028 .........(.....(
-  0x00005ae8 08818080 28000000 ffffffff 34000000 ....(.......4...
-  0x00005af8 00000000 e0000000 00000000 00000000 ................
-  0x00005b08 00000000 00040000 00000000 04040000 ................
-  0x00005b18 00044000 00000c81 80802800 04780000 ..@.......(..x..
-  0x00005b28 00000000 00000000 042f0800 0c000000 ........./......
-  0x00005b38 18000000 04120800 0c000000 00000000 ................
-  0x00005b48 04110800 0c000000 00000000 042f0800 ............./..
-  0x00005b58 0b000000 22000000 04120800 0b000000 ...."...........
-  0x00005b68 00000000 04110800 0b000000 00000000 ................
-  0x00005b78 042f0800 0a000000 34000000 04120800 ./......4.......
-  0x00005b88 0a000000 00000000 04110800 0a000000 ................
-  0x00005b98 00000000 04120800 0a000000 00000000 ................
-  0x00005ba8 04120800 0b000000 00000000 04120800 ................
-  0x00005bb8 0c000000 00000000 04370400 7c000000 .........7..|...
-  0x00005bc8 01350000 040a0800 02000000 60012000 .5..........`. .
-  0x00005bd8 03192000 04170c00 00000000 03001800 .. .............
-  0x00005be8 00f02100 04170c00 00000000 02001000 ..!.............
-  0x00005bf8 00f02100 04170c00 00000000 01000800 ..!.............
-  0x00005c08 00f02100 04170c00 00000000 00000000 ..!.............
-  0x00005c18 00f02100 031bff00 041c0800 80030000 ..!.............
-  0x00005c28 40190000 04370400 7c000000 01350000 @....7..|....5..
-  0x00005c38 040a0800 04000000 60012000 03192000 ........`. ... .
-  0x00005c48 04170c00 00000000 03001800 00f02100 ..............!.
-  0x00005c58 04170c00 00000000 02001000 00f02100 ..............!.
-  0x00005c68 04170c00 00000000 01000800 00f02100 ..............!.
-  0x00005c78 04170c00 00000000 00000000 00f02100 ..............!.
-  0x00005c88 031bff00 041c0800 a0010000 b0070000 ................
-  0x00005c98 04370400 7c000000 01350000 040a0800 .7..|....5......
-  0x00005ca8 06000000 60012000 03192000 04170c00 ....`. ... .....
-  0x00005cb8 00000000 03001800 00f02100 04170c00 ..........!.....
-  0x00005cc8 00000000 02001000 00f02100 04170c00 ..........!.....
-  0x00005cd8 00000000 01000800 00f02100 04170c00 ..........!.....
-  0x00005ce8 00000000 00000000 00f02100 031bff00 ..........!.....
-  0x00005cf8 041c0800 00010000 f0020000 00000000 ................
-  0x00005d08 ffffffff 00000000 feffffff 00000000 ................
-  0x00005d18 fdffffff 00000000 fcffffff 00000000 ................
-  0x00005d28 73000000 00000000 00000011 25000536 s...........%..6
-  0x00005d38 24010000 00000000 02000000 0c000000 $...............
-  0x00005d48 b4000000 00000000 02000000 0b000000 ................
-  0x00005d58 44000000 00000000 02000000 0a000000 D...............
-  0x00005d68 00000000 00000000 00000000 00000000 ................
-  0x00005d78 00000000 00000000 00000000 00000000 ................
-  0x00005d88 00000000 00000000 00000000 00000000 ................
-  0x00005d98 00000000 00000000 00000000 00000000 ................
-  0x00005da8 00000000 00000000 00000000 00000000 ................
-  0x00005db8 00000000 00000000 00000000 00000000 ................
-  0x00005dc8 00000000 00000000 00000000 00000000 ................
-  0x00005dd8 00000000 00000000 00000000 00000000 ................
-  0x00005de8 00000000 00000000 00000000 00000000 ................
+  0x00005a28 70030000 12100f00 00000000 00000000 p...............
+  0x00005a38 001a0000 00000000 95030000 12101000 ................
+  0x00005a48 00000000 00000000 80080000 00000000 ................
+  0x00005a58 bb030000 12101100 00000000 00000000 ................
+  0x00005a68 00040000 00000000 ffffffff 24000000 ............$...
+  0x00005a78 00000000 ffffffff ffffffff 0300047c ...............|
+  0x00005a88 ffffffff 0f0c8180 80280008 ff818028 .........(.....(
+  0x00005a98 08818080 28000000 ffffffff 34000000 ....(.......4...
+  0x00005aa8 00000000 00000000 00000000 00000000 ................
+  0x00005ab8 00000000 001a0000 00000000 04040000 ................
+  0x00005ac8 0004e000 00000c81 80802800 046c0500 ..........(..l..
+  0x00005ad8 00000000 00000000 ffffffff 24000000 ............$...
+  0x00005ae8 00000000 ffffffff ffffffff 0300047c ...............|
+  0x00005af8 ffffffff 0f0c8180 80280008 ff818028 .........(.....(
+  0x00005b08 08818080 28000000 ffffffff 34000000 ....(.......4...
+  0x00005b18 00000000 70000000 00000000 00000000 ....p...........
+  0x00005b28 00000000 80080000 00000000 04040000 ................
+  0x00005b38 00046800 00000c81 80802800 04800100 ..h.......(.....
+  0x00005b48 00000000 00000000 ffffffff 24000000 ............$...
+  0x00005b58 00000000 ffffffff ffffffff 0300047c ...............|
+  0x00005b68 ffffffff 0f0c8180 80280008 ff818028 .........(.....(
+  0x00005b78 08818080 28000000 ffffffff 34000000 ....(.......4...
+  0x00005b88 00000000 e0000000 00000000 00000000 ................
+  0x00005b98 00000000 00040000 00000000 04040000 ................
+  0x00005ba8 00044000 00000c81 80802800 04780000 ..@.......(..x..
+  0x00005bb8 00000000 00000000 042f0800 0c000000 ........./......
+  0x00005bc8 18000000 04120800 0c000000 00000000 ................
+  0x00005bd8 04110800 0c000000 00000000 042f0800 ............./..
+  0x00005be8 0b000000 22000000 04120800 0b000000 ...."...........
+  0x00005bf8 00000000 04110800 0b000000 00000000 ................
+  0x00005c08 042f0800 0a000000 34000000 04120800 ./......4.......
+  0x00005c18 0a000000 00000000 04110800 0a000000 ................
+  0x00005c28 00000000 04120800 0a000000 00000000 ................
+  0x00005c38 04120800 0b000000 00000000 04120800 ................
+  0x00005c48 0c000000 00000000 04370400 7c000000 .........7..|...
+  0x00005c58 01350000 040a0800 02000000 60012000 .5..........`. .
+  0x00005c68 03192000 04170c00 00000000 03001800 .. .............
+  0x00005c78 00f02100 04170c00 00000000 02001000 ..!.............
+  0x00005c88 00f02100 04170c00 00000000 01000800 ..!.............
+  0x00005c98 00f02100 04170c00 00000000 00000000 ..!.............
+  0x00005ca8 00f02100 031bff00 041c0800 80030000 ..!.............
+  0x00005cb8 40190000 04370400 7c000000 01350000 @....7..|....5..
+  0x00005cc8 040a0800 04000000 60012000 03192000 ........`. ... .
+  0x00005cd8 04170c00 00000000 03001800 00f02100 ..............!.
+  0x00005ce8 04170c00 00000000 02001000 00f02100 ..............!.
+  0x00005cf8 04170c00 00000000 01000800 00f02100 ..............!.
+  0x00005d08 04170c00 00000000 00000000 00f02100 ..............!.
+  0x00005d18 031bff00 041c0800 a0010000 b0070000 ................
+  0x00005d28 04370400 7c000000 01350000 040a0800 .7..|....5......
+  0x00005d38 06000000 60012000 03192000 04170c00 ....`. ... .....
+  0x00005d48 00000000 03001800 00f02100 04170c00 ..........!.....
+  0x00005d58 00000000 02001000 00f02100 04170c00 ..........!.....
+  0x00005d68 00000000 01000800 00f02100 04170c00 ..........!.....
+  0x00005d78 00000000 00000000 00f02100 031bff00 ..........!.....
+  0x00005d88 041c0800 00010000 f0020000 00000000 ................
+  0x00005d98 ffffffff 00000000 feffffff 00000000 ................
+  0x00005da8 fdffffff 00000000 fcffffff 00000000 ................
+  0x00005db8 73000000 00000000 00000011 25000536 s...........%..6
+  0x00005dc8 24010000 00000000 02000000 0c000000 $...............
+  0x00005dd8 b4000000 00000000 02000000 0b000000 ................
+  0x00005de8 44000000 00000000 02000000 0a000000 D...............
   0x00005df8 00000000 00000000 00000000 00000000 ................
   0x00005e08 00000000 00000000 00000000 00000000 ................
   0x00005e18 00000000 00000000 00000000 00000000 ................
   0x00005e28 00000000 00000000 00000000 00000000 ................
   0x00005e38 00000000 00000000 00000000 00000000 ................
   0x00005e48 00000000 00000000 00000000 00000000 ................
   0x00005e58 00000000 00000000 00000000 00000000 ................
@@ -333,1213 +324,1222 @@
   0x00006198 00000000 00000000 00000000 00000000 ................
   0x000061a8 00000000 00000000 00000000 00000000 ................
   0x000061b8 00000000 00000000 00000000 00000000 ................
   0x000061c8 00000000 00000000 00000000 00000000 ................
   0x000061d8 00000000 00000000 00000000 00000000 ................
   0x000061e8 00000000 00000000 00000000 00000000 ................
   0x000061f8 00000000 00000000 00000000 00000000 ................
-  0x00006208 00000000 00000000 027a0100 000a0000 .........z......
-  0x00006218 000f0000 00e40f00 027a0400 005e0000 .........z...^..
-  0x00006228 000f0000 00e20f00 b97a0600 00460000 .........z...F..
-  0x00006238 000a0000 00e20f00 027a0500 005f0000 .........z..._..
-  0x00006248 000f0000 00ca0f00 81790304 06080000 .........y......
-  0x00006258 00191e0c 00a80e00 81790604 06000000 .........y......
-  0x00006268 00191e0c 00e80e00 81790804 06100000 .........y......
-  0x00006278 00191e0c 00220f00 b97a0400 00000000 ....."...z......
-  0x00006288 00080000 00e40f00 9978043f 01000000 .........x.?....
-  0x00006298 04160108 00e20f00 19790b00 00000000 .........y......
-  0x000062a8 00250000 00280e00 19790a00 00000000 .%...(...y......
-  0x000062b8 00210000 00240e00 247a0b0b 00000000 .!...$..$z......
-  0x000062c8 0a028e07 00ca1f00 1272020b 03000000 .........r......
-  0x000062d8 fffc8e07 00e44f0c 1272100b 06000000 ......O..r......
-  0x000062e8 fffc8e07 00e48f04 10720006 03000000 .........r......
-  0x000062f8 ffe0ff07 00e40f00 0c72000b 02000000 .........r......
-  0x00006308 7052f003 00e40f04 1272070b 00000000 pR.......r......
-  0x00006318 fffc8e07 00e40f04 0c72000b 10000000 .........r......
-  0x00006328 70527000 00c40f00 10720c06 08000000 pRp......r......
-  0x00006338 ffe0ff07 00e40f09 1272000b 08000000 .........r......
-  0x00006348 fffc8e07 00e40f0c 0c72000b 07000000 .........r......
-  0x00006358 70527000 00e40f00 10720303 08000000 pRp......r......
-  0x00006368 ffe0ff07 00e40f00 1272080b 0c000000 .........r......
-  0x00006378 fffc8e07 00e40f04 0c72000b 00000000 .........r......
-  0x00006388 70527000 00c40f00 10720606 03000000 pRp......r......
-  0x00006398 ffe0ff07 00e40f08 1272040b 03000000 .........r......
-  0x000063a8 fffc8e07 00e40f04 0c72000b 08000000 .........r......
-  0x000063b8 70527000 00e40f04 1272050b 06000000 pRp......r......
-  0x000063c8 fffc8e07 00e40f04 0c72000b 04000000 .........r......
-  0x000063d8 70527000 00e40f00 197803ff 1f000000 pRp......x......
-  0x000063e8 0b140100 00c40f00 0c72000b 05000000 .........r......
-  0x000063f8 70527000 00c80f00 0c720010 02000000 pRp......r......
-  0x00006408 70527000 00c80f00 0c720010 07000000 pRp......r......
-  0x00006418 70527000 00c80f00 0c720010 00000000 pRp......r......
-  0x00006428 70527000 00c80f00 0c720010 08000000 pRp......r......
-  0x00006438 70527000 00c80f00 0c720010 04000000 pRp......r......
-  0x00006448 70527000 00c80f00 0c720010 05000000 pRp......r......
-  0x00006458 70527000 00c80f00 0c720002 07000000 pRp......r......
-  0x00006468 70527000 00c80f00 0c720002 00000000 pRp......r......
-  0x00006478 70527000 00c80f00 0c720002 08000000 pRp......r......
-  0x00006488 70527000 00c80f00 0c720002 04000000 pRp......r......
-  0x00006498 70527000 00c80f00 0c720002 05000000 pRp......r......
-  0x000064a8 70527000 00c80f00 0c720007 00000000 pRp......r......
-  0x000064b8 70527000 00c80f00 0c720007 08000000 pRp......r......
-  0x000064c8 70527000 00c80f00 0c720007 04000000 pRp......r......
-  0x000064d8 70527000 00c80f00 0c720007 05000000 pRp......r......
-  0x000064e8 70527000 00c80f00 0c720000 08000000 pRp......r......
-  0x000064f8 70527000 00c80f00 0c720000 04000000 pRp......r......
-  0x00006508 70527000 00c80f00 0c720000 05000000 pRp......r......
-  0x00006518 70527200 00e40f08 0c7a000b 005c0000 pRr......z...\..
-  0x00006528 7060f003 00e40f00 0c720008 04000000 p`.......r......
-  0x00006538 7052f200 00e40f04 0c7a0003 005d0000 pR.......z...]..
-  0x00006548 0061f003 00e40f00 0c720008 05000000 .a.......r......
-  0x00006558 7052f200 00e40f00 0c7c000a 04000000 pR.......|......
-  0x00006568 7010700c 00c40f00 0c720004 05000000 p.p......r......
-  0x00006578 7052f200 00c80f00 1c780000 00000000 pR.......x......
-  0x00006588 70307000 00da0f00 4d890000 00000000 p0p.....M.......
-  0x00006598 00008003 00ea0f00 357403ff 08000000 ........5t......
-  0x000065a8 ff010000 00e20f00 027a2800 005a0000 .........z(..Z..
-  0x000065b8 000f0000 00e40f00 027a2900 005b0000 .........z)..[..
-  0x000065c8 000f0000 00ca0f00 81792428 06400000 .........y$(.@..
-  0x000065d8 001b1e0c 00a40e00 25760a0b 00580000 ........%v...X..
-  0x000065e8 03028e07 00e40f08 81792228 06800000 .........y"(....
-  0x000065f8 001b1e0c 00e80e00 81791e0a 06000000 .........y......
-  0x00006608 001b1e0c 00a80e00 81791228 06c00000 .........y.(....
-  0x00006618 001b1e0c 00280f00 81791a28 06000100 .....(...y.(....
-  0x00006628 001b1e0c 00680f00 81790c28 06400100 .....h...y.(.@..
-  0x00006638 001b1e0c 00280f00 81792628 06000000 .....(...y&(....
-  0x00006648 001b1e0c 00280f00 81792028 06c00100 .....(...y (....
-  0x00006658 001b1e0c 00680f00 81791628 06800100 .....h...y.(....
-  0x00006668 001b1e0c 00620f00 25761010 00580000 .....b..%v...X..
-  0x00006678 03028e07 00c60f00 81791828 06080000 .........y.(....
-  0x00006688 001b1e0c 00680f00 81790e10 06000000 .....h...y......
-  0x00006698 001b1e0c 00680f00 81791428 06880000 .....h...y.(....
-  0x000066a8 001b1e0c 00680f00 81791c28 06480000 .....h...y.(.H..
-  0x000066b8 001b1e0c 00620f00 2072091f 25000000 .....b.. r..%...
-  0x000066c8 00004000 00c44f00 2072061e 25000000 ..@...O. r..%...
-  0x000066d8 00004000 00e40f04 2372091e 24000000 ..@.....#r..$...
-  0x000066e8 09080000 00e40f0c 2372061f 24000000 ........#r..$...
-  0x000066f8 06000000 00e40f04 2072251f 23000000 ........ r%.#...
-  0x00006708 00004000 00e48f08 2072241e 23000000 ..@..... r$.#...
-  0x00006718 00004000 00e40f04 2372231e 22000000 ..@.....#r#."...
-  0x00006728 25080000 00c40f00 2372221f 22000000 %.......#r"."...
-  0x00006738 24000000 00e40f04 2072251f 13000000 $....... r%.....
-  0x00006748 00004000 00e40f0d 2072241e 13000000 ..@..... r$.....
-  0x00006758 00004000 00e40f04 2372131e 12000000 ..@.....#r......
-  0x00006768 25080000 00e40f08 2372121f 12000000 %.......#r......
-  0x00006778 24000000 00e40f04 2072251f 1b000000 $....... r%.....
-  0x00006788 00004000 00c40f02 2072241e 1b000000 ..@..... r$.....
-  0x00006798 00004000 00e40f04 23721b1e 1a000000 ..@.....#r......
-  0x000067a8 25080000 00e40f0c 23721a1f 1a000000 %.......#r......
-  0x000067b8 24000000 00e40f04 2072251f 0d000000 $....... r%.....
-  0x000067c8 00004000 00e40f08 2072241e 0d000000 ..@..... r$.....
-  0x000067d8 00004000 00e40f00 20722b27 1f000000 ..@..... r+'....
-  0x000067e8 00004000 00c40f00 20722a27 1e000000 ..@..... r*'....
-  0x000067f8 00004000 00e40f00 2372251e 0c000000 ..@.....#r%.....
-  0x00006808 25080000 00e40f0c 2372241f 0c000000 %.......#r$.....
-  0x00006818 24000000 00e40f04 20720d1f 21000000 $....... r..!...
-  0x00006828 00004000 00e40f08 20720c1e 21000000 ..@..... r..!...
-  0x00006838 00004000 00e40f00 23722b26 1e000000 ..@.....#r+&....
-  0x00006848 2b080000 00c40f00 23722a26 1f000000 +.......#r*&....
-  0x00006858 2a000000 00e40f00 2072271f 17000000 *....... r'.....
-  0x00006868 00004000 00e40f0c 2072261e 17000000 ..@..... r&.....
-  0x00006878 00004000 00e40f04 2372211e 20000000 ..@.....#r!. ...
-  0x00006888 0d080000 00e40f0c 2372201f 20000000 ........#r . ...
-  0x00006898 0c000000 00e40f04 2372271e 16000000 ........#r'.....
-  0x000068a8 27080000 00e20f08 81790c28 06c80000 '........y.(....
-  0x000068b8 001b1e0c 00a20e00 2372261f 16000000 ........#r&.....
-  0x000068c8 26000000 00c60f00 81791628 06080100 &........y.(....
-  0x000068d8 001b1e0c 00e20e00 23721e18 0e000000 ........#r......
-  0x000068e8 2b000000 00e40f0c 23722b18 0f000000 +.......#r+.....
-  0x000068f8 2a000000 00e40f08 23722a19 0f000000 *.......#r*.....
-  0x00006908 1e010000 00e40f04 23722b19 0e000000 ........#r+.....
-  0x00006918 2b000000 00e20f00 81791e28 06880100 +........y.(....
-  0x00006928 001b1e0c 00280f00 81791828 06480100 .....(...y.(.H..
-  0x00006938 001b1e0c 00620f00 23722e0e 14000000 .....b..#r......
-  0x00006948 23000000 00c40f00 23722c0e 1c000000 #.......#r,.....
-  0x00006958 09000000 00e40f08 23721c0f 1c000000 ........#r......
-  0x00006968 06000000 00e40f04 2372220f 14000000 ........#r".....
-  0x00006978 22000000 00e40f04 2372090f 15000080 ".......#r......
-  0x00006988 2e000000 00e40f00 25762e02 00580000 ........%v...X..
-  0x00006998 03028e07 00c80f00 2372060f 1d000080 ........#r......
-  0x000069a8 2c000000 00e40f0c 23722c0e 1d000000 ,.......#r,.....
-  0x000069b8 1c000000 00e40f04 81791c28 06c80100 .........y.(....
-  0x000069c8 001b1e0c 00220f00 2372220e 15000000 ....."..#r".....
-  0x000069d8 22000000 00e40f04 2372140e 0c000000 ".......#r......
-  0x000069e8 13000000 00e44f0c 2372120f 0c000000 ......O.#r......
-  0x000069f8 12000000 00e40f00 23720c0e 16000000 ........#r......
-  0x00006a08 1b000000 00c48f00 2372160f 16000000 ........#r......
-  0x00006a18 1a000000 00e40f04 23721b0f 0d000080 ........#r......
-  0x00006a28 14000000 00e40f0c 23721a0e 0d000000 ........#r......
-  0x00006a38 12000000 00e20f00 81791428 06500000 .........y.(.P..
-  0x00006a48 001b1e0c 00a20e00 2372230f 17000080 ........#r#.....
-  0x00006a58 0c000000 00c60f00 81790c28 06100000 .........y.(....
-  0x00006a68 001b1e0c 00e80e00 8179122e 06000000 .........y......
-  0x00006a78 001b1e0c 00e20e00 2372020e 17000000 ........#r......
-  0x00006a88 16000000 00e40f04 2372160e 18000000 ........#r......
-  0x00006a98 25000000 00e40f0e 2372240f 18000000 %.......#r$.....
-  0x00006aa8 24000000 00e40f00 2372180e 1e000000 $.......#r......
-  0x00006ab8 27000000 00c40f01 2372260f 1e000000 '.......#r&.....
-  0x00006ac8 26000000 00e40f04 2372250f 19000080 &.......#r%.....
-  0x00006ad8 16000000 00e40f0c 23721e0e 19000000 ........#r......
-  0x00006ae8 24000000 00e20f00 81791628 06900000 $........y.(....
-  0x00006af8 001b1e0c 00220f00 2372270f 1f000080 ....."..#r'.....
-  0x00006b08 18000000 00c60f00 81791828 06d00000 .........y.(....
-  0x00006b18 001b1e0c 00620f00 2372240e 1c000000 .....b..#r$.....
-  0x00006b28 21000000 00e40f0c 2372200f 1c000000 !.......#r .....
-  0x00006b38 20000000 00e40f04 2372210f 1d000080  .......#r!.....
-  0x00006b48 24000000 00e40f08 23721d0e 1d000000 $.......#r......
-  0x00006b58 20000000 00e40f04 23721f0e 1f000000  .......#r......
-  0x00006b68 26000000 00e40f00 81790e28 06500100 &........y.(.P..
-  0x00006b78 001b1e0c 00620f00 23721c0c 12000000 .....b..#r......
-  0x00006b88 2a000000 00c48f00 23722b0c 13000000 *.......#r+.....
-  0x00006b98 2b000000 00e40f08 23721c0d 13000000 +.......#r......
-  0x00006ba8 1c010000 00e40f04 2372200d 12000000 ........#r .....
-  0x00006bb8 2b000000 00e40f00 81790c28 06100100 +........y.(....
-  0x00006bc8 001b1e0c 00e20e00 23720612 14000000 ........#r......
-  0x00006bd8 06000000 00e44f08 23722413 14000000 ......O.#r$.....
-  0x00006be8 2c000000 00e40f04 23720613 15000080 ,.......#r......
-  0x00006bf8 06000000 00c40f00 23722412 15000000 ........#r$.....
-  0x00006c08 24000000 00e40f04 81791428 06900100 $........y.(....
-  0x00006c18 001b1e0c 00a20e00 23722612 16000000 ........#r&.....
-  0x00006c28 09000000 00e40f0d 23722213 16000000 ........#r".....
-  0x00006c38 22000000 00e40f04 23721612 18000000 ".......#r......
-  0x00006c48 1b000000 00e40f0a 23721813 18000000 ........#r......
-  0x00006c58 1a000000 00e40f04 81791a28 06d00100 .........y.(....
-  0x00006c68 001b1e0c 00220f00 23720913 17000080 ....."..#r......
-  0x00006c78 26000000 00c40f00 23721712 17000000 &.......#r......
-  0x00006c88 22000000 00e40f04 23722212 19000000 ".......#r".....
-  0x00006c98 18000000 00e40f00 23721e13 0e000000 ........#r......
-  0x00006ca8 1e000000 00e40f00 25762c07 00580000 ........%v,..X..
-  0x00006cb8 03028e07 00c80f00 23722612 0f000000 ........#r&.....
-  0x00006cc8 1e000000 00e40f04 23721613 19000080 ........#r......
-  0x00006cd8 16000000 00e40f04 23721812 0c000000 ........#r......
-  0x00006ce8 23000000 00e48f0c 23720213 0c000000 #.......#r......
-  0x00006cf8 02000000 00e40f04 23720c12 0e000000 ........#r......
-  0x00006d08 25000000 00e40f00 23722313 0d000080 %.......#r#.....
-  0x00006d18 18000000 00c40f00 23720212 0d000000 ........#r......
-  0x00006d28 02000000 00e40f04 23720713 0f000080 ........#r......
-  0x00006d38 0c000000 00e40f04 23721812 14000000 ........#r......
-  0x00006d48 27000000 00e24f08 81790c28 06180000 '.....O..y.(....
-  0x00006d58 001b1e0c 00a20e00 23721f13 14000000 ........#r......
-  0x00006d68 1f000000 00c60f00 81790e2c 06000000 .........y.,....
-  0x00006d78 001b1e0c 00a20e00 23722513 15000080 ........#r%.....
-  0x00006d88 18000000 00e40f0c 23722a12 15000000 ........#r*.....
-  0x00006d98 1f000000 00e20f04 81791828 06980000 .........y.(....
-  0x00006da8 001b1e0c 00e80e00 81791428 06580000 .........y.(.X..
-  0x00006db8 001b1e0c 00620f00 23721e12 1a000000 .....b..#r......
-  0x00006dc8 21000000 00e40f09 23721a13 1a000000 !.......#r......
-  0x00006dd8 1d000000 00c40f00 23721d13 1b000080 ........#r......
-  0x00006de8 1e000000 00e40f08 81791e28 06d80000 .........y.(....
-  0x00006df8 001b1e0c 00220f00 23721b12 1b000000 ....."..#r......
-  0x00006e08 1a000000 00e40f00 23721c0c 0e000000 ........#r......
-  0x00006e18 1c000000 00e44f0c 2372200c 0f000000 ......O.#r .....
-  0x00006e28 20000000 00e40f08 23721a0d 0f000000  .......#r......
-  0x00006e38 1c010000 00e40f04 23721c0d 0e000000 ........#r......
-  0x00006e48 20000000 00c40f00 2372120e 18000000  .......#r......
-  0x00006e58 09000000 00e28f04 81790c28 06180100 .........y.(....
-  0x00006e68 001b1e0c 00a20e00 2372060e 14000000 ........#r......
-  0x00006e78 06000000 00e40f0e 2372240f 14000000 ........#r$.....
-  0x00006e88 24000000 00e40f04 2372170f 18000000 $.......#r......
-  0x00006e98 17000000 00e40f04 2372180f 19000080 ........#r......
-  0x00006ea8 12000000 00e40f04 2372060f 15000080 ........#r......
-  0x00006eb8 06000000 00e20f08 81791228 06580100 .........y.(.X..
-  0x00006ec8 001b1e0c 00e20e00 2372090e 15000000 ........#r......
-  0x00006ed8 24000000 00c60f00 81791428 06980100 $........y.(....
-  0x00006ee8 001b1e0c 00620f00 2372190e 19000000 .....b..#r......
-  0x00006ef8 17000000 00e40f04 2372200e 1e000000 ........#r .....
-  0x00006f08 16000000 00e40f0d 81791628 06d80100 .........y.(....
-  0x00006f18 001b1e0c 00220f00 2372220f 1e000000 ....."..#r".....
-  0x00006f28 22000000 00e40f04 23721e0e 0c000000 ".......#r......
-  0x00006f38 23000000 00e44f08 2372210f 0c000000 #.....O.#r!.....
-  0x00006f48 02000000 00c40f00 23720c0f 0d000080 ........#r......
-  0x00006f58 1e000000 00e40f04 2372020f 1f000080 ........#r......
-  0x00006f68 20000000 00e40f04 23721e0e 12000000  .......#r......
-  0x00006f78 07000000 00e48f0c 2372240f 12000000 ........#r$.....
-  0x00006f88 26000000 00e40f04 2372120e 14000000 &.......#r......
-  0x00006f98 25000000 00e40f0a 2372140f 14000000 %.......#r......
-  0x00006fa8 2a000000 00c40f00 25762a00 00580000 *.......%v*..X..
-  0x00006fb8 03028e07 00c80f00 2372200e 1f000000 ........#r .....
-  0x00006fc8 22000000 00e40f04 2372220e 0d000000 ".......#r".....
-  0x00006fd8 21000000 00e40f04 2372070f 13000080 !.......#r......
-  0x00006fe8 1e000000 00e40f0c 2372240e 13000000 ........#r$.....
-  0x00006ff8 24000000 00e20f04 81791e28 06600000 $........y.(.`..
-  0x00007008 001b1e0c 00a20e00 23720d0f 15000080 ........#r......
-  0x00007018 12000000 00e40f08 2372000e 15000000 ........#r......
-  0x00007028 14000000 00e20f04 8179122a 06000000 .........y.*....
-  0x00007038 001b1e0c 00e20e00 2372260e 16000000 ........#r&.....
-  0x00007048 1d000000 00c40f01 2372160f 16000000 ........#r......
-  0x00007058 1b000000 00e20f04 81791428 06200000 .........y.(. ..
-  0x00007068 001b1e0c 00e20e00 23721b0f 17000080 ........#r......
-  0x00007078 26000000 00e40f08 2372260e 17000000 &.......#r&.....
-  0x00007088 16000000 00e40f00 81790e28 06a00000 .........y.(....
-  0x00007098 001b1e0c 00280f00 81791628 06e00000 .....(...y.(....
-  0x000070a8 001b1e0c 00620f00 23721a14 12000000 .....b..#r......
-  0x000070b8 1a000000 00c48f00 23721c14 13000000 ........#r......
-  0x000070c8 1c000000 00e40f08 23721412 1e000000 ........#r......
-  0x000070d8 06000000 00e44f0c 23721e13 1e000000 ......O.#r......
-  0x000070e8 09000000 00e40f00 23720915 12000000 ........#r......
-  0x000070f8 1c000000 00e40f04 23720615 13000000 ........#r......
-  0x00007108 1a010000 00e40f00 23721c12 0e000000 ........#r......
-  0x00007118 18000000 00c40f01 23721a13 1f000080 ........#r......
-  0x00007128 14000000 00e40f0c 23720e13 0e000000 ........#r......
-  0x00007138 19000000 00e20f04 81791428 06200100 .........y.(. ..
-  0x00007148 001b1e0c 00a20e00 23721f12 1f000000 ........#r......
-  0x00007158 1e000000 00e40f04 23721e12 16000000 ........#r......
-  0x00007168 02000000 00e20f0a 81791828 06600100 .........y.(.`..
-  0x00007178 001b1e0c 00e20e00 23722013 16000000 ........#r .....
-  0x00007188 20000000 00e40f04 23720213 0f000080  .......#r......
-  0x00007198 1c000000 00c40f00 23721c12 0f000000 ........#r......
-  0x000071a8 0e000000 00e40f04 81790e28 06a00100 .........y.(....
-  0x000071b8 001b1e0c 00220f00 23721d13 17000080 ....."..#r......
-  0x000071c8 1e000000 00e40f0c 23721e12 17000000 ........#r......
-  0x000071d8 20000000 00e40f04 81791628 06e00100  ........y.(....
-  0x000071e8 001b1e0c 00620f00 23720c12 14000000 .....b..#r......
-  0x000071f8 0c000000 00e44f08 23722213 14000000 ......O.#r".....
-  0x00007208 22000000 00c40f00 23721412 18000000 ".......#r......
-  0x00007218 07000000 00e48f08 23720713 15000080 ........#r......
-  0x00007228 0c000000 00e40f04 23722013 18000000 ........#r .....
-  0x00007238 24000000 00e40f00 25762408 00580000 $.......%v$..X..
-  0x00007248 03028e07 00c80f00 23720c12 0e000000 ........#r......
-  0x00007258 0d000000 00e40f0d 23720013 0e000000 ........#r......
-  0x00007268 00000000 00e40f04 23721812 15000000 ........#r......
-  0x00007278 22000000 00e40f04 23720812 16000000 ".......#r......
-  0x00007288 1b000000 00e40f0a 23722213 16000000 ........#r".....
-  0x00007298 26000000 00e40f04 23722113 19000080 &.......#r!.....
-  0x000072a8 14000000 00c40f00 23722012 19000000 ........#r .....
-  0x000072b8 20000000 00e20f04 81791428 06680000  ........y.(.h..
-  0x000072c8 001b1e0c 00a20e00 23721913 0f000080 ........#r......
-  0x000072d8 0c000000 00e40f0c 23720012 0f000000 ........#r......
-  0x000072e8 00000000 00e20f04 81790c24 06000000 .........y.$....
-  0x000072f8 001b1e0c 00a20e00 23721b13 17000080 ........#r......
-  0x00007308 08000000 00e40f08 23722212 17000000 ........#r".....
-  0x00007318 22000000 00e20f00 81790e28 06280000 "........y.(.(..
-  0x00007328 001b1e0c 00e80e00 81791228 06a80000 .........y.(....
-  0x00007338 001b1e0c 00280f00 81791628 06e80000 .....(...y.(....
-  0x00007348 001b1e0c 00620f00 2372230d 14000000 .....b..#r#.....
-  0x00007358 1f000000 00c44f00 2372090e 0d000000 ......O.#r......
-  0x00007368 09000000 00e48f04 2372060e 0c000000 ........#r......
-  0x00007378 06000000 00e40f00 2372020c 12000000 ........#r......
-  0x00007388 02000000 00e40f0d 23721c0d 12000000 ........#r......
-  0x00007398 1c000000 00e40f00 23721f0f 0c000000 ........#r......
-  0x000073a8 09000000 00e40f00 23721a0c 14000000 ........#r......
-  0x000073b8 1a000000 00e20f00 81790828 06280100 .........y.(.(..
-  0x000073c8 001b1e0c 00a20e00 2372020d 13000080 ........#r......
-  0x000073d8 02000000 00c40f00 23721c0c 13000000 ........#r......
-  0x000073e8 1c000000 00e40f04 2372060f 0d000000 ........#r......
-  0x000073f8 06010000 00e20f00 81791228 06680100 .........y.(.h..
-  0x00007408 001b1e0c 00e20e00 2372140c 16000000 ........#r......
-  0x00007418 1d000000 00c60f02 81790e28 06a80100 .........y.(....
-  0x00007428 001b1e0c 00220f00 23721e0d 16000000 ....."..#r......
-  0x00007438 1e000000 00e40f04 23721a0d 15000080 ........#r......
-  0x00007448 1a000000 00e40f0c 2372230c 15000000 ........#r#.....
-  0x00007458 23000000 00e40f04 2372160d 17000080 #.......#r......
-  0x00007468 14000000 00e40f08 81791428 06e80100 .........y.(....
-  0x00007478 001b1e0c 00620f00 2372170c 17000000 .....b..#r......
-  0x00007488 1e000000 00c40f00 25762604 00580000 ........%v&..X..
-  0x00007498 03028e07 00c80f00 23721e0c 08000000 ........#r......
-  0x000074a8 07000000 00e44f0c 2372180d 08000000 ......O.#r......
-  0x000074b8 18000000 00e40f04 2372080c 12000000 ........#r......
-  0x000074c8 21000000 00e48f0c 2372200d 12000000 !.......#r .....
-  0x000074d8 20000000 00e40f04 2372120c 0e000000  .......#r......
-  0x000074e8 19000000 00e40f01 2372070d 09000080 ........#r......
-  0x000074f8 1e000000 00c40f00 23720e0d 0e000000 ........#r......
-  0x00007508 00000000 00e40f04 23721d0d 0f000080 ........#r......
-  0x00007518 12000000 00e40f04 2372120c 14000000 ........#r......
-  0x00007528 1b000000 00e40f0e 23721e0d 14000000 ........#r......
-  0x00007538 22000000 00e40f04 2372180c 09000000 ".......#r......
-  0x00007548 18000000 00e40f00 2372190d 13000080 ........#r......
-  0x00007558 08000000 00c40f00 2372000c 13000000 ........#r......
-  0x00007568 20000000 00e20f04 81790828 06300000  ........y.(.0..
-  0x00007578 001b1e0c 00a20e00 2372040c 0f000000 ........#r......
-  0x00007588 0e000000 00e40f04 23721b0d 15000080 ........#r......
-  0x00007598 12000000 00e20f08 81790e26 06000000 .........y.&....
-  0x000075a8 001b1e0c 00a20e00 23721e0c 15000000 ........#r......
-  0x000075b8 1e000000 00c60f00 81790c28 06700000 .........y.(.p..
-  0x000075c8 001b1e0c 00e80e00 81791228 06b00000 .........y.(....
-  0x000075d8 001b1e0c 00280f00 81791428 06f00000 .....(...y.(....
-  0x000075e8 001b1e0c 00620f00 23720608 0e000000 .....b..#r......
-  0x000075f8 06000000 00e44f04 23721f08 0f000000 ......O.#r......
-  0x00007608 1f000000 00c40f00 23721a0e 0c000000 ........#r......
-  0x00007618 1a000000 00e48f0c 2372230f 0c000000 ........#r#.....
-  0x00007628 23000000 00e40f04 2372080e 12000000 #.......#r......
-  0x00007638 02000000 00e40f0d 2372020f 0d000080 ........#r......
-  0x00007648 1a000000 00e40f0c 2372200f 12000000 ........#r .....
-  0x00007658 1c000000 00e40f00 23721a0e 0d000000 ........#r......
-  0x00007668 23000000 00c40f00 23720609 0f000000 #.......#r......
-  0x00007678 06010000 00e20f04 81790c28 06300100 .........y.(.0..
-  0x00007688 001b1e0c 00a20e00 23721f09 0e000000 ........#r......
-  0x00007698 1f000000 00e40f00 23721c0f 13000080 ........#r......
-  0x000076a8 08000000 00e40f0c 81790828 06700100 .........y.(.p..
-  0x000076b8 001b1e0c 00e20e00 2372160e 14000000 ........#r......
-  0x000076c8 16000000 00e40f0e 2372170f 14000000 ........#r......
-  0x000076d8 17000000 00e40f00 2372200e 13000000 ........#r .....
-  0x000076e8 20000000 00c40f00 2372160f 15000080  .......#r......
-  0x000076f8 16000000 00e20f08 81791228 06b00100 .........y.(....
-  0x00007708 001b1e0c 00220f00 2372170e 15000000 ....."..#r......
-  0x00007718 17000000 00c60f00 81791428 06f00100 .........y.(....
-  0x00007728 001b1e0c 00620f00 25763005 00580000 .....b..%v0..X..
-  0x00007738 03028e07 00c80f00 2372220e 0c000000 ........#r".....
-  0x00007748 07000000 00e44f0c 2372180f 0c000000 ......O.#r......
-  0x00007758 18000000 00e40f04 23720c0e 08000000 ........#r......
-  0x00007768 19000000 00e48f08 2372080f 08000000 ........#r......
-  0x00007778 00000000 00e40f04 2372000f 0d000080 ........#r......
-  0x00007788 22000000 00e40f04 2372070f 09000080 ".......#r......
-  0x00007798 0c000000 00c40f00 2372220e 09000000 ........#r".....
-  0x000077a8 08000000 00e40f04 2372080e 12000000 ........#r......
-  0x000077b8 1d000000 00e40f0d 2372040f 12000000 ........#r......
-  0x000077c8 04000000 00e40f04 23720c0e 14000000 ........#r......
-  0x000077d8 1b000000 00e40f0e 23721e0f 14000000 ........#r......
-  0x000077e8 1e000000 00e40f00 2372180e 0d000000 ........#r......
-  0x000077f8 18000000 00c40f00 2372190f 13000080 ........#r......
-  0x00007808 08000000 00e40f0c 2372140e 13000000 ........#r......
-  0x00007818 04000000 00e20f00 81790830 06000000 .........y.0....
-  0x00007828 001b1e0c 00a20e00 2372210f 15000080 ........#r!.....
-  0x00007838 0c000000 00c60f00 81790428 06380000 .........y.(.8..
-  0x00007848 001b1e0c 00a80e00 81790c28 06780000 .........y.(.x..
-  0x00007858 001b1e0c 00e20e00 2372150e 15000000 ........#r......
-  0x00007868 1e000000 00c60f00 81790e28 06b80000 .........y.(....
-  0x00007878 001b1e0c 00280f00 81791228 06f80000 .....(...y.(....
-  0x00007888 001b1e0c 00620f00 23720304 09000000 .....b..#r......
-  0x00007898 1f000000 00e44f04 23720604 08000000 ......O.#r......
-  0x000078a8 06000000 00e40f00 23721a09 0c000000 ........#r......
-  0x000078b8 1a000000 00e48f08 23720408 0c000000 ........#r......
-  0x000078c8 02000000 00c40f00 23720305 08000000 ........#r......
-  0x000078d8 03000000 00e40f04 23720205 09000000 ........#r......
-  0x000078e8 06010000 00e40f00 23720508 0d000000 ........#r......
-  0x000078f8 1a000000 00e40f0c 23720608 0e000000 ........#r......
-  0x00007908 1c000000 00e20f0d 81791a28 06380100 .........y.(.8..
-  0x00007918 001b1e0c 00a20e00 23722009 0e000000 ........#r .....
-  0x00007928 20000000 00e40f04 23720e08 12000000  .......#r......
-  0x00007938 16000000 00e20f02 81791c28 06f80100 .........y.(....
-  0x00007948 001b1e0c 00e20e00 23720409 0d000080 ........#r......
-  0x00007958 04000000 00c40f00 23721209 12000000 ........#r......
-  0x00007968 17000000 00e20f04 81790c28 06b80100 .........y.(....
-  0x00007978 001b1e0c 00280f00 81791628 06780100 .....(...y.(.x..
-  0x00007988 001b1e0c 00620f00 23720609 0f000080 .....b..#r......
-  0x00007998 06000000 00e40f04 23720e09 13000080 ........#r......
-  0x000079a8 0e000000 00e20f00 8679000a 02000000 .........y......
-  0x000079b8 061b100c 00e80f00 86790010 04000000 .........y......
-  0x000079c8 061b100c 00e20f00 23720008 1a000000 ........#r......
-  0x000079d8 00000000 00c44f00 23721a09 1a000000 ......O.#r......
-  0x000079e8 18000000 00e40f04 23721509 1c000000 ........#r......
-  0x000079f8 15000000 00e48f0c 23721c08 1c000000 ........#r......
-  0x00007a08 21000000 00e40f04 23721409 0c000000 !.......#r......
-  0x00007a18 14000000 00e40f09 23720c08 0c000000 ........#r......
-  0x00007a28 19000000 00e40f04 23721808 16000000 ........#r......
-  0x00007a38 07000000 00c40f02 23722209 16000000 ........#r".....
-  0x00007a48 22000000 00e40f04 23720708 0f000000 ".......#r......
-  0x00007a58 20000000 00e40f04 23720f08 13000000  .......#r......
-  0x00007a68 12000000 00e40f04 23721308 1b000000 ........#r......
-  0x00007a78 1a000000 00e40f0c 23721209 1b000080 ........#r......
-  0x00007a88 00000000 00e40f00 23721b08 17000000 ........#r......
-  0x00007a98 22000000 00c40f00 23721a09 17000080 ".......#r......
-  0x00007aa8 18000000 00e20f04 8679002e 06000000 .........y......
-  0x00007ab8 061b100c 00e20f00 23721708 0d000000 ........#r......
-  0x00007ac8 14000000 00e40f0c 23721609 0d000080 ........#r......
-  0x00007ad8 0c000000 00e20f04 8679002c 0e000000 .........y.,....
-  0x00007ae8 061b100c 00e20f00 23721508 1d000000 ........#r......
-  0x00007af8 15000000 00e40f08 23721409 1d000080 ........#r......
-  0x00007b08 1c000000 00e20f00 8679002a 12000000 .........y.*....
-  0x00007b18 061b100c 00e80f00 86790024 1a000000 .........y.$....
-  0x00007b28 061b100c 00e80f00 86790026 16000000 .........y.&....
-  0x00007b38 061b100c 00e80f00 86790030 14000000 .........y.0....
-  0x00007b48 061b100c 00e20f00 4d790000 00000000 ........My......
-  0x00007b58 00008003 00ea0f00 47790000 f0ffffff ........Gy......
-  0x00007b68 ffff8303 00c00f00 18790000 00000000 .........y......
-  0x00007b78 00000000 00c00f00 18790000 00000000 .........y......
-  0x00007b88 00000000 00c00f00 18790000 00000000 .........y......
-  0x00007b98 00000000 00c00f00 18790000 00000000 .........y......
-  0x00007ba8 00000000 00c00f00 18790000 00000000 .........y......
-  0x00007bb8 00000000 00c00f00 18790000 00000000 .........y......
-  0x00007bc8 00000000 00c00f00 18790000 00000000 .........y......
-  0x00007bd8 00000000 00c00f00 18790000 00000000 .........y......
-  0x00007be8 00000000 00c00f00 18790000 00000000 .........y......
-  0x00007bf8 00000000 00c00f00 18790000 00000000 .........y......
-  0x00007c08 00000000 00c00f00 027a0100 000a0000 .........z......
-  0x00007c18 000f0000 00e40f00 027a0200 005e0000 .........z...^..
-  0x00007c28 000f0000 00e20f00 b97a0600 00460000 .........z...F..
-  0x00007c38 000a0000 00e20f00 027a0300 005f0000 .........z..._..
-  0x00007c48 000f0000 00ca0f00 81790402 06080000 .........y......
-  0x00007c58 00191e0c 00a80000 81790502 06000000 .........y......
-  0x00007c68 00191e0c 00e20000 b97a0400 00000000 .........z......
-  0x00007c78 00080000 00e40f00 9978043f 01000000 .........x.?....
-  0x00007c88 04160108 00e20f00 19790000 00000000 .........y......
-  0x00007c98 00250000 00680e00 19790900 00000000 .%...h...y......
-  0x00007ca8 00210000 00640e00 247a0000 00000000 .!...d..$z......
-  0x00007cb8 09028e07 00ca2f00 197803ff 1f000000 ....../..x......
-  0x00007cc8 00140100 00e41f00 12720700 04000000 .........r......
-  0x00007cd8 fffc8e07 00e44f0c 10720b05 04000000 ......O..r......
-  0x00007ce8 ffe0ff07 00e48f00 12720500 05000000 .........r......
-  0x00007cf8 fffc8e07 00e40f04 0c720000 07000000 .........r......
-  0x00007d08 7052f003 00e40f04 12720600 0b000000 pR.......r......
-  0x00007d18 fffc8e07 00c40f00 0c720000 05000000 .........r......
-  0x00007d28 70527000 00c80f00 0c720000 06000000 pRp......r......
-  0x00007d38 70527200 00e40f0c 0c7a0000 005c0000 pRr......z...\..
-  0x00007d48 7060f003 00e40f00 0c720005 07000000 p`.......r......
-  0x00007d58 7052f200 00e40f00 0c7a0003 005d0000 pR.......z...]..
-  0x00007d68 0061f003 00e40f00 0c720005 06000000 .a.......r......
-  0x00007d78 7052f200 00e40f00 0c7c0009 04000000 pR.......|......
-  0x00007d88 7010700c 00c40f00 0c720007 06000000 p.p......r......
-  0x00007d98 7052f200 00c80f00 1c780000 00000000 pR.......x......
-  0x00007da8 70307000 00da0f00 4d890000 00000000 p0p.....M.......
-  0x00007db8 00008003 00ea0f00 117a0800 00580000 .........z...X..
-  0x00007dc8 ff188007 00e40f04 027a0e00 005a0000 .........z...Z..
-  0x00007dd8 000f0000 00e40f00 027a0f00 005b0000 .........z...[..
-  0x00007de8 000f0000 00e40f00 117a0900 00590000 .........z...Y..
-  0x00007df8 031c0f00 00c60f00 8179020e 06000000 .........y......
-  0x00007e08 001b1e0c 00a80e00 81791408 06000000 .........y......
-  0x00007e18 001b1e0c 00a80e00 8179100e 06200000 .........y... ..
-  0x00007e28 001b1e0c 00e80e00 81790a0e 06400000 .........y...@..
-  0x00007e38 001b1e0c 00280f00 8179160e 06600000 .....(...y...`..
-  0x00007e48 001b1e0c 00620f00 357400ff 08000000 .....b..5t......
-  0x00007e58 ff010000 00c60f00 8179120e 06280000 .........y...(..
-  0x00007e68 001b1e0c 006e0f00 25760c05 00580000 .....n..%v...X..
-  0x00007e78 00028e07 00c80f00 20721903 15000000 ........ r......
-  0x00007e88 00004000 00e44f04 20720403 14000000 ..@...O. r......
-  0x00007e98 00004000 00e40f00 20720315 11000000 ..@..... r......
-  0x00007ea8 00004000 00e48f0c 20720514 11000000 ..@..... r......
-  0x00007eb8 00004000 00e40f04 20721115 0b000000 ..@..... r......
-  0x00007ec8 00004000 00e40f09 20721814 0b000000 ..@..... r......
-  0x00007ed8 00004000 00c40f00 23721902 14000000 ..@.....#r......
-  0x00007ee8 19080000 00e40f04 23720402 15000000 ........#r......
-  0x00007ef8 04000000 00e40f00 23720214 10000000 ........#r......
-  0x00007f08 03080000 00e40f0c 23720515 10000000 ........#r......
-  0x00007f18 05000000 00e40f04 23720314 0a000000 ........#r......
-  0x00007f28 11080000 00e40f08 23721815 0a000000 ........#r......
-  0x00007f38 18000000 00e20f04 8179100c 06000000 .........y......
-  0x00007f48 001b1e0c 00a20e00 20721b15 17000000 ........ r......
-  0x00007f58 00004000 00c60f02 81790a0e 06080000 ..@......y......
-  0x00007f68 001b1e0c 00a20e00 20721a14 17000000 ........ r......
-  0x00007f78 00004000 00e40f04 23721b14 16000000 ..@.....#r......
-  0x00007f88 1b080000 00e40f08 23721a15 16000000 ........#r......
-  0x00007f98 1a000000 00e40f00 8179140e 06480000 .........y...H..
-  0x00007fa8 001b1e0c 00e80e00 8179160e 06680000 .........y...h..
-  0x00007fb8 001b1e0c 00220f00 23721c0a 10000000 ....."..#r......
-  0x00007fc8 19000000 00c44f00 2372040a 11000000 ......O.#r......
-  0x00007fd8 04000000 00e40f08 23720a10 12000000 ........#r......
-  0x00007fe8 02000000 00e40f00 2372020b 11000000 ........#r......
-  0x00007ff8 1c010000 00e40f04 23720b0b 10000000 ........#r......
-  0x00008008 04000000 00e40f00 23720411 13000080 ........#r......
-  0x00008018 0a000000 00e40f04 23720511 12000000 ........#r......
-  0x00008028 05000000 00c40f00 23720a10 14000000 ........#r......
-  0x00008038 03000000 00e48f0c 23721310 13000000 ........#r......
-  0x00008048 05000000 00e40f00 23720311 15000080 ........#r......
-  0x00008058 0a000000 00e40f04 23720511 14000000 ........#r......
-  0x00008068 18000000 00e40f00 25761c07 00580000 ........%v...X..
-  0x00008078 00028e07 00c80f00 23721210 16000000 ........#r......
-  0x00008088 1b000000 00e20f0d 8179181c 06000000 .........y......
-  0x00008098 001b1e0c 00a20e00 23720a11 16000000 ........#r......
-  0x000080a8 1a000000 00e40f04 23720510 15000000 ........#r......
-  0x000080b8 05000000 00e20f04 81791a0e 06300000 .........y...0..
-  0x000080c8 001b1e0c 00a20e00 23720711 17000080 ........#r......
-  0x000080d8 12000000 00e40f08 23720a10 17000000 ........#r......
-  0x000080e8 0a000000 00e20f00 8179140e 06100000 .........y......
-  0x000080f8 001b1e0c 00e80e00 8179100e 06500000 .........y...P..
-  0x00008108 001b1e0c 00280f00 8179160e 06700000 .....(...y...p..
-  0x00008118 001b1e0c 00620f00 25761e06 00580000 .....b..%v...X..
-  0x00008128 00028e07 00c80f00 23720418 1a000000 ........#r......
-  0x00008138 04000000 00e44f08 23721319 1a000000 ......O.#r......
-  0x00008148 13000000 00e40f04 23720214 18000000 ........#r......
-  0x00008158 02000000 00e48f04 23720b14 19000000 ........#r......
-  0x00008168 0b000000 00e40f00 23721218 10000000 ........#r......
-  0x00008178 03000000 00e40f09 23720519 10000000 ........#r......
-  0x00008188 05000000 00c40f00 23720018 16000000 ........#r......
-  0x00008198 07000000 00e40f0e 23721619 16000000 ........#r......
-  0x000081a8 0a000000 00e20f04 8179060e 06180000 .........y......
-  0x000081b8 001b1e0c 00a20e00 23720319 11000080 ........#r......
-  0x000081c8 12000000 00e40f00 23720215 19000000 ........#r......
-  0x000081d8 02010000 00e40f04 23721118 11000000 ........#r......
-  0x000081e8 05000000 00e40f00 23721515 18000000 ........#r......
-  0x000081f8 0b000000 00c40f00 23720419 1b000080 ........#r......
-  0x00008208 04000000 00e20f04 81790a1e 06000000 .........y......
-  0x00008218 001b1e0c 00a20e00 23720519 17000080 ........#r......
-  0x00008228 00000000 00e40f00 23721b18 1b000000 ........#r......
-  0x00008238 13000000 00e40f04 23720018 17000000 ........#r......
-  0x00008248 16000000 00e20f00 8179120e 06380000 .........y...8..
-  0x00008258 001b1e0c 00e80e00 8179160e 06580000 .........y...X..
-  0x00008268 001b1e0c 00280f00 8179180e 06780000 .....(...y...x..
-  0x00008278 001b1e0c 00620f00 23721506 0b000000 .....b..#r......
-  0x00008288 15000000 00c44f00 23720206 0a000000 ......O.#r......
-  0x00008298 02000000 00e40f00 23721b0b 12000000 ........#r......
-  0x000082a8 1b000000 00e48f0c 2372040a 12000000 ........#r......
-  0x000082b8 04000000 00e40f04 2372110b 16000000 ........#r......
-  0x000082c8 11000000 00e40f0d 2372160a 16000000 ........#r......
-  0x000082d8 03000000 00e40f00 2372000b 18000000 ........#r......
-  0x000082e8 00000000 00c40f02 2372180a 18000000 ........#r......
-  0x000082f8 05000000 00e40f04 23721507 0a000000 ........#r......
-  0x00008308 15000000 00e40f04 23721407 0b000000 ........#r......
-  0x00008318 02010000 00e40f00 2372070a 13000000 ........#r......
-  0x00008328 1b000000 00e40f0c 2372060b 13000080 ........#r......
-  0x00008338 04000000 00e40f00 2372110a 17000000 ........#r......
-  0x00008348 11000000 00c40f00 2372100b 17000080 ........#r......
-  0x00008358 16000000 00e40f04 2372030a 19000000 ........#r......
-  0x00008368 00000000 00e40f08 2372020b 19000080 ........#r......
-  0x00008378 18000000 00e20f00 86790008 14000000 .........y......
-  0x00008388 061b100c 00e80f00 8679000c 06000000 .........y......
-  0x00008398 061b100c 00e80f00 8679001c 10000000 .........y......
-  0x000083a8 061b100c 00e80f00 8679001e 02000000 .........y......
-  0x000083b8 061b100c 00e20f00 4d790000 00000000 ........My......
-  0x000083c8 00008003 00ea0f00 47790000 f0ffffff ........Gy......
-  0x000083d8 ffff8303 00c00f00 18790000 00000000 .........y......
-  0x000083e8 00000000 00c00f00 18790000 00000000 .........y......
-  0x000083f8 00000000 00c00f00 18790000 00000000 .........y......
-  0x00008408 00000000 00c00f00 18790000 00000000 .........y......
-  0x00008418 00000000 00c00f00 18790000 00000000 .........y......
-  0x00008428 00000000 00c00f00 18790000 00000000 .........y......
-  0x00008438 00000000 00c00f00 18790000 00000000 .........y......
-  0x00008448 00000000 00c00f00 18790000 00000000 .........y......
-  0x00008458 00000000 00c00f00 18790000 00000000 .........y......
-  0x00008468 00000000 00c00f00 18790000 00000000 .........y......
+  0x00006208 00000000 00000000 00000000 00000000 ................
+  0x00006218 00000000 00000000 00000000 00000000 ................
+  0x00006228 00000000 00000000 00000000 00000000 ................
+  0x00006238 00000000 00000000 00000000 00000000 ................
+  0x00006248 00000000 00000000 00000000 00000000 ................
+  0x00006258 00000000 00000000 00000000 00000000 ................
+  0x00006268 00000000 00000000 00000000 00000000 ................
+  0x00006278 00000000 00000000 00000000 00000000 ................
+  0x00006288 00000000 00000000 00000000 00000000 ................
+  0x00006298 00000000 00000000 027a0100 000a0000 .........z......
+  0x000062a8 000f0000 00e40f00 027a0400 005e0000 .........z...^..
+  0x000062b8 000f0000 00e20f00 b97a0600 00460000 .........z...F..
+  0x000062c8 000a0000 00e20f00 027a0500 005f0000 .........z..._..
+  0x000062d8 000f0000 00ca0f00 81790304 06080000 .........y......
+  0x000062e8 00191e0c 00a80e00 81790604 06000000 .........y......
+  0x000062f8 00191e0c 00e80e00 81790804 06100000 .........y......
+  0x00006308 00191e0c 00220f00 b97a0400 00000000 ....."...z......
+  0x00006318 00080000 00e40f00 9978043f 01000000 .........x.?....
+  0x00006328 04160108 00e20f00 19790b00 00000000 .........y......
+  0x00006338 00250000 00280e00 19790a00 00000000 .%...(...y......
+  0x00006348 00210000 00240e00 247a0b0b 00000000 .!...$..$z......
+  0x00006358 0a028e07 00ca1f00 1272020b 03000000 .........r......
+  0x00006368 fffc8e07 00e44f0c 1272100b 06000000 ......O..r......
+  0x00006378 fffc8e07 00e48f04 10720006 03000000 .........r......
+  0x00006388 ffe0ff07 00e40f00 0c72000b 02000000 .........r......
+  0x00006398 7052f003 00e40f04 1272070b 00000000 pR.......r......
+  0x000063a8 fffc8e07 00e40f04 0c72000b 10000000 .........r......
+  0x000063b8 70527000 00c40f00 10720c06 08000000 pRp......r......
+  0x000063c8 ffe0ff07 00e40f09 1272000b 08000000 .........r......
+  0x000063d8 fffc8e07 00e40f0c 0c72000b 07000000 .........r......
+  0x000063e8 70527000 00e40f00 10720303 08000000 pRp......r......
+  0x000063f8 ffe0ff07 00e40f00 1272080b 0c000000 .........r......
+  0x00006408 fffc8e07 00e40f04 0c72000b 00000000 .........r......
+  0x00006418 70527000 00c40f00 10720606 03000000 pRp......r......
+  0x00006428 ffe0ff07 00e40f08 1272040b 03000000 .........r......
+  0x00006438 fffc8e07 00e40f04 0c72000b 08000000 .........r......
+  0x00006448 70527000 00e40f04 1272050b 06000000 pRp......r......
+  0x00006458 fffc8e07 00e40f04 0c72000b 04000000 .........r......
+  0x00006468 70527000 00e40f00 197803ff 1f000000 pRp......x......
+  0x00006478 0b140100 00c40f00 0c72000b 05000000 .........r......
+  0x00006488 70527000 00c80f00 0c720010 02000000 pRp......r......
+  0x00006498 70527000 00c80f00 0c720010 07000000 pRp......r......
+  0x000064a8 70527000 00c80f00 0c720010 00000000 pRp......r......
+  0x000064b8 70527000 00c80f00 0c720010 08000000 pRp......r......
+  0x000064c8 70527000 00c80f00 0c720010 04000000 pRp......r......
+  0x000064d8 70527000 00c80f00 0c720010 05000000 pRp......r......
+  0x000064e8 70527000 00c80f00 0c720002 07000000 pRp......r......
+  0x000064f8 70527000 00c80f00 0c720002 00000000 pRp......r......
+  0x00006508 70527000 00c80f00 0c720002 08000000 pRp......r......
+  0x00006518 70527000 00c80f00 0c720002 04000000 pRp......r......
+  0x00006528 70527000 00c80f00 0c720002 05000000 pRp......r......
+  0x00006538 70527000 00c80f00 0c720007 00000000 pRp......r......
+  0x00006548 70527000 00c80f00 0c720007 08000000 pRp......r......
+  0x00006558 70527000 00c80f00 0c720007 04000000 pRp......r......
+  0x00006568 70527000 00c80f00 0c720007 05000000 pRp......r......
+  0x00006578 70527000 00c80f00 0c720000 08000000 pRp......r......
+  0x00006588 70527000 00c80f00 0c720000 04000000 pRp......r......
+  0x00006598 70527000 00c80f00 0c720000 05000000 pRp......r......
+  0x000065a8 70527200 00e40f08 0c7a000b 005c0000 pRr......z...\..
+  0x000065b8 7060f003 00e40f00 0c720008 04000000 p`.......r......
+  0x000065c8 7052f200 00e40f04 0c7a0003 005d0000 pR.......z...]..
+  0x000065d8 0061f003 00e40f00 0c720008 05000000 .a.......r......
+  0x000065e8 7052f200 00e40f00 0c7c000a 04000000 pR.......|......
+  0x000065f8 7010700c 00c40f00 0c720004 05000000 p.p......r......
+  0x00006608 7052f200 00c80f00 1c780000 00000000 pR.......x......
+  0x00006618 70307000 00da0f00 4d890000 00000000 p0p.....M.......
+  0x00006628 00008003 00ea0f00 357403ff 08000000 ........5t......
+  0x00006638 ff010000 00e20f00 027a2800 005a0000 .........z(..Z..
+  0x00006648 000f0000 00e40f00 027a2900 005b0000 .........z)..[..
+  0x00006658 000f0000 00ca0f00 81792428 06400000 .........y$(.@..
+  0x00006668 001b1e0c 00a40e00 25760a0b 00580000 ........%v...X..
+  0x00006678 03028e07 00e40f08 81792228 06800000 .........y"(....
+  0x00006688 001b1e0c 00e80e00 81791e0a 06000000 .........y......
+  0x00006698 001b1e0c 00a80e00 81791228 06c00000 .........y.(....
+  0x000066a8 001b1e0c 00280f00 81791a28 06000100 .....(...y.(....
+  0x000066b8 001b1e0c 00680f00 81790c28 06400100 .....h...y.(.@..
+  0x000066c8 001b1e0c 00280f00 81792628 06000000 .....(...y&(....
+  0x000066d8 001b1e0c 00280f00 81792028 06c00100 .....(...y (....
+  0x000066e8 001b1e0c 00680f00 81791628 06800100 .....h...y.(....
+  0x000066f8 001b1e0c 00620f00 25761010 00580000 .....b..%v...X..
+  0x00006708 03028e07 00c60f00 81791828 06080000 .........y.(....
+  0x00006718 001b1e0c 00680f00 81790e10 06000000 .....h...y......
+  0x00006728 001b1e0c 00680f00 81791428 06880000 .....h...y.(....
+  0x00006738 001b1e0c 00680f00 81791c28 06480000 .....h...y.(.H..
+  0x00006748 001b1e0c 00620f00 2072091f 25000000 .....b.. r..%...
+  0x00006758 00004000 00c44f00 2072061e 25000000 ..@...O. r..%...
+  0x00006768 00004000 00e40f04 2372091e 24000000 ..@.....#r..$...
+  0x00006778 09080000 00e40f0c 2372061f 24000000 ........#r..$...
+  0x00006788 06000000 00e40f04 2072251f 23000000 ........ r%.#...
+  0x00006798 00004000 00e48f08 2072241e 23000000 ..@..... r$.#...
+  0x000067a8 00004000 00e40f04 2372231e 22000000 ..@.....#r#."...
+  0x000067b8 25080000 00c40f00 2372221f 22000000 %.......#r"."...
+  0x000067c8 24000000 00e40f04 2072251f 13000000 $....... r%.....
+  0x000067d8 00004000 00e40f0d 2072241e 13000000 ..@..... r$.....
+  0x000067e8 00004000 00e40f04 2372131e 12000000 ..@.....#r......
+  0x000067f8 25080000 00e40f08 2372121f 12000000 %.......#r......
+  0x00006808 24000000 00e40f04 2072251f 1b000000 $....... r%.....
+  0x00006818 00004000 00c40f02 2072241e 1b000000 ..@..... r$.....
+  0x00006828 00004000 00e40f04 23721b1e 1a000000 ..@.....#r......
+  0x00006838 25080000 00e40f0c 23721a1f 1a000000 %.......#r......
+  0x00006848 24000000 00e40f04 2072251f 0d000000 $....... r%.....
+  0x00006858 00004000 00e40f08 2072241e 0d000000 ..@..... r$.....
+  0x00006868 00004000 00e40f00 20722b27 1f000000 ..@..... r+'....
+  0x00006878 00004000 00c40f00 20722a27 1e000000 ..@..... r*'....
+  0x00006888 00004000 00e40f00 2372251e 0c000000 ..@.....#r%.....
+  0x00006898 25080000 00e40f0c 2372241f 0c000000 %.......#r$.....
+  0x000068a8 24000000 00e40f04 20720d1f 21000000 $....... r..!...
+  0x000068b8 00004000 00e40f08 20720c1e 21000000 ..@..... r..!...
+  0x000068c8 00004000 00e40f00 23722b26 1e000000 ..@.....#r+&....
+  0x000068d8 2b080000 00c40f00 23722a26 1f000000 +.......#r*&....
+  0x000068e8 2a000000 00e40f00 2072271f 17000000 *....... r'.....
+  0x000068f8 00004000 00e40f0c 2072261e 17000000 ..@..... r&.....
+  0x00006908 00004000 00e40f04 2372211e 20000000 ..@.....#r!. ...
+  0x00006918 0d080000 00e40f0c 2372201f 20000000 ........#r . ...
+  0x00006928 0c000000 00e40f04 2372271e 16000000 ........#r'.....
+  0x00006938 27080000 00e20f08 81790c28 06c80000 '........y.(....
+  0x00006948 001b1e0c 00a20e00 2372261f 16000000 ........#r&.....
+  0x00006958 26000000 00c60f00 81791628 06080100 &........y.(....
+  0x00006968 001b1e0c 00e20e00 23721e18 0e000000 ........#r......
+  0x00006978 2b000000 00e40f0c 23722b18 0f000000 +.......#r+.....
+  0x00006988 2a000000 00e40f08 23722a19 0f000000 *.......#r*.....
+  0x00006998 1e010000 00e40f04 23722b19 0e000000 ........#r+.....
+  0x000069a8 2b000000 00e20f00 81791e28 06880100 +........y.(....
+  0x000069b8 001b1e0c 00280f00 81791828 06480100 .....(...y.(.H..
+  0x000069c8 001b1e0c 00620f00 23722e0e 14000000 .....b..#r......
+  0x000069d8 23000000 00c40f00 23722c0e 1c000000 #.......#r,.....
+  0x000069e8 09000000 00e40f08 23721c0f 1c000000 ........#r......
+  0x000069f8 06000000 00e40f04 2372220f 14000000 ........#r".....
+  0x00006a08 22000000 00e40f04 2372090f 15000080 ".......#r......
+  0x00006a18 2e000000 00e40f00 25762e02 00580000 ........%v...X..
+  0x00006a28 03028e07 00c80f00 2372060f 1d000080 ........#r......
+  0x00006a38 2c000000 00e40f0c 23722c0e 1d000000 ,.......#r,.....
+  0x00006a48 1c000000 00e40f04 81791c28 06c80100 .........y.(....
+  0x00006a58 001b1e0c 00220f00 2372220e 15000000 ....."..#r".....
+  0x00006a68 22000000 00e40f04 2372140e 0c000000 ".......#r......
+  0x00006a78 13000000 00e44f0c 2372120f 0c000000 ......O.#r......
+  0x00006a88 12000000 00e40f00 23720c0e 16000000 ........#r......
+  0x00006a98 1b000000 00c48f00 2372160f 16000000 ........#r......
+  0x00006aa8 1a000000 00e40f04 23721b0f 0d000080 ........#r......
+  0x00006ab8 14000000 00e40f0c 23721a0e 0d000000 ........#r......
+  0x00006ac8 12000000 00e20f00 81791428 06500000 .........y.(.P..
+  0x00006ad8 001b1e0c 00a20e00 2372230f 17000080 ........#r#.....
+  0x00006ae8 0c000000 00c60f00 81790c28 06100000 .........y.(....
+  0x00006af8 001b1e0c 00e80e00 8179122e 06000000 .........y......
+  0x00006b08 001b1e0c 00e20e00 2372020e 17000000 ........#r......
+  0x00006b18 16000000 00e40f04 2372160e 18000000 ........#r......
+  0x00006b28 25000000 00e40f0e 2372240f 18000000 %.......#r$.....
+  0x00006b38 24000000 00e40f00 2372180e 1e000000 $.......#r......
+  0x00006b48 27000000 00c40f01 2372260f 1e000000 '.......#r&.....
+  0x00006b58 26000000 00e40f04 2372250f 19000080 &.......#r%.....
+  0x00006b68 16000000 00e40f0c 23721e0e 19000000 ........#r......
+  0x00006b78 24000000 00e20f00 81791628 06900000 $........y.(....
+  0x00006b88 001b1e0c 00220f00 2372270f 1f000080 ....."..#r'.....
+  0x00006b98 18000000 00c60f00 81791828 06d00000 .........y.(....
+  0x00006ba8 001b1e0c 00620f00 2372240e 1c000000 .....b..#r$.....
+  0x00006bb8 21000000 00e40f0c 2372200f 1c000000 !.......#r .....
+  0x00006bc8 20000000 00e40f04 2372210f 1d000080  .......#r!.....
+  0x00006bd8 24000000 00e40f08 23721d0e 1d000000 $.......#r......
+  0x00006be8 20000000 00e40f04 23721f0e 1f000000  .......#r......
+  0x00006bf8 26000000 00e40f00 81790e28 06500100 &........y.(.P..
+  0x00006c08 001b1e0c 00620f00 23721c0c 12000000 .....b..#r......
+  0x00006c18 2a000000 00c48f00 23722b0c 13000000 *.......#r+.....
+  0x00006c28 2b000000 00e40f08 23721c0d 13000000 +.......#r......
+  0x00006c38 1c010000 00e40f04 2372200d 12000000 ........#r .....
+  0x00006c48 2b000000 00e40f00 81790c28 06100100 +........y.(....
+  0x00006c58 001b1e0c 00e20e00 23720612 14000000 ........#r......
+  0x00006c68 06000000 00e44f08 23722413 14000000 ......O.#r$.....
+  0x00006c78 2c000000 00e40f04 23720613 15000080 ,.......#r......
+  0x00006c88 06000000 00c40f00 23722412 15000000 ........#r$.....
+  0x00006c98 24000000 00e40f04 81791428 06900100 $........y.(....
+  0x00006ca8 001b1e0c 00a20e00 23722612 16000000 ........#r&.....
+  0x00006cb8 09000000 00e40f0d 23722213 16000000 ........#r".....
+  0x00006cc8 22000000 00e40f04 23721612 18000000 ".......#r......
+  0x00006cd8 1b000000 00e40f0a 23721813 18000000 ........#r......
+  0x00006ce8 1a000000 00e40f04 81791a28 06d00100 .........y.(....
+  0x00006cf8 001b1e0c 00220f00 23720913 17000080 ....."..#r......
+  0x00006d08 26000000 00c40f00 23721712 17000000 &.......#r......
+  0x00006d18 22000000 00e40f04 23722212 19000000 ".......#r".....
+  0x00006d28 18000000 00e40f00 23721e13 0e000000 ........#r......
+  0x00006d38 1e000000 00e40f00 25762c07 00580000 ........%v,..X..
+  0x00006d48 03028e07 00c80f00 23722612 0f000000 ........#r&.....
+  0x00006d58 1e000000 00e40f04 23721613 19000080 ........#r......
+  0x00006d68 16000000 00e40f04 23721812 0c000000 ........#r......
+  0x00006d78 23000000 00e48f0c 23720213 0c000000 #.......#r......
+  0x00006d88 02000000 00e40f04 23720c12 0e000000 ........#r......
+  0x00006d98 25000000 00e40f00 23722313 0d000080 %.......#r#.....
+  0x00006da8 18000000 00c40f00 23720212 0d000000 ........#r......
+  0x00006db8 02000000 00e40f04 23720713 0f000080 ........#r......
+  0x00006dc8 0c000000 00e40f04 23721812 14000000 ........#r......
+  0x00006dd8 27000000 00e24f08 81790c28 06180000 '.....O..y.(....
+  0x00006de8 001b1e0c 00a20e00 23721f13 14000000 ........#r......
+  0x00006df8 1f000000 00c60f00 81790e2c 06000000 .........y.,....
+  0x00006e08 001b1e0c 00a20e00 23722513 15000080 ........#r%.....
+  0x00006e18 18000000 00e40f0c 23722a12 15000000 ........#r*.....
+  0x00006e28 1f000000 00e20f04 81791828 06980000 .........y.(....
+  0x00006e38 001b1e0c 00e80e00 81791428 06580000 .........y.(.X..
+  0x00006e48 001b1e0c 00620f00 23721e12 1a000000 .....b..#r......
+  0x00006e58 21000000 00e40f09 23721a13 1a000000 !.......#r......
+  0x00006e68 1d000000 00c40f00 23721d13 1b000080 ........#r......
+  0x00006e78 1e000000 00e40f08 81791e28 06d80000 .........y.(....
+  0x00006e88 001b1e0c 00220f00 23721b12 1b000000 ....."..#r......
+  0x00006e98 1a000000 00e40f00 23721c0c 0e000000 ........#r......
+  0x00006ea8 1c000000 00e44f0c 2372200c 0f000000 ......O.#r .....
+  0x00006eb8 20000000 00e40f08 23721a0d 0f000000  .......#r......
+  0x00006ec8 1c010000 00e40f04 23721c0d 0e000000 ........#r......
+  0x00006ed8 20000000 00c40f00 2372120e 18000000  .......#r......
+  0x00006ee8 09000000 00e28f04 81790c28 06180100 .........y.(....
+  0x00006ef8 001b1e0c 00a20e00 2372060e 14000000 ........#r......
+  0x00006f08 06000000 00e40f0e 2372240f 14000000 ........#r$.....
+  0x00006f18 24000000 00e40f04 2372170f 18000000 $.......#r......
+  0x00006f28 17000000 00e40f04 2372180f 19000080 ........#r......
+  0x00006f38 12000000 00e40f04 2372060f 15000080 ........#r......
+  0x00006f48 06000000 00e20f08 81791228 06580100 .........y.(.X..
+  0x00006f58 001b1e0c 00e20e00 2372090e 15000000 ........#r......
+  0x00006f68 24000000 00c60f00 81791428 06980100 $........y.(....
+  0x00006f78 001b1e0c 00620f00 2372190e 19000000 .....b..#r......
+  0x00006f88 17000000 00e40f04 2372200e 1e000000 ........#r .....
+  0x00006f98 16000000 00e40f0d 81791628 06d80100 .........y.(....
+  0x00006fa8 001b1e0c 00220f00 2372220f 1e000000 ....."..#r".....
+  0x00006fb8 22000000 00e40f04 23721e0e 0c000000 ".......#r......
+  0x00006fc8 23000000 00e44f08 2372210f 0c000000 #.....O.#r!.....
+  0x00006fd8 02000000 00c40f00 23720c0f 0d000080 ........#r......
+  0x00006fe8 1e000000 00e40f04 2372020f 1f000080 ........#r......
+  0x00006ff8 20000000 00e40f04 23721e0e 12000000  .......#r......
+  0x00007008 07000000 00e48f0c 2372240f 12000000 ........#r$.....
+  0x00007018 26000000 00e40f04 2372120e 14000000 &.......#r......
+  0x00007028 25000000 00e40f0a 2372140f 14000000 %.......#r......
+  0x00007038 2a000000 00c40f00 25762a00 00580000 *.......%v*..X..
+  0x00007048 03028e07 00c80f00 2372200e 1f000000 ........#r .....
+  0x00007058 22000000 00e40f04 2372220e 0d000000 ".......#r".....
+  0x00007068 21000000 00e40f04 2372070f 13000080 !.......#r......
+  0x00007078 1e000000 00e40f0c 2372240e 13000000 ........#r$.....
+  0x00007088 24000000 00e20f04 81791e28 06600000 $........y.(.`..
+  0x00007098 001b1e0c 00a20e00 23720d0f 15000080 ........#r......
+  0x000070a8 12000000 00e40f08 2372000e 15000000 ........#r......
+  0x000070b8 14000000 00e20f04 8179122a 06000000 .........y.*....
+  0x000070c8 001b1e0c 00e20e00 2372260e 16000000 ........#r&.....
+  0x000070d8 1d000000 00c40f01 2372160f 16000000 ........#r......
+  0x000070e8 1b000000 00e20f04 81791428 06200000 .........y.(. ..
+  0x000070f8 001b1e0c 00e20e00 23721b0f 17000080 ........#r......
+  0x00007108 26000000 00e40f08 2372260e 17000000 &.......#r&.....
+  0x00007118 16000000 00e40f00 81790e28 06a00000 .........y.(....
+  0x00007128 001b1e0c 00280f00 81791628 06e00000 .....(...y.(....
+  0x00007138 001b1e0c 00620f00 23721a14 12000000 .....b..#r......
+  0x00007148 1a000000 00c48f00 23721c14 13000000 ........#r......
+  0x00007158 1c000000 00e40f08 23721412 1e000000 ........#r......
+  0x00007168 06000000 00e44f0c 23721e13 1e000000 ......O.#r......
+  0x00007178 09000000 00e40f00 23720915 12000000 ........#r......
+  0x00007188 1c000000 00e40f04 23720615 13000000 ........#r......
+  0x00007198 1a010000 00e40f00 23721c12 0e000000 ........#r......
+  0x000071a8 18000000 00c40f01 23721a13 1f000080 ........#r......
+  0x000071b8 14000000 00e40f0c 23720e13 0e000000 ........#r......
+  0x000071c8 19000000 00e20f04 81791428 06200100 .........y.(. ..
+  0x000071d8 001b1e0c 00a20e00 23721f12 1f000000 ........#r......
+  0x000071e8 1e000000 00e40f04 23721e12 16000000 ........#r......
+  0x000071f8 02000000 00e20f0a 81791828 06600100 .........y.(.`..
+  0x00007208 001b1e0c 00e20e00 23722013 16000000 ........#r .....
+  0x00007218 20000000 00e40f04 23720213 0f000080  .......#r......
+  0x00007228 1c000000 00c40f00 23721c12 0f000000 ........#r......
+  0x00007238 0e000000 00e40f04 81790e28 06a00100 .........y.(....
+  0x00007248 001b1e0c 00220f00 23721d13 17000080 ....."..#r......
+  0x00007258 1e000000 00e40f0c 23721e12 17000000 ........#r......
+  0x00007268 20000000 00e40f04 81791628 06e00100  ........y.(....
+  0x00007278 001b1e0c 00620f00 23720c12 14000000 .....b..#r......
+  0x00007288 0c000000 00e44f08 23722213 14000000 ......O.#r".....
+  0x00007298 22000000 00c40f00 23721412 18000000 ".......#r......
+  0x000072a8 07000000 00e48f08 23720713 15000080 ........#r......
+  0x000072b8 0c000000 00e40f04 23722013 18000000 ........#r .....
+  0x000072c8 24000000 00e40f00 25762408 00580000 $.......%v$..X..
+  0x000072d8 03028e07 00c80f00 23720c12 0e000000 ........#r......
+  0x000072e8 0d000000 00e40f0d 23720013 0e000000 ........#r......
+  0x000072f8 00000000 00e40f04 23721812 15000000 ........#r......
+  0x00007308 22000000 00e40f04 23720812 16000000 ".......#r......
+  0x00007318 1b000000 00e40f0a 23722213 16000000 ........#r".....
+  0x00007328 26000000 00e40f04 23722113 19000080 &.......#r!.....
+  0x00007338 14000000 00c40f00 23722012 19000000 ........#r .....
+  0x00007348 20000000 00e20f04 81791428 06680000  ........y.(.h..
+  0x00007358 001b1e0c 00a20e00 23721913 0f000080 ........#r......
+  0x00007368 0c000000 00e40f0c 23720012 0f000000 ........#r......
+  0x00007378 00000000 00e20f04 81790c24 06000000 .........y.$....
+  0x00007388 001b1e0c 00a20e00 23721b13 17000080 ........#r......
+  0x00007398 08000000 00e40f08 23722212 17000000 ........#r".....
+  0x000073a8 22000000 00e20f00 81790e28 06280000 "........y.(.(..
+  0x000073b8 001b1e0c 00e80e00 81791228 06a80000 .........y.(....
+  0x000073c8 001b1e0c 00280f00 81791628 06e80000 .....(...y.(....
+  0x000073d8 001b1e0c 00620f00 2372230d 14000000 .....b..#r#.....
+  0x000073e8 1f000000 00c44f00 2372090e 0d000000 ......O.#r......
+  0x000073f8 09000000 00e48f04 2372060e 0c000000 ........#r......
+  0x00007408 06000000 00e40f00 2372020c 12000000 ........#r......
+  0x00007418 02000000 00e40f0d 23721c0d 12000000 ........#r......
+  0x00007428 1c000000 00e40f00 23721f0f 0c000000 ........#r......
+  0x00007438 09000000 00e40f00 23721a0c 14000000 ........#r......
+  0x00007448 1a000000 00e20f00 81790828 06280100 .........y.(.(..
+  0x00007458 001b1e0c 00a20e00 2372020d 13000080 ........#r......
+  0x00007468 02000000 00c40f00 23721c0c 13000000 ........#r......
+  0x00007478 1c000000 00e40f04 2372060f 0d000000 ........#r......
+  0x00007488 06010000 00e20f00 81791228 06680100 .........y.(.h..
+  0x00007498 001b1e0c 00e20e00 2372140c 16000000 ........#r......
+  0x000074a8 1d000000 00c60f02 81790e28 06a80100 .........y.(....
+  0x000074b8 001b1e0c 00220f00 23721e0d 16000000 ....."..#r......
+  0x000074c8 1e000000 00e40f04 23721a0d 15000080 ........#r......
+  0x000074d8 1a000000 00e40f0c 2372230c 15000000 ........#r#.....
+  0x000074e8 23000000 00e40f04 2372160d 17000080 #.......#r......
+  0x000074f8 14000000 00e40f08 81791428 06e80100 .........y.(....
+  0x00007508 001b1e0c 00620f00 2372170c 17000000 .....b..#r......
+  0x00007518 1e000000 00c40f00 25762604 00580000 ........%v&..X..
+  0x00007528 03028e07 00c80f00 23721e0c 08000000 ........#r......
+  0x00007538 07000000 00e44f0c 2372180d 08000000 ......O.#r......
+  0x00007548 18000000 00e40f04 2372080c 12000000 ........#r......
+  0x00007558 21000000 00e48f0c 2372200d 12000000 !.......#r .....
+  0x00007568 20000000 00e40f04 2372120c 0e000000  .......#r......
+  0x00007578 19000000 00e40f01 2372070d 09000080 ........#r......
+  0x00007588 1e000000 00c40f00 23720e0d 0e000000 ........#r......
+  0x00007598 00000000 00e40f04 23721d0d 0f000080 ........#r......
+  0x000075a8 12000000 00e40f04 2372120c 14000000 ........#r......
+  0x000075b8 1b000000 00e40f0e 23721e0d 14000000 ........#r......
+  0x000075c8 22000000 00e40f04 2372180c 09000000 ".......#r......
+  0x000075d8 18000000 00e40f00 2372190d 13000080 ........#r......
+  0x000075e8 08000000 00c40f00 2372000c 13000000 ........#r......
+  0x000075f8 20000000 00e20f04 81790828 06300000  ........y.(.0..
+  0x00007608 001b1e0c 00a20e00 2372040c 0f000000 ........#r......
+  0x00007618 0e000000 00e40f04 23721b0d 15000080 ........#r......
+  0x00007628 12000000 00e20f08 81790e26 06000000 .........y.&....
+  0x00007638 001b1e0c 00a20e00 23721e0c 15000000 ........#r......
+  0x00007648 1e000000 00c60f00 81790c28 06700000 .........y.(.p..
+  0x00007658 001b1e0c 00e80e00 81791228 06b00000 .........y.(....
+  0x00007668 001b1e0c 00280f00 81791428 06f00000 .....(...y.(....
+  0x00007678 001b1e0c 00620f00 23720608 0e000000 .....b..#r......
+  0x00007688 06000000 00e44f04 23721f08 0f000000 ......O.#r......
+  0x00007698 1f000000 00c40f00 23721a0e 0c000000 ........#r......
+  0x000076a8 1a000000 00e48f0c 2372230f 0c000000 ........#r#.....
+  0x000076b8 23000000 00e40f04 2372080e 12000000 #.......#r......
+  0x000076c8 02000000 00e40f0d 2372020f 0d000080 ........#r......
+  0x000076d8 1a000000 00e40f0c 2372200f 12000000 ........#r .....
+  0x000076e8 1c000000 00e40f00 23721a0e 0d000000 ........#r......
+  0x000076f8 23000000 00c40f00 23720609 0f000000 #.......#r......
+  0x00007708 06010000 00e20f04 81790c28 06300100 .........y.(.0..
+  0x00007718 001b1e0c 00a20e00 23721f09 0e000000 ........#r......
+  0x00007728 1f000000 00e40f00 23721c0f 13000080 ........#r......
+  0x00007738 08000000 00e40f0c 81790828 06700100 .........y.(.p..
+  0x00007748 001b1e0c 00e20e00 2372160e 14000000 ........#r......
+  0x00007758 16000000 00e40f0e 2372170f 14000000 ........#r......
+  0x00007768 17000000 00e40f00 2372200e 13000000 ........#r .....
+  0x00007778 20000000 00c40f00 2372160f 15000080  .......#r......
+  0x00007788 16000000 00e20f08 81791228 06b00100 .........y.(....
+  0x00007798 001b1e0c 00220f00 2372170e 15000000 ....."..#r......
+  0x000077a8 17000000 00c60f00 81791428 06f00100 .........y.(....
+  0x000077b8 001b1e0c 00620f00 25763005 00580000 .....b..%v0..X..
+  0x000077c8 03028e07 00c80f00 2372220e 0c000000 ........#r".....
+  0x000077d8 07000000 00e44f0c 2372180f 0c000000 ......O.#r......
+  0x000077e8 18000000 00e40f04 23720c0e 08000000 ........#r......
+  0x000077f8 19000000 00e48f08 2372080f 08000000 ........#r......
+  0x00007808 00000000 00e40f04 2372000f 0d000080 ........#r......
+  0x00007818 22000000 00e40f04 2372070f 09000080 ".......#r......
+  0x00007828 0c000000 00c40f00 2372220e 09000000 ........#r".....
+  0x00007838 08000000 00e40f04 2372080e 12000000 ........#r......
+  0x00007848 1d000000 00e40f0d 2372040f 12000000 ........#r......
+  0x00007858 04000000 00e40f04 23720c0e 14000000 ........#r......
+  0x00007868 1b000000 00e40f0e 23721e0f 14000000 ........#r......
+  0x00007878 1e000000 00e40f00 2372180e 0d000000 ........#r......
+  0x00007888 18000000 00c40f00 2372190f 13000080 ........#r......
+  0x00007898 08000000 00e40f0c 2372140e 13000000 ........#r......
+  0x000078a8 04000000 00e20f00 81790830 06000000 .........y.0....
+  0x000078b8 001b1e0c 00a20e00 2372210f 15000080 ........#r!.....
+  0x000078c8 0c000000 00c60f00 81790428 06380000 .........y.(.8..
+  0x000078d8 001b1e0c 00a80e00 81790c28 06780000 .........y.(.x..
+  0x000078e8 001b1e0c 00e20e00 2372150e 15000000 ........#r......
+  0x000078f8 1e000000 00c60f00 81790e28 06b80000 .........y.(....
+  0x00007908 001b1e0c 00280f00 81791228 06f80000 .....(...y.(....
+  0x00007918 001b1e0c 00620f00 23720304 09000000 .....b..#r......
+  0x00007928 1f000000 00e44f04 23720604 08000000 ......O.#r......
+  0x00007938 06000000 00e40f00 23721a09 0c000000 ........#r......
+  0x00007948 1a000000 00e48f08 23720408 0c000000 ........#r......
+  0x00007958 02000000 00c40f00 23720305 08000000 ........#r......
+  0x00007968 03000000 00e40f04 23720205 09000000 ........#r......
+  0x00007978 06010000 00e40f00 23720508 0d000000 ........#r......
+  0x00007988 1a000000 00e40f0c 23720608 0e000000 ........#r......
+  0x00007998 1c000000 00e20f0d 81791a28 06380100 .........y.(.8..
+  0x000079a8 001b1e0c 00a20e00 23722009 0e000000 ........#r .....
+  0x000079b8 20000000 00e40f04 23720e08 12000000  .......#r......
+  0x000079c8 16000000 00e20f02 81791c28 06f80100 .........y.(....
+  0x000079d8 001b1e0c 00e20e00 23720409 0d000080 ........#r......
+  0x000079e8 04000000 00c40f00 23721209 12000000 ........#r......
+  0x000079f8 17000000 00e20f04 81790c28 06b80100 .........y.(....
+  0x00007a08 001b1e0c 00280f00 81791628 06780100 .....(...y.(.x..
+  0x00007a18 001b1e0c 00620f00 23720609 0f000080 .....b..#r......
+  0x00007a28 06000000 00e40f04 23720e09 13000080 ........#r......
+  0x00007a38 0e000000 00e20f00 8679000a 02000000 .........y......
+  0x00007a48 061b100c 00e80f00 86790010 04000000 .........y......
+  0x00007a58 061b100c 00e20f00 23720008 1a000000 ........#r......
+  0x00007a68 00000000 00c44f00 23721a09 1a000000 ......O.#r......
+  0x00007a78 18000000 00e40f04 23721509 1c000000 ........#r......
+  0x00007a88 15000000 00e48f0c 23721c08 1c000000 ........#r......
+  0x00007a98 21000000 00e40f04 23721409 0c000000 !.......#r......
+  0x00007aa8 14000000 00e40f09 23720c08 0c000000 ........#r......
+  0x00007ab8 19000000 00e40f04 23721808 16000000 ........#r......
+  0x00007ac8 07000000 00c40f02 23722209 16000000 ........#r".....
+  0x00007ad8 22000000 00e40f04 23720708 0f000000 ".......#r......
+  0x00007ae8 20000000 00e40f04 23720f08 13000000  .......#r......
+  0x00007af8 12000000 00e40f04 23721308 1b000000 ........#r......
+  0x00007b08 1a000000 00e40f0c 23721209 1b000080 ........#r......
+  0x00007b18 00000000 00e40f00 23721b08 17000000 ........#r......
+  0x00007b28 22000000 00c40f00 23721a09 17000080 ".......#r......
+  0x00007b38 18000000 00e20f04 8679002e 06000000 .........y......
+  0x00007b48 061b100c 00e20f00 23721708 0d000000 ........#r......
+  0x00007b58 14000000 00e40f0c 23721609 0d000080 ........#r......
+  0x00007b68 0c000000 00e20f04 8679002c 0e000000 .........y.,....
+  0x00007b78 061b100c 00e20f00 23721508 1d000000 ........#r......
+  0x00007b88 15000000 00e40f08 23721409 1d000080 ........#r......
+  0x00007b98 1c000000 00e20f00 8679002a 12000000 .........y.*....
+  0x00007ba8 061b100c 00e80f00 86790024 1a000000 .........y.$....
+  0x00007bb8 061b100c 00e80f00 86790026 16000000 .........y.&....
+  0x00007bc8 061b100c 00e80f00 86790030 14000000 .........y.0....
+  0x00007bd8 061b100c 00e20f00 4d790000 00000000 ........My......
+  0x00007be8 00008003 00ea0f00 47790000 f0ffffff ........Gy......
+  0x00007bf8 ffff8303 00c00f00 18790000 00000000 .........y......
+  0x00007c08 00000000 00c00f00 18790000 00000000 .........y......
+  0x00007c18 00000000 00c00f00 18790000 00000000 .........y......
+  0x00007c28 00000000 00c00f00 18790000 00000000 .........y......
+  0x00007c38 00000000 00c00f00 18790000 00000000 .........y......
+  0x00007c48 00000000 00c00f00 18790000 00000000 .........y......
+  0x00007c58 00000000 00c00f00 18790000 00000000 .........y......
+  0x00007c68 00000000 00c00f00 18790000 00000000 .........y......
+  0x00007c78 00000000 00c00f00 18790000 00000000 .........y......
+  0x00007c88 00000000 00c00f00 18790000 00000000 .........y......
+  0x00007c98 00000000 00c00f00 027a0100 000a0000 .........z......
+  0x00007ca8 000f0000 00e40f00 027a0200 005e0000 .........z...^..
+  0x00007cb8 000f0000 00e20f00 b97a0600 00460000 .........z...F..
+  0x00007cc8 000a0000 00e20f00 027a0300 005f0000 .........z..._..
+  0x00007cd8 000f0000 00ca0f00 81790402 06080000 .........y......
+  0x00007ce8 00191e0c 00a80000 81790502 06000000 .........y......
+  0x00007cf8 00191e0c 00e20000 b97a0400 00000000 .........z......
+  0x00007d08 00080000 00e40f00 9978043f 01000000 .........x.?....
+  0x00007d18 04160108 00e20f00 19790000 00000000 .........y......
+  0x00007d28 00250000 00680e00 19790900 00000000 .%...h...y......
+  0x00007d38 00210000 00640e00 247a0000 00000000 .!...d..$z......
+  0x00007d48 09028e07 00ca2f00 197803ff 1f000000 ....../..x......
+  0x00007d58 00140100 00e41f00 12720700 04000000 .........r......
+  0x00007d68 fffc8e07 00e44f0c 10720b05 04000000 ......O..r......
+  0x00007d78 ffe0ff07 00e48f00 12720500 05000000 .........r......
+  0x00007d88 fffc8e07 00e40f04 0c720000 07000000 .........r......
+  0x00007d98 7052f003 00e40f04 12720600 0b000000 pR.......r......
+  0x00007da8 fffc8e07 00c40f00 0c720000 05000000 .........r......
+  0x00007db8 70527000 00c80f00 0c720000 06000000 pRp......r......
+  0x00007dc8 70527200 00e40f0c 0c7a0000 005c0000 pRr......z...\..
+  0x00007dd8 7060f003 00e40f00 0c720005 07000000 p`.......r......
+  0x00007de8 7052f200 00e40f00 0c7a0003 005d0000 pR.......z...]..
+  0x00007df8 0061f003 00e40f00 0c720005 06000000 .a.......r......
+  0x00007e08 7052f200 00e40f00 0c7c0009 04000000 pR.......|......
+  0x00007e18 7010700c 00c40f00 0c720007 06000000 p.p......r......
+  0x00007e28 7052f200 00c80f00 1c780000 00000000 pR.......x......
+  0x00007e38 70307000 00da0f00 4d890000 00000000 p0p.....M.......
+  0x00007e48 00008003 00ea0f00 117a0800 00580000 .........z...X..
+  0x00007e58 ff188007 00e40f04 027a0e00 005a0000 .........z...Z..
+  0x00007e68 000f0000 00e40f00 027a0f00 005b0000 .........z...[..
+  0x00007e78 000f0000 00e40f00 117a0900 00590000 .........z...Y..
+  0x00007e88 031c0f00 00c60f00 8179020e 06000000 .........y......
+  0x00007e98 001b1e0c 00a80e00 81791408 06000000 .........y......
+  0x00007ea8 001b1e0c 00a80e00 8179100e 06200000 .........y... ..
+  0x00007eb8 001b1e0c 00e80e00 81790a0e 06400000 .........y...@..
+  0x00007ec8 001b1e0c 00280f00 8179160e 06600000 .....(...y...`..
+  0x00007ed8 001b1e0c 00620f00 357400ff 08000000 .....b..5t......
+  0x00007ee8 ff010000 00c60f00 8179120e 06280000 .........y...(..
+  0x00007ef8 001b1e0c 006e0f00 25760c05 00580000 .....n..%v...X..
+  0x00007f08 00028e07 00c80f00 20721903 15000000 ........ r......
+  0x00007f18 00004000 00e44f04 20720403 14000000 ..@...O. r......
+  0x00007f28 00004000 00e40f00 20720315 11000000 ..@..... r......
+  0x00007f38 00004000 00e48f0c 20720514 11000000 ..@..... r......
+  0x00007f48 00004000 00e40f04 20721115 0b000000 ..@..... r......
+  0x00007f58 00004000 00e40f09 20721814 0b000000 ..@..... r......
+  0x00007f68 00004000 00c40f00 23721902 14000000 ..@.....#r......
+  0x00007f78 19080000 00e40f04 23720402 15000000 ........#r......
+  0x00007f88 04000000 00e40f00 23720214 10000000 ........#r......
+  0x00007f98 03080000 00e40f0c 23720515 10000000 ........#r......
+  0x00007fa8 05000000 00e40f04 23720314 0a000000 ........#r......
+  0x00007fb8 11080000 00e40f08 23721815 0a000000 ........#r......
+  0x00007fc8 18000000 00e20f04 8179100c 06000000 .........y......
+  0x00007fd8 001b1e0c 00a20e00 20721b15 17000000 ........ r......
+  0x00007fe8 00004000 00c60f02 81790a0e 06080000 ..@......y......
+  0x00007ff8 001b1e0c 00a20e00 20721a14 17000000 ........ r......
+  0x00008008 00004000 00e40f04 23721b14 16000000 ..@.....#r......
+  0x00008018 1b080000 00e40f08 23721a15 16000000 ........#r......
+  0x00008028 1a000000 00e40f00 8179140e 06480000 .........y...H..
+  0x00008038 001b1e0c 00e80e00 8179160e 06680000 .........y...h..
+  0x00008048 001b1e0c 00220f00 23721c0a 10000000 ....."..#r......
+  0x00008058 19000000 00c44f00 2372040a 11000000 ......O.#r......
+  0x00008068 04000000 00e40f08 23720a10 12000000 ........#r......
+  0x00008078 02000000 00e40f00 2372020b 11000000 ........#r......
+  0x00008088 1c010000 00e40f04 23720b0b 10000000 ........#r......
+  0x00008098 04000000 00e40f00 23720411 13000080 ........#r......
+  0x000080a8 0a000000 00e40f04 23720511 12000000 ........#r......
+  0x000080b8 05000000 00c40f00 23720a10 14000000 ........#r......
+  0x000080c8 03000000 00e48f0c 23721310 13000000 ........#r......
+  0x000080d8 05000000 00e40f00 23720311 15000080 ........#r......
+  0x000080e8 0a000000 00e40f04 23720511 14000000 ........#r......
+  0x000080f8 18000000 00e40f00 25761c07 00580000 ........%v...X..
+  0x00008108 00028e07 00c80f00 23721210 16000000 ........#r......
+  0x00008118 1b000000 00e20f0d 8179181c 06000000 .........y......
+  0x00008128 001b1e0c 00a20e00 23720a11 16000000 ........#r......
+  0x00008138 1a000000 00e40f04 23720510 15000000 ........#r......
+  0x00008148 05000000 00e20f04 81791a0e 06300000 .........y...0..
+  0x00008158 001b1e0c 00a20e00 23720711 17000080 ........#r......
+  0x00008168 12000000 00e40f08 23720a10 17000000 ........#r......
+  0x00008178 0a000000 00e20f00 8179140e 06100000 .........y......
+  0x00008188 001b1e0c 00e80e00 8179100e 06500000 .........y...P..
+  0x00008198 001b1e0c 00280f00 8179160e 06700000 .....(...y...p..
+  0x000081a8 001b1e0c 00620f00 25761e06 00580000 .....b..%v...X..
+  0x000081b8 00028e07 00c80f00 23720418 1a000000 ........#r......
+  0x000081c8 04000000 00e44f08 23721319 1a000000 ......O.#r......
+  0x000081d8 13000000 00e40f04 23720214 18000000 ........#r......
+  0x000081e8 02000000 00e48f04 23720b14 19000000 ........#r......
+  0x000081f8 0b000000 00e40f00 23721218 10000000 ........#r......
+  0x00008208 03000000 00e40f09 23720519 10000000 ........#r......
+  0x00008218 05000000 00c40f00 23720018 16000000 ........#r......
+  0x00008228 07000000 00e40f0e 23721619 16000000 ........#r......
+  0x00008238 0a000000 00e20f04 8179060e 06180000 .........y......
+  0x00008248 001b1e0c 00a20e00 23720319 11000080 ........#r......
+  0x00008258 12000000 00e40f00 23720215 19000000 ........#r......
+  0x00008268 02010000 00e40f04 23721118 11000000 ........#r......
+  0x00008278 05000000 00e40f00 23721515 18000000 ........#r......
+  0x00008288 0b000000 00c40f00 23720419 1b000080 ........#r......
+  0x00008298 04000000 00e20f04 81790a1e 06000000 .........y......
+  0x000082a8 001b1e0c 00a20e00 23720519 17000080 ........#r......
+  0x000082b8 00000000 00e40f00 23721b18 1b000000 ........#r......
+  0x000082c8 13000000 00e40f04 23720018 17000000 ........#r......
+  0x000082d8 16000000 00e20f00 8179120e 06380000 .........y...8..
+  0x000082e8 001b1e0c 00e80e00 8179160e 06580000 .........y...X..
+  0x000082f8 001b1e0c 00280f00 8179180e 06780000 .....(...y...x..
+  0x00008308 001b1e0c 00620f00 23721506 0b000000 .....b..#r......
+  0x00008318 15000000 00c44f00 23720206 0a000000 ......O.#r......
+  0x00008328 02000000 00e40f00 23721b0b 12000000 ........#r......
+  0x00008338 1b000000 00e48f0c 2372040a 12000000 ........#r......
+  0x00008348 04000000 00e40f04 2372110b 16000000 ........#r......
+  0x00008358 11000000 00e40f0d 2372160a 16000000 ........#r......
+  0x00008368 03000000 00e40f00 2372000b 18000000 ........#r......
+  0x00008378 00000000 00c40f02 2372180a 18000000 ........#r......
+  0x00008388 05000000 00e40f04 23721507 0a000000 ........#r......
+  0x00008398 15000000 00e40f04 23721407 0b000000 ........#r......
+  0x000083a8 02010000 00e40f00 2372070a 13000000 ........#r......
+  0x000083b8 1b000000 00e40f0c 2372060b 13000080 ........#r......
+  0x000083c8 04000000 00e40f00 2372110a 17000000 ........#r......
+  0x000083d8 11000000 00c40f00 2372100b 17000080 ........#r......
+  0x000083e8 16000000 00e40f04 2372030a 19000000 ........#r......
+  0x000083f8 00000000 00e40f08 2372020b 19000080 ........#r......
+  0x00008408 18000000 00e20f00 86790008 14000000 .........y......
+  0x00008418 061b100c 00e80f00 8679000c 06000000 .........y......
+  0x00008428 061b100c 00e80f00 8679001c 10000000 .........y......
+  0x00008438 061b100c 00e80f00 8679001e 02000000 .........y......
+  0x00008448 061b100c 00e20f00 4d790000 00000000 ........My......
+  0x00008458 00008003 00ea0f00 47790000 f0ffffff ........Gy......
+  0x00008468 ffff8303 00c00f00 18790000 00000000 .........y......
   0x00008478 00000000 00c00f00 18790000 00000000 .........y......
-  0x00008488 00000000 00c00f00 027a0100 000a0000 .........z......
-  0x00008498 000f0000 00e40f00 027a0300 005f0000 .........z..._..
-  0x000084a8 000f0000 00e20f00 b97a0600 00460000 .........z...F..
-  0x000084b8 000a0000 00e20f00 027a0200 005e0000 .........z...^..
-  0x000084c8 000f0000 00ca0f00 81790302 06000000 .........y......
-  0x000084d8 00191e0c 00a20e00 b97a0400 00000000 .........z......
-  0x000084e8 00080000 00e40f00 9978043f 01000000 .........x.?....
-  0x000084f8 04160108 00e20f00 19790000 00000000 .........y......
-  0x00008508 00250000 00280e00 19790700 00000000 .%...(...y......
-  0x00008518 00210000 00240e00 247a0000 00000000 .!...$..$z......
-  0x00008528 07028e07 00ca1f00 0c7a0000 005c0000 .........z...\..
-  0x00008538 7060f003 00e40f00 197809ff 1f000000 p`.......x......
-  0x00008548 00140100 00c80f00 0c7a0009 005d0000 .........z...]..
-  0x00008558 0061f003 00c80f00 0c7c0007 04000000 .a.......|......
-  0x00008568 70647008 00e40f00 12720500 03000000 pdp......r......
-  0x00008578 fffc8e07 00c84f00 0c720000 05000000 ......O..r......
-  0x00008588 70267000 00da0f00 4d090000 00000000 p&p.....M.......
-  0x00008598 00008003 00ea0f00 117a0200 00580000 .........z...X..
-  0x000085a8 ff188007 00e20f04 357404ff 08000000 ........5t......
-  0x000085b8 ff010000 00e20f00 027a1200 005a0000 .........z...Z..
-  0x000085c8 000f0000 00e40f00 027a1300 005b0000 .........z...[..
-  0x000085d8 000f0000 00e40f00 117a0300 00590000 .........z...Y..
-  0x000085e8 091c0f00 00c60f00 81791012 06000000 .........y......
-  0x000085f8 001b1e0c 00a80e00 81790e02 06000000 .........y......
-  0x00008608 001b1e0c 00a20e00 25760405 00580000 ........%v...X..
-  0x00008618 04028e07 00c60f00 81790c12 06100000 .........y......
-  0x00008628 001b1e0c 00e80e00 81790812 06080000 .........y......
-  0x00008638 001b1e0c 00280f00 81790604 06000000 .....(...y......
-  0x00008648 001b1e0c 00280f00 81790a12 06180000 .....(...y......
-  0x00008658 001b1e0c 00620f00 20720010 0f000000 .....b.. r......
-  0x00008668 00004000 00c44f00 20721511 0f000000 ..@...O. r......
-  0x00008678 00004000 00e40f00 2072140e 0d000000 ..@..... r......
-  0x00008688 00004000 00e48f08 20720d0f 0d000000 ..@..... r......
-  0x00008698 00004000 00e40f00 23720011 0e000000 ..@.....#r......
-  0x000086a8 00000000 00e40f08 23721510 0e000000 ........#r......
-  0x000086b8 15080000 00e40f00 2372140f 0c000000 ........#r......
-  0x000086c8 14000000 00c40f00 23720d0e 0c000000 ........#r......
-  0x000086d8 0d080000 00e40f00 23720c09 06000000 ........#r......
-  0x000086e8 00000000 00e40f09 23720008 06000000 ........#r......
-  0x000086f8 15000000 00e40f00 23721407 0a000000 ........#r......
-  0x00008708 14000000 00e40f0a 23720a06 0a000000 ........#r......
-  0x00008718 0d000000 00e40f00 23720d08 07000000 ........#r......
-  0x00008728 0c000000 00c40f00 23720c09 07000000 ........#r......
-  0x00008738 00010000 00e40f00 23720906 0b000000 ........#r......
-  0x00008748 14000000 00e40f08 23720807 0b000080 ........#r......
-  0x00008758 0a000000 00e20f00 86790002 0c000000 .........y......
-  0x00008768 061b100c 00e80f00 86790004 08000000 .........y......
-  0x00008778 061b100c 00e20f00 4d790000 00000000 ........My......
-  0x00008788 00008003 00ea0f00 47790000 f0ffffff ........Gy......
-  0x00008798 ffff8303 00c00f00 18790000 00000000 .........y......
-  0x000087a8 00000000 00c00f00 18790000 00000000 .........y......
-  0x000087b8 00000000 00c00f00 18790000 00000000 .........y......
-  0x000087c8 00000000 00c00f00 18790000 00000000 .........y......
-  0x000087d8 00000000 00c00f00 18790000 00000000 .........y......
-  0x000087e8 00000000 00c00f00 18790000 00000000 .........y......
-  0x000087f8 00000000 00c00f00 18790000 00000000 .........y......
-  0x00008808 00000000 00c00f00 18790000 00000000 .........y......
-  0x00008818 00000000 00c00f00 18790000 00000000 .........y......
-  0x00008828 00000000 00c00f00 18790000 00000000 .........y......
+  0x00008488 00000000 00c00f00 18790000 00000000 .........y......
+  0x00008498 00000000 00c00f00 18790000 00000000 .........y......
+  0x000084a8 00000000 00c00f00 18790000 00000000 .........y......
+  0x000084b8 00000000 00c00f00 18790000 00000000 .........y......
+  0x000084c8 00000000 00c00f00 18790000 00000000 .........y......
+  0x000084d8 00000000 00c00f00 18790000 00000000 .........y......
+  0x000084e8 00000000 00c00f00 18790000 00000000 .........y......
+  0x000084f8 00000000 00c00f00 18790000 00000000 .........y......
+  0x00008508 00000000 00c00f00 18790000 00000000 .........y......
+  0x00008518 00000000 00c00f00 027a0100 000a0000 .........z......
+  0x00008528 000f0000 00e40f00 027a0300 005f0000 .........z..._..
+  0x00008538 000f0000 00e20f00 b97a0600 00460000 .........z...F..
+  0x00008548 000a0000 00e20f00 027a0200 005e0000 .........z...^..
+  0x00008558 000f0000 00ca0f00 81790302 06000000 .........y......
+  0x00008568 00191e0c 00a20e00 b97a0400 00000000 .........z......
+  0x00008578 00080000 00e40f00 9978043f 01000000 .........x.?....
+  0x00008588 04160108 00e20f00 19790000 00000000 .........y......
+  0x00008598 00250000 00280e00 19790700 00000000 .%...(...y......
+  0x000085a8 00210000 00240e00 247a0000 00000000 .!...$..$z......
+  0x000085b8 07028e07 00ca1f00 0c7a0000 005c0000 .........z...\..
+  0x000085c8 7060f003 00e40f00 197809ff 1f000000 p`.......x......
+  0x000085d8 00140100 00c80f00 0c7a0009 005d0000 .........z...]..
+  0x000085e8 0061f003 00c80f00 0c7c0007 04000000 .a.......|......
+  0x000085f8 70647008 00e40f00 12720500 03000000 pdp......r......
+  0x00008608 fffc8e07 00c84f00 0c720000 05000000 ......O..r......
+  0x00008618 70267000 00da0f00 4d090000 00000000 p&p.....M.......
+  0x00008628 00008003 00ea0f00 117a0200 00580000 .........z...X..
+  0x00008638 ff188007 00e20f04 357404ff 08000000 ........5t......
+  0x00008648 ff010000 00e20f00 027a1200 005a0000 .........z...Z..
+  0x00008658 000f0000 00e40f00 027a1300 005b0000 .........z...[..
+  0x00008668 000f0000 00e40f00 117a0300 00590000 .........z...Y..
+  0x00008678 091c0f00 00c60f00 81791012 06000000 .........y......
+  0x00008688 001b1e0c 00a80e00 81790e02 06000000 .........y......
+  0x00008698 001b1e0c 00a20e00 25760405 00580000 ........%v...X..
+  0x000086a8 04028e07 00c60f00 81790c12 06100000 .........y......
+  0x000086b8 001b1e0c 00e80e00 81790812 06080000 .........y......
+  0x000086c8 001b1e0c 00280f00 81790604 06000000 .....(...y......
+  0x000086d8 001b1e0c 00280f00 81790a12 06180000 .....(...y......
+  0x000086e8 001b1e0c 00620f00 20720010 0f000000 .....b.. r......
+  0x000086f8 00004000 00c44f00 20721511 0f000000 ..@...O. r......
+  0x00008708 00004000 00e40f00 2072140e 0d000000 ..@..... r......
+  0x00008718 00004000 00e48f08 20720d0f 0d000000 ..@..... r......
+  0x00008728 00004000 00e40f00 23720011 0e000000 ..@.....#r......
+  0x00008738 00000000 00e40f08 23721510 0e000000 ........#r......
+  0x00008748 15080000 00e40f00 2372140f 0c000000 ........#r......
+  0x00008758 14000000 00c40f00 23720d0e 0c000000 ........#r......
+  0x00008768 0d080000 00e40f00 23720c09 06000000 ........#r......
+  0x00008778 00000000 00e40f09 23720008 06000000 ........#r......
+  0x00008788 15000000 00e40f00 23721407 0a000000 ........#r......
+  0x00008798 14000000 00e40f0a 23720a06 0a000000 ........#r......
+  0x000087a8 0d000000 00e40f00 23720d08 07000000 ........#r......
+  0x000087b8 0c000000 00c40f00 23720c09 07000000 ........#r......
+  0x000087c8 00010000 00e40f00 23720906 0b000000 ........#r......
+  0x000087d8 14000000 00e40f08 23720807 0b000080 ........#r......
+  0x000087e8 0a000000 00e20f00 86790002 0c000000 .........y......
+  0x000087f8 061b100c 00e80f00 86790004 08000000 .........y......
+  0x00008808 061b100c 00e20f00 4d790000 00000000 ........My......
+  0x00008818 00008003 00ea0f00 47790000 f0ffffff ........Gy......
+  0x00008828 ffff8303 00c00f00 18790000 00000000 .........y......
   0x00008838 00000000 00c00f00 18790000 00000000 .........y......
   0x00008848 00000000 00c00f00 18790000 00000000 .........y......
   0x00008858 00000000 00c00f00 18790000 00000000 .........y......
   0x00008868 00000000 00c00f00 18790000 00000000 .........y......
   0x00008878 00000000 00c00f00 18790000 00000000 .........y......
-  0x00008888 00000000 00c00f00 00000000 00000000 ................
-  0x00008898 00000000 00000000 00000000 00000000 ................
-  0x000088a8 00000000 00000000 00000000 00000000 ................
-  0x000088b8 00000000 00000000 00000000 00000000 ................
-  0x000088c8 00000000 00000000 01000000 03000000 ................
-  0x000088d8 00000000 00000000 00000000 00000000 ................
-  0x000088e8 40000000 00000000 70030000 00000000 @.......p.......
-  0x000088f8 00000000 00000000 01000000 00000000 ................
-  0x00008908 00000000 00000000 0b000000 03000000 ................
-  0x00008918 00000000 00000000 00000000 00000000 ................
-  0x00008928 b0030000 00000000 e1030000 00000000 ................
-  0x00008938 00000000 00000000 01000000 00000000 ................
-  0x00008948 00000000 00000000 13000000 02000000 ................
-  0x00008958 00000000 00000000 00000000 00000000 ................
-  0x00008968 98070000 00000000 38010000 00000000 ........8.......
-  0x00008978 02000000 0a000000 08000000 00000000 ................
-  0x00008988 18000000 00000000 15030000 01000000 ................
-  0x00008998 00000000 00000000 00000000 00000000 ................
-  0x000089a8 d0080000 00000000 50010000 00000000 ........P.......
-  0x000089b8 00000000 00000000 01000000 00000000 ................
-  0x000089c8 00000000 00000000 29000000 00000070 ........)......p
-  0x000089d8 00000000 00000000 00000000 00000000 ................
-  0x000089e8 200a0000 00000000 90000000 00000000  ...............
-  0x000089f8 03000000 00000000 04000000 00000000 ................
-  0x00008a08 00000000 00000000 5d000000 00000070 ........]......p
-  0x00008a18 40000000 00000000 00000000 00000000 @...............
-  0x00008a28 b00a0000 00000000 6c000000 00000000 ........l.......
-  0x00008a38 03000000 0f000000 04000000 00000000 ................
-  0x00008a48 00000000 00000000 51010000 00000070 ........Q......p
-  0x00008a58 40000000 00000000 00000000 00000000 @...............
-  0x00008a68 1c0b0000 00000000 6c000000 00000000 ........l.......
-  0x00008a78 03000000 10000000 04000000 00000000 ................
-  0x00008a88 00000000 00000000 49020000 00000070 ........I......p
-  0x00008a98 40000000 00000000 00000000 00000000 @...............
-  0x00008aa8 880b0000 00000000 6c000000 00000000 ........l.......
-  0x00008ab8 03000000 11000000 04000000 00000000 ................
-  0x00008ac8 00000000 00000000 45030000 01000070 ........E......p
-  0x00008ad8 00000000 00000000 00000000 00000000 ................
-  0x00008ae8 f40b0000 00000000 20000000 00000000 ........ .......
-  0x00008af8 03000000 00000000 04000000 00000000 ................
-  0x00008b08 08000000 00000000 61030000 0b000070 ........a......p
-  0x00008b18 00000000 00000000 00000000 00000000 ................
-  0x00008b28 180c0000 00000000 10000000 00000000 ................
-  0x00008b38 00000000 00000000 08000000 00000000 ................
-  0x00008b48 08000000 00000000 22030000 09000000 ........".......
-  0x00008b58 40000000 00000000 00000000 00000000 @...............
-  0x00008b68 280c0000 00000000 30000000 00000000 (.......0.......
-  0x00008b78 03000000 04000000 08000000 00000000 ................
-  0x00008b88 10000000 00000000 bb000000 01000000 ................
-  0x00008b98 42000000 00000000 00000000 00000000 B...............
-  0x00008ba8 580c0000 00000000 80010000 00000000 X...............
-  0x00008bb8 00000000 0f000000 04000000 00000000 ................
-  0x00008bc8 00000000 00000000 b1010000 01000000 ................
-  0x00008bd8 42000000 00000000 00000000 00000000 B...............
-  0x00008be8 d80d0000 00000000 80010000 00000000 ................
-  0x00008bf8 00000000 10000000 04000000 00000000 ................
-  0x00008c08 00000000 00000000 a9020000 01000000 ................
-  0x00008c18 42000000 00000000 00000000 00000000 B...............
-  0x00008c28 580f0000 00000000 80010000 00000000 X...............
-  0x00008c38 00000000 11000000 04000000 00000000 ................
-  0x00008c48 00000000 00000000 32000000 01000000 ........2.......
-  0x00008c58 06000000 00000000 00000000 00000000 ................
-  0x00008c68 00110000 00000000 001a0000 00000000 ................
-  0x00008c78 03000000 0a000034 80000000 00000000 .......4........
-  0x00008c88 00000000 00000000 25010000 01000000 ........%.......
-  0x00008c98 06000000 00000000 00000000 00000000 ................
-  0x00008ca8 002b0000 00000000 80080000 00000000 .+..............
-  0x00008cb8 03000000 0b000022 80000000 00000000 ......."........
-  0x00008cc8 00000000 00000000 1d020000 01000000 ................
-  0x00008cd8 06000000 00000000 00000000 00000000 ................
-  0x00008ce8 80330000 00000000 00040000 00000000 .3..............
-  0x00008cf8 03000000 0c000018 80000000 00000000 ................
-  0x00008d08 00000000 00000000 06000000 05000000 ................
-  0x00008d18 003c0000 00000000 00000000 00000000 .<..............
-  0x00008d28 00000000 00000000 a8000000 00000000 ................
-  0x00008d38 a8000000 00000000 08000000 00000000 ................
-  0x00008d48 01000000 05000000 580c0000 00000000 ........X.......
-  0x00008d58 00000000 00000000 00000000 00000000 ................
-  0x00008d68 282b0000 00000000 282b0000 00000000 (+......(+......
-  0x00008d78 08000000 00000000 01000000 05000000 ................
-  0x00008d88 003c0000 00000000 00000000 00000000 .<..............
-  0x00008d98 00000000 00000000 a8000000 00000000 ................
-  0x00008da8 a8000000 00000000 08000000 00000000 ................
-  0x00008db8 01000101 58000000 481f0000 00000000 ....X...H.......
-  0x00008dc8 451f0000 48000000 04000800 50000000 E...H.......P...
-  0x00008dd8 00000000 00000000 11200000 00000000 ......... ......
-  0x00008de8 00000000 00000000 9e620000 00000000 .........b......
-  0x00008df8 00000000 00000000 50000000 00000000 ........P.......
-  0x00008e08 00000000 00000000 3c0a2f2f 0300f31e ........<.//....
-  0x00008e18 0a2e7665 7273696f 6e20382e 340a2e74 ..version 8.4..t
-  0x00008e28 61726765 7420736d 5f38300a 2e616464 arget sm_80..add
-  0x00008e38 72657373 5f73697a 65203634 0a3100ff ress_size 64.1..
-  0x00008e48 31697369 626c6520 2e656e74 7279205f 1isible .entry _
-  0x00008e58 5a313961 6374696f 6e4f6e53 696e676c Z19actionOnSingl
-  0x00008e68 65517562 69745036 666c6f61 74325330 eQubitP6float2S0
-  0x00008e78 5f6d506d 280a2e70 6172616d 202e7536 _mPm(..param .u6
-  0x00008e88 34330013 115f3100 3f5f302c 3b00261f 43..._1.?_0,;.&.
-  0x00008e98 313b0027 1f323b00 27f30833 0a290a7b 1;.'.2;.'..3.).{
-  0x00008ea8 0a2e7265 67202e70 72656420 25703c36 ..reg .pred %p<6
-  0x00008eb8 3e3b1200 95663332 2025663c 34351200 >;...f32 %f<45..
-  0x00008ec8 10621200 36723c38 1100f201 36342025 .b..6r<8....64 %
-  0x00008ed8 72643c31 333e3b0a 0a0a6c64 8a00222e rd<13>;...ld..".
-  0x00008ee8 7518004f 322c205b 9000193d 305d3b44 u..O2, [...=0];D
-  0x00008ef8 001f3344 001c1f31 4400001f 3444001c ..3D...1D...4D..
-  0x00008f08 1f324400 001f3544 001c9133 5d3b0a6d .2D...5D...3];.m
-  0x00008f18 6f762e75 3401a832 2c20256e 7469642e ov.u4..2, %ntid.
-  0x00008f28 7816007c 332c2025 63746117 0044342c x..|3, %cta..D4,
-  0x00008f38 20252c00 7161642e 6c6f2e73 18002335  %,.qad.lo.s..#5
-  0x00008f48 2c340001 4f00f403 72343b0a 63767461 ,4..O...r4;.cvta
-  0x00008f58 2e746f2e 676c6f62 616cab00 21362cb1 .to.global..!6,.
-  0x00008f68 0001c400 041a0001 41004036 2c205b20 ........A.@6, [ 
-  0x00008f78 00535d3b 0a6f72ce 0124312c 5a001136 .S];.or..$1,Z..6
-  0x00008f88 5000432e 73363470 0012641c 00923b0a P.C.s64p..d...;.
-  0x00008f98 73657470 2e676560 00357031 2c1c0073 setp.ge`.5p1,..s
-  0x00008fa8 64343b0a 7368725f 0013379b 00173132 d4;.shr_..7...12
-  0x00008fb8 00001900 3370322c d6002172 377a0003 ....3p2,..!r7z..
-  0x00008fc8 6c022333 2c1c0014 70320022 65717b00 l.#3,...p2."eq{.
-  0x00008fd8 25703496 00183132 0024352c 3700ff08 %p4...12.$5,7...
-  0x00008fe8 343b0a40 25703520 62726120 244c5f5f 4;.@%p5 bra $L__
-  0x00008ff8 4242305f 323b0a12 0104019a 002f6432 BB0_2;......./d2
-  0x00009008 31010511 381f0018 33310121 76320003 1...8...31.!v2..
-  0x00009018 307b2566 e9003266 327d3b01 20385df1 0{%f..2f2};. 8].
-  0x00009028 00146cf9 0214390b 0182333b 0a616464 ..l...9...3;.add
-  0x00009038 2e731700 3631302c 76001f39 57000300 .s..610,v..9W...
-  0x00009048 cb002366 36570010 31fa0233 6d756c74 ..#f6W..1..3mult
-  0x00009058 03005700 02780018 35170001 57002166 ..W..x..5...W.!f
-  0x00009068 32390054 3b0a7375 62180025 312c3500 29.T;.sub..%1,5.
-  0x00009078 1f30c500 04013600 243133c7 00232b38 .0....6.$13..#+8
-  0x00009088 71004577 696465ef 0122312c 11021a38 q.Ewide.."1,...8
-  0x00009098 ce00003c 0004ce00 2f313161 00041136 ...<..../11a...6
-  0x000090a8 61001437 d1000043 0363666d 612e726e a..7...C.cfma.rn
-  0x000090b8 a5001132 bd000388 00022d00 1831dd00 ...2......-..1..
-  0x000090c8 223231a2 00010600 19371a00 15320f01 "21......7...2..
-  0x000090d8 1c365500 15331201 0150012c 32322100 .6U..3...P.,22!.
-  0x000090e8 17345600 0176001f 32e70104 12324100 .4V..v..2....2A.
-  0x000090f8 15362201 3931365d 86000160 012d3235 .6".916]...`.-25
-  0x00009108 96011233 96011d36 97013533 312c3800 ...3...6..531,8.
-  0x00009118 1f339801 041133bc 00163398 012c3234 .3....3...3..,24
-  0x00009128 39011133 5a002633 32c30019 33390121 9..3Z.&32...39.!
-  0x00009138 33371400 0f390100 2633389a 001c3556 37...9..&38...5V
-  0x00009148 0007cf00 0255001b 38220027 34307800 .....U..8".'40x.
-  0x00009158 0264001c 39230017 31d40101 23002832 .d..9#..1...#.(2
-  0x00009168 34020135 34322cfa 011032e4 031b7402 4..542,...2...t.
-  0x00009178 0103fc02 342c207b 2d003c34 317d6500 ....4, {-.<41}e.
-  0x00009188 1733e000 01ab0029 34306500 26342c26 .3.....)40e.&4,&
-  0x00009198 011f3765 00051332 6500012d 00653433 ..7e...2e..-.e43
-  0x000091a8 7d3b0a0a 3704903a 0a726574 3b0a0a7d };..7..:.ret;..}
-  0x000091b8 35081f2e 3408084f 446f7562 34081c0e 5...4..ODoub4...
-  0x000091c8 33000e34 080f3b00 241f313b 00271f32 3..4..;.$.1;.'.2
-  0x000091d8 3b00270f 3408012c 31373508 3c313631 ;.'.4..,175.<161
-  0x000091e8 36082d31 3237082f 32303708 060e9300 6.-127./207.....
-  0x000091f8 0f37082b 0e44000f 37081f0e 44000f37 .7.+.D..7...D..7
-  0x00009208 081f0e44 000f3708 091f3421 08031f35 ...D..7...4!...5
-  0x00009218 4e08021f 36370804 15374c07 1634e707 N...67...7L..4..
-  0x00009228 0f370814 233634fb 05043808 30637674 .7..#64...8.0cvt
-  0x00009238 6f00031a 00023907 1c374f08 0172001f o.....9..7O..r..
-  0x00009248 38490000 13384900 2d2b384b 0021392c 8I...8I.-+8K.!9,
-  0x00009258 2100074b 0015324b 00193990 0617398f !..K..2K..9...9.
-  0x00009268 061c3847 00037b07 17394800 15334800 ..8G..{..9H..3H.
-  0x00009278 23313068 08136ef4 06267031 1c000c1b #10h..n..&p1....
-  0x00009288 00067f00 69323b0a 616e64b6 081131bb ....i2;.and...1.
-  0x00009298 080c3300 15343300 19333300 09b7080a ..3..43..33.....
-  0x000092a8 33002436 2c35010a 66002337 2c1d002c 3.$6,5..f.#7,..,
-  0x000092b8 70353300 15383300 0a660023 392c1d00 p53..83..f.#9,..
-  0x000092c8 2c703733 00021601 1e323400 01f30702 ,p73.....24.....
-  0x000092d8 1f002f70 39000a03 044d0022 6c746301 ../p9....M."ltc.
-  0x000092e8 1170f005 031d000a 010a0241 08163502 .p.........A..5.
-  0x000092f8 0a226c74 1a001170 820701a2 023a7231 ."lt...p.....:r1
-  0x00009308 31820024 342c2000 2a703104 01363135 1..$4, .*p1..615
-  0x00009318 2c210065 313b0a6e 6f741b00 11361500 ,!.e1;.not...6..
-  0x00009328 1135060a 27313607 0a1f3107 0a082f31 .5..'16...1.../1
-  0x00009338 30080a0b 2f313109 0a162a31 310a0a2f 0.../11...*11../
-  0x00009348 31320b0a 0427332c 7a002f31 320d0a11 12...'3,z./12...
-  0x00009358 2f335d0d 0a5a2f31 310e0a03 1f340e0a /3]..Z/11....4..
-  0x00009368 0328352c d1001f34 6300041a 360f0a1f .(5,...4c...6...
-  0x00009378 350f0a2d 06e10002 0f0a0655 080f7f00 5..-.......U....
-  0x00009388 0103180a 1634e200 2f3136e3 00011336 .....4../16....6
-  0x00009398 17030be3 0001c303 05e3001f 36640004 ............6d..
-  0x000093a8 11376400 14386400 1d37b909 01c30003 .7d..8d..7......
-  0x000093b8 8b001437 9f0a06e3 00025b09 02a20a28 ...7......[....(
-  0x000093c8 3238e300 02ed0802 40001f33 33020411 28......@..33...
-  0x000093d8 33380026 3335e300 2f3234e3 00011338 38.&35../24....8
-  0x000093e8 350e0be3 0028392c e3001f38 64000411 5....(9,...8d...
-  0x000093f8 38640014 3964001c 39e30002 b409038b 8d..9d..9.......
-  0x00009408 00022d00 1833e300 03bc0914 353e0a07 ..-..3......5>..
-  0x00009418 1a001634 ba0b0b9b 0a253435 f2020119 ...4.....%45....
-  0x00009428 022c3434 21001c36 770a1d34 44001737 .,44!..6w..4D..7
-  0x00009438 3f020246 000c3c0c 2734389f 01010c00 ?..F..<.'48.....
-  0x00009448 2c343723 001739a2 01026900 0c260b27 ,47#..9...i..&.'
-  0x00009458 35300201 012f001f 34f10d05 01d20016 50.../..4.......
-  0x00009468 35410448 2b33325d 13011135 f8001e35 5A.H+32]...5...5
-  0x00009478 eb032235 363a000d ec033635 372c3800 .."56:....657,8.
-  0x00009488 0fa70204 1135db00 26353977 003b3430 .....5..&59w.;40
-  0x00009498 5dc50011 365b0026 35382e01 1935490c ]...6[.&58...5I.
-  0x000094a8 22363344 000e8d03 3536342c 40001f36 "63D....564,@..6
-  0x000094b8 38050411 36a00027 36368200 1d388200 8...6..'66...8..
-  0x000094c8 015c0026 36356a01 28363482 00223730 .\.&65j.(64.."70
-  0x000094d8 44000e2c 03353731 2c40001f 37f10404 D..,.571,@..7...
-  0x000094e8 1137a000 1737f104 2c353682 0011375c .7...7..,56...7\
-  0x000094f8 00022a00 02cb0219 37910422 37374400 ..*.....7.."77D.
-  0x00009508 0ecb0226 37389f01 0ccc0226 3739d401 ...&78.....&79..
-  0x00009518 0261000c 41022738 307c0102 64000c67 .a..A.'80|..d..g
-  0x00009528 0d273831 7f010146 002c3830 23001732 .'81...F.,80#..2
-  0x00009538 4001014c 002c3831 23001733 43010169 @..L.,81#..3C..i
-  0x00009548 001c382e 0f273834 0401016f 001f38d4 ..8..'84...o..8.
-  0x00009558 01041138 6a001738 d4013836 345d1501 ...8j..8..864]..
-  0x00009568 12383f00 01270009 cd022239 303a000d .8?..'...."90:..
-  0x00009578 cd023539 312c3800 1f39c901 0411399b ..591,8..9....9.
-  0x00009588 001739c9 013b3732 5dc50011 395b0026 ..9..;72]...9[.&
-  0x00009598 39322e01 1939c901 22393744 000ecd02 92...9.."97D....
-  0x000095a8 3639382c 40001f37 82000403 5a071630 698,@..7....Z..0
-  0x000095b8 83001d38 50032131 305e0026 39396c01 ...8P.!10^.&99l.
-  0x000095c8 28393884 00213130 6a013e31 3030d102 (98..!10j.>100..
-  0x000095d8 46313035 2c44002f 31306207 05223036 F105,D./10b.."06
-  0x000095e8 20001737 8a000d58 031131e2 05042d00  ..7...X..1...-.
-  0x000095f8 02d80229 31309101 12313208 3e313037 ...)10...12.>107
-  0x00009608 db023631 3132ae01 0cdc0236 313133e4 ..6112.....6113.
-  0x00009618 0122362c 2f000d24 0017348e 01123725 ."6,/..$..4...7%
-  0x00009628 001d3325 00173593 01034a00 1d342500 ..3%..5...J..4%.
-  0x00009638 17365401 02c9002d 31352500 18375801 .6T....-15%..7X.
-  0x00009648 0370001d 36260018 38150112 3926000f .p..6&..8...9&..
-  0x00009658 f1010422 31312000 1732f201 3939365d ..."11 ..2..996]
-  0x00009668 26010245 06032a00 1a351b00 13343e00 &..E..*..5...4>.
-  0x00009678 0df00212 317d1104 3d001f32 e8010502 ....1}..=..2....
-  0x00009688 c0112731 32e8014c 3130345d d4000287 ..'12..L104]....
-  0x00009698 12042e00 0334000a 8c000251 083e3132 .....4.....Q.>12
-  0x000096a8 37fb0213 31e81103 46002f33 318d0004 7...1...F./31...
-  0x000096b8 03871118 335a090e ec131231 9412032e ....3Z.....1....
-  0x000096c8 00038701 2a33328d 0013384a 000f0203 ....*32...8J....
-  0x000096d8 00039301 0446000f 9e080412 31a21237 .....F......1..7
-  0x000096e8 3134318d 001e328d 03026b08 032e0003 141...2...k.....
-  0x000096f8 03030be7 02037308 2f343103 0300046e ......s./41....n
-  0x00009708 081f3004 03022734 37fb0102 2a000d6a ..0...'47...*..j
-  0x00009718 0812316b 08049c01 0206030d 6d081231 ..1k........m..1
-  0x00009728 6e08049f 0102c201 0d700812 31710804 n........p..1q..
-  0x00009738 5b010208 032d3439 26001831 5e010252 [....-49&..1^..R
-  0x00009748 002d3530 26001832 1a01027f 002d3531 .-50&..2.....-51
-  0x00009758 260008c5 09017100 293530af 01353534 &.....q.)50..554
-  0x00009768 2c0c0a2f 34338213 05123382 13032e00 ,../43....3.....
-  0x00009778 4d313533 7d690017 35630701 69002a38 M153}i..5c..i.*8
-  0x00009788 34690026 362caa07 0feb1306 14356900 4i.&6,.......5i.
-  0x00009798 22362c56 000e6900 1837f204 1238c201 "6,V..i..7...8..
-  0x000097a8 0a830203 9107033f 052f3131 6d000514 .......?./11m...
-  0x000097b8 376d0002 30002e35 376d0018 395c0203 7m..0..57m..9\..
-  0x000097c8 27001932 6d003836 302ca902 1f356d00 '..2m.860,...5m.
-  0x000097d8 0513396d 00033000 263539c7 141f31c7 ..9m..0.&59...1.
-  0x000097e8 140f1438 8412af54 7269706c 65476174 ...8...TripleGat
-  0x000097f8 65c61408 0f320012 0ec5140f 3a001c1f e....2......:...
-  0x00009808 313a0026 1f323a00 260ff61c 021c31c2 1:.&.2:.&.....1.
-  0x00009818 14363630 39b01402 c2142d32 34c2142f .6609.....-24../
-  0x00009828 3332c214 021231f6 130f4001 160f3914 32....1...@...9.
-  0x00009838 001f3243 001b1f31 0415010f 43001b1f ..2C...1....C...
-  0x00009848 32430000 1f344300 1b2f335d 5b110523 2C...4C../3][..#
-  0x00009858 352c2e12 06b0141f 38c61402 1f39f314 5,......8....9..
-  0x00009868 032f3130 de140401 be080136 00247238 ./10.......6.$r8
-  0x00009878 e4132e6c 64db1400 41032d35 5d2f1421 ...ld...A.-5]/.!
-  0x00009888 322c2000 072f1425 312c5600 2f31320d 2, ../.%1,V./12.
-  0x00009898 15071f35 c4140001 11090a10 1517324e ...5..........2N
-  0x000098a8 000a1a12 23382c9a 00023200 0b4a001d ....#8,...2..J..
-  0x000098b8 340f1517 334a001f 34980000 14399800 4...3J..4....9..
-  0x000098c8 2e313699 001d3516 1517344f 001a351c .16...5...4O..5.
-  0x000098d8 1017309a 001d394b 0013363a 10074c00 ..0...9K..6:..L.
-  0x000098e8 17354c00 1a364c00 1731ad15 0e4c0002 .5L..6L..1...L..
-  0x000098f8 18002731 314c0017 364c001f 37881c01 ..'11L..6L..7...
-  0x00009908 0353001d 364d0015 38631305 4d001737 .S..6M..8c..M..7
-  0x00009918 4d001f38 fc15022f 3131fd15 072f3131 M..8.../11.../11
-  0x00009928 fe151f2f 3131ff15 201331cf 1f0f0016 .../11.. .1.....
-  0x00009938 19049c1f 0c011601 39001f38 01160302 ........9..8....
-  0x00009948 35001936 35000114 00023b00 2d313037 5..65.....;.-107
-  0x00009958 00070801 1a373700 26332c3f 160d0b01 .....77.&3,?....
-  0x00009968 053c142f 2572d315 081d3337 00020f01 .<./%r....37....
-  0x00009978 0e420101 2902021f 0001f515 0b370002 .B..)........7..
-  0x00009988 12010e45 01019609 021f003c 70313737 ...E.......<p177
-  0x00009998 0001d209 1f724801 00017c14 021f003d .....rH...|....=
-  0x000099a8 70313937 00021401 0e4a0101 c90b021f p197.....J......
-  0x000099b8 003d7032 31370006 13010a4a 0101070c .=p217.....J....
-  0x000099c8 021f003d 70323337 00011301 1e321301 ...=p237.....2..
-  0x000099d8 01d50902 1f003d70 32353700 15383700 ......=p257..87.
-  0x000099e8 0a130101 8f1e021f 002d7032 13012533 .........-p2..%3
-  0x000099f8 3037000a 1301013b 0c021f00 2d703213 07.....;....-p2.
-  0x00009a08 01253332 37000a13 0101a60a 021f003d .%327..........=
-  0x00009a18 70333137 00153437 000a1301 016c0a02 p317..47.....l..
-  0x00009a28 1f003d70 33333700 0113011e 33dc0001 ..=p337.....3...
-  0x00009a38 300c021f 002d7033 13012533 3837000b 0....-p3..%387..
-  0x00009a48 dc002439 2c1f003c 70333737 00253430 ..$9,..<p377.%40
-  0x00009a58 37000adc 0001d109 021f003d 70333937 7..........=p397
-  0x00009a68 00153237 000adc00 01131502 1f002d70 ..27..........-p
-  0x00009a78 34130101 030a2e72 34a50001 a20c021f 4......r4.......
-  0x00009a88 003d7034 33370015 3637000b a5002437 .=p437..67....$7
-  0x00009a98 2c1f003d 70343537 00153837 000ba500 ,..=p457..87....
-  0x00009aa8 24392c1f 003c7034 37370001 830c2e72 $9,..<p477.....r
-  0x00009ab8 356e0001 760c021f 003d7034 39370015 5n..v....=p497..
-  0x00009ac8 3237000a 6e000161 0c021f00 3d703531 27..n..a....=p51
-  0x00009ad8 370002d7 000f3700 0024352c 1f003e70 7.....7..$5,..>p
-  0x00009ae8 3533bd1a 14336e1a 0abf1a01 170c041f 53...3n.........
-  0x00009af8 00296433 c01a0447 080dc01a 01320c03 .)d3...G.....2..
-  0x00009b08 5d1c2a31 39870024 382c2100 3a703536 ].*19..$8,!.:p56
-  0x00009b18 1b002639 2c210019 35c11a01 c30b3170 ..&9,!..5.....1p
-  0x00009b28 3539c11a 273630c1 1a1f32c1 1a091434 59..'60...2....4
-  0x00009b38 c11a2f6c 64110f00 09a11a00 23100f46 ../ld.......#..F
-  0x00009b48 00040184 012f6431 1119052f 31311219 ...../d1.../11..
-  0x00009b58 051e3512 190fc61a 062f375d c61a5b3f ..5....../7]..[?
-  0x00009b68 342b3800 19061f31 0019051f 3500190a 4+8....1....5...
-  0x00009b78 010f0107 c61a0d00 19012406 048a0002 ..........$.....
-  0x00009b88 b20f0fc6 1a481f34 c61a0323 32304705 .....H.4...#20G.
-  0x00009b98 0ae30001 7c0005e3 001f3246 0104021c ....|.....2F....
-  0x00009ba8 1005c61a 2c3231e3 00273331 27190fc6 ....,21..'31'...
-  0x00009bb8 1a4e1f34 c61a0314 324e050b e3000062 .N.4....2N.....b
-  0x00009bc8 0006e300 0f640005 1938c61a 2f3233c6 .....d...8../23.
-  0x00009bd8 1a2d06e3 0002c61a 06fa100f 7f000102 .-..............
-  0x00009be8 5c122634 36e3002f 3332e300 0113348c \.&46../32....4.
-  0x00009bf8 050be300 003e0006 e3000f25 1404023b .....>.....%...;
-  0x00009c08 121435a3 141d326f 1d02c411 038b0001 ..5...2o........
-  0x00009c18 2d002834 34e30001 46050359 1b0ade11 -.(44...F..Y....
-  0x00009c28 02951102 40001f35 7f000413 35341a06 ....@..5....54..
-  0x00009c38 e3002f34 30e30001 13360106 0be30000 ../40....6......
-  0x00009c48 560206e3 000f5d04 0402f410 1436ec13 V.....]......6..
-  0x00009c58 1d326f1d 028b1a02 8b00022d 00283535 .2o........-.(55
-  0x00009c68 e300021d 1901a805 38663631 e3000214 ........8f61....
-  0x00009c78 19024000 2f36357f 00040238 001738e3 ..@./65....8..8.
-  0x00009c88 000f6f04 01027809 1d36e300 00730106 ..o...x..6...s..
-  0x00009c98 e3000f6f 040402cb 1a1437c2 051d326f ...o......7...2o
-  0x00009ca8 041137c3 00028b00 03f81a18 36e30002 ..7.........6...
-  0x00009cb8 c41a2236 38470008 e30003be 1a014000 .."68G........@.
-  0x00009cc8 1f376201 0402c81a 263739e3 002f3536 .7b.....&79../56
-  0x00009cd8 e3000002 240a1c37 e30001e8 0305e300 ....$..7........
-  0x00009ce8 0ff02805 02a81a14 38b5051d 336f0402 ..(.....8...3o..
-  0x00009cf8 6b18028b 00243832 e91306e3 00353837 k....$82.....587
-  0x00009d08 2c571b29 38331a00 1f38521e 0616387e ,W.)83...8R...8~
-  0x00009d18 06015f00 1c385615 1839c805 1237881a .._..8V..9...7..
-  0x00009d28 0c230008 cb051436 a51a0a23 0017322b .#.....6...#..2+
-  0x00009d38 0514387a 1a0a2300 1c33521e 1c393319 ..8z..#..3R..93.
-  0x00009d48 2739348e 04123919 190c2300 01c80126 '94...9...#....&
-  0x00009d58 3335b104 2f393406 1b0202f1 03019109 35../94.........
-  0x00009d68 2c663916 01263937 f4030214 041c39ba ,f9..&97......9.
-  0x00009d78 16273938 54031431 181b0a23 00173957 .'98T..1...#..9W
-  0x00009d88 031430eb 1a092300 038f1903 b8021232 ..0...#........2
-  0x00009d98 c7190d24 001731bc 0222312c 37000d25 ...$..1.."1,7..%
-  0x00009da8 0017321e 02123325 000fab18 0505401b ..2...3%......@.
-  0x00009db8 06d0020b a41c0301 16032a00 0b980826 ..........*....&
-  0x00009dc8 382ca81b 0a9b0838 30392c3d 000f3c08 8,.....809,=..<.
-  0x00009dd8 0502db08 36313131 80000ead 1c03201b ....6111...... .
-  0x00009de8 042d0002 43081a30 81180153 03004900 .-..C..0...S..I.
-  0x00009df8 0e460803 151b0546 000fbd04 0404171b .F.....F........
-  0x00009e08 1731bf04 0fb61c00 03ae0826 31379e02 .1.........&17..
-  0x00009e18 013d1b07 8c0002b7 0803411b 0aef0705 .=........A.....
-  0x00009e28 c91a0246 000f8e07 0505121b 07f4070f ...F............
-  0x00009e38 b81c0002 40032731 3295073a 3132338c ....@.'12..:123.
-  0x00009e48 00133949 000e9807 050e1b03 46000f93 ..9I........F...
-  0x00009e58 21040412 1b163335 0b02dc1b 0a8c0002 !.....35........
-  0x00009e68 6903032d 00022a03 39313330 8c000175 i..-..*.9130...u
-  0x00009e78 0e04461b 0b1f1904 0d1b0346 000f7e05 ..F........F..~.
-  0x00009e88 0405111b 0780050f e81b0102 6d08032e ............m...
-  0x00009e98 00027103 39313337 8d0002b0 0803461b ..q.9137......F.
-  0x00009ea8 0aeb0605 64180246 000fb408 0505111b ....d..F........
-  0x00009eb8 07b6080e e81b05b3 1a273435 b6030a59 .........'45...Y
-  0x00009ec8 0804b01a 2e343695 0604a61a 0346002f .....46......F./
-  0x00009ed8 35308d00 04243532 321a068d 000fe81b 50...$522.......
-  0x00009ee8 0002a704 032e0002 3c0601ce 1a088d00 ........<.......
-  0x00009ef8 02f9192e 35333f06 283135f2 030c4206 ....53?.(15...B.
-  0x00009f08 04c61902 2b040369 000de804 283630cd ....+..i....(60.
-  0x00009f18 03036c00 0dea0402 490504d0 0302f303 ..l.....I.......
-  0x00009f28 1d36eb04 02542304 8d0302e8 1b2d3631 .6...T#......-61
-  0x00009f38 26001833 90030272 001d3685 1f02db08 &..3...r..6.....
-  0x00009f48 27313254 063d3136 33260018 35500303 '12T.=163&..5P..
-  0x00009f58 72000d87 1f022d09 030d0302 5a063d31 r.....-.....Z.=1
-  0x00009f68 36352600 17371003 03e0012d 36362600 65&..7.....-66&.
-  0x00009f78 1838cc02 0310010d 181d02dc 2304cf02 .8..........#...
-  0x00009f88 02f2021d 367c0128 37308b02 023d011d ....6|.(70...=..
-  0x00009f98 367c0128 37318e02 020d002d 37302600 6|.(71.....-70&.
-  0x00009fa8 18324a02 0263012f 37319e02 04133720 .2J..c./71....7 
-  0x00009fb8 0008a70d 3932385d 5c02027f 092f3137 ....928]\..../17
-  0x00009fc8 69060002 cd062f31 37690600 02e60805 i...../17i......
-  0x00009fd8 3d000f69 06050242 24273138 69062e31 =..i...B$'18i..1
-  0x00009fe8 33c60402 dd232831 386a061a 376a0602 3....#(18j..7j..
-  0x00009ff8 cb211231 70240b6a 06029909 0546000f .!.1p$.j.....F..
-  0x0000a008 6a060502 a0092731 386a062e 3134c604 j.....'18j..14..
-  0x0000a018 034e0927 3837b802 1a386b06 0334221f .N.'87...8k..4".
-  0x0000a028 386b0601 032b2203 46002f39 328d0004 8k...+".F./92...
-  0x0000a038 024b0927 31396b06 2e3135c6 0402e608 .K.'19k..15.....
-  0x0000a048 2831396c 062a3933 8d001339 4a000e6c (19l.*93...9J..l
-  0x0000a058 061232de 08054600 0f6c0604 1232e108 ..2...F..l...2..
-  0x0000a068 38323032 cf0f0dc6 041232fe 23273230 8202......2.#'20
-  0x0000a078 6d063832 30308d00 1232b822 2f32306d m.8200...2."/20m
-  0x0000a088 06001232 96080546 000f6d06 041232df ...2...F..m...2.
-  0x0000a098 08283230 6d061d36 86071232 120b032e .(20m..6...2....
-  0x0000a0a8 00027b03 2932306d 06123212 0b2f3230 ..{.)20m..2../20
-  0x0000a0b8 6d060012 32970804 46002f31 338d0004 m...2...F./13...
-  0x0000a0c8 02e10828 32316d06 1d37c102 1132b411 ...(21m..7...2..
-  0x0000a0d8 042e0002 bc033932 31348d00 0450110f ......9214...P..
-  0x0000a0e8 6d060012 32980804 46000f10 110602e2 m...2...F.......
-  0x0000a0f8 08283232 6d061d38 c1021132 cc0e042e .(22m..8...2....
-  0x0000a108 00026d06 3a323231 8d001337 4a000e6d ..m.:221...7J..m
-  0x0000a118 06283232 f6030c6d 06373232 392f0403 .(22...m.7229/..
-  0x0000a128 69000cf1 04383233 30d00303 6c001d39 i....8230...l..9
-  0x0000a138 26001831 d303024c 002d3330 26001832 &..1...L.-30&..2
-  0x0000a148 8f031238 26001d31 26001833 9203022c ...8&..1&..3...,
-  0x0000a158 002d3332 26001834 4e03026e 012d3333 .-32&..4N..n.-33
-  0x0000a168 26001835 51030372 001d3426 0017360d &..5Q..r..4&..6.
-  0x0000a178 03026d06 3d323335 26001737 10030333 ..m.=235&..7...3
-  0x0000a188 032d3336 26001838 cc021231 26001d37 .-36&..8...1&..7
-  0x0000a198 26001839 cf020372 000d7c01 2834308b &..9...r..|.(40.
-  0x0000a1a8 02123226 000d7c01 2834318e 02020d00 ..2&..|.(41.....
-  0x0000a1b8 2d343026 0018324a 02123326 000f6d06 -40&..2J..3&..m.
-  0x0000a1c8 04233234 2000086d 06393932 5d5c0202 .#24 ..m.992]\..
-  0x0000a1d8 93242e32 346d0632 3234381b 000e6d06 .$.24m.2248...m.
-  0x0000a1e8 13323801 043d000f 6d060413 32850117 .28..=..m...2...
-  0x0000a1f8 356d062e 3230c604 02501203 2e000377 5m..20...P.....w
-  0x0000a208 02293439 8c000259 122f3235 6d060012 .)49...Y./25m...
-  0x0000a218 32cb0905 46000f6d 06041232 cf093832 2...F..m...2..82
-  0x0000a228 35388d00 0ec60403 ed012735 37b80229 58........'57..)
-  0x0000a238 35368d00 026e092f 32356d06 00123264 56...n./25m...2d
-  0x0000a248 09044600 2f36328d 00040265 09273236 ..F./62....e.'26
-  0x0000a258 6d063e32 31368d00 02630027 3634f902 m.>216...c.'64..
-  0x0000a268 2a36338d 0013394a 000f6d06 0002e708 *63...9J..m.....
-  0x0000a278 0546000f 6d060503 6e022737 328d002d .F..m...n.'72..-
-  0x0000a288 32348d00 02111228 32376d06 2937308d 24.....(27m.)70.
-  0x0000a298 00025412 2f32376d 0601029a 08054600 ..T./27m......F.
-  0x0000a2a8 0f6d0605 02e30818 325a123d 3233328d .m......2Z.=232.
-  0x0000a2b8 00034605 2737387b 030afd11 13321f03 ..F.'78{.....2..
-  0x0000a2c8 1f376d06 01029a08 0446002f 38338d00 .7m......F./83..
-  0x0000a2d8 0402e408 37323836 8d000e12 2f123233 ....7286..../.23
-  0x0000a2e8 12283238 6d062938 348d0002 35122f32 .(28m.)84...5./2
-  0x0000a2f8 386d0601 029a0804 46000fcf 2c051332 8m......F...,..2
-  0x0000a308 32122839 338d000e c10202cd 11283239 2.(93........(29
-  0x0000a318 6d060ad5 2c1232cd 112f3239 6d060102 m...,.2../29m...
-  0x0000a328 9a082f32 346d0603 02db0827 32346d06 ../24m.....'24m.
-  0x0000a338 0dc21112 33e40828 32356d06 0dc41112 ....3..(25m.....
-  0x0000a348 33a80527 32356d06 1d33c511 1233a805 3..'25m..3...3..
-  0x0000a358 2732356d 063d3330 31260018 33920312 '25m.=301&..3...
-  0x0000a368 3726001d 32260018 344e0312 3926001d 7&..2&..4N..9&..
-  0x0000a378 33260018 35510303 72001d34 26001736 3&..5Q..r..4&..6
-  0x0000a388 0d0302ea 003d3330 35260017 37100302 .....=305&..7...
-  0x0000a398 33033d33 30362600 1838cc02 12312600 3.=306&..8...1&.
-  0x0000a3a8 1d372600 1839cf02 0372000d 7c01024f .7&..9...r..|..O
-  0x0000a3b8 0e273238 6d063d33 30392600 18318e02 .'28m.=309&..1..
-  0x0000a3c8 0272002d 31302600 18324a02 12332600 .r.-10&..2J..3&.
-  0x0000a3d8 0f6d0604 23333120 00076d06 15321316 .m..#31 ..m..2..
-  0x0000a3e8 025c0212 330c022e 33316d06 1233950e .\..3...31m..3..
-  0x0000a3f8 2e33316d 06123385 09053d00 0f6d0604 .31m..3...=..m..
-  0x0000a408 1233cf09 2833326d 0601c413 0ad50003 .3..(32m........
-  0x0000a418 d80e2732 30770229 31398c00 03d50e1f ..'20w.)19......
-  0x0000a428 326d0600 1233cb09 0546000f 6d060413 2m...3...F..m...
-  0x0000a438 33840227 32388d00 0ed11312 33710903 3..'28......3q..
-  0x0000a448 2e000434 00096d06 12336e09 2f33326d ...4..m..3n./32m
-  0x0000a458 06001333 351b0346 000f371b 06031f16 ...35..F..7.....
-  0x0000a468 09391b0e d2131333 ec022733 34f9020a .9.....3..'34...
-  0x0000a478 dc1a1333 35031f33 6d060012 33e70805 ...35..3m...3...
-  0x0000a488 46000f6d 06041233 e8082833 346d060e F..m...3..(34m..
-  0x0000a498 d3131233 9b0f032e 00033a03 2934308d ...3......:.)40.
-  0x0000a4a8 0002980f 2f33346d 06001233 9a080546 ..../34m...3...F
-  0x0000a4b8 000f6d06 041233e3 08283334 6d060ed4 ..m...3..(34m...
-  0x0000a4c8 131233dc 0f032e00 037b0329 34378d00 ..3......{.)47..
-  0x0000a4d8 0226122f 33346d06 0012339a 08044600 .&./34m...3...F.
-  0x0000a4e8 2f35338d 000402e4 08273335 6d061e33 /53......'35m..3
-  0x0000a4f8 d4131233 5d12032e 0003bc03 2935348d ...3].......)54.
-  0x0000a508 0003a300 1f356d06 00133360 04034600 .....5m...3`..F.
-  0x0000a518 2f36308d 000402e4 08273336 6d061e33 /60......'36m..3
-  0x0000a528 d4131233 e1112733 366d063a 3336318d ...3..'36m.:361.
-  0x0000a538 0013374a 000e6d06 12339a08 2f33316d ..7J..m..3../31m
-  0x0000a548 06021233 db082633 316d061d 33cb1112 ...3..&31m..3...
-  0x0000a558 33e40827 33326d06 1d33cb11 38333731 3..'32m..3..8371
-  0x0000a568 d303024c 000dcb11 38333732 8f03029c ...L....8372....
-  0x0000a578 002d3731 26001833 92030272 002d3732 .-71&..3...r.-72
-  0x0000a588 26001834 4e0302ca 001d376d 06020e09 &..4N.....7m....
-  0x0000a598 2833336d 061d376d 06025709 2833346d (33m..7m..W.(34m
-  0x0000a5a8 061d372f 01026109 2833346d 062d3736 ..7/..a.(34m.-76
-  0x0000a5b8 26001838 cc021231 26000d6d 06026606 &..8...1&..m..f.
-  0x0000a5c8 2833346d 060d8e36 38333830 8b02023d (34m...68380...=
-  0x0000a5d8 012d3739 26001831 8e02020d 000d9436 .-79&..1.......6
-  0x0000a5e8 38333832 4a020263 012f3831 9e020404 8382J..c./81....
-  0x0000a5f8 20001834 281f2930 5d5c0202 a00e2f33  ..4(.)0]\..../3
-  0x0000a608 386d0600 02950e2f 33386d06 00028509 8m...../38m.....
-  0x0000a618 053d000f 6d060502 cf093833 39318100 .=..m.....8391..
-  0x0000a628 0ec60404 d80e1730 77022938 398c0004 .......0w.)89...
-  0x0000a638 26120f6d 060102cb 09054600 0f6d0605 &..m......F..m..
-  0x0000a648 02cf0927 33396d06 1e33d413 12347109 ...'39m..3...4q.
-  0x0000a658 032e0003 b8022839 368d0012 346e092f ......(96...4n./
-  0x0000a668 33396d06 00123464 09034600 3f343032 39m...4d..F.?402
-  0x0000a678 8d000312 34650927 34306d06 1e33d413 ....4e.'40m..3..
-  0x0000a688 1234f408 032e0013 330d0009 1d041234 .4......3......4
-  0x0000a698 f1081234 90090a6d 061234e7 08054600 ...4...m..4...F.
-  0x0000a6a8 0f6d0604 1234e808 2734316d 061e33d4 .m...4..'41m..3.
-  0x0000a6b8 1312349b 0f273431 6d063934 31308d00 ..4..'41m.9410..
-  0x0000a6c8 02bd012f 34316d06 00123476 04054600 .../41m...4v..F.
-  0x0000a6d8 0f6d0604 1234e308 2734316d 061e33d4 .m...4..'41m..3.
-  0x0000a6e8 131234dc 0f032e00 027b0339 3431378d ..4......{.9417.
-  0x0000a6f8 00022612 2f34316d 06001234 9a080446 ..&./41m...4...F
-  0x0000a708 002f3233 8d000402 e4083834 32368d00 ./23......8426..
-  0x0000a718 0dc10212 345d1227 34326d06 39343234 ....4].'42m.9424
-  0x0000a728 8d00025b 122f3432 6d060012 349a0804 ...[./42m...4...
-  0x0000a738 46002f33 308d0004 02e40837 3433338d F./30......7433.
-  0x0000a748 000ed413 1234e111 2734336d 063a3433 .....4..'43m.:43
-  0x0000a758 318d0013 374a000e 6d062834 33f6030c 1...7J..m.(43...
-  0x0000a768 6d063734 33392f04 0369000c f1043834 m.7439/..i....84
-  0x0000a778 3430d003 036c001d 39260018 31d30302 40...l..9&..1...
-  0x0000a788 4c000dcb 111234a8 05273339 6d063d34 L.....4..'39m.=4
-  0x0000a798 34312600 18339203 0272002d 34322600 41&..3...r.-42&.
-  0x0000a7a8 18344e03 026e012d 34332600 18355103 .4N..n.-43&..5Q.
-  0x0000a7b8 0372001d 34260017 360d0302 6d063d34 .r..4&..6...m.=4
-  0x0000a7c8 34352600 17371003 0333030d cc361234 45&..7...3...6.4
-  0x0000a7d8 66062734 316d063d 34343726 001839cf f.'41m.=447&..9.
-  0x0000a7e8 02037200 0d7c0128 35308b02 0278002d ..r..|.(50...x.-
-  0x0000a7f8 34392600 18318e02 020d002d 35302600 49&..1.....-50&.
-  0x0000a808 18324a02 12332600 0f6d0604 23343520 .2J..3&..m..#45 
-  0x0000a818 00086d06 01e51507 5c0202a0 0e2e3435 ..m.....\.....45
-  0x0000a828 6d061234 950e2e34 356d0612 34850905 m..4...45m..4...
-  0x0000a838 3d000f6d 06041334 13012736 31810001 =..m...4..'61...
-  0x0000a848 c8130ad5 0002d80e 032e0003 77022935 ............w.)5
-  0x0000a858 398c0002 d50e2f34 366d0600 1234cb09 9...../46m...4..
-  0x0000a868 0546000f 6d060412 34cf0919 34dd240e .F..m...4...4.$.
-  0x0000a878 d4131334 7b012736 37b8020a 80241334 ...4{.'67....$.4
-  0x0000a888 c4011f36 6d060102 64090446 002f3732 ...6m...d..F./72
-  0x0000a898 8d000402 65093834 37358d00 0ec60402 ....e.8475......
-  0x0000a8a8 f408032e 0003f902 2a37338d 0013394a ........*73...9J
-  0x0000a8b8 000f6d06 0002e708 0546000f 6d060502 ..m......F..m...
-  0x0000a8c8 e8082734 386d061e 34d41312 349b0f28 ..'48m..4...4..(
-  0x0000a8d8 34386d06 2938308d 0002980f 2f34386d 48m.)80...../48m
-  0x0000a8e8 0601029a 08054600 0f6d0605 02e30827 ......F..m.....'
-  0x0000a8f8 34386d06 1e34d413 1234dc0f 032e0003 48m..4...4......
-  0x0000a908 7b031a38 6d060226 122f3438 6d060102 {..8m..&./48m...
-  0x0000a918 9a080446 002f3933 8d000402 e4082734 ...F./93......'4
-  0x0000a928 396d061e 34d41312 345d1228 34396d06 9m..4...4].(49m.
-  0x0000a938 2839348d 0012355b 122f3439 6d060013 (94...5[./49m...
-  0x0000a948 359a0802 46003f35 30308d00 031235e4 5...F.?500....5.
-  0x0000a958 08273530 6d061e34 d4131235 e1112735 .'50m..4...5..'5
-  0x0000a968 306d063a 3530318d 00123716 000f6d06 0m.:501...7...m.
-  0x0000a978 00283530 f6030c6d 06373530 392f0403 .(50...m.7509/..
-  0x0000a988 69000cf1 04383531 30d00303 6c001d39 i....8510...l..9
-  0x0000a998 26001831 d303024c 000dcb11 38353132 &..1...L....8512
-  0x0000a9a8 8f031238 26001d31 26001833 92030272 ...8&..1&..3...r
-  0x0000a9b8 002d3132 26001834 4e03026e 012d3133 .-12&..4N..n.-13
-  0x0000a9c8 26001835 51030372 001d3426 0017360d &..5Q..r..4&..6.
-  0x0000a9d8 0302e205 3d353135 26001737 10030233 ....=515&..7...3
-  0x0000a9e8 033d3531 36260018 38cc0202 52002d31 .=516&..8...R.-1
-  0x0000a9f8 37260018 39cf0203 72000d7c 01024f0e 7&..9...r..|..O.
-  0x0000aa08 2734396d 063d3531 39260018 318e0202 '49m.=519&..1...
-  0x0000aa18 72002d32 30260018 324a0212 3326000f r.-20&..2J..3&..
-  0x0000aa28 6d060423 35322000 18349e02 29385d5c m..#52 ..4..)8]\
-  0x0000aa38 02039a01 1e326d06 1335db01 1e326d06 .....2m..5...2m.
-  0x0000aa48 12358509 053d000f 6d060412 35cf0927 .5...=..m...5..'
-  0x0000aa58 35336d06 1134c813 0ad50002 d80e032e 53m..4..........
-  0x0000aa68 00037702 2932398c 0002d50e 2f35336d ..w.)29...../53m
-  0x0000aa78 06001235 cb090546 000f6d06 041235cf ...5...F..m...5.
-  0x0000aa88 09283533 6d060ed4 13133519 0f273337 .(53m.....5..'37
-  0x0000aa98 b8022933 368d0002 6e092f35 336d0600 ..)36...n./53m..
-  0x0000aaa8 12356409 0446002f 34328d00 04031317 .5d..F./42......
-  0x0000aab8 18346d06 0ed41312 35f40803 2e0003f9 .4m.....5.......
-  0x0000aac8 022a3433 8d001339 4a000e6d 06133505 .*43...9J..m..5.
-  0x0000aad8 03044600 0f6d0604 1235e808 37353532 ..F..m...5..7552
-  0x0000aae8 8d000ed4 1312359b 0f032e00 03770029 ......5......w.)
-  0x0000aaf8 35308d00 02980f2f 35356d06 0012359a 50...../55m...5.
-  0x0000ab08 08054600 0f6d0604 1235e308 38353539 ..F..m...5..8559
-  0x0000ab18 8d000d87 071235dc 0f032e00 037b030a ......5......{..
-  0x0000ab28 3c481235 26122f35 356d0600 12359a08 <H.5&./55m...5..
-  0x0000ab38 0446002f 36338d00 0402e408 37353636 .F./63......7566
-  0x0000ab48 8d000ed4 1312355d 12032e00 03bc030a ......5]........
-  0x0000ab58 47481235 5b122f35 366d0601 04320002 GH.5[./56m...2..
-  0x0000ab68 46002f37 308d0004 033b0406 4e483e34 F./70....;..NH>4
-  0x0000ab78 2b35d413 1235e111 2835376d 062a3731 +5...5..(57m.*71
-  0x0000ab88 8d001337 4a000f6d 0600029a 082f3532 ...7J..m...../52
-  0x0000ab98 6d060302 db082735 326d060d cb111235 m.....'52m.....5
-  0x0000aba8 e4082835 336d060d cb113835 3831d303 ..(53m....8581..
-  0x0000abb8 024c000d cb113835 38328f03 029c000d .L....8582......
-  0x0000abc8 62483835 38339203 0272000d 65483835 bH8583...r..eH85
-  0x0000abd8 38344e03 02ca002d 38332600 18355103 84N....-83&..5Q.
-  0x0000abe8 0372000d 6d060257 09030d03 0368032d .r..m..W.....h.-
-  0x0000abf8 38352600 17371003 0333032d 38362600 85&..7...3.-86&.
-  0x0000ac08 1838cc02 0252002d 38372600 1839cf02 .8...R.-87&..9..
-  0x0000ac18 0372000d 7c012839 308b0202 3d010d53 .r..|.(90...=..S
-  0x0000ac28 2e383539 318e0202 0d000d56 2e12358b .8591......V..5.
-  0x0000ac38 09283537 6d060d59 2e373539 33192f12 .(57m..Y.7593./.
-  0x0000ac48 32ad280a e0022639 34cc472f 3837d142 2.(...&94.G/87.B
-  0x0000ac58 0c032e00 2d3539a7 43123542 07044529 ....-59.C.5B..E)
-  0x0000ac68 026b000b 4b03023f 07059229 1f37d142 .k..K..?...).7.B
-  0x0000ac78 0c033000 2d3539ab 43293539 45231232 ..0.-59.C)59E#.2
-  0x0000ac88 ab1c0b6d 0028382c 92230f6d 00052432 ...m.(8,.#.m..$2
-  0x0000ac98 316d0022 382c5a00 0e6d0018 39451d12 1m."8,Z..m..9E..
-  0x0000aca8 32ab1609 6d001336 091d0492 1d0f6d00 2...m..6......m.
-  0x0000acb8 0603ee44 0330003c 3539396d 001236dc ...D.0.<599m..6.
-  0x0000acc8 0a283336 6d001b38 6d002832 2c92170f .(36m..8m.(2,...
-  0x0000acd8 6d000603 f2440330 002d3630 44593836 m....D.0.-60DY86
-  0x0000ace8 30334511 1232ab0a 0b6d0028 342c9211 03E..2...m.(4,..
-  0x0000acf8 0f6d0006 03210203 30002d36 30210212 .m...!..0.-60!..
-  0x0000ad08 368e1027 35306d00 2b35326d 0028362c 6..'50m.+52m.(6,
-  0x0000ad18 920b0f6d 00060321 02033000 2d363021 ...m...!..0.-60!
-  0x0000ad28 02293630 4505026d 001b396d 0028382c .)60E..m..9m.(8,
-  0x0000ad38 92050f6d 00051333 21020330 00363630 ...m...3!..0.660
-  0x0000ad48 375f4515 325f4550 0a7d0a0a 00000000 7_E.2_EP.}......
+  0x00008888 00000000 00c00f00 18790000 00000000 .........y......
+  0x00008898 00000000 00c00f00 18790000 00000000 .........y......
+  0x000088a8 00000000 00c00f00 18790000 00000000 .........y......
+  0x000088b8 00000000 00c00f00 18790000 00000000 .........y......
+  0x000088c8 00000000 00c00f00 18790000 00000000 .........y......
+  0x000088d8 00000000 00c00f00 18790000 00000000 .........y......
+  0x000088e8 00000000 00c00f00 18790000 00000000 .........y......
+  0x000088f8 00000000 00c00f00 18790000 00000000 .........y......
+  0x00008908 00000000 00c00f00 18790000 00000000 .........y......
+  0x00008918 00000000 00c00f00 00000000 00000000 ................
+  0x00008928 00000000 00000000 00000000 00000000 ................
+  0x00008938 00000000 00000000 00000000 00000000 ................
+  0x00008948 00000000 00000000 00000000 00000000 ................
+  0x00008958 00000000 00000000 01000000 03000000 ................
+  0x00008968 00000000 00000000 00000000 00000000 ................
+  0x00008978 40000000 00000000 70030000 00000000 @.......p.......
+  0x00008988 00000000 00000000 01000000 00000000 ................
+  0x00008998 00000000 00000000 0b000000 03000000 ................
+  0x000089a8 00000000 00000000 00000000 00000000 ................
+  0x000089b8 b0030000 00000000 e1030000 00000000 ................
+  0x000089c8 00000000 00000000 01000000 00000000 ................
+  0x000089d8 00000000 00000000 13000000 02000000 ................
+  0x000089e8 00000000 00000000 00000000 00000000 ................
+  0x000089f8 98070000 00000000 38010000 00000000 ........8.......
+  0x00008a08 02000000 0a000000 08000000 00000000 ................
+  0x00008a18 18000000 00000000 15030000 01000000 ................
+  0x00008a28 00000000 00000000 00000000 00000000 ................
+  0x00008a38 d0080000 00000000 50010000 00000000 ........P.......
+  0x00008a48 00000000 00000000 01000000 00000000 ................
+  0x00008a58 00000000 00000000 29000000 00000070 ........)......p
+  0x00008a68 00000000 00000000 00000000 00000000 ................
+  0x00008a78 200a0000 00000000 90000000 00000000  ...............
+  0x00008a88 03000000 00000000 04000000 00000000 ................
+  0x00008a98 00000000 00000000 5d000000 00000070 ........]......p
+  0x00008aa8 40000000 00000000 00000000 00000000 @...............
+  0x00008ab8 b00a0000 00000000 6c000000 00000000 ........l.......
+  0x00008ac8 03000000 0f000000 04000000 00000000 ................
+  0x00008ad8 00000000 00000000 51010000 00000070 ........Q......p
+  0x00008ae8 40000000 00000000 00000000 00000000 @...............
+  0x00008af8 1c0b0000 00000000 6c000000 00000000 ........l.......
+  0x00008b08 03000000 10000000 04000000 00000000 ................
+  0x00008b18 00000000 00000000 49020000 00000070 ........I......p
+  0x00008b28 40000000 00000000 00000000 00000000 @...............
+  0x00008b38 880b0000 00000000 6c000000 00000000 ........l.......
+  0x00008b48 03000000 11000000 04000000 00000000 ................
+  0x00008b58 00000000 00000000 45030000 01000070 ........E......p
+  0x00008b68 00000000 00000000 00000000 00000000 ................
+  0x00008b78 f40b0000 00000000 20000000 00000000 ........ .......
+  0x00008b88 03000000 00000000 04000000 00000000 ................
+  0x00008b98 08000000 00000000 61030000 0b000070 ........a......p
+  0x00008ba8 00000000 00000000 00000000 00000000 ................
+  0x00008bb8 180c0000 00000000 10000000 00000000 ................
+  0x00008bc8 00000000 00000000 08000000 00000000 ................
+  0x00008bd8 08000000 00000000 22030000 09000000 ........".......
+  0x00008be8 40000000 00000000 00000000 00000000 @...............
+  0x00008bf8 280c0000 00000000 30000000 00000000 (.......0.......
+  0x00008c08 03000000 04000000 08000000 00000000 ................
+  0x00008c18 10000000 00000000 bb000000 01000000 ................
+  0x00008c28 42000000 00000000 00000000 00000000 B...............
+  0x00008c38 580c0000 00000000 80010000 00000000 X...............
+  0x00008c48 00000000 0f000000 04000000 00000000 ................
+  0x00008c58 00000000 00000000 b1010000 01000000 ................
+  0x00008c68 42000000 00000000 00000000 00000000 B...............
+  0x00008c78 d80d0000 00000000 80010000 00000000 ................
+  0x00008c88 00000000 10000000 04000000 00000000 ................
+  0x00008c98 00000000 00000000 a9020000 01000000 ................
+  0x00008ca8 42000000 00000000 00000000 00000000 B...............
+  0x00008cb8 580f0000 00000000 80010000 00000000 X...............
+  0x00008cc8 00000000 11000000 04000000 00000000 ................
+  0x00008cd8 00000000 00000000 32000000 01000000 ........2.......
+  0x00008ce8 06000000 00000000 00000000 00000000 ................
+  0x00008cf8 00110000 00000000 001a0000 00000000 ................
+  0x00008d08 03000000 0a000034 80000000 00000000 .......4........
+  0x00008d18 00000000 00000000 25010000 01000000 ........%.......
+  0x00008d28 06000000 00000000 00000000 00000000 ................
+  0x00008d38 002b0000 00000000 80080000 00000000 .+..............
+  0x00008d48 03000000 0b000022 80000000 00000000 ......."........
+  0x00008d58 00000000 00000000 1d020000 01000000 ................
+  0x00008d68 06000000 00000000 00000000 00000000 ................
+  0x00008d78 80330000 00000000 00040000 00000000 .3..............
+  0x00008d88 03000000 0c000018 80000000 00000000 ................
+  0x00008d98 00000000 00000000 06000000 05000000 ................
+  0x00008da8 003c0000 00000000 00000000 00000000 .<..............
+  0x00008db8 00000000 00000000 a8000000 00000000 ................
+  0x00008dc8 a8000000 00000000 08000000 00000000 ................
+  0x00008dd8 01000000 05000000 580c0000 00000000 ........X.......
+  0x00008de8 00000000 00000000 00000000 00000000 ................
+  0x00008df8 282b0000 00000000 282b0000 00000000 (+......(+......
+  0x00008e08 08000000 00000000 01000000 05000000 ................
+  0x00008e18 003c0000 00000000 00000000 00000000 .<..............
+  0x00008e28 00000000 00000000 a8000000 00000000 ................
+  0x00008e38 a8000000 00000000 08000000 00000000 ................
+  0x00008e48 01000101 58000000 481f0000 00000000 ....X...H.......
+  0x00008e58 451f0000 48000000 04000800 50000000 E...H.......P...
+  0x00008e68 00000000 00000000 11200000 00000000 ......... ......
+  0x00008e78 00000000 00000000 9e620000 00000000 .........b......
+  0x00008e88 00000000 00000000 50000000 00000000 ........P.......
+  0x00008e98 00000000 00000000 3c0a2f2f 0300f31e ........<.//....
+  0x00008ea8 0a2e7665 7273696f 6e20382e 340a2e74 ..version 8.4..t
+  0x00008eb8 61726765 7420736d 5f38300a 2e616464 arget sm_80..add
+  0x00008ec8 72657373 5f73697a 65203634 0a3100ff ress_size 64.1..
+  0x00008ed8 31697369 626c6520 2e656e74 7279205f 1isible .entry _
+  0x00008ee8 5a313961 6374696f 6e4f6e53 696e676c Z19actionOnSingl
+  0x00008ef8 65517562 69745036 666c6f61 74325330 eQubitP6float2S0
+  0x00008f08 5f6d506d 280a2e70 6172616d 202e7536 _mPm(..param .u6
+  0x00008f18 34330013 115f3100 3f5f302c 3b00261f 43..._1.?_0,;.&.
+  0x00008f28 313b0027 1f323b00 27f30833 0a290a7b 1;.'.2;.'..3.).{
+  0x00008f38 0a2e7265 67202e70 72656420 25703c36 ..reg .pred %p<6
+  0x00008f48 3e3b1200 95663332 2025663c 34351200 >;...f32 %f<45..
+  0x00008f58 10621200 36723c38 1100f201 36342025 .b..6r<8....64 %
+  0x00008f68 72643c31 333e3b0a 0a0a6c64 8a00222e rd<13>;...ld..".
+  0x00008f78 7518004f 322c205b 9000193d 305d3b44 u..O2, [...=0];D
+  0x00008f88 001f3344 001c1f31 4400001f 3444001c ..3D...1D...4D..
+  0x00008f98 1f324400 001f3544 001c9133 5d3b0a6d .2D...5D...3];.m
+  0x00008fa8 6f762e75 3401a832 2c20256e 7469642e ov.u4..2, %ntid.
+  0x00008fb8 7816007c 332c2025 63746117 0044342c x..|3, %cta..D4,
+  0x00008fc8 20252c00 7161642e 6c6f2e73 18002335  %,.qad.lo.s..#5
+  0x00008fd8 2c340001 4f00f403 72343b0a 63767461 ,4..O...r4;.cvta
+  0x00008fe8 2e746f2e 676c6f62 616cab00 21362cb1 .to.global..!6,.
+  0x00008ff8 0001c400 041a0001 41004036 2c205b20 ........A.@6, [ 
+  0x00009008 00535d3b 0a6f72ce 0124312c 5a001136 .S];.or..$1,Z..6
+  0x00009018 5000432e 73363470 0012641c 00923b0a P.C.s64p..d...;.
+  0x00009028 73657470 2e676560 00357031 2c1c0073 setp.ge`.5p1,..s
+  0x00009038 64343b0a 7368725f 0013379b 00173132 d4;.shr_..7...12
+  0x00009048 00001900 3370322c d6002172 377a0003 ....3p2,..!r7z..
+  0x00009058 6c022333 2c1c0014 70320022 65717b00 l.#3,...p2."eq{.
+  0x00009068 25703496 00183132 0024352c 3700ff08 %p4...12.$5,7...
+  0x00009078 343b0a40 25703520 62726120 244c5f5f 4;.@%p5 bra $L__
+  0x00009088 4242305f 323b0a12 0104019a 002f6432 BB0_2;......./d2
+  0x00009098 31010511 381f0018 33310121 76320003 1...8...31.!v2..
+  0x000090a8 307b2566 e9003266 327d3b01 20385df1 0{%f..2f2};. 8].
+  0x000090b8 00146cf9 0214390b 0182333b 0a616464 ..l...9...3;.add
+  0x000090c8 2e731700 3631302c 76001f39 57000300 .s..610,v..9W...
+  0x000090d8 cb002366 36570010 31fa0233 6d756c74 ..#f6W..1..3mult
+  0x000090e8 03005700 02780018 35170001 57002166 ..W..x..5...W.!f
+  0x000090f8 32390054 3b0a7375 62180025 312c3500 29.T;.sub..%1,5.
+  0x00009108 1f30c500 04013600 243133c7 00232b38 .0....6.$13..#+8
+  0x00009118 71004577 696465ef 0122312c 11021a38 q.Ewide.."1,...8
+  0x00009128 ce00003c 0004ce00 2f313161 00041136 ...<..../11a...6
+  0x00009138 61001437 d1000043 0363666d 612e726e a..7...C.cfma.rn
+  0x00009148 a5001132 bd000388 00022d00 1831dd00 ...2......-..1..
+  0x00009158 223231a2 00010600 19371a00 15320f01 "21......7...2..
+  0x00009168 1c365500 15331201 0150012c 32322100 .6U..3...P.,22!.
+  0x00009178 17345600 0176001f 32e70104 12324100 .4V..v..2....2A.
+  0x00009188 15362201 3931365d 86000160 012d3235 .6".916]...`.-25
+  0x00009198 96011233 96011d36 97013533 312c3800 ...3...6..531,8.
+  0x000091a8 1f339801 041133bc 00163398 012c3234 .3....3...3..,24
+  0x000091b8 39011133 5a002633 32c30019 33390121 9..3Z.&32...39.!
+  0x000091c8 33371400 0f390100 2633389a 001c3556 37...9..&38...5V
+  0x000091d8 0007cf00 0255001b 38220027 34307800 .....U..8".'40x.
+  0x000091e8 0264001c 39230017 31d40101 23002832 .d..9#..1...#.(2
+  0x000091f8 34020135 34322cfa 011032e4 031b7402 4..542,...2...t.
+  0x00009208 0103fc02 342c207b 2d003c34 317d6500 ....4, {-.<41}e.
+  0x00009218 1733e000 01ab0029 34306500 26342c26 .3.....)40e.&4,&
+  0x00009228 011f3765 00051332 6500012d 00653433 ..7e...2e..-.e43
+  0x00009238 7d3b0a0a 3704903a 0a726574 3b0a0a7d };..7..:.ret;..}
+  0x00009248 35081f2e 3408084f 446f7562 34081c0e 5...4..ODoub4...
+  0x00009258 33000e34 080f3b00 241f313b 00271f32 3..4..;.$.1;.'.2
+  0x00009268 3b00270f 3408012c 31373508 3c313631 ;.'.4..,175.<161
+  0x00009278 36082d31 3237082f 32303708 060e9300 6.-127./207.....
+  0x00009288 0f37082b 0e44000f 37081f0e 44000f37 .7.+.D..7...D..7
+  0x00009298 081f0e44 000f3708 091f3421 08031f35 ...D..7...4!...5
+  0x000092a8 4e08021f 36370804 15374c07 1634e707 N...67...7L..4..
+  0x000092b8 0f370814 233634fb 05043808 30637674 .7..#64...8.0cvt
+  0x000092c8 6f00031a 00023907 1c374f08 0172001f o.....9..7O..r..
+  0x000092d8 38490000 13384900 2d2b384b 0021392c 8I...8I.-+8K.!9,
+  0x000092e8 2100074b 0015324b 00193990 0617398f !..K..2K..9...9.
+  0x000092f8 061c3847 00037b07 17394800 15334800 ..8G..{..9H..3H.
+  0x00009308 23313068 08136ef4 06267031 1c000c1b #10h..n..&p1....
+  0x00009318 00067f00 69323b0a 616e64b6 081131bb ....i2;.and...1.
+  0x00009328 080c3300 15343300 19333300 09b7080a ..3..43..33.....
+  0x00009338 33002436 2c35010a 66002337 2c1d002c 3.$6,5..f.#7,..,
+  0x00009348 70353300 15383300 0a660023 392c1d00 p53..83..f.#9,..
+  0x00009358 2c703733 00021601 1e323400 01f30702 ,p73.....24.....
+  0x00009368 1f002f70 39000a03 044d0022 6c746301 ../p9....M."ltc.
+  0x00009378 1170f005 031d000a 010a0241 08163502 .p.........A..5.
+  0x00009388 0a226c74 1a001170 820701a2 023a7231 ."lt...p.....:r1
+  0x00009398 31820024 342c2000 2a703104 01363135 1..$4, .*p1..615
+  0x000093a8 2c210065 313b0a6e 6f741b00 11361500 ,!.e1;.not...6..
+  0x000093b8 1135060a 27313607 0a1f3107 0a082f31 .5..'16...1.../1
+  0x000093c8 30080a0b 2f313109 0a162a31 310a0a2f 0.../11...*11../
+  0x000093d8 31320b0a 0427332c 7a002f31 320d0a11 12...'3,z./12...
+  0x000093e8 2f335d0d 0a5a2f31 310e0a03 1f340e0a /3]..Z/11....4..
+  0x000093f8 0328352c d1001f34 6300041a 360f0a1f .(5,...4c...6...
+  0x00009408 350f0a2d 06e10002 0f0a0655 080f7f00 5..-.......U....
+  0x00009418 0103180a 1634e200 2f3136e3 00011336 .....4../16....6
+  0x00009428 17030be3 0001c303 05e3001f 36640004 ............6d..
+  0x00009438 11376400 14386400 1d37b909 01c30003 .7d..8d..7......
+  0x00009448 8b001437 9f0a06e3 00025b09 02a20a28 ...7......[....(
+  0x00009458 3238e300 02ed0802 40001f33 33020411 28......@..33...
+  0x00009468 33380026 3335e300 2f3234e3 00011338 38.&35../24....8
+  0x00009478 350e0be3 0028392c e3001f38 64000411 5....(9,...8d...
+  0x00009488 38640014 3964001c 39e30002 b409038b 8d..9d..9.......
+  0x00009498 00022d00 1833e300 03bc0914 353e0a07 ..-..3......5>..
+  0x000094a8 1a001634 ba0b0b9b 0a253435 f2020119 ...4.....%45....
+  0x000094b8 022c3434 21001c36 770a1d34 44001737 .,44!..6w..4D..7
+  0x000094c8 3f020246 000c3c0c 2734389f 01010c00 ?..F..<.'48.....
+  0x000094d8 2c343723 001739a2 01026900 0c260b27 ,47#..9...i..&.'
+  0x000094e8 35300201 012f001f 34f10d05 01d20016 50.../..4.......
+  0x000094f8 35410448 2b33325d 13011135 f8001e35 5A.H+32]...5...5
+  0x00009508 eb032235 363a000d ec033635 372c3800 .."56:....657,8.
+  0x00009518 0fa70204 1135db00 26353977 003b3430 .....5..&59w.;40
+  0x00009528 5dc50011 365b0026 35382e01 1935490c ]...6[.&58...5I.
+  0x00009538 22363344 000e8d03 3536342c 40001f36 "63D....564,@..6
+  0x00009548 38050411 36a00027 36368200 1d388200 8...6..'66...8..
+  0x00009558 015c0026 36356a01 28363482 00223730 .\.&65j.(64.."70
+  0x00009568 44000e2c 03353731 2c40001f 37f10404 D..,.571,@..7...
+  0x00009578 1137a000 1737f104 2c353682 0011375c .7...7..,56...7\
+  0x00009588 00022a00 02cb0219 37910422 37374400 ..*.....7.."77D.
+  0x00009598 0ecb0226 37389f01 0ccc0226 3739d401 ...&78.....&79..
+  0x000095a8 0261000c 41022738 307c0102 64000c67 .a..A.'80|..d..g
+  0x000095b8 0d273831 7f010146 002c3830 23001732 .'81...F.,80#..2
+  0x000095c8 4001014c 002c3831 23001733 43010169 @..L.,81#..3C..i
+  0x000095d8 001c382e 0f273834 0401016f 001f38d4 ..8..'84...o..8.
+  0x000095e8 01041138 6a001738 d4013836 345d1501 ...8j..8..864]..
+  0x000095f8 12383f00 01270009 cd022239 303a000d .8?..'...."90:..
+  0x00009608 cd023539 312c3800 1f39c901 0411399b ..591,8..9....9.
+  0x00009618 001739c9 013b3732 5dc50011 395b0026 ..9..;72]...9[.&
+  0x00009628 39322e01 1939c901 22393744 000ecd02 92...9.."97D....
+  0x00009638 3639382c 40001f37 82000403 5a071630 698,@..7....Z..0
+  0x00009648 83001d38 50032131 305e0026 39396c01 ...8P.!10^.&99l.
+  0x00009658 28393884 00213130 6a013e31 3030d102 (98..!10j.>100..
+  0x00009668 46313035 2c44002f 31306207 05223036 F105,D./10b.."06
+  0x00009678 20001737 8a000d58 031131e2 05042d00  ..7...X..1...-.
+  0x00009688 02d80229 31309101 12313208 3e313037 ...)10...12.>107
+  0x00009698 db023631 3132ae01 0cdc0236 313133e4 ..6112.....6113.
+  0x000096a8 0122362c 2f000d24 0017348e 01123725 ."6,/..$..4...7%
+  0x000096b8 001d3325 00173593 01034a00 1d342500 ..3%..5...J..4%.
+  0x000096c8 17365401 02c9002d 31352500 18375801 .6T....-15%..7X.
+  0x000096d8 0370001d 36260018 38150112 3926000f .p..6&..8...9&..
+  0x000096e8 f1010422 31312000 1732f201 3939365d ..."11 ..2..996]
+  0x000096f8 26010245 06032a00 1a351b00 13343e00 &..E..*..5...4>.
+  0x00009708 0df00212 317d1104 3d001f32 e8010502 ....1}..=..2....
+  0x00009718 c0112731 32e8014c 3130345d d4000287 ..'12..L104]....
+  0x00009728 12042e00 0334000a 8c000251 083e3132 .....4.....Q.>12
+  0x00009738 37fb0213 31e81103 46002f33 318d0004 7...1...F./31...
+  0x00009748 03871118 335a090e ec131231 9412032e ....3Z.....1....
+  0x00009758 00038701 2a33328d 0013384a 000f0203 ....*32...8J....
+  0x00009768 00039301 0446000f 9e080412 31a21237 .....F......1..7
+  0x00009778 3134318d 001e328d 03026b08 032e0003 141...2...k.....
+  0x00009788 03030be7 02037308 2f343103 0300046e ......s./41....n
+  0x00009798 081f3004 03022734 37fb0102 2a000d6a ..0...'47...*..j
+  0x000097a8 0812316b 08049c01 0206030d 6d081231 ..1k........m..1
+  0x000097b8 6e08049f 0102c201 0d700812 31710804 n........p..1q..
+  0x000097c8 5b010208 032d3439 26001831 5e010252 [....-49&..1^..R
+  0x000097d8 002d3530 26001832 1a01027f 002d3531 .-50&..2.....-51
+  0x000097e8 260008c5 09017100 293530af 01353534 &.....q.)50..554
+  0x000097f8 2c0c0a2f 34338213 05123382 13032e00 ,../43....3.....
+  0x00009808 4d313533 7d690017 35630701 69002a38 M153}i..5c..i.*8
+  0x00009818 34690026 362caa07 0feb1306 14356900 4i.&6,.......5i.
+  0x00009828 22362c56 000e6900 1837f204 1238c201 "6,V..i..7...8..
+  0x00009838 0a830203 9107033f 052f3131 6d000514 .......?./11m...
+  0x00009848 376d0002 30002e35 376d0018 395c0203 7m..0..57m..9\..
+  0x00009858 27001932 6d003836 302ca902 1f356d00 '..2m.860,...5m.
+  0x00009868 0513396d 00033000 263539c7 141f31c7 ..9m..0.&59...1.
+  0x00009878 140f1438 8412af54 7269706c 65476174 ...8...TripleGat
+  0x00009888 65c61408 0f320012 0ec5140f 3a001c1f e....2......:...
+  0x00009898 313a0026 1f323a00 260ff61c 021c31c2 1:.&.2:.&.....1.
+  0x000098a8 14363630 39b01402 c2142d32 34c2142f .6609.....-24../
+  0x000098b8 3332c214 021231f6 130f4001 160f3914 32....1...@...9.
+  0x000098c8 001f3243 001b1f31 0415010f 43001b1f ..2C...1....C...
+  0x000098d8 32430000 1f344300 1b2f335d 5b110523 2C...4C../3][..#
+  0x000098e8 352c2e12 06b0141f 38c61402 1f39f314 5,......8....9..
+  0x000098f8 032f3130 de140401 be080136 00247238 ./10.......6.$r8
+  0x00009908 e4132e6c 64db1400 41032d35 5d2f1421 ...ld...A.-5]/.!
+  0x00009918 322c2000 072f1425 312c5600 2f31320d 2, ../.%1,V./12.
+  0x00009928 15071f35 c4140001 11090a10 1517324e ...5..........2N
+  0x00009938 000a1a12 23382c9a 00023200 0b4a001d ....#8,...2..J..
+  0x00009948 340f1517 334a001f 34980000 14399800 4...3J..4....9..
+  0x00009958 2e313699 001d3516 1517344f 001a351c .16...5...4O..5.
+  0x00009968 1017309a 001d394b 0013363a 10074c00 ..0...9K..6:..L.
+  0x00009978 17354c00 1a364c00 1731ad15 0e4c0002 .5L..6L..1...L..
+  0x00009988 18002731 314c0017 364c001f 37881c01 ..'11L..6L..7...
+  0x00009998 0353001d 364d0015 38631305 4d001737 .S..6M..8c..M..7
+  0x000099a8 4d001f38 fc15022f 3131fd15 072f3131 M..8.../11.../11
+  0x000099b8 fe151f2f 3131ff15 201331cf 1f0f0016 .../11.. .1.....
+  0x000099c8 19049c1f 0c011601 39001f38 01160302 ........9..8....
+  0x000099d8 35001936 35000114 00023b00 2d313037 5..65.....;.-107
+  0x000099e8 00070801 1a373700 26332c3f 160d0b01 .....77.&3,?....
+  0x000099f8 053c142f 2572d315 081d3337 00020f01 .<./%r....37....
+  0x00009a08 0e420101 2902021f 0001f515 0b370002 .B..)........7..
+  0x00009a18 12010e45 01019609 021f003c 70313737 ...E.......<p177
+  0x00009a28 0001d209 1f724801 00017c14 021f003d .....rH...|....=
+  0x00009a38 70313937 00021401 0e4a0101 c90b021f p197.....J......
+  0x00009a48 003d7032 31370006 13010a4a 0101070c .=p217.....J....
+  0x00009a58 021f003d 70323337 00011301 1e321301 ...=p237.....2..
+  0x00009a68 01d50902 1f003d70 32353700 15383700 ......=p257..87.
+  0x00009a78 0a130101 8f1e021f 002d7032 13012533 .........-p2..%3
+  0x00009a88 3037000a 1301013b 0c021f00 2d703213 07.....;....-p2.
+  0x00009a98 01253332 37000a13 0101a60a 021f003d .%327..........=
+  0x00009aa8 70333137 00153437 000a1301 016c0a02 p317..47.....l..
+  0x00009ab8 1f003d70 33333700 0113011e 33dc0001 ..=p337.....3...
+  0x00009ac8 300c021f 002d7033 13012533 3837000b 0....-p3..%387..
+  0x00009ad8 dc002439 2c1f003c 70333737 00253430 ..$9,..<p377.%40
+  0x00009ae8 37000adc 0001d109 021f003d 70333937 7..........=p397
+  0x00009af8 00153237 000adc00 01131502 1f002d70 ..27..........-p
+  0x00009b08 34130101 030a2e72 34a50001 a20c021f 4......r4.......
+  0x00009b18 003d7034 33370015 3637000b a5002437 .=p437..67....$7
+  0x00009b28 2c1f003d 70343537 00153837 000ba500 ,..=p457..87....
+  0x00009b38 24392c1f 003c7034 37370001 830c2e72 $9,..<p477.....r
+  0x00009b48 356e0001 760c021f 003d7034 39370015 5n..v....=p497..
+  0x00009b58 3237000a 6e000161 0c021f00 3d703531 27..n..a....=p51
+  0x00009b68 370002d7 000f3700 0024352c 1f003e70 7.....7..$5,..>p
+  0x00009b78 3533bd1a 14336e1a 0abf1a01 170c041f 53...3n.........
+  0x00009b88 00296433 c01a0447 080dc01a 01320c03 .)d3...G.....2..
+  0x00009b98 5d1c2a31 39870024 382c2100 3a703536 ].*19..$8,!.:p56
+  0x00009ba8 1b002639 2c210019 35c11a01 c30b3170 ..&9,!..5.....1p
+  0x00009bb8 3539c11a 273630c1 1a1f32c1 1a091434 59..'60...2....4
+  0x00009bc8 c11a2f6c 64110f00 09a11a00 23100f46 ../ld.......#..F
+  0x00009bd8 00040184 012f6431 1119052f 31311219 ...../d1.../11..
+  0x00009be8 051e3512 190fc61a 062f375d c61a5b3f ..5....../7]..[?
+  0x00009bf8 342b3800 19061f31 0019051f 3500190a 4+8....1....5...
+  0x00009c08 010f0107 c61a0d00 19012406 048a0002 ..........$.....
+  0x00009c18 b20f0fc6 1a481f34 c61a0323 32304705 .....H.4...#20G.
+  0x00009c28 0ae30001 7c0005e3 001f3246 0104021c ....|.....2F....
+  0x00009c38 1005c61a 2c3231e3 00273331 27190fc6 ....,21..'31'...
+  0x00009c48 1a4e1f34 c61a0314 324e050b e3000062 .N.4....2N.....b
+  0x00009c58 0006e300 0f640005 1938c61a 2f3233c6 .....d...8../23.
+  0x00009c68 1a2d06e3 0002c61a 06fa100f 7f000102 .-..............
+  0x00009c78 5c122634 36e3002f 3332e300 0113348c \.&46../32....4.
+  0x00009c88 050be300 003e0006 e3000f25 1404023b .....>.....%...;
+  0x00009c98 121435a3 141d326f 1d02c411 038b0001 ..5...2o........
+  0x00009ca8 2d002834 34e30001 46050359 1b0ade11 -.(44...F..Y....
+  0x00009cb8 02951102 40001f35 7f000413 35341a06 ....@..5....54..
+  0x00009cc8 e3002f34 30e30001 13360106 0be30000 ../40....6......
+  0x00009cd8 560206e3 000f5d04 0402f410 1436ec13 V.....]......6..
+  0x00009ce8 1d326f1d 028b1a02 8b00022d 00283535 .2o........-.(55
+  0x00009cf8 e300021d 1901a805 38663631 e3000214 ........8f61....
+  0x00009d08 19024000 2f36357f 00040238 001738e3 ..@./65....8..8.
+  0x00009d18 000f6f04 01027809 1d36e300 00730106 ..o...x..6...s..
+  0x00009d28 e3000f6f 040402cb 1a1437c2 051d326f ...o......7...2o
+  0x00009d38 041137c3 00028b00 03f81a18 36e30002 ..7.........6...
+  0x00009d48 c41a2236 38470008 e30003be 1a014000 .."68G........@.
+  0x00009d58 1f376201 0402c81a 263739e3 002f3536 .7b.....&79../56
+  0x00009d68 e3000002 240a1c37 e30001e8 0305e300 ....$..7........
+  0x00009d78 0ff02805 02a81a14 38b5051d 336f0402 ..(.....8...3o..
+  0x00009d88 6b18028b 00243832 e91306e3 00353837 k....$82.....587
+  0x00009d98 2c571b29 38331a00 1f38521e 0616387e ,W.)83...8R...8~
+  0x00009da8 06015f00 1c385615 1839c805 1237881a .._..8V..9...7..
+  0x00009db8 0c230008 cb051436 a51a0a23 0017322b .#.....6...#..2+
+  0x00009dc8 0514387a 1a0a2300 1c33521e 1c393319 ..8z..#..3R..93.
+  0x00009dd8 2739348e 04123919 190c2300 01c80126 '94...9...#....&
+  0x00009de8 3335b104 2f393406 1b0202f1 03019109 35../94.........
+  0x00009df8 2c663916 01263937 f4030214 041c39ba ,f9..&97......9.
+  0x00009e08 16273938 54031431 181b0a23 00173957 .'98T..1...#..9W
+  0x00009e18 031430eb 1a092300 038f1903 b8021232 ..0...#........2
+  0x00009e28 c7190d24 001731bc 0222312c 37000d25 ...$..1.."1,7..%
+  0x00009e38 0017321e 02123325 000fab18 0505401b ..2...3%......@.
+  0x00009e48 06d0020b a41c0301 16032a00 0b980826 ..........*....&
+  0x00009e58 382ca81b 0a9b0838 30392c3d 000f3c08 8,.....809,=..<.
+  0x00009e68 0502db08 36313131 80000ead 1c03201b ....6111...... .
+  0x00009e78 042d0002 43081a30 81180153 03004900 .-..C..0...S..I.
+  0x00009e88 0e460803 151b0546 000fbd04 0404171b .F.....F........
+  0x00009e98 1731bf04 0fb61c00 03ae0826 31379e02 .1.........&17..
+  0x00009ea8 013d1b07 8c0002b7 0803411b 0aef0705 .=........A.....
+  0x00009eb8 c91a0246 000f8e07 0505121b 07f4070f ...F............
+  0x00009ec8 b81c0002 40032731 3295073a 3132338c ....@.'12..:123.
+  0x00009ed8 00133949 000e9807 050e1b03 46000f93 ..9I........F...
+  0x00009ee8 21040412 1b163335 0b02dc1b 0a8c0002 !.....35........
+  0x00009ef8 6903032d 00022a03 39313330 8c000175 i..-..*.9130...u
+  0x00009f08 0e04461b 0b1f1904 0d1b0346 000f7e05 ..F........F..~.
+  0x00009f18 0405111b 0780050f e81b0102 6d08032e ............m...
+  0x00009f28 00027103 39313337 8d0002b0 0803461b ..q.9137......F.
+  0x00009f38 0aeb0605 64180246 000fb408 0505111b ....d..F........
+  0x00009f48 07b6080e e81b05b3 1a273435 b6030a59 .........'45...Y
+  0x00009f58 0804b01a 2e343695 0604a61a 0346002f .....46......F./
+  0x00009f68 35308d00 04243532 321a068d 000fe81b 50...$522.......
+  0x00009f78 0002a704 032e0002 3c0601ce 1a088d00 ........<.......
+  0x00009f88 02f9192e 35333f06 283135f2 030c4206 ....53?.(15...B.
+  0x00009f98 04c61902 2b040369 000de804 283630cd ....+..i....(60.
+  0x00009fa8 03036c00 0dea0402 490504d0 0302f303 ..l.....I.......
+  0x00009fb8 1d36eb04 02542304 8d0302e8 1b2d3631 .6...T#......-61
+  0x00009fc8 26001833 90030272 001d3685 1f02db08 &..3...r..6.....
+  0x00009fd8 27313254 063d3136 33260018 35500303 '12T.=163&..5P..
+  0x00009fe8 72000d87 1f022d09 030d0302 5a063d31 r.....-.....Z.=1
+  0x00009ff8 36352600 17371003 03e0012d 36362600 65&..7.....-66&.
+  0x0000a008 1838cc02 0310010d 181d02dc 2304cf02 .8..........#...
+  0x0000a018 02f2021d 367c0128 37308b02 023d011d ....6|.(70...=..
+  0x0000a028 367c0128 37318e02 020d002d 37302600 6|.(71.....-70&.
+  0x0000a038 18324a02 0263012f 37319e02 04133720 .2J..c./71....7 
+  0x0000a048 0008a70d 3932385d 5c02027f 092f3137 ....928]\..../17
+  0x0000a058 69060002 cd062f31 37690600 02e60805 i...../17i......
+  0x0000a068 3d000f69 06050242 24273138 69062e31 =..i...B$'18i..1
+  0x0000a078 33c60402 dd232831 386a061a 376a0602 3....#(18j..7j..
+  0x0000a088 cb211231 70240b6a 06029909 0546000f .!.1p$.j.....F..
+  0x0000a098 6a060502 a0092731 386a062e 3134c604 j.....'18j..14..
+  0x0000a0a8 034e0927 3837b802 1a386b06 0334221f .N.'87...8k..4".
+  0x0000a0b8 386b0601 032b2203 46002f39 328d0004 8k...+".F./92...
+  0x0000a0c8 024b0927 31396b06 2e3135c6 0402e608 .K.'19k..15.....
+  0x0000a0d8 2831396c 062a3933 8d001339 4a000e6c (19l.*93...9J..l
+  0x0000a0e8 061232de 08054600 0f6c0604 1232e108 ..2...F..l...2..
+  0x0000a0f8 38323032 cf0f0dc6 041232fe 23273230 8202......2.#'20
+  0x0000a108 6d063832 30308d00 1232b822 2f32306d m.8200...2."/20m
+  0x0000a118 06001232 96080546 000f6d06 041232df ...2...F..m...2.
+  0x0000a128 08283230 6d061d36 86071232 120b032e .(20m..6...2....
+  0x0000a138 00027b03 2932306d 06123212 0b2f3230 ..{.)20m..2../20
+  0x0000a148 6d060012 32970804 46002f31 338d0004 m...2...F./13...
+  0x0000a158 02e10828 32316d06 1d37c102 1132b411 ...(21m..7...2..
+  0x0000a168 042e0002 bc033932 31348d00 0450110f ......9214...P..
+  0x0000a178 6d060012 32980804 46000f10 110602e2 m...2...F.......
+  0x0000a188 08283232 6d061d38 c1021132 cc0e042e .(22m..8...2....
+  0x0000a198 00026d06 3a323231 8d001337 4a000e6d ..m.:221...7J..m
+  0x0000a1a8 06283232 f6030c6d 06373232 392f0403 .(22...m.7229/..
+  0x0000a1b8 69000cf1 04383233 30d00303 6c001d39 i....8230...l..9
+  0x0000a1c8 26001831 d303024c 002d3330 26001832 &..1...L.-30&..2
+  0x0000a1d8 8f031238 26001d31 26001833 9203022c ...8&..1&..3...,
+  0x0000a1e8 002d3332 26001834 4e03026e 012d3333 .-32&..4N..n.-33
+  0x0000a1f8 26001835 51030372 001d3426 0017360d &..5Q..r..4&..6.
+  0x0000a208 03026d06 3d323335 26001737 10030333 ..m.=235&..7...3
+  0x0000a218 032d3336 26001838 cc021231 26001d37 .-36&..8...1&..7
+  0x0000a228 26001839 cf020372 000d7c01 2834308b &..9...r..|.(40.
+  0x0000a238 02123226 000d7c01 2834318e 02020d00 ..2&..|.(41.....
+  0x0000a248 2d343026 0018324a 02123326 000f6d06 -40&..2J..3&..m.
+  0x0000a258 04233234 2000086d 06393932 5d5c0202 .#24 ..m.992]\..
+  0x0000a268 93242e32 346d0632 3234381b 000e6d06 .$.24m.2248...m.
+  0x0000a278 13323801 043d000f 6d060413 32850117 .28..=..m...2...
+  0x0000a288 356d062e 3230c604 02501203 2e000377 5m..20...P.....w
+  0x0000a298 02293439 8c000259 122f3235 6d060012 .)49...Y./25m...
+  0x0000a2a8 32cb0905 46000f6d 06041232 cf093832 2...F..m...2..82
+  0x0000a2b8 35388d00 0ec60403 ed012735 37b80229 58........'57..)
+  0x0000a2c8 35368d00 026e092f 32356d06 00123264 56...n./25m...2d
+  0x0000a2d8 09044600 2f36328d 00040265 09273236 ..F./62....e.'26
+  0x0000a2e8 6d063e32 31368d00 02630027 3634f902 m.>216...c.'64..
+  0x0000a2f8 2a36338d 0013394a 000f6d06 0002e708 *63...9J..m.....
+  0x0000a308 0546000f 6d060503 6e022737 328d002d .F..m...n.'72..-
+  0x0000a318 32348d00 02111228 32376d06 2937308d 24.....(27m.)70.
+  0x0000a328 00025412 2f32376d 0601029a 08054600 ..T./27m......F.
+  0x0000a338 0f6d0605 02e30818 325a123d 3233328d .m......2Z.=232.
+  0x0000a348 00034605 2737387b 030afd11 13321f03 ..F.'78{.....2..
+  0x0000a358 1f376d06 01029a08 0446002f 38338d00 .7m......F./83..
+  0x0000a368 0402e408 37323836 8d000e12 2f123233 ....7286..../.23
+  0x0000a378 12283238 6d062938 348d0002 35122f32 .(28m.)84...5./2
+  0x0000a388 386d0601 029a0804 46000fcf 2c051332 8m......F...,..2
+  0x0000a398 32122839 338d000e c10202cd 11283239 2.(93........(29
+  0x0000a3a8 6d060ad5 2c1232cd 112f3239 6d060102 m...,.2../29m...
+  0x0000a3b8 9a082f32 346d0603 02db0827 32346d06 ../24m.....'24m.
+  0x0000a3c8 0dc21112 33e40828 32356d06 0dc41112 ....3..(25m.....
+  0x0000a3d8 33a80527 32356d06 1d33c511 1233a805 3..'25m..3...3..
+  0x0000a3e8 2732356d 063d3330 31260018 33920312 '25m.=301&..3...
+  0x0000a3f8 3726001d 32260018 344e0312 3926001d 7&..2&..4N..9&..
+  0x0000a408 33260018 35510303 72001d34 26001736 3&..5Q..r..4&..6
+  0x0000a418 0d0302ea 003d3330 35260017 37100302 .....=305&..7...
+  0x0000a428 33033d33 30362600 1838cc02 12312600 3.=306&..8...1&.
+  0x0000a438 1d372600 1839cf02 0372000d 7c01024f .7&..9...r..|..O
+  0x0000a448 0e273238 6d063d33 30392600 18318e02 .'28m.=309&..1..
+  0x0000a458 0272002d 31302600 18324a02 12332600 .r.-10&..2J..3&.
+  0x0000a468 0f6d0604 23333120 00076d06 15321316 .m..#31 ..m..2..
+  0x0000a478 025c0212 330c022e 33316d06 1233950e .\..3...31m..3..
+  0x0000a488 2e33316d 06123385 09053d00 0f6d0604 .31m..3...=..m..
+  0x0000a498 1233cf09 2833326d 0601c413 0ad50003 .3..(32m........
+  0x0000a4a8 d80e2732 30770229 31398c00 03d50e1f ..'20w.)19......
+  0x0000a4b8 326d0600 1233cb09 0546000f 6d060413 2m...3...F..m...
+  0x0000a4c8 33840227 32388d00 0ed11312 33710903 3..'28......3q..
+  0x0000a4d8 2e000434 00096d06 12336e09 2f33326d ...4..m..3n./32m
+  0x0000a4e8 06001333 351b0346 000f371b 06031f16 ...35..F..7.....
+  0x0000a4f8 09391b0e d2131333 ec022733 34f9020a .9.....3..'34...
+  0x0000a508 dc1a1333 35031f33 6d060012 33e70805 ...35..3m...3...
+  0x0000a518 46000f6d 06041233 e8082833 346d060e F..m...3..(34m..
+  0x0000a528 d3131233 9b0f032e 00033a03 2934308d ...3......:.)40.
+  0x0000a538 0002980f 2f33346d 06001233 9a080546 ..../34m...3...F
+  0x0000a548 000f6d06 041233e3 08283334 6d060ed4 ..m...3..(34m...
+  0x0000a558 131233dc 0f032e00 037b0329 34378d00 ..3......{.)47..
+  0x0000a568 0226122f 33346d06 0012339a 08044600 .&./34m...3...F.
+  0x0000a578 2f35338d 000402e4 08273335 6d061e33 /53......'35m..3
+  0x0000a588 d4131233 5d12032e 0003bc03 2935348d ...3].......)54.
+  0x0000a598 0003a300 1f356d06 00133360 04034600 .....5m...3`..F.
+  0x0000a5a8 2f36308d 000402e4 08273336 6d061e33 /60......'36m..3
+  0x0000a5b8 d4131233 e1112733 366d063a 3336318d ...3..'36m.:361.
+  0x0000a5c8 0013374a 000e6d06 12339a08 2f33316d ..7J..m..3../31m
+  0x0000a5d8 06021233 db082633 316d061d 33cb1112 ...3..&31m..3...
+  0x0000a5e8 33e40827 33326d06 1d33cb11 38333731 3..'32m..3..8371
+  0x0000a5f8 d303024c 000dcb11 38333732 8f03029c ...L....8372....
+  0x0000a608 002d3731 26001833 92030272 002d3732 .-71&..3...r.-72
+  0x0000a618 26001834 4e0302ca 001d376d 06020e09 &..4N.....7m....
+  0x0000a628 2833336d 061d376d 06025709 2833346d (33m..7m..W.(34m
+  0x0000a638 061d372f 01026109 2833346d 062d3736 ..7/..a.(34m.-76
+  0x0000a648 26001838 cc021231 26000d6d 06026606 &..8...1&..m..f.
+  0x0000a658 2833346d 060d8e36 38333830 8b02023d (34m...68380...=
+  0x0000a668 012d3739 26001831 8e02020d 000d9436 .-79&..1.......6
+  0x0000a678 38333832 4a020263 012f3831 9e020404 8382J..c./81....
+  0x0000a688 20001834 281f2930 5d5c0202 a00e2f33  ..4(.)0]\..../3
+  0x0000a698 386d0600 02950e2f 33386d06 00028509 8m...../38m.....
+  0x0000a6a8 053d000f 6d060502 cf093833 39318100 .=..m.....8391..
+  0x0000a6b8 0ec60404 d80e1730 77022938 398c0004 .......0w.)89...
+  0x0000a6c8 26120f6d 060102cb 09054600 0f6d0605 &..m......F..m..
+  0x0000a6d8 02cf0927 33396d06 1e33d413 12347109 ...'39m..3...4q.
+  0x0000a6e8 032e0003 b8022839 368d0012 346e092f ......(96...4n./
+  0x0000a6f8 33396d06 00123464 09034600 3f343032 39m...4d..F.?402
+  0x0000a708 8d000312 34650927 34306d06 1e33d413 ....4e.'40m..3..
+  0x0000a718 1234f408 032e0013 330d0009 1d041234 .4......3......4
+  0x0000a728 f1081234 90090a6d 061234e7 08054600 ...4...m..4...F.
+  0x0000a738 0f6d0604 1234e808 2734316d 061e33d4 .m...4..'41m..3.
+  0x0000a748 1312349b 0f273431 6d063934 31308d00 ..4..'41m.9410..
+  0x0000a758 02bd012f 34316d06 00123476 04054600 .../41m...4v..F.
+  0x0000a768 0f6d0604 1234e308 2734316d 061e33d4 .m...4..'41m..3.
+  0x0000a778 131234dc 0f032e00 027b0339 3431378d ..4......{.9417.
+  0x0000a788 00022612 2f34316d 06001234 9a080446 ..&./41m...4...F
+  0x0000a798 002f3233 8d000402 e4083834 32368d00 ./23......8426..
+  0x0000a7a8 0dc10212 345d1227 34326d06 39343234 ....4].'42m.9424
+  0x0000a7b8 8d00025b 122f3432 6d060012 349a0804 ...[./42m...4...
+  0x0000a7c8 46002f33 308d0004 02e40837 3433338d F./30......7433.
+  0x0000a7d8 000ed413 1234e111 2734336d 063a3433 .....4..'43m.:43
+  0x0000a7e8 318d0013 374a000e 6d062834 33f6030c 1...7J..m.(43...
+  0x0000a7f8 6d063734 33392f04 0369000c f1043834 m.7439/..i....84
+  0x0000a808 3430d003 036c001d 39260018 31d30302 40...l..9&..1...
+  0x0000a818 4c000dcb 111234a8 05273339 6d063d34 L.....4..'39m.=4
+  0x0000a828 34312600 18339203 0272002d 34322600 41&..3...r.-42&.
+  0x0000a838 18344e03 026e012d 34332600 18355103 .4N..n.-43&..5Q.
+  0x0000a848 0372001d 34260017 360d0302 6d063d34 .r..4&..6...m.=4
+  0x0000a858 34352600 17371003 0333030d cc361234 45&..7...3...6.4
+  0x0000a868 66062734 316d063d 34343726 001839cf f.'41m.=447&..9.
+  0x0000a878 02037200 0d7c0128 35308b02 0278002d ..r..|.(50...x.-
+  0x0000a888 34392600 18318e02 020d002d 35302600 49&..1.....-50&.
+  0x0000a898 18324a02 12332600 0f6d0604 23343520 .2J..3&..m..#45 
+  0x0000a8a8 00086d06 01e51507 5c0202a0 0e2e3435 ..m.....\.....45
+  0x0000a8b8 6d061234 950e2e34 356d0612 34850905 m..4...45m..4...
+  0x0000a8c8 3d000f6d 06041334 13012736 31810001 =..m...4..'61...
+  0x0000a8d8 c8130ad5 0002d80e 032e0003 77022935 ............w.)5
+  0x0000a8e8 398c0002 d50e2f34 366d0600 1234cb09 9...../46m...4..
+  0x0000a8f8 0546000f 6d060412 34cf0919 34dd240e .F..m...4...4.$.
+  0x0000a908 d4131334 7b012736 37b8020a 80241334 ...4{.'67....$.4
+  0x0000a918 c4011f36 6d060102 64090446 002f3732 ...6m...d..F./72
+  0x0000a928 8d000402 65093834 37358d00 0ec60402 ....e.8475......
+  0x0000a938 f408032e 0003f902 2a37338d 0013394a ........*73...9J
+  0x0000a948 000f6d06 0002e708 0546000f 6d060502 ..m......F..m...
+  0x0000a958 e8082734 386d061e 34d41312 349b0f28 ..'48m..4...4..(
+  0x0000a968 34386d06 2938308d 0002980f 2f34386d 48m.)80...../48m
+  0x0000a978 0601029a 08054600 0f6d0605 02e30827 ......F..m.....'
+  0x0000a988 34386d06 1e34d413 1234dc0f 032e0003 48m..4...4......
+  0x0000a998 7b031a38 6d060226 122f3438 6d060102 {..8m..&./48m...
+  0x0000a9a8 9a080446 002f3933 8d000402 e4082734 ...F./93......'4
+  0x0000a9b8 396d061e 34d41312 345d1228 34396d06 9m..4...4].(49m.
+  0x0000a9c8 2839348d 0012355b 122f3439 6d060013 (94...5[./49m...
+  0x0000a9d8 359a0802 46003f35 30308d00 031235e4 5...F.?500....5.
+  0x0000a9e8 08273530 6d061e34 d4131235 e1112735 .'50m..4...5..'5
+  0x0000a9f8 306d063a 3530318d 00123716 000f6d06 0m.:501...7...m.
+  0x0000aa08 00283530 f6030c6d 06373530 392f0403 .(50...m.7509/..
+  0x0000aa18 69000cf1 04383531 30d00303 6c001d39 i....8510...l..9
+  0x0000aa28 26001831 d303024c 000dcb11 38353132 &..1...L....8512
+  0x0000aa38 8f031238 26001d31 26001833 92030272 ...8&..1&..3...r
+  0x0000aa48 002d3132 26001834 4e03026e 012d3133 .-12&..4N..n.-13
+  0x0000aa58 26001835 51030372 001d3426 0017360d &..5Q..r..4&..6.
+  0x0000aa68 0302e205 3d353135 26001737 10030233 ....=515&..7...3
+  0x0000aa78 033d3531 36260018 38cc0202 52002d31 .=516&..8...R.-1
+  0x0000aa88 37260018 39cf0203 72000d7c 01024f0e 7&..9...r..|..O.
+  0x0000aa98 2734396d 063d3531 39260018 318e0202 '49m.=519&..1...
+  0x0000aaa8 72002d32 30260018 324a0212 3326000f r.-20&..2J..3&..
+  0x0000aab8 6d060423 35322000 18349e02 29385d5c m..#52 ..4..)8]\
+  0x0000aac8 02039a01 1e326d06 1335db01 1e326d06 .....2m..5...2m.
+  0x0000aad8 12358509 053d000f 6d060412 35cf0927 .5...=..m...5..'
+  0x0000aae8 35336d06 1134c813 0ad50002 d80e032e 53m..4..........
+  0x0000aaf8 00037702 2932398c 0002d50e 2f35336d ..w.)29...../53m
+  0x0000ab08 06001235 cb090546 000f6d06 041235cf ...5...F..m...5.
+  0x0000ab18 09283533 6d060ed4 13133519 0f273337 .(53m.....5..'37
+  0x0000ab28 b8022933 368d0002 6e092f35 336d0600 ..)36...n./53m..
+  0x0000ab38 12356409 0446002f 34328d00 04031317 .5d..F./42......
+  0x0000ab48 18346d06 0ed41312 35f40803 2e0003f9 .4m.....5.......
+  0x0000ab58 022a3433 8d001339 4a000e6d 06133505 .*43...9J..m..5.
+  0x0000ab68 03044600 0f6d0604 1235e808 37353532 ..F..m...5..7552
+  0x0000ab78 8d000ed4 1312359b 0f032e00 03770029 ......5......w.)
+  0x0000ab88 35308d00 02980f2f 35356d06 0012359a 50...../55m...5.
+  0x0000ab98 08054600 0f6d0604 1235e308 38353539 ..F..m...5..8559
+  0x0000aba8 8d000d87 071235dc 0f032e00 037b030a ......5......{..
+  0x0000abb8 3c481235 26122f35 356d0600 12359a08 <H.5&./55m...5..
+  0x0000abc8 0446002f 36338d00 0402e408 37353636 .F./63......7566
+  0x0000abd8 8d000ed4 1312355d 12032e00 03bc030a ......5]........
+  0x0000abe8 47481235 5b122f35 366d0601 04320002 GH.5[./56m...2..
+  0x0000abf8 46002f37 308d0004 033b0406 4e483e34 F./70....;..NH>4
+  0x0000ac08 2b35d413 1235e111 2835376d 062a3731 +5...5..(57m.*71
+  0x0000ac18 8d001337 4a000f6d 0600029a 082f3532 ...7J..m...../52
+  0x0000ac28 6d060302 db082735 326d060d cb111235 m.....'52m.....5
+  0x0000ac38 e4082835 336d060d cb113835 3831d303 ..(53m....8581..
+  0x0000ac48 024c000d cb113835 38328f03 029c000d .L....8582......
+  0x0000ac58 62483835 38339203 0272000d 65483835 bH8583...r..eH85
+  0x0000ac68 38344e03 02ca002d 38332600 18355103 84N....-83&..5Q.
+  0x0000ac78 0372000d 6d060257 09030d03 0368032d .r..m..W.....h.-
+  0x0000ac88 38352600 17371003 0333032d 38362600 85&..7...3.-86&.
+  0x0000ac98 1838cc02 0252002d 38372600 1839cf02 .8...R.-87&..9..
+  0x0000aca8 0372000d 7c012839 308b0202 3d010d53 .r..|.(90...=..S
+  0x0000acb8 2e383539 318e0202 0d000d56 2e12358b .8591......V..5.
+  0x0000acc8 09283537 6d060d59 2e373539 33192f12 .(57m..Y.7593./.
+  0x0000acd8 32ad280a e0022639 34cc472f 3837d142 2.(...&94.G/87.B
+  0x0000ace8 0c032e00 2d3539a7 43123542 07044529 ....-59.C.5B..E)
+  0x0000acf8 026b000b 4b03023f 07059229 1f37d142 .k..K..?...).7.B
+  0x0000ad08 0c033000 2d3539ab 43293539 45231232 ..0.-59.C)59E#.2
+  0x0000ad18 ab1c0b6d 0028382c 92230f6d 00052432 ...m.(8,.#.m..$2
+  0x0000ad28 316d0022 382c5a00 0e6d0018 39451d12 1m."8,Z..m..9E..
+  0x0000ad38 32ab1609 6d001336 091d0492 1d0f6d00 2...m..6......m.
+  0x0000ad48 0603ee44 0330003c 3539396d 001236dc ...D.0.<599m..6.
+  0x0000ad58 0a283336 6d001b38 6d002832 2c92170f .(36m..8m.(2,...
+  0x0000ad68 6d000603 f2440330 002d3630 44593836 m....D.0.-60DY86
+  0x0000ad78 30334511 1232ab0a 0b6d0028 342c9211 03E..2...m.(4,..
+  0x0000ad88 0f6d0006 03210203 30002d36 30210212 .m...!..0.-60!..
+  0x0000ad98 368e1027 35306d00 2b35326d 0028362c 6..'50m.+52m.(6,
+  0x0000ada8 920b0f6d 00060321 02033000 2d363021 ...m...!..0.-60!
+  0x0000adb8 02293630 4505026d 001b396d 0028382c .)60E..m..9m.(8,
+  0x0000adc8 92050f6d 00051333 21020330 00363630 ...m...3!..0.660
+  0x0000add8 375f4515 325f4550 0a7d0a0a 00000000 7_E.2_EP.}......
```

#### readelf --wide --decompress --hex-dump=.eh_frame_hdr {}

```diff
@@ -1,30 +1,30 @@
 
 Hex dump of section '.eh_frame_hdr':
-  0x0000ad58 011b033b ac010000 34000000 d86dffff ...;....4....m..
-  0x0000ad68 c8010000 f871ffff 18080000 7873ffff .....q......xs..
-  0x0000ad78 f0010000 8873ffff 08020000 9873ffff .....s.......s..
-  0x0000ad88 20020000 b873ffff 38020000 d873ffff  ....s..8....s..
-  0x0000ad98 50020000 f873ffff 68020000 1874ffff P....s..h....t..
-  0x0000ada8 80020000 3874ffff 98020000 5874ffff ....8t......Xt..
-  0x0000adb8 b0020000 7874ffff c8020000 9874ffff ....xt.......t..
-  0x0000adc8 e0020000 0875ffff 00030000 7875ffff .....u......xu..
-  0x0000add8 20030000 d875ffff 40030000 6876ffff  ....u..@...hv..
-  0x0000ade8 58030000 e876ffff 70030000 6877ffff X....v..p...hw..
-  0x0000adf8 90030000 a877ffff a8030000 f877ffff .....w.......w..
-  0x0000ae08 c0030000 6878ffff e0030000 a878ffff ....hx.......x..
-  0x0000ae18 f8030000 e878ffff 10040000 2879ffff .....x......(y..
-  0x0000ae28 28040000 f879ffff 48040000 c87affff (....y..H....z..
-  0x0000ae38 68040000 987bffff 88040000 e87bffff h....{.......{..
-  0x0000ae48 a0040000 587cffff b8040000 f87dffff ....X|.......}..
-  0x0000ae58 d0040000 987fffff e8040000 3881ffff ............8...
-  0x0000ae68 00050000 d882ffff 18050000 7884ffff ............x...
-  0x0000ae78 30050000 e884ffff 48050000 3885ffff 0.......H...8...
-  0x0000ae88 60050000 5886ffff 78050000 8886ffff `...X...x.......
-  0x0000ae98 90050000 e886ffff d0050000 1887ffff ................
-  0x0000aea8 e8050000 1889ffff 00060000 b88bffff ................
-  0x0000aeb8 50060000 888cffff 80060000 988cffff P...............
-  0x0000aec8 98060000 f891ffff e8060000 c892ffff ................
-  0x0000aed8 18070000 d892ffff 30070000 8897ffff ........0.......
-  0x0000aee8 80070000 5898ffff b0070000 6898ffff ....X.......h...
-  0x0000aef8 c8070000 889cffff 60080000          ........`...
+  0x0000ade8 011b033b ac010000 34000000 886dffff ...;....4....m..
+  0x0000adf8 c8010000 b871ffff 18080000 3873ffff .....q......8s..
+  0x0000ae08 f0010000 4873ffff 08020000 5873ffff ....Hs......Xs..
+  0x0000ae18 20020000 7873ffff 38020000 9873ffff  ...xs..8....s..
+  0x0000ae28 50020000 b873ffff 68020000 d873ffff P....s..h....s..
+  0x0000ae38 80020000 f873ffff 98020000 1874ffff .....s.......t..
+  0x0000ae48 b0020000 3874ffff c8020000 5874ffff ....8t......Xt..
+  0x0000ae58 e0020000 c874ffff 00030000 3875ffff .....t......8u..
+  0x0000ae68 20030000 9875ffff 40030000 2876ffff  ....u..@...(v..
+  0x0000ae78 58030000 a876ffff 70030000 2877ffff X....v..p...(w..
+  0x0000ae88 90030000 6877ffff a8030000 b877ffff ....hw.......w..
+  0x0000ae98 c0030000 2878ffff e0030000 6878ffff ....(x......hx..
+  0x0000aea8 f8030000 a878ffff 10040000 e878ffff .....x.......x..
+  0x0000aeb8 28040000 b879ffff 48040000 887affff (....y..H....z..
+  0x0000aec8 68040000 587bffff 88040000 a87bffff h...X{.......{..
+  0x0000aed8 a0040000 187cffff b8040000 b87dffff .....|.......}..
+  0x0000aee8 d0040000 587fffff e8040000 f880ffff ....X...........
+  0x0000aef8 00050000 9882ffff 18050000 3884ffff ............8...
+  0x0000af08 30050000 a884ffff 48050000 f884ffff 0.......H.......
+  0x0000af18 60050000 1886ffff 78050000 4886ffff `.......x...H...
+  0x0000af28 90050000 a886ffff d0050000 d886ffff ................
+  0x0000af38 e8050000 d888ffff 00060000 788bffff ............x...
+  0x0000af48 50060000 488cffff 80060000 588cffff P...H.......X...
+  0x0000af58 98060000 b891ffff e8060000 8892ffff ................
+  0x0000af68 18070000 9892ffff 30070000 6897ffff ........0...h...
+  0x0000af78 80070000 3898ffff b0070000 4898ffff ....8.......H...
+  0x0000af88 c8070000 689cffff 60080000          ....h...`...
```

#### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,112 +1,112 @@
 
 Hex dump of section '.eh_frame':
-  0x0000af08 14000000 00000000 017a5200 01781001 .........zR..x..
-  0x0000af18 1b0c0708 90010000 24000000 1c000000 ........$.......
-  0x0000af28 086cffff 20040000 000e1046 0e184a0f .l.. ......F..J.
-  0x0000af38 0b770880 003f1a3b 2a332422 00000000 .w...?.;*3$"....
-  0x0000af48 14000000 44000000 8071ffff 05000000 ....D....q......
-  0x0000af58 00000000 00000000 14000000 5c000000 ............\...
-  0x0000af68 7871ffff 0c000000 00000000 00000000 xq..............
-  0x0000af78 14000000 74000000 7071ffff 17000000 ....t...pq......
-  0x0000af88 00000000 00000000 14000000 8c000000 ................
-  0x0000af98 7871ffff 16000000 00000000 00000000 xq..............
-  0x0000afa8 14000000 a4000000 8071ffff 17000000 .........q......
-  0x0000afb8 00000000 00000000 14000000 bc000000 ................
-  0x0000afc8 8871ffff 17000000 00000000 00000000 .q..............
-  0x0000afd8 14000000 d4000000 9071ffff 17000000 .........q......
-  0x0000afe8 00000000 00000000 14000000 ec000000 ................
-  0x0000aff8 9871ffff 17000000 00000000 00000000 .q..............
-  0x0000b008 14000000 04010000 a071ffff 17000000 .........q......
-  0x0000b018 00000000 00000000 14000000 1c010000 ................
-  0x0000b028 a871ffff 16000000 00000000 00000000 .q..............
-  0x0000b038 1c000000 34010000 b071ffff 61000000 ....4....q..a...
-  0x0000b048 00410e10 8302470e 2002570e 10410e08 .A....G. .W..A..
-  0x0000b058 1c000000 54010000 0072ffff 6a000000 ....T....r..j...
-  0x0000b068 00410e10 8302470e 2002600e 10410e08 .A....G. .`..A..
-  0x0000b078 1c000000 74010000 5072ffff 5e000000 ....t...Pr..^...
-  0x0000b088 00410e10 8302470e 2002540e 10410e08 .A....G. .T..A..
-  0x0000b098 14000000 94010000 9072ffff 83000000 .........r......
-  0x0000b0a8 0002540e 206e0e08 14000000 ac010000 ..T. n..........
-  0x0000b0b8 0873ffff 78000000 00024c0e 206b0e08 .s..x.....L. k..
-  0x0000b0c8 1c000000 c4010000 7073ffff 75000000 ........ps..u...
-  0x0000b0d8 00640e20 730a0e08 410b0000 00000000 .d. s...A.......
-  0x0000b0e8 14000000 e4010000 d073ffff 33000000 .........s..3...
-  0x0000b0f8 00000000 00000000 14000000 fc010000 ................
-  0x0000b108 f873ffff 41000000 00000000 00000000 .s..A...........
-  0x0000b118 1c000000 14020000 3074ffff 69000000 ........0t..i...
-  0x0000b128 00410e10 8302470e 20025f0e 10410e08 .A....G. ._..A..
-  0x0000b138 14000000 34020000 8074ffff 33000000 ....4....t..3...
-  0x0000b148 00000000 00000000 14000000 4c020000 ............L...
-  0x0000b158 a874ffff 33000000 00000000 00000000 .t..3...........
-  0x0000b168 14000000 64020000 d074ffff 3a000000 ....d....t..:...
-  0x0000b178 00000000 00000000 1c000000 7c020000 ............|...
-  0x0000b188 f874ffff c5000000 00410e10 8302470e .t.......A....G.
-  0x0000b198 2002bb0e 10410e08 1c000000 9c020000  ....A..........
-  0x0000b1a8 a875ffff c8000000 00410e10 8302470e .u.......A....G.
-  0x0000b1b8 2002be0e 10410e08 1c000000 bc020000  ....A..........
-  0x0000b1c8 5876ffff c2000000 00410e10 8302470e Xv.......A....G.
-  0x0000b1d8 2002b80e 10410e08 14000000 dc020000  ....A..........
-  0x0000b1e8 0877ffff 41000000 00000000 00000000 .w..A...........
-  0x0000b1f8 14000000 f4020000 4077ffff 65000000 ........@w..e...
-  0x0000b208 00000000 00000000 14000000 0c030000 ................
-  0x0000b218 9877ffff 92010000 00000000 00000000 .w..............
-  0x0000b228 14000000 24030000 2079ffff a0010000 ....$... y......
-  0x0000b238 00000000 00000000 14000000 3c030000 ............<...
-  0x0000b248 a87affff a0010000 00000000 00000000 .z..............
-  0x0000b258 14000000 54030000 307cffff a0010000 ....T...0|......
-  0x0000b268 00000000 00000000 14000000 6c030000 ............l...
-  0x0000b278 b87dffff a0010000 00000000 00000000 .}..............
-  0x0000b288 14000000 84030000 407fffff 6b000000 ........@...k...
-  0x0000b298 00000000 00000000 14000000 9c030000 ................
-  0x0000b2a8 987fffff 41000000 00440e20 7c0e0800 ....A....D. |...
-  0x0000b2b8 14000000 b4030000 d07fffff 1e010000 ................
-  0x0000b2c8 00000000 00000000 14000000 cc030000 ................
-  0x0000b2d8 d880ffff 2f000000 00000000 00000000 ..../...........
-  0x0000b2e8 3c000000 e4030000 f080ffff 52000000 <...........R...
-  0x0000b2f8 00490e10 8c02460e 18860344 0e208304 .I....F....D. ..
-  0x0000b308 660a0e18 460e1042 0e08470b 410e1843 f...F..B..G.A..C
-  0x0000b318 0e10420e 0841c3c6 cc000000 00000000 ..B..A..........
-  0x0000b328 14000000 24040000 1081ffff 21000000 ....$.......!...
-  0x0000b338 00000000 00000000 14000000 3c040000 ............<...
-  0x0000b348 2881ffff fe010000 00000000 00000000 (...............
-  0x0000b358 4c000000 54040000 1083ffff 96020000 L...T...........
-  0x0000b368 00420e10 8f02530e 188e0353 0e208d04 .B....S....S. ..
-  0x0000b378 520e288c 05520e30 8606500e 38830766 R.(..R.0..P.8..f
-  0x0000b388 0ea00203 dd010a0e 38410e30 410e2842 ........8A.0A.(B
-  0x0000b398 0e20420e 18420e10 420e0847 0b000000 . B..B..B..G....
-  0x0000b3a8 2c000000 a4040000 6085ffff c9000000 ,.......`.......
-  0x0000b3b8 00470e90 0102900e 98014b0e a0015e0e .G........K...^.
-  0x0000b3c8 9801410e 9001470e 08000000 00000000 ..A...G.........
-  0x0000b3d8 14000000 d4040000 0086ffff 05000000 ................
-  0x0000b3e8 00000000 00000000 4c000000 ec040000 ........L.......
-  0x0000b3f8 f885ffff 5d050000 00420e10 8f02490e ....]....B....I.
-  0x0000b408 188e0351 0e208d04 4d0e288c 054f0e30 ...Q. ..M.(..O.0
-  0x0000b418 8606500e 38830772 0e800203 c5020a0e ..P.8..r........
-  0x0000b428 38440e30 410e2842 0e20420e 18420e10 8D.0A.(B. B..B..
-  0x0000b438 420e084c 0b000000 2c000000 3c050000 B..L....,...<...
-  0x0000b448 088bffff c9000000 00470e90 0102900e .........G......
-  0x0000b458 98014b0e a0015e0e 9801410e 9001470e ..K...^...A...G.
-  0x0000b468 08000000 00000000 14000000 6c050000 ............l...
-  0x0000b478 a88bffff 05000000 00000000 00000000 ................
-  0x0000b488 4c000000 84050000 a08bffff a6040000 L...............
-  0x0000b498 00420e10 8f02490e 188e0351 0e208d04 .B....I....Q. ..
-  0x0000b4a8 4f0e288c 054d0e30 8606500e 38830756 O.(..M.0..P.8..V
-  0x0000b4b8 0ee00103 a2020a0e 38440e30 410e2842 ........8D.0A.(B
-  0x0000b4c8 0e20420e 18420e10 420e084b 0b000000 . B..B..B..K....
-  0x0000b4d8 2c000000 d4050000 0090ffff c9000000 ,...............
-  0x0000b4e8 00470e90 0102900e 98014b0e a0015e0e .G........K...^.
-  0x0000b4f8 9801410e 9001470e 08000000 00000000 ..A...G.........
-  0x0000b508 14000000 04060000 a090ffff 05000000 ................
-  0x0000b518 00000000 00000000 4c000000 1c060000 ........L.......
-  0x0000b528 9890ffff 19040000 00420e10 8f02490e .........B....I.
-  0x0000b538 188e034d 0e208d04 450e288c 05410e30 ...M. ..E.(..A.0
-  0x0000b548 8606440e 38830747 0ea00103 53020a0e ..D.8..G....S...
-  0x0000b558 38440e30 410e2842 0e20420e 18420e10 8D.0A.(B. B..B..
-  0x0000b568 420e0847 0b000000 44000000 6c060000 B..G....D...l...
-  0x0000b578 d869ffff ba000000 00410e10 86024e0e .i.......A....N.
-  0x0000b588 184b0e20 4f0e284c 0e30500e 10480e18 .K. O.(L.0P..H..
-  0x0000b598 560e2045 0e28420e 30490e10 480e1856 V. E.(B.0I..H..V
-  0x0000b5a8 0e20450e 28420e30 500e104d 0e080000 . E.(B.0P..M....
-  0x0000b5b8 14000000 b4060000 2094ffff 0e000000 ........ .......
-  0x0000b5c8 00000000 00000000 00000000          ............
+  0x0000af98 14000000 00000000 017a5200 01781001 .........zR..x..
+  0x0000afa8 1b0c0708 90010000 24000000 1c000000 ........$.......
+  0x0000afb8 b86bffff 30040000 000e1046 0e184a0f .k..0......F..J.
+  0x0000afc8 0b770880 003f1a3b 2a332422 00000000 .w...?.;*3$"....
+  0x0000afd8 14000000 44000000 4071ffff 05000000 ....D...@q......
+  0x0000afe8 00000000 00000000 14000000 5c000000 ............\...
+  0x0000aff8 3871ffff 0c000000 00000000 00000000 8q..............
+  0x0000b008 14000000 74000000 3071ffff 17000000 ....t...0q......
+  0x0000b018 00000000 00000000 14000000 8c000000 ................
+  0x0000b028 3871ffff 16000000 00000000 00000000 8q..............
+  0x0000b038 14000000 a4000000 4071ffff 17000000 ........@q......
+  0x0000b048 00000000 00000000 14000000 bc000000 ................
+  0x0000b058 4871ffff 17000000 00000000 00000000 Hq..............
+  0x0000b068 14000000 d4000000 5071ffff 17000000 ........Pq......
+  0x0000b078 00000000 00000000 14000000 ec000000 ................
+  0x0000b088 5871ffff 17000000 00000000 00000000 Xq..............
+  0x0000b098 14000000 04010000 6071ffff 17000000 ........`q......
+  0x0000b0a8 00000000 00000000 14000000 1c010000 ................
+  0x0000b0b8 6871ffff 16000000 00000000 00000000 hq..............
+  0x0000b0c8 1c000000 34010000 7071ffff 61000000 ....4...pq..a...
+  0x0000b0d8 00410e10 8302470e 2002570e 10410e08 .A....G. .W..A..
+  0x0000b0e8 1c000000 54010000 c071ffff 6a000000 ....T....q..j...
+  0x0000b0f8 00410e10 8302470e 2002600e 10410e08 .A....G. .`..A..
+  0x0000b108 1c000000 74010000 1072ffff 5e000000 ....t....r..^...
+  0x0000b118 00410e10 8302470e 2002540e 10410e08 .A....G. .T..A..
+  0x0000b128 14000000 94010000 5072ffff 83000000 ........Pr......
+  0x0000b138 0002540e 206e0e08 14000000 ac010000 ..T. n..........
+  0x0000b148 c872ffff 78000000 00024c0e 206b0e08 .r..x.....L. k..
+  0x0000b158 1c000000 c4010000 3073ffff 75000000 ........0s..u...
+  0x0000b168 00640e20 730a0e08 410b0000 00000000 .d. s...A.......
+  0x0000b178 14000000 e4010000 9073ffff 33000000 .........s..3...
+  0x0000b188 00000000 00000000 14000000 fc010000 ................
+  0x0000b198 b873ffff 41000000 00000000 00000000 .s..A...........
+  0x0000b1a8 1c000000 14020000 f073ffff 69000000 .........s..i...
+  0x0000b1b8 00410e10 8302470e 20025f0e 10410e08 .A....G. ._..A..
+  0x0000b1c8 14000000 34020000 4074ffff 33000000 ....4...@t..3...
+  0x0000b1d8 00000000 00000000 14000000 4c020000 ............L...
+  0x0000b1e8 6874ffff 33000000 00000000 00000000 ht..3...........
+  0x0000b1f8 14000000 64020000 9074ffff 3a000000 ....d....t..:...
+  0x0000b208 00000000 00000000 1c000000 7c020000 ............|...
+  0x0000b218 b874ffff c5000000 00410e10 8302470e .t.......A....G.
+  0x0000b228 2002bb0e 10410e08 1c000000 9c020000  ....A..........
+  0x0000b238 6875ffff c8000000 00410e10 8302470e hu.......A....G.
+  0x0000b248 2002be0e 10410e08 1c000000 bc020000  ....A..........
+  0x0000b258 1876ffff c2000000 00410e10 8302470e .v.......A....G.
+  0x0000b268 2002b80e 10410e08 14000000 dc020000  ....A..........
+  0x0000b278 c876ffff 41000000 00000000 00000000 .v..A...........
+  0x0000b288 14000000 f4020000 0077ffff 65000000 .........w..e...
+  0x0000b298 00000000 00000000 14000000 0c030000 ................
+  0x0000b2a8 5877ffff 92010000 00000000 00000000 Xw..............
+  0x0000b2b8 14000000 24030000 e078ffff a0010000 ....$....x......
+  0x0000b2c8 00000000 00000000 14000000 3c030000 ............<...
+  0x0000b2d8 687affff a0010000 00000000 00000000 hz..............
+  0x0000b2e8 14000000 54030000 f07bffff a0010000 ....T....{......
+  0x0000b2f8 00000000 00000000 14000000 6c030000 ............l...
+  0x0000b308 787dffff a0010000 00000000 00000000 x}..............
+  0x0000b318 14000000 84030000 007fffff 6b000000 ............k...
+  0x0000b328 00000000 00000000 14000000 9c030000 ................
+  0x0000b338 587fffff 41000000 00440e20 7c0e0800 X...A....D. |...
+  0x0000b348 14000000 b4030000 907fffff 1e010000 ................
+  0x0000b358 00000000 00000000 14000000 cc030000 ................
+  0x0000b368 9880ffff 2f000000 00000000 00000000 ..../...........
+  0x0000b378 3c000000 e4030000 b080ffff 52000000 <...........R...
+  0x0000b388 00490e10 8c02460e 18860344 0e208304 .I....F....D. ..
+  0x0000b398 660a0e18 460e1042 0e08470b 410e1843 f...F..B..G.A..C
+  0x0000b3a8 0e10420e 0841c3c6 cc000000 00000000 ..B..A..........
+  0x0000b3b8 14000000 24040000 d080ffff 21000000 ....$.......!...
+  0x0000b3c8 00000000 00000000 14000000 3c040000 ............<...
+  0x0000b3d8 e880ffff fe010000 00000000 00000000 ................
+  0x0000b3e8 4c000000 54040000 d082ffff 96020000 L...T...........
+  0x0000b3f8 00420e10 8f02530e 188e0353 0e208d04 .B....S....S. ..
+  0x0000b408 520e288c 05520e30 8606500e 38830766 R.(..R.0..P.8..f
+  0x0000b418 0ea00203 dd010a0e 38410e30 410e2842 ........8A.0A.(B
+  0x0000b428 0e20420e 18420e10 420e0847 0b000000 . B..B..B..G....
+  0x0000b438 2c000000 a4040000 2085ffff c9000000 ,....... .......
+  0x0000b448 00470e90 0102900e 98014b0e a0015e0e .G........K...^.
+  0x0000b458 9801410e 9001470e 08000000 00000000 ..A...G.........
+  0x0000b468 14000000 d4040000 c085ffff 05000000 ................
+  0x0000b478 00000000 00000000 4c000000 ec040000 ........L.......
+  0x0000b488 b885ffff 5d050000 00420e10 8f02490e ....]....B....I.
+  0x0000b498 188e0351 0e208d04 4d0e288c 054f0e30 ...Q. ..M.(..O.0
+  0x0000b4a8 8606500e 38830772 0e800203 c5020a0e ..P.8..r........
+  0x0000b4b8 38440e30 410e2842 0e20420e 18420e10 8D.0A.(B. B..B..
+  0x0000b4c8 420e084c 0b000000 2c000000 3c050000 B..L....,...<...
+  0x0000b4d8 c88affff c9000000 00470e90 0102900e .........G......
+  0x0000b4e8 98014b0e a0015e0e 9801410e 9001470e ..K...^...A...G.
+  0x0000b4f8 08000000 00000000 14000000 6c050000 ............l...
+  0x0000b508 688bffff 05000000 00000000 00000000 h...............
+  0x0000b518 4c000000 84050000 608bffff cb040000 L.......`.......
+  0x0000b528 00420e10 8f02490e 188e0351 0e208d04 .B....I....Q. ..
+  0x0000b538 4f0e288c 05500e30 86064d0e 38830756 O.(..P.0..M.8..V
+  0x0000b548 0ee00103 ba020a0e 38440e30 410e2842 ........8D.0A.(B
+  0x0000b558 0e20420e 18420e10 420e084b 0b000000 . B..B..B..K....
+  0x0000b568 2c000000 d4050000 e08fffff c9000000 ,...............
+  0x0000b578 00470e90 0102900e 98014b0e a0015e0e .G........K...^.
+  0x0000b588 9801410e 9001470e 08000000 00000000 ..A...G.........
+  0x0000b598 14000000 04060000 8090ffff 05000000 ................
+  0x0000b5a8 00000000 00000000 4c000000 1c060000 ........L.......
+  0x0000b5b8 7890ffff 19040000 00420e10 8f02490e x........B....I.
+  0x0000b5c8 188e034d 0e208d04 450e288c 05410e30 ...M. ..E.(..A.0
+  0x0000b5d8 8606440e 38830747 0ea00103 53020a0e ..D.8..G....S...
+  0x0000b5e8 38440e30 410e2842 0e20420e 18420e10 8D.0A.(B. B..B..
+  0x0000b5f8 420e0847 0b000000 44000000 6c060000 B..G....D...l...
+  0x0000b608 9869ffff ba000000 00410e10 86024e0e .i.......A....N.
+  0x0000b618 184b0e20 4f0e284c 0e30500e 10480e18 .K. O.(L.0P..H..
+  0x0000b628 560e2045 0e28420e 30490e10 480e1856 V. E.(B.0I..H..V
+  0x0000b638 0e20450e 28420e30 500e104d 0e080000 . E.(B.0P..M....
+  0x0000b648 14000000 b4060000 0094ffff 0e000000 ................
+  0x0000b658 00000000 00000000 00000000          ............
```

#### readelf --wide --decompress --hex-dump=.init_array {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.init_array':
-  0x0020bd60 c0200000 00000000 501f0000 00000000 . ......P.......
+  0x0020bd60 10210000 00000000 a01f0000 00000000 .!..............
```

#### readelf --wide --decompress --hex-dump=.fini_array {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.fini_array':
-  0x0020bd70 80200000 00000000                   . ......
+  0x0020bd70 d0200000 00000000                   . ......
```

#### readelf --wide --decompress --hex-dump=.got.plt {}

```diff
@@ -1,38 +1,39 @@
 
 Hex dump of section '.got.plt':
  NOTE: This section has relocations against it, but these have NOT been applied to this dump.
   0x0020c000 78bd2000 00000000 00000000 00000000 x. .............
-  0x0020c010 00000000 00000000 461b0000 00000000 ........F.......
-  0x0020c020 561b0000 00000000 661b0000 00000000 V.......f.......
-  0x0020c030 761b0000 00000000 861b0000 00000000 v...............
-  0x0020c040 961b0000 00000000 a61b0000 00000000 ................
-  0x0020c050 b61b0000 00000000 c61b0000 00000000 ................
-  0x0020c060 d61b0000 00000000 e61b0000 00000000 ................
-  0x0020c070 f61b0000 00000000 061c0000 00000000 ................
-  0x0020c080 161c0000 00000000 261c0000 00000000 ........&.......
-  0x0020c090 361c0000 00000000 461c0000 00000000 6.......F.......
-  0x0020c0a0 561c0000 00000000 661c0000 00000000 V.......f.......
-  0x0020c0b0 761c0000 00000000 861c0000 00000000 v...............
-  0x0020c0c0 961c0000 00000000 a61c0000 00000000 ................
-  0x0020c0d0 b61c0000 00000000 c61c0000 00000000 ................
-  0x0020c0e0 d61c0000 00000000 e61c0000 00000000 ................
-  0x0020c0f0 f61c0000 00000000 061d0000 00000000 ................
-  0x0020c100 161d0000 00000000 261d0000 00000000 ........&.......
-  0x0020c110 361d0000 00000000 461d0000 00000000 6.......F.......
-  0x0020c120 561d0000 00000000 661d0000 00000000 V.......f.......
-  0x0020c130 761d0000 00000000 861d0000 00000000 v...............
-  0x0020c140 961d0000 00000000 a61d0000 00000000 ................
-  0x0020c150 b61d0000 00000000 c61d0000 00000000 ................
-  0x0020c160 d61d0000 00000000 e61d0000 00000000 ................
-  0x0020c170 f61d0000 00000000 061e0000 00000000 ................
-  0x0020c180 161e0000 00000000 261e0000 00000000 ........&.......
-  0x0020c190 361e0000 00000000 461e0000 00000000 6.......F.......
-  0x0020c1a0 561e0000 00000000 661e0000 00000000 V.......f.......
-  0x0020c1b0 761e0000 00000000 861e0000 00000000 v...............
-  0x0020c1c0 961e0000 00000000 a61e0000 00000000 ................
-  0x0020c1d0 b61e0000 00000000 c61e0000 00000000 ................
-  0x0020c1e0 d61e0000 00000000 e61e0000 00000000 ................
-  0x0020c1f0 f61e0000 00000000 061f0000 00000000 ................
-  0x0020c200 161f0000 00000000 261f0000 00000000 ........&.......
-  0x0020c210 361f0000 00000000 461f0000 00000000 6.......F.......
+  0x0020c010 00000000 00000000 861b0000 00000000 ................
+  0x0020c020 961b0000 00000000 a61b0000 00000000 ................
+  0x0020c030 b61b0000 00000000 c61b0000 00000000 ................
+  0x0020c040 d61b0000 00000000 e61b0000 00000000 ................
+  0x0020c050 f61b0000 00000000 061c0000 00000000 ................
+  0x0020c060 161c0000 00000000 261c0000 00000000 ........&.......
+  0x0020c070 361c0000 00000000 461c0000 00000000 6.......F.......
+  0x0020c080 561c0000 00000000 661c0000 00000000 V.......f.......
+  0x0020c090 761c0000 00000000 861c0000 00000000 v...............
+  0x0020c0a0 961c0000 00000000 a61c0000 00000000 ................
+  0x0020c0b0 b61c0000 00000000 c61c0000 00000000 ................
+  0x0020c0c0 d61c0000 00000000 e61c0000 00000000 ................
+  0x0020c0d0 f61c0000 00000000 061d0000 00000000 ................
+  0x0020c0e0 161d0000 00000000 261d0000 00000000 ........&.......
+  0x0020c0f0 361d0000 00000000 461d0000 00000000 6.......F.......
+  0x0020c100 561d0000 00000000 661d0000 00000000 V.......f.......
+  0x0020c110 761d0000 00000000 861d0000 00000000 v...............
+  0x0020c120 961d0000 00000000 a61d0000 00000000 ................
+  0x0020c130 b61d0000 00000000 c61d0000 00000000 ................
+  0x0020c140 d61d0000 00000000 e61d0000 00000000 ................
+  0x0020c150 f61d0000 00000000 061e0000 00000000 ................
+  0x0020c160 161e0000 00000000 261e0000 00000000 ........&.......
+  0x0020c170 361e0000 00000000 461e0000 00000000 6.......F.......
+  0x0020c180 561e0000 00000000 661e0000 00000000 V.......f.......
+  0x0020c190 761e0000 00000000 861e0000 00000000 v...............
+  0x0020c1a0 961e0000 00000000 a61e0000 00000000 ................
+  0x0020c1b0 b61e0000 00000000 c61e0000 00000000 ................
+  0x0020c1c0 d61e0000 00000000 e61e0000 00000000 ................
+  0x0020c1d0 f61e0000 00000000 061f0000 00000000 ................
+  0x0020c1e0 161f0000 00000000 261f0000 00000000 ........&.......
+  0x0020c1f0 361f0000 00000000 461f0000 00000000 6.......F.......
+  0x0020c200 561f0000 00000000 661f0000 00000000 V.......f.......
+  0x0020c210 761f0000 00000000 861f0000 00000000 v...............
+  0x0020c220 961f0000 00000000                   ........
```

#### readelf --wide --decompress --hex-dump=.data {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.data':
-  0x0020c220 20c22000 00000000                    . .....
+  0x0020c228 28c22000 00000000                   (. .....
```

#### readelf --wide --decompress --hex-dump=.nvFatBinSegment {}

```diff
@@ -1,5 +1,5 @@
 
 Hex dump of section '.nvFatBinSegment':
-  0x0020c228 b1436246 01000000 b8500000 00000000 .CbF.....P......
-  0x0020c238 00000000 00000000                   ........
+  0x0020c230 b1436246 01000000 48510000 00000000 .CbF....HQ......
+  0x0020c240 00000000 00000000                   ........
```

#### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,10 +1,10 @@
 
 Hex dump of section '.strtab':
-  0x00000000 00746d70 7866745f 30303030 34616363 .tmpxft_00004acc
+  0x00000000 00746d70 7866745f 30303030 35373135 .tmpxft_00005715
   0x00000010 5f303030 30303030 302d365f 7467715f _00000000-6_tgq_
   0x00000020 73696d75 6c61746f 722e6375 64616665 simulator.cudafe
   0x00000030 312e6370 70006661 7462696e 44617461 1.cpp.fatbinData
   0x00000040 005f5a4c 32365f5f 63756461 556e7265 ._ZL26__cudaUnre
   0x00000050 67697374 65724269 6e617279 5574696c gisterBinaryUtil
   0x00000060 76005f5a 4c32305f 5f637564 61466174 v._ZL20__cudaFat
   0x00000070 43756269 6e48616e 646c6500 5f5a4c32 CubinHandle._ZL2
@@ -28,132 +28,134 @@
   0x00000190 66696e69 005f696e 6974005f 44594e41 fini._init._DYNA
   0x000001a0 4d494300 5f5f544d 435f454e 445f5f00 MIC.__TMC_END__.
   0x000001b0 5f474c4f 42414c5f 4f464653 45545f54 _GLOBAL_OFFSET_T
   0x000001c0 41424c45 5f005f5a 31316370 68617365 ABLE_._Z11cphase
   0x000001d0 5f676174 65503666 6c6f6174 32660065 _gateP6float2f.e
   0x000001e0 78656375 74655f63 69726375 6974005f xecute_circuit._
   0x000001f0 5a376164 5f676174 65503666 6c6f6174 Z7ad_gateP6float
-  0x00000200 32660063 7564614d 616c6c6f 6340406c 2f.cudaMalloc@@l
-  0x00000210 69626375 64617274 2e736f2e 3132005f ibcudart.so.12._
-  0x00000220 5a346861 7368504b 63005f5a 3770645f Z4hashPKc._Z7pd_
-  0x00000230 67617465 5036666c 6f617432 66005f5a gateP6float2f._Z
-  0x00000240 35305f5f 64657669 63655f73 7475625f 50__device_stub_
-  0x00000250 5f5a3138 61637469 6f6e4f6e 54726970 _Z18actionOnTrip
-  0x00000260 6c654761 74655036 666c6f61 74325330 leGateP6float2S0
-  0x00000270 5f6d506d 5036666c 6f617432 53305f6d _mPmP6float2S0_m
-  0x00000280 506d005f 5a36795f 67617465 5036666c Pm._Z6y_gateP6fl
-  0x00000290 6f617432 00637564 614c6175 6e63684b oat2.cudaLaunchK
-  0x000002a0 65726e65 6c40406c 69626375 64617274 ernel@@libcudart
-  0x000002b0 2e736f2e 3132005f 5a323274 6f66665f .so.12._Z22toff_
-  0x000002c0 67617465 5f746172 6765745f 736d616c gate_target_smal
-  0x000002d0 6c503666 6c6f6174 32005f5a 37636f6d lP6float2._Z7com
-  0x000002e0 70617265 504b7653 305f005f 65646174 parePKvS0_._edat
-  0x000002f0 61005f5a 32336672 65645f67 6174655f a._Z23fred_gate_
-  0x00000300 636f6e74 726f6c5f 736d616c 6c503666 control_smallP6f
-  0x00000310 6c6f6174 32005f5f 63756461 556e7265 loat2.__cudaUnre
-  0x00000320 67697374 65724661 7442696e 61727940 gisterFatBinary@
-  0x00000330 406c6962 63756461 72742e73 6f2e3132 @libcudart.so.12
-  0x00000340 005f5a32 31667265 645f6761 74655f63 ._Z21fred_gate_c
-  0x00000350 6f6e7472 6f6c5f6d 69645036 666c6f61 ontrol_midP6floa
-  0x00000360 7432005f 5a323363 6e6f745f 67617465 t2._Z23cnot_gate
-  0x00000370 5f636f6e 74726f6c 5f736d61 6c6c5036 _control_smallP6
-  0x00000380 666c6f61 7432005f 5a377279 5f676174 float2._Z7ry_gat
-  0x00000390 65503666 6c6f6174 32660073 696e636f eP6float2f.sinco
-  0x000003a0 73664040 474c4942 435f322e 322e3500 sf@@GLIBC_2.2.5.
-  0x000003b0 5f5f6378 615f6669 6e616c69 7a654040 __cxa_finalize@@
-  0x000003c0 474c4942 435f322e 322e3500 5f5a3231 GLIBC_2.2.5._Z21
-  0x000003d0 66726564 5f676174 655f636f 6e74726f fred_gate_contro
-  0x000003e0 6c5f6269 67503666 6c6f6174 32005f5a l_bigP6float2._Z
-  0x000003f0 38737963 5f676174 65503666 6c6f6174 8syc_gateP6float
-  0x00000400 32005f5a 38727878 5f676174 65503666 2._Z8rxx_gateP6f
-  0x00000410 6c6f6174 3266005f 5a323074 6f66665f loat2f._Z20toff_
-  0x00000420 67617465 5f746172 6765745f 6d696450 gate_target_midP
-  0x00000430 36666c6f 61743200 5f5a3872 7a7a5f67 6float2._Z8rzz_g
-  0x00000440 61746550 36666c6f 61743266 00646f75 ateP6float2f.dou
-  0x00000450 626c6547 61746541 6374696f 6e005f5a bleGateAction._Z
-  0x00000460 39697349 6e417272 61795050 4b635063 9isInArrayPPKcPc
-  0x00000470 69005f5a 3231636e 6f745f67 6174655f i._Z21cnot_gate_
-  0x00000480 636f6e74 726f6c5f 62696750 36666c6f control_bigP6flo
-  0x00000490 61743200 5f5a3678 5f676174 65503666 at2._Z6x_gateP6f
-  0x000004a0 6c6f6174 32005f5a 32306765 6e657261 loat2._Z20genera
-  0x000004b0 74655f62 696e6172 795f6461 74616600 te_binary_dataf.
-  0x000004c0 5f5a3673 5f676174 65503666 6c6f6174 _Z6s_gateP6float
-  0x000004d0 32005f5a 31316461 6d705f69 5f676174 2._Z11damp_i_gat
-  0x000004e0 65503666 6c6f6174 3266005f 5a313069 eP6float2f._Z10i
-  0x000004f0 73776170 5f676174 65503666 6c6f6174 swap_gateP6float
-  0x00000500 32005f5f 6378615f 61746578 69744040 2.__cxa_atexit@@
-  0x00000510 474c4942 435f322e 322e3500 5f5f6375 GLIBC_2.2.5.__cu
-  0x00000520 64615265 67697374 65724661 7442696e daRegisterFatBin
-  0x00000530 61727940 406c6962 63756461 72742e73 ary@@libcudart.s
-  0x00000540 6f2e3132 0074696d 65404047 4c494243 o.12.time@@GLIBC
-  0x00000550 5f322e32 2e350073 72616e64 4040474c _2.2.5.srand@@GL
-  0x00000560 4942435f 322e322e 35005f5a 36745f67 IBC_2.2.5._Z6t_g
-  0x00000570 61746550 36666c6f 61743200 5f5a3133 ateP6float2._Z13
-  0x00000580 6e6f726d 616c697a 6174696f 6e503666 normalizationP6f
-  0x00000590 6c6f6174 3269005f 5a367a5f 67617465 loat2i._Z6z_gate
-  0x000005a0 5036666c 6f617432 005f5a31 39616374 P6float2._Z19act
-  0x000005b0 696f6e4f 6e446f75 626c6551 75626974 ionOnDoubleQubit
-  0x000005c0 5036666c 6f617432 53305f6d 506d005f P6float2S0_mPm._
-  0x000005d0 5a35315f 5f646576 6963655f 73747562 Z51__device_stub
-  0x000005e0 5f5f5a31 39616374 696f6e4f 6e446f75 __Z19actionOnDou
-  0x000005f0 626c6551 75626974 5036666c 6f617432 bleQubitP6float2
-  0x00000600 53305f6d 506d5036 666c6f61 74325330 S0_mPmP6float2S0
-  0x00000610 5f6d506d 005f5a37 67657470 726f6250 _mPm._Z7getprobP
-  0x00000620 36666c6f 61743250 666d0066 72656540 6float2Pfm.free@
-  0x00000630 40474c49 42435f32 2e322e35 00637564 @GLIBC_2.2.5.cud
-  0x00000640 614d656d 63707940 406c6962 63756461 aMemcpy@@libcuda
-  0x00000650 72742e73 6f2e3132 005f5a38 7464675f rt.so.12._Z8tdg_
-  0x00000660 67617465 5036666c 6f617432 005f5a37 gateP6float2._Z7
-  0x00000670 637a5f67 61746550 36666c6f 61743200 cz_gateP6float2.
-  0x00000680 5f5a3138 61637469 6f6e4f6e 54726970 _Z18actionOnTrip
-  0x00000690 6c654761 74655036 666c6f61 74325330 leGateP6float2S0
-  0x000006a0 5f6d506d 006d616c 6c6f6340 40474c49 _mPm.malloc@@GLI
-  0x000006b0 42435f32 2e322e35 005f656e 64005f5a BC_2.2.5._end._Z
-  0x000006c0 35315f5f 64657669 63655f73 7475625f 51__device_stub_
-  0x000006d0 5f5a3139 61637469 6f6e4f6e 53696e67 _Z19actionOnSing
-  0x000006e0 6c655175 62697450 36666c6f 61743253 leQubitP6float2S
-  0x000006f0 305f6d50 6d503666 6c6f6174 3253305f 0_mPmP6float2S0_
-  0x00000700 6d506d00 5f5a3134 67657441 72726179 mPm._Z14getArray
-  0x00000710 4c656e67 74685069 005f5a38 7364675f LengthPi._Z8sdg_
-  0x00000720 67617465 5036666c 6f617432 00737472 gateP6float2.str
-  0x00000730 636d7040 40474c49 42435f32 2e322e35 cmp@@GLIBC_2.2.5
-  0x00000740 005f5f63 75646152 65676973 74657246 .__cudaRegisterF
-  0x00000750 756e6374 696f6e40 406c6962 63756461 unction@@libcuda
-  0x00000760 72742e73 6f2e3132 00637564 61467265 rt.so.12.cudaFre
-  0x00000770 6540406c 69626375 64617274 2e736f2e e@@libcudart.so.
-  0x00000780 3132005f 5a323074 6f66665f 67617465 12._Z20toff_gate
-  0x00000790 5f746172 6765745f 62696750 36666c6f _target_bigP6flo
-  0x000007a0 61743200 5f5a3872 79795f67 61746550 at2._Z8ryy_gateP
-  0x000007b0 36666c6f 61743266 005f5f62 73735f73 6float2f.__bss_s
-  0x000007c0 74617274 00707574 73404047 4c494243 tart.puts@@GLIBC
-  0x000007d0 5f322e32 2e350073 696e676c 65476174 _2.2.5.singleGat
-  0x000007e0 65416374 696f6e00 5f5a3139 61637469 eAction._Z19acti
-  0x000007f0 6f6e4f6e 53696e67 6c655175 62697450 onOnSingleQubitP
-  0x00000800 36666c6f 61743253 305f6d50 6d005f5a 6float2S0_mPm._Z
-  0x00000810 31316964 656e7469 74794d61 74503666 11identityMatP6f
-  0x00000820 6c6f6174 3269005f 5f637564 61506f70 loat2i.__cudaPop
-  0x00000830 43616c6c 436f6e66 69677572 6174696f CallConfiguratio
-  0x00000840 6e40406c 69626375 64617274 2e736f2e n@@libcudart.so.
-  0x00000850 31320063 75646144 65766963 6553796e 12.cudaDeviceSyn
-  0x00000860 6368726f 6e697a65 40406c69 62637564 chronize@@libcud
-  0x00000870 6172742e 736f2e31 32005f49 544d5f64 art.so.12._ITM_d
-  0x00000880 65726567 69737465 72544d43 6c6f6e65 eregisterTMClone
-  0x00000890 5461626c 65005f5a 37727a5f 67617465 Table._Z7rz_gate
-  0x000008a0 5036666c 6f617432 66005f5f 63756461 P6float2f.__cuda
-  0x000008b0 50757368 43616c6c 436f6e66 69677572 PushCallConfigur
-  0x000008c0 6174696f 6e40406c 69626375 64617274 ation@@libcudart
-  0x000008d0 2e736f2e 3132005f 5a36685f 67617465 .so.12._Z6h_gate
-  0x000008e0 5036666c 6f617432 00737172 74664040 P6float2.sqrtf@@
-  0x000008f0 474c4942 435f322e 322e3500 5f5f6375 GLIBC_2.2.5.__cu
-  0x00000900 64615265 67697374 65724661 7442696e daRegisterFatBin
-  0x00000910 61727945 6e644040 6c696263 75646172 aryEnd@@libcudar
-  0x00000920 742e736f 2e313200 74726970 6c654761 t.so.12.tripleGa
-  0x00000930 74654163 74696f6e 005f5a39 73776170 teAction._Z9swap
-  0x00000940 5f676174 65503666 6c6f6174 32005f5f _gateP6float2.__
-  0x00000950 676d6f6e 5f737461 72745f5f 005f5a37 gmon_start__._Z7
-  0x00000960 72785f67 61746550 36666c6f 61743266 rx_gateP6float2f
-  0x00000970 0071736f 72744040 474c4942 435f322e .qsort@@GLIBC_2.
-  0x00000980 322e3500 5f49544d 5f726567 69737465 2.5._ITM_registe
-  0x00000990 72544d43 6c6f6e65 5461626c 65006375 rTMCloneTable.cu
-  0x000009a0 64615365 74446576 69636540 406c6962 daSetDevice@@lib
-  0x000009b0 63756461 72742e73 6f2e3132 00       cudart.so.12.
+  0x00000200 32660070 72696e74 66404047 4c494243 2f.printf@@GLIBC
+  0x00000210 5f322e32 2e350063 7564614d 616c6c6f _2.2.5.cudaMallo
+  0x00000220 6340406c 69626375 64617274 2e736f2e c@@libcudart.so.
+  0x00000230 3132005f 5a346861 7368504b 63005f5a 12._Z4hashPKc._Z
+  0x00000240 3770645f 67617465 5036666c 6f617432 7pd_gateP6float2
+  0x00000250 66005f5a 35305f5f 64657669 63655f73 f._Z50__device_s
+  0x00000260 7475625f 5f5a3138 61637469 6f6e4f6e tub__Z18actionOn
+  0x00000270 54726970 6c654761 74655036 666c6f61 TripleGateP6floa
+  0x00000280 74325330 5f6d506d 5036666c 6f617432 t2S0_mPmP6float2
+  0x00000290 53305f6d 506d005f 5a36795f 67617465 S0_mPm._Z6y_gate
+  0x000002a0 5036666c 6f617432 00637564 614c6175 P6float2.cudaLau
+  0x000002b0 6e63684b 65726e65 6c40406c 69626375 nchKernel@@libcu
+  0x000002c0 64617274 2e736f2e 3132005f 5a323274 dart.so.12._Z22t
+  0x000002d0 6f66665f 67617465 5f746172 6765745f off_gate_target_
+  0x000002e0 736d616c 6c503666 6c6f6174 32005f5a smallP6float2._Z
+  0x000002f0 37636f6d 70617265 504b7653 305f005f 7comparePKvS0_._
+  0x00000300 65646174 61005f5a 32336672 65645f67 edata._Z23fred_g
+  0x00000310 6174655f 636f6e74 726f6c5f 736d616c ate_control_smal
+  0x00000320 6c503666 6c6f6174 32005f5f 63756461 lP6float2.__cuda
+  0x00000330 556e7265 67697374 65724661 7442696e UnregisterFatBin
+  0x00000340 61727940 406c6962 63756461 72742e73 ary@@libcudart.s
+  0x00000350 6f2e3132 005f5a32 31667265 645f6761 o.12._Z21fred_ga
+  0x00000360 74655f63 6f6e7472 6f6c5f6d 69645036 te_control_midP6
+  0x00000370 666c6f61 7432005f 5a323363 6e6f745f float2._Z23cnot_
+  0x00000380 67617465 5f636f6e 74726f6c 5f736d61 gate_control_sma
+  0x00000390 6c6c5036 666c6f61 7432005f 5a377279 llP6float2._Z7ry
+  0x000003a0 5f676174 65503666 6c6f6174 32660073 _gateP6float2f.s
+  0x000003b0 696e636f 73664040 474c4942 435f322e incosf@@GLIBC_2.
+  0x000003c0 322e3500 5f5f6378 615f6669 6e616c69 2.5.__cxa_finali
+  0x000003d0 7a654040 474c4942 435f322e 322e3500 ze@@GLIBC_2.2.5.
+  0x000003e0 5f5a3231 66726564 5f676174 655f636f _Z21fred_gate_co
+  0x000003f0 6e74726f 6c5f6269 67503666 6c6f6174 ntrol_bigP6float
+  0x00000400 32005f5a 38737963 5f676174 65503666 2._Z8syc_gateP6f
+  0x00000410 6c6f6174 32005f5a 38727878 5f676174 loat2._Z8rxx_gat
+  0x00000420 65503666 6c6f6174 3266005f 5a323074 eP6float2f._Z20t
+  0x00000430 6f66665f 67617465 5f746172 6765745f off_gate_target_
+  0x00000440 6d696450 36666c6f 61743200 5f5a3872 midP6float2._Z8r
+  0x00000450 7a7a5f67 61746550 36666c6f 61743266 zz_gateP6float2f
+  0x00000460 00646f75 626c6547 61746541 6374696f .doubleGateActio
+  0x00000470 6e005f5a 39697349 6e417272 61795050 n._Z9isInArrayPP
+  0x00000480 4b635063 69005f5a 3231636e 6f745f67 KcPci._Z21cnot_g
+  0x00000490 6174655f 636f6e74 726f6c5f 62696750 ate_control_bigP
+  0x000004a0 36666c6f 61743200 5f5a3678 5f676174 6float2._Z6x_gat
+  0x000004b0 65503666 6c6f6174 32005f5a 32306765 eP6float2._Z20ge
+  0x000004c0 6e657261 74655f62 696e6172 795f6461 nerate_binary_da
+  0x000004d0 74616600 5f5a3673 5f676174 65503666 taf._Z6s_gateP6f
+  0x000004e0 6c6f6174 32005f5a 31316461 6d705f69 loat2._Z11damp_i
+  0x000004f0 5f676174 65503666 6c6f6174 3266005f _gateP6float2f._
+  0x00000500 5a313069 73776170 5f676174 65503666 Z10iswap_gateP6f
+  0x00000510 6c6f6174 32005f5f 6378615f 61746578 loat2.__cxa_atex
+  0x00000520 69744040 474c4942 435f322e 322e3500 it@@GLIBC_2.2.5.
+  0x00000530 5f5f6375 64615265 67697374 65724661 __cudaRegisterFa
+  0x00000540 7442696e 61727940 406c6962 63756461 tBinary@@libcuda
+  0x00000550 72742e73 6f2e3132 0074696d 65404047 rt.so.12.time@@G
+  0x00000560 4c494243 5f322e32 2e350073 72616e64 LIBC_2.2.5.srand
+  0x00000570 4040474c 4942435f 322e322e 35005f5a @@GLIBC_2.2.5._Z
+  0x00000580 36745f67 61746550 36666c6f 61743200 6t_gateP6float2.
+  0x00000590 5f5a3133 6e6f726d 616c697a 6174696f _Z13normalizatio
+  0x000005a0 6e503666 6c6f6174 3269005f 5a367a5f nP6float2i._Z6z_
+  0x000005b0 67617465 5036666c 6f617432 005f5a31 gateP6float2._Z1
+  0x000005c0 39616374 696f6e4f 6e446f75 626c6551 9actionOnDoubleQ
+  0x000005d0 75626974 5036666c 6f617432 53305f6d ubitP6float2S0_m
+  0x000005e0 506d005f 5a35315f 5f646576 6963655f Pm._Z51__device_
+  0x000005f0 73747562 5f5f5a31 39616374 696f6e4f stub__Z19actionO
+  0x00000600 6e446f75 626c6551 75626974 5036666c nDoubleQubitP6fl
+  0x00000610 6f617432 53305f6d 506d5036 666c6f61 oat2S0_mPmP6floa
+  0x00000620 74325330 5f6d506d 005f5a37 67657470 t2S0_mPm._Z7getp
+  0x00000630 726f6250 36666c6f 61743250 666d0066 robP6float2Pfm.f
+  0x00000640 72656540 40474c49 42435f32 2e322e35 ree@@GLIBC_2.2.5
+  0x00000650 00637564 614d656d 63707940 406c6962 .cudaMemcpy@@lib
+  0x00000660 63756461 72742e73 6f2e3132 005f5a38 cudart.so.12._Z8
+  0x00000670 7464675f 67617465 5036666c 6f617432 tdg_gateP6float2
+  0x00000680 005f5a37 637a5f67 61746550 36666c6f ._Z7cz_gateP6flo
+  0x00000690 61743200 5f5a3138 61637469 6f6e4f6e at2._Z18actionOn
+  0x000006a0 54726970 6c654761 74655036 666c6f61 TripleGateP6floa
+  0x000006b0 74325330 5f6d506d 006d616c 6c6f6340 t2S0_mPm.malloc@
+  0x000006c0 40474c49 42435f32 2e322e35 005f656e @GLIBC_2.2.5._en
+  0x000006d0 64005f5a 35315f5f 64657669 63655f73 d._Z51__device_s
+  0x000006e0 7475625f 5f5a3139 61637469 6f6e4f6e tub__Z19actionOn
+  0x000006f0 53696e67 6c655175 62697450 36666c6f SingleQubitP6flo
+  0x00000700 61743253 305f6d50 6d503666 6c6f6174 at2S0_mPmP6float
+  0x00000710 3253305f 6d506d00 5f5a3134 67657441 2S0_mPm._Z14getA
+  0x00000720 72726179 4c656e67 74685069 005f5a38 rrayLengthPi._Z8
+  0x00000730 7364675f 67617465 5036666c 6f617432 sdg_gateP6float2
+  0x00000740 00737472 636d7040 40474c49 42435f32 .strcmp@@GLIBC_2
+  0x00000750 2e322e35 005f5f63 75646152 65676973 .2.5.__cudaRegis
+  0x00000760 74657246 756e6374 696f6e40 406c6962 terFunction@@lib
+  0x00000770 63756461 72742e73 6f2e3132 00637564 cudart.so.12.cud
+  0x00000780 61467265 6540406c 69626375 64617274 aFree@@libcudart
+  0x00000790 2e736f2e 3132005f 5a323074 6f66665f .so.12._Z20toff_
+  0x000007a0 67617465 5f746172 6765745f 62696750 gate_target_bigP
+  0x000007b0 36666c6f 61743200 5f5a3872 79795f67 6float2._Z8ryy_g
+  0x000007c0 61746550 36666c6f 61743266 005f5f62 ateP6float2f.__b
+  0x000007d0 73735f73 74617274 00707574 73404047 ss_start.puts@@G
+  0x000007e0 4c494243 5f322e32 2e350073 696e676c LIBC_2.2.5.singl
+  0x000007f0 65476174 65416374 696f6e00 5f5a3139 eGateAction._Z19
+  0x00000800 61637469 6f6e4f6e 53696e67 6c655175 actionOnSingleQu
+  0x00000810 62697450 36666c6f 61743253 305f6d50 bitP6float2S0_mP
+  0x00000820 6d005f5a 31316964 656e7469 74794d61 m._Z11identityMa
+  0x00000830 74503666 6c6f6174 3269005f 5f637564 tP6float2i.__cud
+  0x00000840 61506f70 43616c6c 436f6e66 69677572 aPopCallConfigur
+  0x00000850 6174696f 6e40406c 69626375 64617274 ation@@libcudart
+  0x00000860 2e736f2e 31320063 75646144 65766963 .so.12.cudaDevic
+  0x00000870 6553796e 6368726f 6e697a65 40406c69 eSynchronize@@li
+  0x00000880 62637564 6172742e 736f2e31 32005f49 bcudart.so.12._I
+  0x00000890 544d5f64 65726567 69737465 72544d43 TM_deregisterTMC
+  0x000008a0 6c6f6e65 5461626c 65005f5a 37727a5f loneTable._Z7rz_
+  0x000008b0 67617465 5036666c 6f617432 66005f5f gateP6float2f.__
+  0x000008c0 63756461 50757368 43616c6c 436f6e66 cudaPushCallConf
+  0x000008d0 69677572 6174696f 6e40406c 69626375 iguration@@libcu
+  0x000008e0 64617274 2e736f2e 3132005f 5a36685f dart.so.12._Z6h_
+  0x000008f0 67617465 5036666c 6f617432 00737172 gateP6float2.sqr
+  0x00000900 74664040 474c4942 435f322e 322e3500 tf@@GLIBC_2.2.5.
+  0x00000910 5f5f6375 64615265 67697374 65724661 __cudaRegisterFa
+  0x00000920 7442696e 61727945 6e644040 6c696263 tBinaryEnd@@libc
+  0x00000930 75646172 742e736f 2e313200 74726970 udart.so.12.trip
+  0x00000940 6c654761 74654163 74696f6e 005f5a39 leGateAction._Z9
+  0x00000950 73776170 5f676174 65503666 6c6f6174 swap_gateP6float
+  0x00000960 32005f5f 676d6f6e 5f737461 72745f5f 2.__gmon_start__
+  0x00000970 005f5a37 72785f67 61746550 36666c6f ._Z7rx_gateP6flo
+  0x00000980 61743266 0071736f 72744040 474c4942 at2f.qsort@@GLIB
+  0x00000990 435f322e 322e3500 5f49544d 5f726567 C_2.2.5._ITM_reg
+  0x000009a0 69737465 72544d43 6c6f6e65 5461626c isterTMCloneTabl
+  0x000009b0 65006375 64615365 74446576 69636540 e.cudaSetDevice@
+  0x000009c0 406c6962 63756461 72742e73 6f2e3132 @libcudart.so.12
+  0x000009d0 00                                  .
```

### Comparing `tgqSim-0.1.6/tgqSim.egg-info/PKG-INFO` & `tgqSim-0.1.7/tgqSim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgqSim
-Version: 0.1.6
+Version: 0.1.7
 Summary: TGQ量子模拟器
 Home-page: UNKNOWN
 Author: tiangongqs
 License: MIT
 Keywords: tgq,quantum,simulator
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

