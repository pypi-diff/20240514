# Comparing `tmp/c4m_pdk_ihpsg13g2-0.0.2.post1.tar.gz` & `tmp/c4m_pdk_ihpsg13g2-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4m_pdk_ihpsg13g2-0.0.2.post1.tar", last modified: Fri May  3 15:17:34 2024, max compression
+gzip compressed data, was "c4m_pdk_ihpsg13g2-0.0.3.tar", last modified: Tue May 14 11:16:44 2024, max compression
```

## Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1.tar` & `c4m_pdk_ihpsg13g2-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      992 2024-04-29 12:22:37.734462 c4m_pdk_ihpsg13g2-0.0.2.post1/LICENSE.md
--rw-r--r--   0        0        0     5389 2024-05-03 14:55:33.303077 c4m_pdk_ihpsg13g2-0.0.2.post1/README.md
--rw-r--r--   0        0        0      449 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/__init__.py
--rw-r--r--   0        0        0     4572 2024-04-29 11:09:33.917013 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/_io_compliance.py
--rw-r--r--   0        0        0     6918 2024-04-29 11:12:09.911800 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/io.py
--rw-r--r--   0        0        0      517 2024-04-29 11:12:20.003724 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/klayout.py
--rw-r--r--   0        0        0       23 2024-05-03 15:17:33.895843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/__init__.py
--rw-r--r--   0        0        0      775 2024-05-03 15:17:33.915843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/all.spice
--rw-r--r--   0        0        0    24555 2024-05-03 15:17:33.907843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/cornerMOShv.lib
--rw-r--r--   0        0        0    22926 2024-05-03 15:17:33.903843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/cornerMOSlv.lib
--rw-r--r--   0        0        0     2460 2024-05-03 15:17:33.911843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/cornerRES.lib
--rw-r--r--   0        0        0     3580 2024-05-03 15:17:33.915843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/diodes.lib
--rw-r--r--   0        0        0     1900 2024-05-03 15:17:33.907843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/resistors_mod.lib
--rw-r--r--   0        0        0     1039 2024-05-03 15:17:33.911843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/resistors_parm.lib
--rw-r--r--   0        0        0     1045 2024-05-03 15:17:33.911843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/resistors_stat.lib
--rw-r--r--   0        0        0     6144 2024-05-03 15:17:33.903843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_mod.lib
--rw-r--r--   0        0        0    40662 2024-05-03 15:17:33.903843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_parm.lib
--rw-r--r--   0        0        0     4027 2024-05-03 15:17:33.907843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_stat.lib
--rw-r--r--   0        0        0     6110 2024-05-03 15:17:33.895843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_mod.lib
--rw-r--r--   0        0        0    40995 2024-05-03 15:17:33.899843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_parm.lib
--rw-r--r--   0        0        0     3667 2024-05-03 15:17:33.899843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_stat.lib
--rw-r--r--   0        0        0    18379 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/pdkmaster.py
--rw-r--r--   0        0        0     2617 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/pyspice.py
--rw-r--r--   0        0        0     4300 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/stdcell.py
--rw-r--r--   0        0        0     1563 2024-05-03 15:17:34.827837 c4m_pdk_ihpsg13g2-0.0.2.post1/pyproject.toml
--rw-r--r--   0        0        0       12 2024-05-03 15:17:34.823837 c4m_pdk_ihpsg13g2-0.0.2.post1/version.txt
--rw-r--r--   0        0        0     5852 1970-01-01 00:00:00.000000 c4m_pdk_ihpsg13g2-0.0.2.post1/PKG-INFO
+-rw-r--r--   0        0        0      992 2024-04-29 12:22:37.734462 c4m_pdk_ihpsg13g2-0.0.3/LICENSE.md
+-rw-r--r--   0        0        0     5552 2024-05-13 16:42:35.930939 c4m_pdk_ihpsg13g2-0.0.3/README.md
+-rw-r--r--   0        0        0      449 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/__init__.py
+-rw-r--r--   0        0        0     4572 2024-04-29 11:09:33.917013 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/_io_compliance.py
+-rw-r--r--   0        0        0     6918 2024-04-29 11:12:09.911800 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/io.py
+-rw-r--r--   0        0        0      517 2024-04-29 11:12:20.003724 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/klayout.py
+-rw-r--r--   0        0        0       23 2024-05-07 14:17:03.642346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/__init__.py
+-rw-r--r--   0        0        0      775 2024-05-07 14:17:03.662346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/all.spice
+-rw-r--r--   0        0        0    24555 2024-05-07 14:17:03.654346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/cornerMOShv.lib
+-rw-r--r--   0        0        0    22926 2024-05-07 14:17:03.646346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/cornerMOSlv.lib
+-rw-r--r--   0        0        0     2460 2024-05-07 14:17:03.658346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/cornerRES.lib
+-rw-r--r--   0        0        0     3580 2024-05-07 14:17:03.658346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/diodes.lib
+-rw-r--r--   0        0        0     1935 2024-05-07 14:17:03.654346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/resistors_mod.lib
+-rw-r--r--   0        0        0     1039 2024-05-07 14:17:03.654346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/resistors_parm.lib
+-rw-r--r--   0        0        0     1045 2024-05-07 14:17:03.658346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/resistors_stat.lib
+-rw-r--r--   0        0        0     6144 2024-05-07 14:17:03.650346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_mod.lib
+-rw-r--r--   0        0        0    40662 2024-05-07 14:17:03.650346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_parm.lib
+-rw-r--r--   0        0        0     4027 2024-05-07 14:17:03.650346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_stat.lib
+-rw-r--r--   0        0        0     6110 2024-05-07 14:17:03.642346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_mod.lib
+-rw-r--r--   0        0        0    40995 2024-05-07 14:17:03.642346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_parm.lib
+-rw-r--r--   0        0        0     3667 2024-05-07 14:17:03.646346 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_stat.lib
+-rw-r--r--   0        0        0    18379 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/pdkmaster.py
+-rw-r--r--   0        0        0     2617 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/pyspice.py
+-rw-r--r--   0        0        0     4300 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/stdcell.py
+-rw-r--r--   0        0        0     1551 2024-05-14 11:16:44.088064 c4m_pdk_ihpsg13g2-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        6 2024-05-14 11:16:44.084064 c4m_pdk_ihpsg13g2-0.0.3/version.txt
+-rw-r--r--   0        0        0     6003 1970-01-01 00:00:00.000000 c4m_pdk_ihpsg13g2-0.0.3/PKG-INFO
```

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/LICENSE.md` & `c4m_pdk_ihpsg13g2-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/README.md` & `c4m_pdk_ihpsg13g2-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 This is the Chips4Makers' PDK for the SG13G2 open source PDK.
 
 # Versions
 
