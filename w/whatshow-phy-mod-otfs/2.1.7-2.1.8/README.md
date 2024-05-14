# Comparing `tmp/whatshow_phy_mod_otfs-2.1.7.tar.gz` & `tmp/whatshow_phy_mod_otfs-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatshow_phy_mod_otfs-2.1.7.tar", last modified: Sun May 12 11:06:45 2024, max compression
+gzip compressed data, was "whatshow_phy_mod_otfs-2.1.8.tar", last modified: Tue May 14 01:03:50 2024, max compression
```

## Comparing `whatshow_phy_mod_otfs-2.1.7.tar` & `whatshow_phy_mod_otfs-2.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 11:06:45.361482 whatshow_phy_mod_otfs-2.1.7/
--rw-rw-rw-   0        0        0    13032 2024-05-12 11:06:45.359807 whatshow_phy_mod_otfs-2.1.7/PKG-INFO
--rw-rw-rw-   0        0        0    12916 2024-05-12 11:06:42.000000 whatshow_phy_mod_otfs-2.1.7/README.md
--rw-rw-rw-   0        0        0       42 2024-05-12 11:06:45.361482 whatshow_phy_mod_otfs-2.1.7/setup.cfg
--rw-rw-rw-   0        0        0      365 2024-05-12 11:06:42.000000 whatshow_phy_mod_otfs-2.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:06:45.345136 whatshow_phy_mod_otfs-2.1.7/whatshow_phy_mod_otfs/
--rw-rw-rw-   0        0        0    26642 2024-05-12 11:06:42.000000 whatshow_phy_mod_otfs-2.1.7/whatshow_phy_mod_otfs/OTFS.py
--rw-rw-rw-   0        0        0    16003 2024-05-12 11:06:42.000000 whatshow_phy_mod_otfs-2.1.7/whatshow_phy_mod_otfs/OTFSDetector.py
--rw-rw-rw-   0        0        0    28494 2024-05-12 11:06:42.000000 whatshow_phy_mod_otfs-2.1.7/whatshow_phy_mod_otfs/OTFSResGrid.py
--rw-rw-rw-   0        0        0      100 2024-05-12 11:06:42.000000 whatshow_phy_mod_otfs-2.1.7/whatshow_phy_mod_otfs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:06:45.356785 whatshow_phy_mod_otfs-2.1.7/whatshow_phy_mod_otfs.egg-info/
--rw-rw-rw-   0        0        0    13032 2024-05-12 11:06:45.000000 whatshow_phy_mod_otfs-2.1.7/whatshow_phy_mod_otfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-05-12 11:06:45.000000 whatshow_phy_mod_otfs-2.1.7/whatshow_phy_mod_otfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 11:06:45.000000 whatshow_phy_mod_otfs-2.1.7/whatshow_phy_mod_otfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-05-12 11:06:45.000000 whatshow_phy_mod_otfs-2.1.7/whatshow_phy_mod_otfs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 01:03:50.449023 whatshow_phy_mod_otfs-2.1.8/
+-rw-rw-rw-   0        0        0    13032 2024-05-14 01:03:50.447028 whatshow_phy_mod_otfs-2.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0    12916 2024-05-14 01:03:47.000000 whatshow_phy_mod_otfs-2.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-14 01:03:50.449023 whatshow_phy_mod_otfs-2.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      365 2024-05-14 01:03:47.000000 whatshow_phy_mod_otfs-2.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 01:03:50.430566 whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs/
+-rw-rw-rw-   0        0        0    26568 2024-05-14 01:03:47.000000 whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs/OTFS.py
+-rw-rw-rw-   0        0        0    16003 2024-05-14 01:03:47.000000 whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs/OTFSDetector.py
+-rw-rw-rw-   0        0        0    28494 2024-05-14 01:03:47.000000 whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs/OTFSResGrid.py
+-rw-rw-rw-   0        0        0      100 2024-05-14 01:03:47.000000 whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 01:03:50.445011 whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs.egg-info/
+-rw-rw-rw-   0        0        0    13032 2024-05-14 01:03:50.000000 whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-05-14 01:03:50.000000 whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 01:03:50.000000 whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-14 01:03:50.000000 whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs.egg-info/top_level.txt
```

### Comparing `whatshow_phy_mod_otfs-2.1.7/PKG-INFO` & `whatshow_phy_mod_otfs-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: whatshow_phy_mod_otfs
-Version: 2.1.7
+Version: 2.1.8
 Description-Content-Type: text/markdown
 
 # OTFS Modulation
