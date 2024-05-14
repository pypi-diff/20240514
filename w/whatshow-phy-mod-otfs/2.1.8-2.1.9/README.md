# Comparing `tmp/whatshow_phy_mod_otfs-2.1.8.tar.gz` & `tmp/whatshow_phy_mod_otfs-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatshow_phy_mod_otfs-2.1.8.tar", last modified: Tue May 14 01:03:50 2024, max compression
+gzip compressed data, was "whatshow_phy_mod_otfs-2.1.9.tar", last modified: Tue May 14 03:05:00 2024, max compression
```

## Comparing `whatshow_phy_mod_otfs-2.1.8.tar` & `whatshow_phy_mod_otfs-2.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 01:03:50.449023 whatshow_phy_mod_otfs-2.1.8/
--rw-rw-rw-   0        0        0    13032 2024-05-14 01:03:50.447028 whatshow_phy_mod_otfs-2.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    12916 2024-05-14 01:03:47.000000 whatshow_phy_mod_otfs-2.1.8/README.md
--rw-rw-rw-   0        0        0       42 2024-05-14 01:03:50.449023 whatshow_phy_mod_otfs-2.1.8/setup.cfg
--rw-rw-rw-   0        0        0      365 2024-05-14 01:03:47.000000 whatshow_phy_mod_otfs-2.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 01:03:50.430566 whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs/
--rw-rw-rw-   0        0        0    26568 2024-05-14 01:03:47.000000 whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs/OTFS.py
--rw-rw-rw-   0        0        0    16003 2024-05-14 01:03:47.000000 whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs/OTFSDetector.py
--rw-rw-rw-   0        0        0    28494 2024-05-14 01:03:47.000000 whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs/OTFSResGrid.py
--rw-rw-rw-   0        0        0      100 2024-05-14 01:03:47.000000 whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 01:03:50.445011 whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs.egg-info/
--rw-rw-rw-   0        0        0    13032 2024-05-14 01:03:50.000000 whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-05-14 01:03:50.000000 whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 01:03:50.000000 whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-05-14 01:03:50.000000 whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 03:05:00.270898 whatshow_phy_mod_otfs-2.1.9/
+-rw-rw-rw-   0        0        0    13032 2024-05-14 03:05:00.254977 whatshow_phy_mod_otfs-2.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    12916 2024-05-14 03:04:53.000000 whatshow_phy_mod_otfs-2.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-14 03:05:00.270898 whatshow_phy_mod_otfs-2.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      365 2024-05-14 03:04:53.000000 whatshow_phy_mod_otfs-2.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:05:00.131270 whatshow_phy_mod_otfs-2.1.9/whatshow_phy_mod_otfs/
+-rw-rw-rw-   0        0        0    26599 2024-05-14 03:04:53.000000 whatshow_phy_mod_otfs-2.1.9/whatshow_phy_mod_otfs/OTFS.py
+-rw-rw-rw-   0        0        0    16003 2024-05-14 03:04:53.000000 whatshow_phy_mod_otfs-2.1.9/whatshow_phy_mod_otfs/OTFSDetector.py
+-rw-rw-rw-   0        0        0    28494 2024-05-14 03:04:53.000000 whatshow_phy_mod_otfs-2.1.9/whatshow_phy_mod_otfs/OTFSResGrid.py
+-rw-rw-rw-   0        0        0      100 2024-05-14 03:04:53.000000 whatshow_phy_mod_otfs-2.1.9/whatshow_phy_mod_otfs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:05:00.253970 whatshow_phy_mod_otfs-2.1.9/whatshow_phy_mod_otfs.egg-info/
+-rw-rw-rw-   0        0        0    13032 2024-05-14 03:04:59.000000 whatshow_phy_mod_otfs-2.1.9/whatshow_phy_mod_otfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-05-14 03:04:59.000000 whatshow_phy_mod_otfs-2.1.9/whatshow_phy_mod_otfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 03:04:59.000000 whatshow_phy_mod_otfs-2.1.9/whatshow_phy_mod_otfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-14 03:04:59.000000 whatshow_phy_mod_otfs-2.1.9/whatshow_phy_mod_otfs.egg-info/top_level.txt
```

### Comparing `whatshow_phy_mod_otfs-2.1.8/PKG-INFO` & `whatshow_phy_mod_otfs-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: whatshow_phy_mod_otfs
-Version: 2.1.8
+Version: 2.1.9
 Description-Content-Type: text/markdown
 
 # OTFS Modulation