-* [v0.0.2](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.1): build infrastructure and dependencies update; no major code changes but KLayout PCell lib support added.
+* [v0.0.3](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.3):
+  * Critical fix IOPadVdd
+  * Improved generation of all the files for upstreaming
+* [v0.0.2](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.2): build infrastructure and dependencies update; no major code changes but KLayout PCell lib support added.
 * [v0.0.1](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.1): First public release; main achievement is that code can generate a version of the IO library ready for upstreaming to [IHP-Open-PDK](https://github.com/IHP-GmbH/IHP-Open-PDK/).  
   It can also generate standard cells but these have not been used yet in P&R.
 
 ## Alpha Version of Code
 
 This is an alpha version of the IHP SG13G2 PDK, if it breaks you need to keep the pieces. E.g. hiccups are still expected when using this code base. For further discussion you can use the [Chips4Makers matrix channel](https://matrix.to/#/#Chips4Makers_community:gitter.im). Certainly interested to be made aware about usage of this project.
```

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/_io_compliance.py` & `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/_io_compliance.py`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/io.py` & `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/io.py`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/klayout.py` & `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/klayout.py`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/all.spice` & `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/all.spice`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/cornerMOShv.lib` & `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/cornerMOShv.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/cornerMOSlv.lib` & `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/cornerMOSlv.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/cornerRES.lib` & `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/cornerRES.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/diodes.lib` & `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/diodes.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/resistors_mod.lib` & `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/resistors_mod.lib`

 * *Files 13% similar despite different names*

```diff
@@ -33,41 +33,41 @@
 * value is taken from extraction routine
 .subckt Rparasitic 1 2 
 .param R=0 w=0 l=0 TC1=0.00353 TC2=0
 R1 1 2 R=r*res_rpara TC1=TC1 TC2=TC2 
 .ends Rparasitic
 
 .subckt rsil 1 3
-.param w=0.5e-6 l=0.5e-6 b=0
+.param w=0.5e-6 l=0.5e-6 b=0 m=1
 +kappa=1.85
 +ps=0.18e-6
 +leff=(b+1)*l+(2/kappa*weff+ps)*b
 +res_rzspec=2*rzspec/w
 +weff=w+0.01e-6
 +rzspec=4.5e-6
-R1 1 2 res_rsil L=leff W=weff
-R2 2 3 R=res_rzspec TC1=3100e-6 TC2=0.3e-6
+R1 1 2 res_rsil L=leff W=weff m=m
+R2 2 3 R=res_rzspec TC1=3100e-6 TC2=0.3e-6 m=m
 .ends rsil
 
 .subckt rhigh 1 3 
-.param w=0.5e-6 l=0.96e-6 b=0 
+.param w=0.5e-6 l=0.96e-6 b=0 m=1
 +kappa=1.85
 +ps=0.18e-6
 +leff=(b+1)*l+(2/kappa*weff+ps)*b
 +res_rzspec=2*rzspec/w
 +weff=w-0.04e-6
 +rzspec=80e-6
-R1 1 2 res_rhigh L=leff W=weff
-R2 2 3 R=res_rzspec TC1=-2300e-6 TC2=2.1e-6
+R1 1 2 res_rhigh L=leff W=weff m=m
+R2 2 3 R=res_rzspec TC1=-2300e-6 TC2=2.1e-6 m=m
 .ends rhigh
 
 .subckt rppd 1 3 
-.param w=0.5e-6 l=0.5e-6 b=0
+.param w=0.5e-6 l=0.5e-6 b=0 m=1
 +kappa=1.85
 +ps=0.18e-6
 +leff=(b+1)*l+(2/kappa*weff+ps)*b
 +res_rzspec=2*rzspec/w
 +weff=w+0.006e-6
 +rzspec=35e-6
-R1 1 2 res_rppd L=leff W=weff
-R2 2 3 R=res_rzspec TC1=-950e-6
+R1 1 2 res_rppd L=leff W=weff m=m
+R2 2 3 R=res_rzspec TC1=-950e-6 m=m
 .ends rppd
```

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/resistors_parm.lib` & `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/resistors_parm.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/resistors_stat.lib` & `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/resistors_stat.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_mod.lib` & `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_mod.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_parm.lib` & `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_parm.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_stat.lib` & `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_stat.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_mod.lib` & `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_mod.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_parm.lib` & `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_parm.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_stat.lib` & `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_stat.lib`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/pdkmaster.py` & `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/pdkmaster.py`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/pyspice.py` & `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/pyspice.py`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/stdcell.py` & `c4m_pdk_ihpsg13g2-0.0.3/c4m/pdk/ihpsg13g2/stdcell.py`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/pyproject.toml` & `c4m_pdk_ihpsg13g2-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 authors = [
     { name = "Chips4Makers contributors" },
 ]
 dependencies = [
     "PDKMaster~=0.11.0.post2",
     "pdkmaster-io-klayout~=0.1.1.post1",
     "c4m-flexcell~=0.4.2.post3",
-    "c4m-flexio~=0.4.2.post2",
+    "c4m-flexio~=0.4.3",
 ]
 requires-python = "~=3.8"
 readme = "README.md"
-version = "0.0.2.post1"
+version = "0.0.3"
 
 [project.license]
 text = "GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `c4m_pdk_ihpsg13g2-0.0.2.post1/PKG-INFO` & `c4m_pdk_ihpsg13g2-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: c4m-pdk-ihpsg13g2
-Version: 0.0.2.post1
+Version: 0.0.3
 Summary: PDKMaster based PDK for open source IHP SG13G2 process
 Author: Chips4Makers contributors
 License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
 Requires-Python: ~=3.8
 Requires-Dist: PDKMaster~=0.11.0.post2
 Requires-Dist: pdkmaster-io-klayout~=0.1.1.post1
 Requires-Dist: c4m-flexcell~=0.4.2.post3
-Requires-Dist: c4m-flexio~=0.4.2.post2
+Requires-Dist: c4m-flexio~=0.4.3
 Description-Content-Type: text/markdown
 
 This is the Chips4Makers' PDK for the SG13G2 open source PDK.
 
 # Versions
 
-* [v0.0.2](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.1): build infrastructure and dependencies update; no major code changes but KLayout PCell lib support added.
+* [v0.0.3](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.3):
+  * Critical fix IOPadVdd
+  * Improved generation of all the files for upstreaming
+* [v0.0.2](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.2): build infrastructure and dependencies update; no major code changes but KLayout PCell lib support added.
 * [v0.0.1](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.1): First public release; main achievement is that code can generate a version of the IO library ready for upstreaming to [IHP-Open-PDK](https://github.com/IHP-GmbH/IHP-Open-PDK/).  
   It can also generate standard cells but these have not been used yet in P&R.
 
 ## Alpha Version of Code
 
 This is an alpha version of the IHP SG13G2 PDK, if it breaks you need to keep the pieces. E.g. hiccups are still expected when using this code base. For further discussion you can use the [Chips4Makers matrix channel](https://matrix.to/#/#Chips4Makers_community:gitter.im). Certainly interested to be made aware about usage of this project.
```