-[![PyPi](https://img.shields.io/badge/PyPi-2.1.7-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.7-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
+[![PyPi](https://img.shields.io/badge/PyPi-2.1.8-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.8-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
 
 This repository is a fundamental toolbox of OTFS modulation crossing `matlab` and `python`. This repositiory is based on papers below:
 > Raviteja, P., Phan, K. T., Hong, Y., & Viterbo, E. (2018). Interference cancellation and iterative detection for orthogonal time frequency space modulation. *IEEE transactions on wireless communications, 17(10)*, 6501-6515.
 
 > Raviteja, P., Phan, K. T., & Hong, Y. (2019). Embedded pilot-aided channel estimation for OTFS in delayâ€“Doppler channels. *IEEE transactions on vehicular technology, 68(5)*, 4906-4917.
 
 ## How to use
```

### Comparing `whatshow_phy_mod_otfs-2.1.7/README.md` & `whatshow_phy_mod_otfs-2.1.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # OTFS Modulation
-[![PyPi](https://img.shields.io/badge/PyPi-2.1.7-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.7-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
+[![PyPi](https://img.shields.io/badge/PyPi-2.1.8-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.8-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
 
 This repository is a fundamental toolbox of OTFS modulation crossing `matlab` and `python`. This repositiory is based on papers below:
 > Raviteja, P., Phan, K. T., Hong, Y., & Viterbo, E. (2018). Interference cancellation and iterative detection for orthogonal time frequency space modulation. *IEEE transactions on wireless communications, 17(10)*, 6501-6515.
 
 > Raviteja, P., Phan, K. T., & Hong, Y. (2019). Embedded pilot-aided channel estimation for OTFS in delay–Doppler channels. *IEEE transactions on vehicular technology, 68(5)*, 4906-4917.
 
 ## How to use
```

### Comparing `whatshow_phy_mod_otfs-2.1.7/whatshow_phy_mod_otfs/OTFS.py` & `whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs/OTFS.py`

 * *Files 1% similar despite different names*

```diff
@@ -526,22 +526,22 @@
         H_DD = self.zeros(self.sig_len, self.sig_len);      # intialize the return channel
         dftmat = self.dftmtx(self.nTimeslotNum);            # DFT matrix
         idftmat = np.conj(dftmat);                          # IDFT matrix
         piMat = self.eye(self.sig_len);                     # permutation matrix (from the delay) -> pi
         # accumulate all paths
         for tap_id in range(p):
             if self.batch_size == self.BATCH_SIZE_NO:
-                hi = self.chan_coef[tap_id];
-                li = self.delay_taps[tap_id];
-                ki = self.doppler_taps[tap_id];
+                hi = his[tap_id];
+                li = lis[tap_id];
+                ki = kis[tap_id];
                 
             else:
-                hi = self.chan_coef[..., tap_id];
-                li = self.delay_taps[..., tap_id];
-                ki = np.expand_dims(self.doppler_taps[..., tap_id], axis=-1);
+                hi = his[..., tap_id];
+                li = lis[..., tap_id];
+                ki = np.expand_dims(kis[..., tap_id], axis=-1);
             # delay
             piMati = self.circshift(piMat, li);
             # Doppler            
             deltaMat_diag = np.exp(2j*np.pi*ki/(self.sig_len)*self.buildTimeSequence(li));
             deltaMati = self.diag(deltaMat_diag);
             # Pi, Qi & Ti
             Pi = self.kron(dftmat, self.eye(self.nSubcarNum)) @ piMati;
```

### Comparing `whatshow_phy_mod_otfs-2.1.7/whatshow_phy_mod_otfs/OTFSDetector.py` & `whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs/OTFSDetector.py`

 * *Files identical despite different names*

### Comparing `whatshow_phy_mod_otfs-2.1.7/whatshow_phy_mod_otfs/OTFSResGrid.py` & `whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs/OTFSResGrid.py`

 * *Files identical despite different names*

### Comparing `whatshow_phy_mod_otfs-2.1.7/whatshow_phy_mod_otfs.egg-info/PKG-INFO` & `whatshow_phy_mod_otfs-2.1.8/whatshow_phy_mod_otfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: whatshow-phy-mod-otfs
-Version: 2.1.7
+Version: 2.1.8
 Description-Content-Type: text/markdown
 
 # OTFS Modulation
-[![PyPi](https://img.shields.io/badge/PyPi-2.1.7-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.7-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
+[![PyPi](https://img.shields.io/badge/PyPi-2.1.8-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.8-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
 
 This repository is a fundamental toolbox of OTFS modulation crossing `matlab` and `python`. This repositiory is based on papers below:
 > Raviteja, P., Phan, K. T., Hong, Y., & Viterbo, E. (2018). Interference cancellation and iterative detection for orthogonal time frequency space modulation. *IEEE transactions on wireless communications, 17(10)*, 6501-6515.
 
 > Raviteja, P., Phan, K. T., & Hong, Y. (2019). Embedded pilot-aided channel estimation for OTFS in delayâ€“Doppler channels. *IEEE transactions on vehicular technology, 68(5)*, 4906-4917.
 
 ## How to use
```