-[![PyPi](https://img.shields.io/badge/PyPi-2.1.8-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.8-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
+[![PyPi](https://img.shields.io/badge/PyPi-2.1.9-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.9-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
 
 This repository is a fundamental toolbox of OTFS modulation crossing `matlab` and `python`. This repositiory is based on papers below:
 > Raviteja, P., Phan, K. T., Hong, Y., & Viterbo, E. (2018). Interference cancellation and iterative detection for orthogonal time frequency space modulation. *IEEE transactions on wireless communications, 17(10)*, 6501-6515.
 
 > Raviteja, P., Phan, K. T., & Hong, Y. (2019). Embedded pilot-aided channel estimation for OTFS in delayâ€“Doppler channels. *IEEE transactions on vehicular technology, 68(5)*, 4906-4917.
 
 ## How to use
```

### Comparing `whatshow_phy_mod_otfs-2.1.8/README.md` & `whatshow_phy_mod_otfs-2.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # OTFS Modulation
-[![PyPi](https://img.shields.io/badge/PyPi-2.1.8-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.8-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
+[![PyPi](https://img.shields.io/badge/PyPi-2.1.9-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.9-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
 
 This repository is a fundamental toolbox of OTFS modulation crossing `matlab` and `python`. This repositiory is based on papers below:
 > Raviteja, P., Phan, K. T., Hong, Y., & Viterbo, E. (2018). Interference cancellation and iterative detection for orthogonal time frequency space modulation. *IEEE transactions on wireless communications, 17(10)*, 6501-6515.
 
 > Raviteja, P., Phan, K. T., & Hong, Y. (2019). Embedded pilot-aided channel estimation for OTFS in delay–Doppler channels. *IEEE transactions on vehicular technology, 68(5)*, 4906-4917.
 
 ## How to use
```

### Comparing `whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs/OTFS.py` & `whatshow_phy_mod_otfs-2.1.9/whatshow_phy_mod_otfs/OTFS.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,30 +301,31 @@
     '''
     Get the channel matrix in Delay Doppler Domain
     @his:   the channel gains
     @lis:   the channel delays
     @kis:   the channel Dopplers
     @data_only: whether the channel is only for data (by default true). If you want to get the entire H_DD when using pilos and/or guards, you should manullay set it to false.
     '''
-    def getChannel(self, *, his=None, lis=None, kis=None, data_only=True):
+    def getChannel(self, *args, data_only=True):
         # input check & init
-        if his is not None:
-            his = np.asarray(his);
-            lis = np.asarray(lis);
-            kis = np.asarray(kis);
-            if not self.isvector(his) and not self.isvector(lis) and not self.isvector(kis):
-                raise Exception("The input CSI must be vectors.");
-            p = his.shape[-1];
-            if p != lis.shape[-1] and p != kis.shape[-1]:
-                raise Exception("The input CSI (gains, delays and dopplers) must have the same length.");
-        else:
-            p = self.taps_num;
-            his = self.chan_coef;
-            lis = self.delay_taps;
-            kis = self.doppler_taps;
+        p = self.taps_num;
+        his = self.chan_coef;
+        lis = self.delay_taps;
+        kis = self.doppler_taps;
+        if len(args) > 0:
+            if len(args) >= 3:
+                his = np.asarray(args[0]);
+                lis = np.asarray(args[1]);
+                kis = np.asarray(args[2]); 
+                if not self.isvector(his) and not self.isvector(lis) and not self.isvector(kis):
+                    raise Exception("The input CSI must be vectors.");
+                p = his.shape[-1];
+                if p != lis.shape[-1] and p != kis.shape[-1]:
+                    raise Exception("The input CSI (gains, delays and dopplers) must have the same length.");
+           
         # build the channel
         if self.pulse_type == self.PULSE_IDEAL:
             H_DD = self.buildIdealChannel(p, his, lis, kis);
         elif self.pulse_type == self.PULSE_RECTA:
             H_DD = self.buildRectaChannel(p, his, lis, kis);
         # remove the channel for PG & CE
         if data_only and self.rg is not None:
```

### Comparing `whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs/OTFSDetector.py` & `whatshow_phy_mod_otfs-2.1.9/whatshow_phy_mod_otfs/OTFSDetector.py`

 * *Files identical despite different names*

### Comparing `whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs/OTFSResGrid.py` & `whatshow_phy_mod_otfs-2.1.9/whatshow_phy_mod_otfs/OTFSResGrid.py`

 * *Files identical despite different names*

### Comparing `whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs.egg-info/PKG-INFO` & `whatshow_phy_mod_otfs-2.1.9/whatshow_phy_mod_otfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: whatshow-phy-mod-otfs
-Version: 2.1.8
+Version: 2.1.9
 Description-Content-Type: text/markdown
 
 # OTFS Modulation
-[![PyPi](https://img.shields.io/badge/PyPi-2.1.8-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.8-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
+[![PyPi](https://img.shields.io/badge/PyPi-2.1.9-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.9-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
 
 This repository is a fundamental toolbox of OTFS modulation crossing `matlab` and `python`. This repositiory is based on papers below:
 > Raviteja, P., Phan, K. T., Hong, Y., & Viterbo, E. (2018). Interference cancellation and iterative detection for orthogonal time frequency space modulation. *IEEE transactions on wireless communications, 17(10)*, 6501-6515.
 
 > Raviteja, P., Phan, K. T., & Hong, Y. (2019). Embedded pilot-aided channel estimation for OTFS in delayâ€“Doppler channels. *IEEE transactions on vehicular technology, 68(5)*, 4906-4917.
 
 ## How to use
```

