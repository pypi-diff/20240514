# Comparing `tmp/pylag-2.1.tar.gz` & `tmp/pylag-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylag-2.1.tar", last modified: Wed Nov 15 05:28:26 2023, max compression
+gzip compressed data, was "pylag-2.2.tar", last modified: Tue May 14 17:37:19 2024, max compression
```

## Comparing `pylag-2.1.tar` & `pylag-2.2.tar`

### file list

```diff
@@ -1,49 +1,48 @@
-drwxr-xr-x   0 drw        (502) staff       (20)        0 2023-11-15 05:28:26.471070 pylag-2.1/
--rw-r--r--   0 drw        (502) staff       (20)       55 2023-07-06 22:07:07.000000 pylag-2.1/.gitignore
--rw-r--r--   0 drw        (502) staff       (20)     1070 2023-07-06 22:07:07.000000 pylag-2.1/LICENSE.md
--rw-r--r--   0 drw        (502) staff       (20)      276 2023-11-15 05:28:26.471170 pylag-2.1/PKG-INFO
--rw-r--r--   0 drw        (502) staff       (20)     1997 2023-07-06 22:07:07.000000 pylag-2.1/README.md
--rw-r--r--   0 drw        (502) staff       (20)      461 2023-11-15 05:23:52.000000 pylag-2.1/changelog.md
-drwxr-xr-x   0 drw        (502) staff       (20)        0 2023-11-15 05:28:26.470325 pylag-2.1/pylag/
--rw-r--r--   0 drw        (502) staff       (20)      460 2023-07-06 22:07:07.000000 pylag-2.1/pylag/__init__.py
--rw-r--r--   0 drw        (502) staff       (20)     1055 2023-11-14 04:23:00.000000 pylag-2.1/pylag/absorber.py
--rw-r--r--   0 drw        (502) staff       (20)    17264 2023-07-06 22:07:07.000000 pylag-2.1/pylag/binning.py
--rw-r--r--   0 drw        (502) staff       (20)    10650 2023-07-06 22:07:07.000000 pylag-2.1/pylag/bispectrum.py
--rw-r--r--   0 drw        (502) staff       (20)     4276 2023-07-06 22:07:07.000000 pylag-2.1/pylag/cepstrum.py
--rw-r--r--   0 drw        (502) staff       (20)    20996 2023-07-06 22:07:07.000000 pylag-2.1/pylag/coherence.py
--rw-r--r--   0 drw        (502) staff       (20)     4763 2023-07-06 22:07:07.000000 pylag-2.1/pylag/continuum.py
--rw-r--r--   0 drw        (502) staff       (20)     1472 2023-07-06 22:07:07.000000 pylag-2.1/pylag/correlation.py
--rw-r--r--   0 drw        (502) staff       (20)    22230 2023-11-14 04:29:27.000000 pylag-2.1/pylag/covariance.py
--rw-r--r--   0 drw        (502) staff       (20)    16855 2023-07-06 22:07:07.000000 pylag-2.1/pylag/cross_spectrum.py
--rw-r--r--   0 drw        (502) staff       (20)     2459 2023-07-06 22:07:07.000000 pylag-2.1/pylag/dcf.py
--rw-r--r--   0 drw        (502) staff       (20)    50547 2023-07-06 22:07:07.000000 pylag-2.1/pylag/entresponse.py
--rw-r--r--   0 drw        (502) staff       (20)     4937 2023-07-06 22:07:07.000000 pylag-2.1/pylag/event_list.py
--rw-r--r--   0 drw        (502) staff       (20)     8724 2023-07-06 22:07:07.000000 pylag-2.1/pylag/fit.py
--rw-r--r--   0 drw        (502) staff       (20)     3926 2023-07-06 22:07:07.000000 pylag-2.1/pylag/fits_spec_model.py
--rw-r--r--   0 drw        (502) staff       (20)     1587 2023-07-06 22:07:07.000000 pylag-2.1/pylag/flux_histogram.py
--rw-r--r--   0 drw        (502) staff       (20)     9928 2023-11-14 04:27:30.000000 pylag-2.1/pylag/fvar.py
--rw-r--r--   0 drw        (502) staff       (20)    20498 2023-07-06 22:07:07.000000 pylag-2.1/pylag/gaussian_process.py
--rw-r--r--   0 drw        (502) staff       (20)     8964 2023-07-06 22:07:07.000000 pylag-2.1/pylag/gaussian_process_celerite.py
--rw-r--r--   0 drw        (502) staff       (20)    13416 2023-11-14 04:30:33.000000 pylag-2.1/pylag/lag_energy_spectrum.py
--rw-r--r--   0 drw        (502) staff       (20)     5826 2023-07-06 22:07:07.000000 pylag-2.1/pylag/lag_frequency_spectrum.py
--rw-r--r--   0 drw        (502) staff       (20)     8621 2023-07-06 22:07:07.000000 pylag-2.1/pylag/lens_lag.py
--rw-r--r--   0 drw        (502) staff       (20)    85968 2023-11-14 04:24:40.000000 pylag-2.1/pylag/lightcurve.py
--rw-r--r--   0 drw        (502) staff       (20)      975 2023-07-06 22:07:07.000000 pylag-2.1/pylag/math_functions.py
--rw-r--r--   0 drw        (502) staff       (20)    53322 2023-07-06 22:07:07.000000 pylag-2.1/pylag/mlcovariance.py
--rw-r--r--   0 drw        (502) staff       (20)    52472 2023-11-14 04:23:00.000000 pylag-2.1/pylag/mlfit.py
--rw-r--r--   0 drw        (502) staff       (20)     8728 2023-07-06 22:07:07.000000 pylag-2.1/pylag/model.py
--rw-r--r--   0 drw        (502) staff       (20)    15536 2023-07-06 22:07:07.000000 pylag-2.1/pylag/periodogram.py
--rw-r--r--   0 drw        (502) staff       (20)    47051 2023-07-06 22:07:07.000000 pylag-2.1/pylag/plotter.py
--rw-r--r--   0 drw        (502) staff       (20)     5377 2023-07-06 22:07:07.000000 pylag-2.1/pylag/response.py
--rw-r--r--   0 drw        (502) staff       (20)     6228 2023-11-14 04:25:44.000000 pylag-2.1/pylag/reverb_model.py
--rw-r--r--   0 drw        (502) staff       (20)    41414 2023-07-06 22:07:07.000000 pylag-2.1/pylag/simulator.py
--rw-r--r--   0 drw        (502) staff       (20)      752 2023-11-14 04:23:00.000000 pylag-2.1/pylag/time.py
--rw-r--r--   0 drw        (502) staff       (20)     2509 2023-07-06 22:07:07.000000 pylag-2.1/pylag/util.py
-drwxr-xr-x   0 drw        (502) staff       (20)        0 2023-11-15 05:28:26.470938 pylag-2.1/pylag.egg-info/
--rw-r--r--   0 drw        (502) staff       (20)      276 2023-11-15 05:28:26.000000 pylag-2.1/pylag.egg-info/PKG-INFO
--rw-r--r--   0 drw        (502) staff       (20)      892 2023-11-15 05:28:26.000000 pylag-2.1/pylag.egg-info/SOURCES.txt
--rw-r--r--   0 drw        (502) staff       (20)        1 2023-11-15 05:28:26.000000 pylag-2.1/pylag.egg-info/dependency_links.txt
--rw-r--r--   0 drw        (502) staff       (20)       20 2023-11-15 05:28:26.000000 pylag-2.1/pylag.egg-info/requires.txt
--rw-r--r--   0 drw        (502) staff       (20)        6 2023-11-15 05:28:26.000000 pylag-2.1/pylag.egg-info/top_level.txt
--rw-r--r--   0 drw        (502) staff       (20)       79 2023-11-15 05:28:26.471541 pylag-2.1/setup.cfg
--rw-r--r--   0 drw        (502) staff       (20)      391 2023-11-15 05:28:08.000000 pylag-2.1/setup.py
+drwxr-xr-x   0 drw       (1000) drw       (1000)        0 2024-05-14 17:37:19.247554 pylag-2.2/
+-rw-r--r--   0 drw       (1000) drw       (1000)     1070 2022-11-29 20:23:26.000000 pylag-2.2/LICENSE.md
+-rw-r--r--   0 drw       (1000) drw       (1000)      341 2024-05-14 17:37:19.247554 pylag-2.2/PKG-INFO
+-rw-r--r--   0 drw       (1000) drw       (1000)     1997 2022-12-06 00:45:06.000000 pylag-2.2/README.md
+drwxr-xr-x   0 drw       (1000) drw       (1000)        0 2024-05-14 17:37:19.245554 pylag-2.2/pylag/
+-rw-r--r--   0 drw       (1000) drw       (1000)      479 2024-02-12 23:49:16.000000 pylag-2.2/pylag/__init__.py
+-rw-r--r--   0 drw       (1000) drw       (1000)     1055 2023-06-27 17:22:08.000000 pylag-2.2/pylag/absorber.py
+-rw-r--r--   0 drw       (1000) drw       (1000)    17264 2023-04-19 18:45:47.000000 pylag-2.2/pylag/binning.py
+-rw-rw-r--   0 drw       (1000) drw       (1000)    10650 2018-07-30 21:30:25.000000 pylag-2.2/pylag/bispectrum.py
+-rw-rw-r--   0 drw       (1000) drw       (1000)     4276 2018-07-24 20:29:44.000000 pylag-2.2/pylag/cepstrum.py
+-rw-rw-r--   0 drw       (1000) drw       (1000)    20819 2024-02-05 23:45:14.000000 pylag-2.2/pylag/coherence.py
+-rw-rw-r--   0 drw       (1000) drw       (1000)     4763 2018-10-22 23:40:24.000000 pylag-2.2/pylag/continuum.py
+-rw-rw-r--   0 drw       (1000) drw       (1000)     1472 2019-04-15 19:05:32.000000 pylag-2.2/pylag/correlation.py
+-rw-r--r--   0 drw       (1000) drw       (1000)    22983 2024-02-06 01:51:54.000000 pylag-2.2/pylag/covariance.py
+-rw-rw-r--   0 drw       (1000) drw       (1000)    17882 2024-02-06 00:14:16.000000 pylag-2.2/pylag/cross_spectrum.py
+-rw-rw-r--   0 drw       (1000) drw       (1000)     2459 2019-08-14 23:28:06.000000 pylag-2.2/pylag/dcf.py
+-rw-r--r--   0 drw       (1000) drw       (1000)    51810 2024-05-08 20:40:51.000000 pylag-2.2/pylag/entresponse.py
+-rw-r--r--   0 drw       (1000) drw       (1000)     4937 2020-01-25 00:35:44.000000 pylag-2.2/pylag/event_list.py
+-rw-r--r--   0 drw       (1000) drw       (1000)    11209 2024-01-29 23:46:20.000000 pylag-2.2/pylag/fit.py
+-rw-r--r--   0 drw       (1000) drw       (1000)     4112 2024-04-30 21:26:30.000000 pylag-2.2/pylag/fits_spec_model.py
+-rw-rw-r--   0 drw       (1000) drw       (1000)     1587 2019-03-29 15:55:35.000000 pylag-2.2/pylag/flux_histogram.py
+-rw-r--r--   0 drw       (1000) drw       (1000)     9928 2023-11-15 18:57:50.000000 pylag-2.2/pylag/fvar.py
+-rw-rw-r--   0 drw       (1000) drw       (1000)    20498 2021-04-20 00:47:47.000000 pylag-2.2/pylag/gaussian_process.py
+-rw-rw-r--   0 drw       (1000) drw       (1000)     8964 2019-03-06 00:13:34.000000 pylag-2.2/pylag/gaussian_process_celerite.py
+-rw-r--r--   0 drw       (1000) drw       (1000)    15240 2024-02-06 02:04:41.000000 pylag-2.2/pylag/lag_energy_spectrum.py
+-rw-rw-r--   0 drw       (1000) drw       (1000)     7034 2024-02-07 19:45:34.000000 pylag-2.2/pylag/lag_frequency_spectrum.py
+-rw-r--r--   0 drw       (1000) drw       (1000)     8621 2021-08-14 18:13:56.000000 pylag-2.2/pylag/lens_lag.py
+-rw-r--r--   0 drw       (1000) drw       (1000)    88490 2024-02-22 22:52:27.000000 pylag-2.2/pylag/lightcurve.py
+-rw-r--r--   0 drw       (1000) drw       (1000)      975 2023-01-11 23:27:24.000000 pylag-2.2/pylag/math_functions.py
+-rw-r--r--   0 drw       (1000) drw       (1000)    53322 2022-08-05 20:10:39.000000 pylag-2.2/pylag/mlcovariance.py
+-rw-r--r--   0 drw       (1000) drw       (1000)    52472 2023-11-14 01:32:35.000000 pylag-2.2/pylag/mlfit.py
+-rw-r--r--   0 drw       (1000) drw       (1000)    10119 2024-02-01 21:49:47.000000 pylag-2.2/pylag/model.py
+-rw-rw-r--   0 drw       (1000) drw       (1000)    19476 2024-02-05 23:52:17.000000 pylag-2.2/pylag/periodogram.py
+-rw-r--r--   0 drw       (1000) drw       (1000)    55900 2024-02-12 23:50:24.000000 pylag-2.2/pylag/plotter.py
+-rw-r--r--   0 drw       (1000) drw       (1000)     5377 2022-08-29 20:14:55.000000 pylag-2.2/pylag/response.py
+-rw-r--r--   0 drw       (1000) drw       (1000)     3661 2024-04-30 21:26:30.000000 pylag-2.2/pylag/reverb_model.py
+-rw-r--r--   0 drw       (1000) drw       (1000)    14567 2024-02-06 02:02:07.000000 pylag-2.2/pylag/rms.py
+-rw-r--r--   0 drw       (1000) drw       (1000)    41414 2023-06-27 18:42:46.000000 pylag-2.2/pylag/simulator.py
+-rw-r--r--   0 drw       (1000) drw       (1000)     1061 2024-03-28 21:32:38.000000 pylag-2.2/pylag/time.py
+-rw-r--r--   0 drw       (1000) drw       (1000)     4899 2024-02-07 19:46:29.000000 pylag-2.2/pylag/util.py
+drwxr-xr-x   0 drw       (1000) drw       (1000)        0 2024-05-14 17:37:19.247554 pylag-2.2/pylag.egg-info/
+-rw-r--r--   0 drw       (1000) drw       (1000)      341 2024-05-14 17:37:19.000000 pylag-2.2/pylag.egg-info/PKG-INFO
+-rw-r--r--   0 drw       (1000) drw       (1000)      881 2024-05-14 17:37:19.000000 pylag-2.2/pylag.egg-info/SOURCES.txt
+-rw-r--r--   0 drw       (1000) drw       (1000)        1 2024-05-14 17:37:19.000000 pylag-2.2/pylag.egg-info/dependency_links.txt
+-rw-r--r--   0 drw       (1000) drw       (1000)       20 2024-05-14 17:37:19.000000 pylag-2.2/pylag.egg-info/requires.txt
+-rw-r--r--   0 drw       (1000) drw       (1000)        6 2024-05-14 17:37:19.000000 pylag-2.2/pylag.egg-info/top_level.txt
+-rw-r--r--   0 drw       (1000) drw       (1000)       79 2024-05-14 17:37:19.247554 pylag-2.2/setup.cfg
+-rw-r--r--   0 drw       (1000) drw       (1000)      391 2024-05-14 17:36:25.000000 pylag-2.2/setup.py
```

### Comparing `pylag-2.1/LICENSE.md` & `pylag-2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pylag-2.1/README.md` & `pylag-2.2/README.md`

 * *Files identical despite different names*

### Comparing `pylag-2.1/pylag/absorber.py` & `pylag-2.2/pylag/absorber.py`

 * *Files identical despite different names*

### Comparing `pylag-2.1/pylag/binning.py` & `pylag-2.2/pylag/binning.py`

 * *Files identical despite different names*

### Comparing `pylag-2.1/pylag/bispectrum.py` & `pylag-2.2/pylag/bispectrum.py`

 * *Files identical despite different names*

### Comparing `pylag-2.1/pylag/cepstrum.py` & `pylag-2.2/pylag/cepstrum.py`

 * *Files identical despite different names*

### Comparing `pylag-2.1/pylag/coherence.py` & `pylag-2.2/pylag/coherence.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,60 +83,42 @@
         self.num_freq = np.array([])
 
         self.bins = bins
 
         if bins is not None:
             self.freq = bins.bin_cent
             self.freq_error = bins.x_error()
-        elif fmin > 0 and fmax > 0:
+        elif fmin is not None and fmax is not None and (fmin > 0 and fmax > 0):
             self.freq = np.mean([fmin, fmax])
             self.freq_error = None
 
         # if we're passed a single pair of light curves, get the cross spectrum
         # and periodograms and count the number of sample frequencies in either
         # the bins or specified range
         if isinstance(lc1, LightCurve) and isinstance(lc2, LightCurve):
             self.cross_spec = CrossSpectrum(lc1, lc2, **kwargs)
             self.per1 = Periodogram(lc1, **kwargs)
             self.per2 = Periodogram(lc2, **kwargs)
-            if bins is not None:
-                self.num_freq = lc1.bin_num_freq(bins)
-                # apply binning to cross spectrum and periodogram
-                self.cross_spec = self.cross_spec.bin(bins)
-                self.per1 = self.per1.bin(bins, calc_error=False)
-                self.per2 = self.per2.bin(bins, calc_error=False)
-            elif fmin > 0 and fmax > 0:
-                self.num_freq = lc1.num_freq_in_range(fmin, fmax)
             self.lc1mean = lc1.mean()
             self.lc2mean = lc2.mean()
 
         # if we're passed lists of light curves, get the stacked cross spectrum
         # and periodograms and count the number of sample frequencies across all
         # the light curves
         elif isinstance(lc1, list) and isinstance(lc2, list):
             self.cross_spec = StackedCrossSpectrum(lc1, lc2, bins, **kwargs)
-            self.per1 = StackedPeriodogram(lc1, bins, calc_error=False, **kwargs)
-            self.per2 = StackedPeriodogram(lc2, bins, calc_error=False, **kwargs)
-            if bins is not None:
-                self.num_freq = np.zeros(bins.num)
-
-                for lc in lc1:
-                    self.num_freq += lc.bin_num_freq(bins)
-            elif fmin > 0 and fmax > 0:
-                self.num_freq = 0
-                for lc in lc1:
-                    self.num_freq += lc.num_freq_in_range(fmin, fmax)
+            self.per1 = StackedPeriodogram(lc1, bins=None, calc_error=False, **kwargs)
+            self.per2 = StackedPeriodogram(lc2, bins=None, calc_error=False, **kwargs)
             self.lc1mean = stacked_mean_count_rate(lc1)
             self.lc2mean = stacked_mean_count_rate(lc2)
 
-        self.coh = self.calculate(bins, fmin, fmax, bias)
-
-        # delete the cross spectrum and periodograms to save some memory once
-        # we've finished the calculation
-        del self.cross_spec, self.per1, self.per2
+        if bins is not None or (fmin is not None and fmax is not None):
+            self.coh, self.num_freq = self.calculate(bins, fmin, fmax, bias)
+        else:
+            self.coh, self.num_freq = np.nan, 0
 
     def calculate(self, bins=None, fmin=None, fmax=None, bias=True):
         """
         pylag.Coherence.calculate(bins=None, fmin=None, fmax=None)
 
         calculate the coherence either in each bin or over a specified frequency
         range. The result is returned either as a numpy array if calculated over
@@ -160,39 +142,53 @@
         -------
         coh : ndarray or float
               The calculated coherence either as a numpy array containing the
               value for each frequency bin or a single float if the coherence is
               calculated over a single frequency range
         """
         if bins is not None:
-            # note the binning is already taken care of in the constructor
-            # since the StackedPeriodogram needs to be binned when created
-            cross_spec = self.cross_spec.crossft
-            per1 = self.per1.periodogram
-            per2 = self.per2.periodogram
+            cross_spec = self.cross_spec.bin(bins).crossft
+            per1 = self.per1.bin(bins).periodogram
+            per2 = self.per2.bin(bins).periodogram
+            num_freq = self.per1.num_freq_in_bins(bins)
         elif fmin > 0 and fmax > 0:
             cross_spec = self.cross_spec.freq_average(fmin, fmax)
             per1 = self.per1.freq_average(fmin, fmax)
             per2 = self.per2.freq_average(fmin, fmax)
+            num_freq = self.per1.num_freq_in_range(fmin, fmax)
 
         if bias:
             pnoise1 = 2 * (self.lc1mean + self.bkg1) / self.lc1mean ** 2
             pnoise2 = 2 * (self.lc2mean + self.bkg2) / self.lc2mean ** 2
-            nbias = (pnoise2 * (per1 - pnoise1) + pnoise1 * (per2 - pnoise2) + pnoise1 * pnoise2) / self.num_freq
+            nbias = (pnoise2 * (per1 - pnoise1) + pnoise1 * (per2 - pnoise2) + pnoise1 * pnoise2) / num_freq
         else:
             nbias = 0
 
         coh = (np.abs(cross_spec) ** 2 - nbias) / (per1 * per2)
-        return coh
+        return coh, num_freq
 
-    def phase_error(self):
-        return np.sqrt((1 - self.coh) / (2 * self.coh * self.num_freq))
+    def phase_error(self, fmin=None, fmax=None, bins=None):
+        if fmin is not None and fmax is not None:
+            coh, num_freq = self.calculate(fmin=fmin, fmax=fmax)
+        elif bins is not None:
+            coh, num_freq = self.calculate(bins=bins)
+        else:
+            coh, num_freq = self.coh, self.num_freq
+        return np.sqrt((1 - coh) / (2 * coh * num_freq))
+
+    def lag_error(self, fmin=None, fmax=None, bins=None):
+        # get the central frequency of the range or bins
+        if fmin is not None and fmax is not None:
+            freq = np.mean([fmin, fmax])
+        elif bins is not None:
+            freq = bins.bin_cent
+        else:
+            freq = self.freq
 
-    def lag_error(self):
-        return self.phase_error() / (2 * np.pi * self.freq)
+        return self.phase_error(fmin, fmax, bins) / (2 * np.pi * freq)
 
     def _getplotdata(self):
         return (self.freq, self.freq_error), self.coh
 
     def _getplotaxes(self):
         return 'Frequency / Hz', 'log', 'Coherence', 'linear'
```

### Comparing `pylag-2.1/pylag/continuum.py` & `pylag-2.2/pylag/continuum.py`

 * *Files identical despite different names*

### Comparing `pylag-2.1/pylag/correlation.py` & `pylag-2.2/pylag/correlation.py`

 * *Files identical despite different names*

### Comparing `pylag-2.1/pylag/covariance.py` & `pylag-2.2/pylag/covariance.py`

 * *Files 7% similar despite different names*

```diff
@@ -86,54 +86,45 @@
         self.num_freq = np.array([])
 
         self.bins = bins
 
         if bins is not None:
             self.freq = bins.bin_cent
             self.freq_error = bins.x_error()
-            self.delta_f = bins.delta_x()
-        elif fmin > 0 and fmax > 0:
+        elif fmin is not None and fmax is not None and (fmin > 0 and fmax > 0):
             self.freq = np.mean([fmin, fmax])
             self.freq_error = None
-            self.delta_f = fmax - fmin
 
         # if we're passed a single pair of light curves, get the cross spectrum
         # and periodograms and count the number of sample frequencies in either
         # the bins or specified range
         if isinstance(lc, LightCurve) and isinstance(reflc, LightCurve):
             self.cross_spec = CrossSpectrum(lc, reflc)
             self.per = Periodogram(reflc)
             self.per_ref = Periodogram(reflc)
-            if bins is not None:
-                self.num_freq = reflc.bin_num_freq(bins)
-            elif fmin > 0 and fmax > 0:
-                self.num_freq = reflc.num_freq_in_range(fmin, fmax)
             self.reflcmean = reflc.mean()
             self.lcmean = lc.mean()
 
         # if we're passed lists of light curves, get the stacked cross spectrum
         # and periodograms and count the number of sample frequencies across all
         # the light curves
         elif isinstance(lc, list) and isinstance(reflc, list):
             self.cross_spec = StackedCrossSpectrum(lc, reflc, bins)
             self.per = StackedPeriodogram(lc, bins)
             self.per_ref = StackedPeriodogram(reflc, bins)
-            if bins is not None:
-                self.num_freq = np.zeros(bins.num)
-
-                for l in reflc:
-                    self.num_freq += l.bin_num_freq(bins)
-            elif fmin > 0 and fmax > 0:
-                self.num_freq = 0
-                for l in reflc:
-                    self.num_freq += l.num_freq_in_range(fmin, fmax)
             self.reflcmean = stacked_mean_count_rate(reflc)
             self.lcmean = stacked_mean_count_rate(lc)
 
-        self.cov, self.error = self.calculate(bins, fmin, fmax, bias)
+        self.pnoise = 2 * (self.lcmean + self.bkg1) / self.lcmean ** 2
+        self.pnoise_ref = 2 * (self.reflcmean + self.bkg2) / self.reflcmean ** 2
+
+        if bins is not None or (fmin is not None and fmax is not None):
+            self.cov, self.error = self.calculate(bins, fmin, fmax, bias)
+        else:
+            self.cov, self.error = np.nan, np.nan
 
     def calculate(self, bins=None, fmin=None, fmax=None, bias=True):
         """
         pylag.Coherence.calculate(bins=None, fmin=None, fmax=None)
 
         calculate the covariance either in each bin or over a specified frequency
         range. The result is returned either as a numpy array if calculated over
@@ -160,38 +151,38 @@
               value for each frequency bin or a single float if the coherence is
               calculated over a single frequency range
         """
         if bins is not None:
             cross_spec = self.cross_spec.bin(self.bins).crossft
             per = self.per.bin(self.bins).periodogram
             per_ref = self.per_ref.bin(self.bins).periodogram
+            num_freq = self.per_ref.num_freq_in_bins(bins)
+            delta_f = bins.delta_x()
         elif fmin > 0 and fmax > 0:
             cross_spec = self.cross_spec.freq_average(fmin, fmax)
             per = self.per.freq_average(fmin, fmax)
             per_ref = self.per_ref.freq_average(fmin, fmax)
+            num_freq = self.per_ref.num_freq_in_range(fmin, fmax)
+            delta_f = fmax - fmin
 
         if bias:
-            pnoise = 2 * (self.lcmean + self.bkg1) / self.lcmean ** 2
-            pnoise_ref = 2 * (self.reflcmean + self.bkg2) / self.reflcmean ** 2
             nbias = (
-                    pnoise_ref * (per - pnoise) + pnoise * (per_ref - pnoise_ref) + pnoise * pnoise_ref) / self.num_freq
+                    self.pnoise_ref * (per - self.pnoise) + self.pnoise * (per_ref - self.pnoise_ref) + self.pnoise * self.pnoise_ref) / num_freq
         else:
-            pnoise = 0
-            pnoise_ref = 0
             nbias = 0
 
-        cov = self.lcmean * np.sqrt(self.delta_f * (np.abs(cross_spec) ** 2 - nbias) / (per_ref - pnoise_ref))
+        cov = self.lcmean * np.sqrt(delta_f * (np.abs(cross_spec) ** 2 - nbias) / (per_ref - self.pnoise_ref))
 
-        # rms = (per - pnoise) * self.lcmean ** 2 * self.delta_f
-        rms_noise = pnoise * self.lcmean ** 2 * self.delta_f
-        rms_ref = (per_ref - pnoise_ref) * self.reflcmean ** 2 * self.delta_f
-        rms_ref_noise = pnoise_ref * self.reflcmean ** 2 * self.delta_f
+        # rms = (per - pnoise) * self.lcmean ** 2 * delta_f
+        rms_noise = self.pnoise * self.lcmean ** 2 * delta_f
+        rms_ref = (per_ref - self.pnoise_ref) * self.reflcmean ** 2 * delta_f
+        rms_ref_noise = self.pnoise_ref * self.reflcmean ** 2 * delta_f
 
         err = np.sqrt((cov ** 2 * rms_ref_noise + rms_ref * rms_noise + rms_noise * rms_ref_noise) / (
-            2 * self.num_freq * rms_ref))
+            2 * num_freq * rms_ref))
 
         return cov, err
 
     def _getplotdata(self):
         return (self.freq, self.freq_error), (self.cov, self.error)
 
     def _getplotaxes(self):
@@ -270,105 +261,100 @@
     def __init__(self, fmin, fmax, lclist=None, lcfiles='', interp_gaps=False, refband=None,
                  bias=True, resample_errors=False, n_samples=100):
         self.en = np.array([])
         self.en_error = np.array([])
         self.cov = np.array([])
         self.error = np.array([])
 
+        self._freq_range = (fmin, fmax)
+
         self.return_sed = True
+        self.bias = bias
 
         if lcfiles != '':
             lclist = EnergyLCList(lcfiles, interp_gaps=interp_gaps)
 
         self.en = np.array(lclist.en)
         self.en_error = np.array(lclist.en_error)
 
-        if resample_errors:
-            printmsg(1, "Constructing covariance spectrum from resampled light curves in %d energy bins" % len(lclist))
-            self.cov, self.error = self.calculate_resample(lclist, fmin, fmax, refband, self.en, bias, n_samples)
-        elif isinstance(lclist[0], LightCurve):
+        if isinstance(lclist[0], LightCurve):
             printmsg(1, "Constructing covariance spectrum in %d energy bins" % len(lclist))
-            self.cov, self.error = self.calculate(lclist.lclist, fmin, fmax, refband, self.en, bias=bias)
+            self.covariances = self.calculate_covariances(lclist.lclist, refband, self.en)
         elif isinstance(lclist[0], list) and isinstance(lclist[0][0], LightCurve):
             printmsg(1, "Constructing covariance spectrum from %d light curves in each of %d energy bins" % (
                 len(lclist[0]), len(lclist)))
-            self.cov, self.error = self.calculate_stacked(lclist.lclist, fmin, fmax, refband, self.en, bias=bias)
+            self.covariances = self.calculate_covariances_stacked(lclist.lclist, refband, self.en)
+
+        self.cov, self.error = self.calculate_spectrum(self._freq_range[0], self._freq_range[1], bias=self.bias)
+
+        if resample_errors:
+            printmsg(1, "Estimating errors from %d resamples" % n_samples)
+            self.error = self.resample_errors(lclist, self._freq_range[0], self._freq_range[1], refband, self.en, bias, n_samples)
 
         self.sed, self.sed_error = self.calculate_sed()
 
-    def calculate(self, lclist, fmin, fmax, refband=None, energies=None, bias=True):
+    @staticmethod
+    def calculate_covariances(lclist, refband=None, energies=None):
         """
-        cov, error = pylag.CovarianceSpectrum.calculate(lclist, fmin, fmax, refband=None, energies=None)
+        cov, error = pylag.CovarianceSpectrum.calculate_covariances(lclist, fmin, fmax, refband=None, energies=None)
 
-        calculate the covariance spectrum from a list of light curves, one in
-        each energy band, averaged over some frequency range.
+        calculate the covariances for each light curve vs the reference band to
+        preparate for the calcation of the covariance spectrum
 
         The covariance is calculated with respect to a reference light curve that is
         computed as the sum of all energy bands, but subtracting the energy band
         of interest for each lag/energy point, so to avoid correlated noise
         between the subject and reference light curves.
 
         Arguments
         ---------
         lclist   : list of LightCurve objects
                    1-dimensional list containing the pylag
                    LightCurve objects for the light curve in each of the energy
                    bands, i.e. [en1_lc, en2_lc, ...]
-        fmin     : float
-                   Lower bound of frequency range
-        fmax     : float
-                   Upper bound of frequency range
         refband  : list of floats
                  : If specified, the reference band will be restricted to this
                    energy range [min, max]. If not specified, the full band will
                    be used for the reference
         energies : ndarray (default=None)
                  : If a specific range of energies is to be used for the reference
                    band rather than the full band, this is the list of central
                    energies of the bands represented by each light curve
-        bias	 : boolean, optional (default=True)
-                   If true, the bias due to Poisson noise will be subtracted from
-                   the magnitude of the cross spectrum and periodograms
 
         Returns
         -------
-        cov   : ndarray
-                numpy array containing the lag of each energy band with respect
-                to the reference band
-        error : ndarray
-                numpy array containing the error in each lag measurement
+        covariances : list of Covariance objects
+                      Covariance foe each energy band
         """
         reflc = LightCurve(t=lclist[0].time)
         for energy_num, lc in enumerate(lclist):
             if refband is not None:
                 if energies[energy_num] < refband[0] or energies[energy_num] > refband[1]:
                     continue
             reflc = reflc + lc
 
-        cov = []
-        error = []
+        covariances = []
         for energy_num, lc in enumerate(lclist):
             thisref = reflc - lc
             # if we're only using a specific reference band, we did not need to
             # subtract the current band if it's outside the range
             if refband is not None:
                 if energies[energy_num] < refband[0] or energies[energy_num] > refband[1]:
                     thisref = reflc
-            cov_obj = Covariance(lc, thisref, fmin=fmin, fmax=fmax, bias=bias)
-            cov.append(cov_obj.cov)
-            error.append(cov_obj.error)
+            covariances.append(Covariance(lc, thisref, fmin=None, fmax=None))
 
-        return np.array(cov), np.array(error)
+        return covariances
 
-    def calculate_stacked(self, lclist, fmin, fmax, refband=None, energies=None, bias=True):
+    @staticmethod
+    def calculate_covariances_stacked(lclist, refband=None, energies=None):
         """
         cov, error = pylag.CovarianceSpectrum.calculate_stacked(lclist, fmin, fmax, refband=None, energies=None)
 
-        calculate the covariance spectrum from a list of light curves, averaged
-        over some frequency range. The covariance is calculated from the cross
+        calculate the covariances from a list of light curves vs the reference
+        band. The covariance is calculated from the cross
         spectrum and coherence stacked over multiple light curve segments in
         each energy band.
 
         The covariance is calculated with respect to a reference light curve that is
         computed as the sum of all energy bands, but subtracting the energy band
         of interest for each lag/energy point, so to avoid correlated noise
         between the subject and reference light curves.
@@ -377,37 +363,27 @@
         ---------
         lclist   : list of lists of LightCurve objects
                    This is a 2-dimensional list (i.e. list of lists). The outer index
                    corresponds to the energy band. For each energy band, there is a
                    list of LightCurve objects that represent the light curves in that
                    energy band from each observation segment.
                    i.e. [[en1_obs1, en1_obs2, ...], [en2_obs1, en2_obs2, ...], ...]
-        fmin     : float
-                   Lower bound of frequency range
-        fmax     : float
-                   Upper bound of frequency range
         refband  : list of floats
                  : If specified, the reference band will be restricted to this
                    energy range [min, max]. If not specified, the full band will
                    be used for the reference
         energies : ndarray (default=None)
                  : If a specific range of energies is to be used for the reference
                    band rather than the full band, this is the list of central
                    energies of the bands represented by each light curve
-        bias	 : boolean, optional (default=True)
-                   If true, the bias due to Poisson noise will be subtracted from
-                   the magnitude of the cross spectrum and periodograms
 
         Returns
         -------
-        cov   : ndarray
-                numpy array containing the covariance of each energy band with respect
-                to the reference band
-        error : ndarray
-                numpy array containing the error in each lag measurement
+        covariances : list of Covariance objects
+                      Covariance foe each energy band
         """
         reflc = []
         # initialise a reference light curve for each of the observations/light
         # curve segments
         for lc in lclist[0]:
             reflc.append(LightCurve(t=lc.time))
         # sum all of the energies (outer index) together to produce a reference
@@ -417,53 +393,89 @@
             # in that range
             if refband is not None:
                 if energies[energy_num] < refband[0] or energies[energy_num] > refband[1]:
                     continue
             for segment_num, segment_lc in enumerate(energy_lcs):
                 reflc[segment_num] = reflc[segment_num] + segment_lc
 
-        cov = []
-        error = []
+        covariances = []
         for energy_num, energy_lclist in enumerate(lclist):
             # subtract this energy band from the reference light curve for each
             # light curve segment to be stacked (subtracting the current band
             # means we don't have correlated noise between the subject and
             # reference bands)
             ref_lclist = []
             for segment_num, segment_lc in enumerate(energy_lclist):
                 # if a reference band is specifed and this energy falls outside that
                 # band, no need to subtract the current band
                 if refband is not None:
                     if energies[energy_num] < refband[0] or energies[energy_num] > refband[1]:
                         ref_lclist.append(reflc[segment_num])
                         continue
                 ref_lclist.append(reflc[segment_num] - segment_lc)
-            # now get the covariance and error
-            cov_obj = Covariance(energy_lclist, ref_lclist, fmin=fmin, fmax=fmax, bias=bias)
-            cov.append(cov_obj.cov)
-            error.append(cov_obj.error)
+            # now get the covariance
+            covariances.append(Covariance(energy_lclist, ref_lclist, fmin=None, fmax=None))
+
+        return covariances
 
+    def calculate_spectrum(self, fmin, fmax, covariances=None, bias=True):
+        """
+        cov, error = pylag.CovarianceSpectrum.calculate_spectrum(fmin, fmax, covariances=None, bias=True)
+
+        calculate the covariance spectrum by averaging the covariances for each band
+        over the requested frequency range.
+
+        Requires that the covariances for each band vs the reference have been pre-calculated
+
+        Arguments
+        ---------
+        fmin        : float
+                      Lower bound of frequency range
+        fmax        : float
+                      Upper bound of frequency range
+        covariances : list of Covariance objects, optional (default=None)
+                      The Covariance object for each band vs. the reference from
+                      which the spectrum is to be calculated. If None, the Covariances
+                      that were pre-calculated when this objected was constructed will be
+                      used
+        bias	    : boolean, optional (default=True)
+                      If true, the bias due to Poisson noise will be subtracted from
+                      the magnitude of the cross spectrum and periodograms
+
+        Returns
+        -------
+        cov   : ndarray
+                numpy array containing the covariance of each energy band with respect
+                to the reference band
+        error : ndarray
+                numpy array containing the error in each covariance measurement
+        """
+        if covariances is None:
+            covariances = self.covariances
+
+        cov, error = zip(*[c.calculate(fmin=fmin, fmax=fmax, bias=bias) for c in covariances])
         return np.array(cov), np.array(error)
 
-    def calculate_resample(self, lclist, fmin, fmax, refband, energies, bias, n_samples):
+    def resample_errors(self, lclist, fmin, fmax, refband, energies, bias, n_samples, mode='std'):
         cov = []
         for n in range(n_samples):
             this_lclist = lclist.resample_noise()
             if isinstance(lclist[0], LightCurve):
-                this_cov, _ = self.calculate(this_lclist.lclist, fmin, fmax, refband, energies, bias)
+                covariances = self.calculate_covariances(this_lclist.lclist, refband, energies)
             elif isinstance(lclist[0], list) and isinstance(lclist[0][0], LightCurve):
-                this_cov, _ = self.calculate_stacked(this_lclist.lclist, fmin, fmax, refband, energies, bias)
+                covariances = self.calculate_covariances_stacked(this_lclist.lclist, refband, energies)
+            this_cov, _ = self.calculate_spectrum(fmin, fmax, covariances, bias)
             cov.append(this_cov)
 
         cov = np.array(cov)
 
-        cov_values = np.mean(cov, axis=0)
-        cov_errors = np.std(cov, axis=0)
+        if mode =='std':
+            cov_errors = np.nanstd(cov, axis=0)
 
-        return cov_values, cov_errors
+        return cov_errors
 
     def calculate_sed(self):
         """
         sed, err = pylag.CovarianceSpectrum.calculate_sed()
 
         Calculatethe covariance in units of E*F_E (the spectral energy distribution),
         the	equivalent of eeufspec in XSPEC.
@@ -485,8 +497,18 @@
     def _getplotaxes(self):
         return 'Energy / keV', 'log', 'Covariance', 'log'
 
     def writeflx(self, filename):
         data = [self.en - self.en_error, self.en + self.en_error, self.cov, self.error]
         np.savetxt(filename, list(zip(*data)), fmt='%15.10g', delimiter=' ')
 
+    def _get_freq_range(self,):
+        return self._freq_range
+
+    def _set_freq_range(self, value):
+        self._freq_range = value
+        self.cov, self.error = self.calculate_spectrum(self._freq_range[0], self._freq_range[1], bias=self.bias)
+        self.sed, self.sed_error = self.calculate_sed()
+
+    freq_range = property(_get_freq_range, _set_freq_range)
+
```

### Comparing `pylag-2.1/pylag/cross_spectrum.py` & `pylag-2.2/pylag/cross_spectrum.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,14 +280,20 @@
                  (in seconds)
 
         """
         avgcross = self.freq_average(fmin, fmax)
         lag = np.angle(avgcross) / (2 * np.pi * np.mean([fmin, fmax]))
         return lag
 
+    def fmin(self):
+        return self.freq[1]
+
+    def fmax(self):
+        return np.max(self.freq)
+
     def cross_power(self, psdslope=0.):
         from .plotter import DataSeries
         if self.ferr is not None:
             xdata = (self.freq, self.ferr)
         else:
             xdata = self.freq
         return DataSeries(x=xdata, y=np.abs(self.freq**-psdslope * self.crossft), xlabel='Frequency / Hz', xscale='log', ylabel='Cross Power', yscale='log')
@@ -393,14 +399,33 @@
         cross_spec : ndarray
                      The average cross spectrum (complex) in each frequency bin
         """
         freq_list = np.hstack([c.freq for c in self.cross_spectra])
         crossft_list = np.hstack([c.crossft for c in self.cross_spectra])
         return self.bins.bin(freq_list, crossft_list)
 
+    def bin(self, bins):
+        """
+        pylag.StackedCrossSpectrum.StackBinnedCrossSpectrum()
+
+        Calculates the average cross spectrum in each frequency bin. The final
+        cross spectrum in each bin is the average over all of the individual
+        frequency points from all of the light curves that fall into that bin.
+
+        Returns
+        -------
+        cross_spec : ndarray
+                     The average cross spectrum (complex) in each frequency bin
+        """
+        freq_list = np.hstack([c.freq for c in self.cross_spectra])
+        crossft_list = np.hstack([c.crossft for c in self.cross_spectra])
+        crossft_bin = bins.bin(freq_list, crossft_list)
+
+        return CrossSpectrum(f=bins.bin_cent, cs=crossft_bin)
+
     def freq_average_slow(self, fmin, fmax):
         """
         csavg = pylag.CrossSpectrum.freq_average(fmin, fmax)
 
         calculate the average value of the cross spectrum over a specified
         frequency interval. The final cross spectrum is the average over all of
         the individual frequency points from all of the light curves that fall
@@ -450,7 +475,13 @@
         freq_list = np.hstack([c.freq for c in self.cross_spectra])
         crossft_list = np.hstack([c.crossft for c in self.cross_spectra])
 
         bin_edges = [fmin, fmax]
         real_mean, _, _ = binned_statistic(freq_list, crossft_list.real, statistic='mean', bins=bin_edges)
         imag_mean, _, _ = binned_statistic(freq_list, crossft_list.imag, statistic='mean', bins=bin_edges)
         return complex(real_mean, imag_mean)
+
+    def fmin(self):
+        return np.min([c.freq[1] for c in self.cross_spectra])
+
+    def fmax(self):
+        return np.max([np.max(c.freq) for c in self.cross_spectra])
```

### Comparing `pylag-2.1/pylag/dcf.py` & `pylag-2.2/pylag/dcf.py`

 * *Files identical despite different names*

### Comparing `pylag-2.1/pylag/entresponse.py` & `pylag-2.2/pylag/entresponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 import matplotlib.pyplot as plt
 import matplotlib.colors as colors
 from scipy.stats import binned_statistic
 
 from .binning import *
 from .plotter import Spectrum
+from .fits_spec_model import FITSSpecModel
 
 from .math_functions import *
 
 
 def weighted_std(values, weights):
     """
     Return the weighted average and standard deviation.
@@ -887,15 +888,20 @@
                      to be used here (e.g. A_Fe=1., Gamma=2., logXi=1.5).
 
         Returns
         --------
         ents : ENTResponse
                pyLag SimEnergyLCList object, containing the full spectral (i.e. the convolved) response.
         """
-        spec = spectrum.spectrum(**kwargs)
+        if isinstance(spectrum, FITSSpecModel):
+            spec = spectrum.spectrum(**kwargs)
+        elif isinstance(spectrum, Spectrum):
+            spec = spectrum
+        else:
+            raise ValueError("spectrum must either be a FITSSpecModel or Spectrum object")
 
         if binspec is not None:
             spec = Spectrum(binspec.bin_cent, binspec.bin(spec.en, spec.spec))
 
         ent_conv = np.zeros((len(enbins), self.ent.shape[1]))
         for i in range(self.ent.shape[1]):
             ent_conv[:,i] = convolve_spectrum(spec.en, spec.spec, self.en_bins.bin_cent/line_en, self.ent[:,i], enbins)
@@ -1018,15 +1024,15 @@
         return "<pylag.entresponse.ENTResponse: (%d, %d) energy, time channels>" % (self.ent.shape[0], self.ent.shape[1])
 
     def __repr__(self):
         return "<pylag.entresponse.ENTResponse: (%d, %d) energy, time channels>" % (self.ent.shape[0], self.ent.shape[1])
 
 
 class ENTResponseSet(object):
-    def __init__(self, response_file):
+    def __init__(self, response_file, interp=False):
         try:
             import h5py
         except ModuleNotFoundError:
             raise ModuleNotFoundError('ENTResponseSet requires h5py to be installed')
 
         with h5py.File(response_file) as hdf:
             en0 = hdf['responses'].attrs['en0']
@@ -1036,25 +1042,46 @@
             self.en_bins = LogBinning(en0, enmax, Nen) if self.logbin_en else LinearBinning(en0, enmax, Nen)
 
             t0 = hdf['responses'].attrs['t0']
             dt = hdf['responses'].attrs['dt']
             Nt = hdf['responses'].attrs['Nt']
             self.time = t0 + dt * np.arange(0, Nt, 1)
 
-            self.heights = np.array(hdf['heights'])
+            self.spin = np.array(hdf['spin'])
             self.incl = np.array(hdf['incl'])
+            self.heights = np.array(hdf['heights'])
             self.tstart = np.array(hdf['tstart'])
             self.responses = np.array(hdf['responses'])
 
-    def get_response(self, incl, h):
-        i_num = np.argmin(np.abs(self.incl - incl))
-        h_num = np.argmin(np.abs(self.heights - h))
+        self.ent_interpolator = None
+        self.tstart_interpolator = None
+        if interp:
+            self.init_interpolator()
+
+    def init_interpolator(self):
+        from scipy.interpolate import RegularGridInterpolator
+
+        vals = [np.trim_zeros(a, 'b') for a in (self.spin, self.incl, self.heights)]
+        self.ent_interpolator = RegularGridInterpolator(tuple(vals), self.responses)
+        self.tstart_interpolator = RegularGridInterpolator(tuple(vals), self.tstart)
+
+    def get_response(self, spin, incl, h):
+        if self.ent_interpolator is not None:
+            ent = self.ent_interpolator([spin, incl, h])[0]
+            tstart = self.tstart_interpolator([spin, incl, h])[0]
+            return ENTResponse(en_bins=self.en_bins, t=self.time, ent=ent,
+                               logbin_en=self.logbin_en, tstart=tstart)
+
+        else:
+            spin_num = np.argmin(np.abs(self.spin - spin))
+            incl_num = np.argmin(np.abs(self.incl - incl))
+            h_num = np.argmin(np.abs(self.heights - h))
 
-        return ENTResponse(en_bins=self.en_bins, t=self.time, ent=self.responses[i_num, h_num],
-                           logbin_en=self.logbin_en, tstart=self.tstart[i_num, h_num])
+            return ENTResponse(en_bins=self.en_bins, t=self.time, ent=self.responses[spin_num, incl_num, h_num],
+                               logbin_en=self.logbin_en, tstart=self.tstart[spin_num, incl_num, h_num])
 
 
 class RadiusENTResponse(object):
     def __init__(self, response_file):
         try:
             import h5py
         except ModuleNotFoundError:
```

### Comparing `pylag-2.1/pylag/event_list.py` & `pylag-2.2/pylag/event_list.py`

 * *Files identical despite different names*

### Comparing `pylag-2.1/pylag/fits_spec_model.py` & `pylag-2.2/pylag/fits_spec_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -84,19 +84,24 @@
         for i in range(self.spectra.shape[0]):
             binspec[i, :] = en_bins.bin(self.energy, self.spectra[i])
         self.spectra = binspec
         self.energy = en_bins.bin_cent
         self.en_low = en_bins.bin_start
         self.en_high = en_bins.bin_end
 
+        # need to reinitialise the interpolator after rebinning
+        if self.interpolator is not None:
+            self.init_interpolator()
+
     def init_interpolator(self):
         from scipy.interpolate import RegularGridInterpolator
 
         spec_array = np.array(self.spectra)
-        spec_array = spec_array.reshape(13, 4, 15, 11, 10, 2999)
+        dim = list(self.param_num_vals) + [len(self.energy)]
+        spec_array = spec_array.reshape(*dim)
 
         vals = [np.trim_zeros(a, 'b') for a in self.param_tab_vals]
         self.interpolator = RegularGridInterpolator(tuple(vals), spec_array)
 
     def __str__(self):
         return "<pylag.fits_spec_model.FITSSpecModel: %s, parameters: %s%s>" % (self.filename, str(self.params), ", interpolation enabled" if self.interpolator is not None else "")
```

### Comparing `pylag-2.1/pylag/flux_histogram.py` & `pylag-2.2/pylag/flux_histogram.py`

 * *Files identical despite different names*

### Comparing `pylag-2.1/pylag/fvar.py` & `pylag-2.2/pylag/fvar.py`

 * *Files identical despite different names*

### Comparing `pylag-2.1/pylag/gaussian_process.py` & `pylag-2.2/pylag/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `pylag-2.1/pylag/gaussian_process_celerite.py` & `pylag-2.2/pylag/gaussian_process_celerite.py`

 * *Files identical despite different names*

### Comparing `pylag-2.1/pylag/lag_energy_spectrum.py` & `pylag-2.2/pylag/lag_energy_spectrum.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,50 +96,50 @@
                  bias=True, calc_error=True):
         self.en = np.array([])
         self.en_error = np.array([])
         self.lag = np.array([])
         self.error = np.array([])
         self.coh = np.array([])
 
+        self._freq_range = (fmin, fmax)
+
         if lcfiles != '':
             lclist = EnergyLCList(lcfiles, interp_gaps=interp_gaps)
 
         self.en = np.array(lclist.en)
         self.en_error = np.array(lclist.en_error)
 
         if isinstance(lclist[0], LightCurve):
             printmsg(1, "Constructing lag energy spectrum in %d energy bins" % len(lclist))
-            self.lag, self.error, self.coh = self.calculate(lclist.lclist, fmin, fmax, refband, self.en, bias, calc_error)
+            self.cross_spec, self.coherence = self.calculate_crossspec(lclist.lclist, refband, self.en, bias, calc_error)
         elif isinstance(lclist[0], list) and isinstance(lclist[0][0], LightCurve):
             printmsg(1, "Constructing lag energy spectrum from %d light curves in each of %d energy bins" % (
                 len(lclist[0]), len(lclist)))
-            self.lag, self.error, self.coh = self.calculate_stacked(lclist.lclist, fmin, fmax, refband, self.en, bias, calc_error)
+            self.cross_spec, self.coherence = self.calculate_crossspec_stacked(lclist.lclist, refband, self.en, bias, calc_error)
+
+        self.lag, self.error = self.calculate_lag(self._freq_range[0], self._freq_range[1])
 
-    def calculate(self, lclist, fmin, fmax, refband=None, energies=None, bias=True, calc_error=True):
+    def calculate_crossspec(self, lclist, refband=None, energies=None, bias=True, calc_error=True):
         """
-        lag, error = pylag.LagEnergySpectrum.calculate(lclist, fmin, fmax, refband=None, energies=None)
+        cross_spec, coherence = pylag.LagEnergySpectrum.ccalculate_crossspec(self, lclist, refband=None, energies=None, bias=True, calc_error=True)
 
-        calculate the lag-energy spectrum from a list of light curves, one in
-        each energy band, averaged over some frequency range.
+        Calculate the cross spectra and coherence in preparation for calculating the lag-energy spectrum
+        from a list of light curves, one in each energy band.
 
-        The lag is calculated with respect to a reference light curve that is
+        The lags/cross spectra are calculated with respect to a reference light curve that is
         computed as the sum of all energy bands, but subtracting the energy band
         of interest for each lag/energy point, so to avoid correlated noise
         between the subject and reference light curves.
 
         Arguments
         ---------
         lclist   : list of LightCurve objects
                    1-dimensional list containing the pylag
                    LightCurve objects for the light curve in each of the energy
                    bands, i.e. [en1_lc, en2_lc, ...]
-        fmin     : float
-                   Lower bound of frequency range
-        fmax     : float
-                   Upper bound of frequency range
         refband  : list of floats
                  : If specified, the reference band will be restricted to this
                    energy range [min, max]. If not specified, the full band will
                    be used for the reference
         energies : ndarray (default=None)
                  : If a specific range of energies is to be used for the reference
                    band rather than the full band, this is the list of central
@@ -161,40 +161,34 @@
         reflc = LightCurve(t=lclist[0].time)
         for energy_num, lc in enumerate(lclist):
             if refband is not None:
                 if energies[energy_num] < refband[0] or energies[energy_num] > refband[1]:
                     continue
             reflc = reflc + lc
 
-        lag = []
-        error = []
-        coh = []
+        cross_spec = []
+        coherence = []
         for lc in lclist:
             thisref = reflc - lc
             # if we're only using a specific reference band, we did not need to
             # subtract the current band if it's outside the range
             if refband is not None:
                 if energies[energy_num] < refband[0] or energies[energy_num] > refband[1]:
                     thisref = reflc
-            lag.append(CrossSpectrum(lc, thisref).lag_average(fmin, fmax))
+            cross_spec.append(CrossSpectrum(lc, thisref))
             if calc_error:
-                coherence_obj = Coherence(lc, reflc, fmin=fmin, fmax=fmax, bias=bias)
-                error.append(coherence_obj.lag_error())
-                coh.append(coherence_obj.coh)
-            else:
-                error.append(np.nan)
-                coh.append(np.nan)
+                coherence.append(Coherence(lc, reflc, fmin=None, fmax=None, bias=bias))
 
-        return np.array(lag), np.array(error), np.array(coh)
+        return cross_spec, coherence
 
-    def calculate_stacked(self, lclist, fmin, fmax, refband=None, energies=None, bias=True, calc_error=True):
+    def calculate_crossspec_stacked(self, lclist, refband=None, energies=None, bias=True, calc_error=True):
         """
-        lag, error = pylag.LagEnergySpectrum.CalculateStacked(lclist, fmin, fmax, refband=None, energies=None)
+        cross_spec, coherence = pylag.LagEnergySpectrum.calculate_crossspec_stacked(self, lclist, refband=None, energies=None, bias=True, calc_error=True)
 
-        calculate the lag-energy spectrum from a list of light curves, averaged
+        Calculate the lag-energy spectrum from a list of light curves, averaged
         over some frequency range. The lag-energy spectrum is calculated from
         the cross spectrum and coherence stacked over multiple light curve
         segments in each energy band.
 
         The lag is calculated with respect to a reference light curve that is
         computed as the sum of all energy bands, but subtracting the energy band
         of interest for each lag/energy point, so to avoid correlated noise
@@ -204,39 +198,32 @@
         ---------
         lclist   : list of lists of LightCurve objects
                    This is a 2-dimensional list (i.e. list of lists). The outer index
                    corresponds to the energy band. For each energy band, there is a
                    list of LightCurve objects that represent the light curves in that
                    energy band from each observation segment.
                    i.e. [[en1_obs1, en1_obs2, ...], [en2_obs1, en2_obs2, ...], ...]
-        fmin     : float
-                   Lower bound of frequency range
-        fmax     : float
-                   Upper bound of frequency range
         refband  : list of floats
                  : If specified, the reference band will be restricted to this
                    energy range [min, max]. If not specified, the full band will
                    be used for the reference
         energies : ndarray (default=None)
                  : If a specific range of energies is to be used for the reference
                    band rather than the full band, this is the list of central
                    energies of the bands represented by each light curve
         bias     : boolean, optional (default=True)
                    If true, the bias due to Poisson noise will be subtracted when
                    calculating coherence
 
         Returns
         -------
-        lag   : ndarray
-                numpy array containing the lag of each energy band with respect
-                to the reference band
-        error : ndarray
-                numpy array containing the error in each lag measurement
-        coh   : ndarray
-                numpy array containing the coherence in each energy band
+        cross_spec : list of CrossSpectrum objects
+                     The cross spectrum for each energy band vs. the reference
+        coherence  : list of Coherence objects
+                     The Coherence between each energy band and the reference
         """
         reflc = []
         # initialise a reference light curve for each of the observations/light
         # curve segments
         for lc in lclist[0]:
             reflc.append(LightCurve(t=lc.time))
         # sum all of the energies (outer index) together to produce a reference
@@ -246,40 +233,93 @@
             # in that range
             if refband is not None:
                 if energies[energy_num] < refband[0] or energies[energy_num] > refband[1]:
                     continue
             for segment_num, segment_lc in enumerate(energy_lcs):
                 reflc[segment_num] = reflc[segment_num] + segment_lc
 
-        lag = []
-        error = []
-        coh = []
+        cross_spec = []
+        coherence = []
         for energy_num, energy_lclist in enumerate(lclist):
             # subtract this energy band from the reference light curve for each
             # light curve segment to be stacked (subtracting the current band
             # means we don't have correlated noise between the subject and
             # reference bands)
             ref_lclist = []
             for segment_num, segment_lc in enumerate(energy_lclist):
                 # if a reference band is specifed and this energy falls outside that
                 # band, no need to subtract the current band
                 if refband is not None:
                     if energies[energy_num] < refband[0] or energies[energy_num] > refband[1]:
                         ref_lclist.append(reflc[segment_num])
                         continue
                 ref_lclist.append(reflc[segment_num] - segment_lc)
-            # now get the lag and error from the stacked cross spectrum and
+            # now get stacked cross spectrum and
             # coherence between the sets of lightcurves for this energy band and
             # for the reference
-            lag.append(StackedCrossSpectrum(energy_lclist, ref_lclist).lag_average(fmin, fmax))
+            cross_spec.append(StackedCrossSpectrum(energy_lclist, ref_lclist))
             if calc_error:
-                coherence_obj = Coherence(energy_lclist, ref_lclist, fmin=fmin, fmax=fmax, bias=bias)
-                error.append(coherence_obj.lag_error())
-                coh.append(coherence_obj.coh)
+                coherence.append(Coherence(energy_lclist, ref_lclist, fmin=None, fmax=None, bias=bias))
+
+        return cross_spec, coherence
+
+    def calculate_lag(self, fmin, fmax, cross_spec=None, coherence=None):
+        """
+        lag, error = pylag.LagEnergySpectrum.calculate_lag(fmin, fmax, , cross_spec=None, coherence=None)
+
+        Ralculate the lag-energy spectrum by averaging the cross spectra for each energy band
+        over the requested frequency range.
+
+        Requires that the cross spectrum and coherence for each band vs the reference have been pre-calculated
 
-        return np.array(lag), np.array(error), np.array(coh)
+        Arguments
+        ---------
+        fmin        : float
+                      Lower bound of frequency range
+        fmax        : float
+                      Upper bound of frequency range
+        cross_spec  : list of CrossSpectrum objects, optional (default=None)
+                      The CrossSpectrum object for each band vs. the reference from
+                      which the lags are to be calculated. If None, the CrossSpectrum objects
+                      that were pre-calculated when this objected was constructed will be
+                      used
+        coherence   : list of CrossSpectrum objects, optional (default=None)
+                      The Coherence object for each band vs. the reference from
+                      which the errors are to be calculated. If None, the Coherence objects
+                      that were pre-calculated when this objected was constructed will be
+                      used
+
+        Returns
+        -------
+        lag   : ndarray
+                numpy array containing the lag of each energy band with respect
+                to the reference band
+        error : ndarray
+                numpy array containing the error in each lag measurement
+        """
+        if cross_spec is None:
+            cross_spec = self.cross_spec
+        if coherence is None:
+            coherence = self.coherence
+
+        lag = np.array([cs.lag_average(fmin, fmax) for cs in cross_spec])
+        if len(coherence) > 0:
+            error = np.array([coh.lag_error(fmin=fmin, fmax=fmax) for coh in coherence])
+        else:
+            error = None
+
+        return lag, error
 
     def _getplotdata(self):
         return (self.en, self.en_error), (self.lag, self.error)
 
     def _getplotaxes(self):
         return 'Energy / keV', 'log', 'Lag / s', 'linear'
+
+    def _get_freq_range(self,):
+        return self._freq_range
+
+    def _set_freq_range(self, value):
+        self._freq_range = value
+        self.lag, self.error = self.calculate_lag(self._freq_range[0], self._freq_range[1])
+
+    freq_range = property(_get_freq_range, _set_freq_range)
```

### Comparing `pylag-2.1/pylag/lag_frequency_spectrum.py` & `pylag-2.2/pylag/lag_frequency_spectrum.py`

 * *Files 17% similar despite different names*

```diff
@@ -71,79 +71,119 @@
            pyLag LightCurve object for the primary or hard band (complex
            conjugated during cross spectrum calculation). If a list of LightCurve
            objects is passed, the stacked lag-frequency spectrum will be calculated
     lc2  : LightCurve or list of LightCurve objects
            pyLag LightCurve object for the reference or soft band
     """
 
-    def __init__(self, bins, lc1=None, lc2=None, lc1files=None, lc2files=None, interp_gaps=False, calc_error=True, resample_errors=False, n_samples=10, calculate_args={}, **kwargs):
-        self.freq = bins.bin_cent
-        self.freq_error = bins.x_error()
-
+    def __init__(self, bins=10, lc1=None, lc2=None, lc1files=None, lc2files=None, interp_gaps=False, calc_error=True, resample_errors=False, n_samples=10, calculate_args={}, **kwargs):
         self.lag = np.array([])
         self.error = np.array([])
 
         if lc1files is not None:
             lc1 = get_lclist(lc1files, interp_gaps=interp_gaps, **kwargs)
         if lc2files is not None:
             lc2 = get_lclist(lc2files, interp_gaps=interp_gaps, **kwargs)
 
+        self.cross_spec, self.coherence = self.calculate_crossspec(lc1, lc2, calc_error, **calculate_args)
+
+        self.fmin = self.cross_spec.fmin()
+        self.fmax = self.cross_spec.fmax()
+
+        if isinstance(bins, Binning):
+            self._bins = bins
+            self._Nf = len(self._bins)
+        elif isinstance(bins, int):
+            self._Nf = bins
+            self._bins = LogBinning(self.fmin, self.fmax, bins)
+        self.freq = self._bins.bin_cent
+        self.freq_error = self._bins.x_error()
+
+        self.lag, self.error = self.calculate_lag(self._bins)
+
         if resample_errors:
-            self.lag, self.error, self.coh = self.calculate_resample(lc1, lc2, bins, n_samples, **calculate_args)
-        else:
-            self.lag, self.error, self.coh = self.calculate(lc1, lc2, bins, calc_error, **calculate_args)
+            self.error = self.resample_errors(lc1, lc2, self._bins, n_samples)
 
     @staticmethod
-    def calculate(lc1, lc2, bins, calc_error=True, **kwargs):
+    def calculate_crossspec(lc1, lc2, calc_error=True, **kwargs):
         if isinstance(lc1, list) and isinstance(lc2, list):
             printmsg(1, "Constructing lag-frequency spectrum from %d pairs of light curves" % len(lc1))
-            cross_spec = StackedCrossSpectrum(lc1, lc2, bins, **kwargs)
-            if calc_error:
-                coh = Coherence(lc1, lc2, bins, **kwargs)
+            cross_spec = StackedCrossSpectrum(lc1, lc2, bins=None, **kwargs)
         elif isinstance(lc1, LightCurve) and isinstance(lc2, LightCurve):
             printmsg(1, "Computing lag-frequency spectrum from pair of light curves")
-            cross_spec = CrossSpectrum(lc1, lc2, **kwargs).bin(bins)
-            if calc_error:
-                coh = Coherence(lc1, lc2, bins, **kwargs)
+            cross_spec = CrossSpectrum(lc1, lc2, **kwargs)
 
-        _, lag = cross_spec.lag_spectrum()
         if calc_error:
-            error = coh.lag_error()
-            coh = coh.coh
+            coherence = Coherence(lc1, lc2, **kwargs)
+        else:
+            coherence = None
+
+        return cross_spec, coherence
+
+    def calculate_lag(self, bins, cross_spec=None, coherence=None):
+        if cross_spec is None:
+            cross_spec = self.cross_spec
+        if coherence is None:
+            coherence = self.coherence
+
+        _, lag = cross_spec.bin(bins).lag_spectrum()
+        if coherence is not None:
+            error = coherence.lag_error(bins=bins)
         else:
             error = None
-            coh = None
 
-        return lag, error, coh
+        return lag, error
 
-    @staticmethod
-    def calculate_resample(lc1, lc2, bins, n_samples=10, **kwargs):
+    def resample_errors(self, lc1, lc2, bins, n_samples=10, **kwargs):
         lags = []
         for n in range(n_samples):
             if isinstance(lc1, list) and isinstance(lc2, list):
                 lc1_resample = []
                 lc2_resample = []
                 for lc in lc1:
                     lc1_resample.append(lc.resample_noise())
                 for lc in lc2:
                     lc2_resample.append(lc.resample_noise())
             elif isinstance(lc1, LightCurve) and isinstance(lc2, LightCurve):
                 lc1_resample = lc1.resample_noise()
                 lc2_resample = lc2.resample_noise()
 
-            l, _, _ = LagFrequencySpectrum.calculate(lc1_resample, lc2_resample, bins, calc_error=False, **kwargs)
+            cs, _ = LagFrequencySpectrum.calculate_crossspec(lc1_resample, lc2_resample, calc_error=False, **kwargs)
+            l, _ = self.calculate_lag(bins, cross_spec=cs, coherence=None)
             lags.append(l)
 
         lags = np.array(lags)
-        lag = np.mean(lags, axis=0)
         error = np.std(lags, axis=0)
 
-        return lag, error, None
+        return error
 
 
     def _getplotdata(self):
         return (self.freq, self.freq_error), (self.lag, self.error)
 
     def _getplotaxes(self):
         return 'Frequency / Hz', 'log', 'Lag / s', 'linear'
 
+    def _get_bins(self,):
+        return self._bins
+
+    def _set_bins(self, value):
+        self._bins = value
+        self.freq = self._bins.bin_cent
+        self.freq_error = self._bins.x_error()
+        self.lag, self.error = self.calculate_lag(self._bins)
+
+    bins = property(_get_bins, _set_bins)
+
+    def _get_Nf(self,):
+        return self._Nf
+
+    def _set_Nf(self, value):
+        self._Nf = value
+        self._bins = LogBinning(self.fmin, self.fmax, self._Nf)
+        self.freq = self._bins.bin_cent
+        self.freq_error = self._bins.x_error()
+        self.lag, self.error = self.calculate_lag(self._bins)
+
+    Nf = property(_get_Nf, _set_Nf)
+
```

### Comparing `pylag-2.1/pylag/lens_lag.py` & `pylag-2.2/pylag/lens_lag.py`

 * *Files identical despite different names*

### Comparing `pylag-2.1/pylag/lightcurve.py` & `pylag-2.2/pylag/lightcurve.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                               Fractional errors from the ERROR columns are combined in
                               quadrature.
                               Light curves must have the same length and time
                               binning.
 
     """
 
-    def __init__(self, filename=None, t=[], r=[], e=[], b=[], be=[], interp_gaps=False, zero_nan=True, trim=False, max_gap=0, **kwargs):
+    def __init__(self, filename=None, t=[], r=[], e=[], b=[], be=[], interp_gaps=False, zero_nan=True, trim=False, max_gap=0, time_format=None, add_bkg=False, **kwargs):
         self.time = np.array(t)
         if len(r) > 0:
             self.rate = np.array(r)
         else:
             self.rate = np.zeros(len(t))
         if len(e) > 0:
             self.error = np.array(e)
@@ -122,29 +122,42 @@
         if len(be) > 0:
             self.bkg_error = np.array(be)
         else:
             self.bkg_error = None
 
         self.telescope = None
         self.instrument = None
+        self.time_format = time_format
+
+        self.tstart = 0
 
         if filename is not None:
             self.filename = filename
             self.read_fits(filename, **kwargs)
 
+        if time_format is None:
+            if self.telescope == 'XMM':
+                self.time_format = 'xmmsec'
+            elif self.telescope == 'CHANDRA':
+                self.time_format = 'cxcsec'
+            elif self.telescope == 'NuSTAR':
+                self.time_format = 'nustarsec'
+
         if len(self.time) > 1:
             self.dt = self.time[1] - self.time[0]
         self.length = len(self.rate)
 
         if interp_gaps:
-            self._interp_gaps(max_gap)
+            self.interp_gaps(max_gap, to_self=True)
         if zero_nan:
             self._zeronan()
         if trim:
             self.trim()
+        if add_bkg:
+            self.add_bkg(to_self=True)
 
         self.filename = filename
 
     def read_fits(self, filename, byte_swap=True, add_tstart=False, time_col='TIME', rate_col='RATE', error_col='ERROR', hdu='RATE', inst=None, bkg=False):
         """
         pylag.LightCurve.read_fits(filename)
 
@@ -208,14 +221,20 @@
 
             if add_tstart:
                 try:
                     tstart = fitsfile[0].header['TSTART']
                     self.time += tstart
                 except:
                     raise AssertionError("pyLag LightCurve ERROR: Could not read TSTART from FITS header")
+            else:
+                try:
+                    tstart = fitsfile[0].header['TSTART']
+                    self.tstart = tstart
+                except:
+                    self.tstart = 0
 
             if bkg:
                 self.bkg_rate = np.array(tabdata['BACKV'])
                 self.bkg_error = np.array(tabdata['BACKE'])
 
             fitsfile.close()
 
@@ -302,15 +321,15 @@
         pylag.LightCurve.zero_time()
 
         Shift the time axis of the light curve to start at zero. The modified
         time axis is stored	back in the original object.
         """
         self.time = self.time - self.time.min()
 
-    def _interp_gaps(self, max_gap=0, min_gap=0, zero_gaps=False):
+    def interp_gaps(self, max_gap=0, min_gap=0, zero_gaps=True, to_self=False):
         """
         pylag.LightCurve._interp_gaps(max_gap=0)
 
         Interpolate over gaps within the light curve for fixing gaps left by GTI
         filters when performing timing analysis.
 
         The missing data points are filled in by linear interpolation between the
@@ -322,41 +341,53 @@
         max_gap : int (optional, default=0)
                   If >0, gaps longer than max_gap time bins will not be interpolated
                   over
         """
         in_gap = False
         gap_count = 0
         longest_gap = 0
+        gap_start = -1
+        gap_end = -1
 
-        for i in range(len(self.rate)):
-            gap_cond = np.isnan(self.rate[i]) or (zero_gaps and self.rate[i] == 0)
+        new_rate = np.array(self.rate)
+        new_error = np.array(self.error)
+
+        for i in range(len(new_rate)):
+            gap_cond = np.isnan(new_rate[i]) or (zero_gaps and new_rate[i] == 0)
             if not in_gap:
                 if gap_cond:
                     in_gap = True
                     gap_start = i - 1
 
             elif in_gap:
                 if not gap_cond:
                     gap_end = i
                     in_gap = False
 
                     gap_length = gap_end - gap_start
 
                     if (gap_length < max_gap or max_gap==0) and gap_length >= min_gap:
                         gap_count += 1
-                        self.rate[gap_start:gap_end] = np.interp(self.time[gap_start:gap_end],
+                        new_rate[gap_start:gap_end] = np.interp(self.time[gap_start:gap_end],
                                                                  [self.time[gap_start], self.time[gap_end]],
-                                                                 [self.rate[gap_start], self.rate[gap_end]])
+                                                                 [new_rate[gap_start], new_rate[gap_end]])
+                        new_error[gap_start:gap_end] = np.sqrt(new_rate[gap_start:gap_end] / self.dt)
 
                         if gap_length > longest_gap:
                             longest_gap = gap_length
 
         printmsg(1, "Patched %d gaps" % gap_count)
         printmsg(1, "Longest gap was %d bins" % longest_gap)
 
+        if to_self:
+            self.rate = new_rate
+            self.error = new_error
+        else:
+            return self._return_lightcurve(t=self.time, r=new_rate, e=new_error)
+
     def _zeronan(self):
         """
         pylag.LightCurve._zeronan()
 
         Replace all instances of nan with zero in the light curve. The modified
         light curve is stored back in the original object.
         """
@@ -385,17 +416,15 @@
         if start < 0:
             start = self.time.min() + abs(start)
         if end < 0:
             end = self.time.max() - abs(end)
         this_t = np.array([t for t in self.time if start < t <= end])
         this_rate = np.array([r for t, r in zip(self.time, self.rate) if start < t <= end])
         this_error = np.array([e for t, e in zip(self.time, self.error) if start < t <= end])
-        segment = LightCurve(t=this_t, r=this_rate, e=this_error)
-        segment.__class__ = self.__class__
-        return segment
+        return self._return_lightcurve(t=this_t, r=this_rate, e=this_error)
 
     def split_segments_time(self, num_segments=1, segment_length=None, use_end=False):
         """
         segments = pylag.LightCurve.split_segments(num_segments=1, segment_length=None)
 
         Divides the light curve into equal time segments which are returned as a
         list of LightCurve objects. The segments are always of equal legnth. If
@@ -453,36 +482,37 @@
         seg_bins = segment_length // np.min(np.diff(self.time)) if segment_length is not None else len(self.rate) // num_segments
 
         num_bins = len(self.rate) - (len(self.rate) % seg_bins) # throw away the end of the light curve
         time_arr = self.time[:num_bins].reshape(-1, seg_bins)
         rate_arr = self.rate[:num_bins].reshape(-1, seg_bins)
         error_arr = self.error[:num_bins].reshape(-1, seg_bins)
 
-        return [LightCurve(t=t, r=r, e=e) for t, r, e in zip(time_arr, rate_arr, error_arr)]
+        return [self._return_lightcurve(t=t, r=r, e=e) for t, r, e in zip(time_arr, rate_arr, error_arr)]
 
     def split_on_gaps(self, min_segment=0):
-        gaps = np.concatenate([[-1], np.argwhere(np.diff(s.time) > np.diff(s.time).min()).flatten(), [len(s.time) - 1]])
-        segs = [(start + 1, end + 1) for start, end in zip(gaps[:-1], gaps[1:])]
+        gaps = np.concatenate([[-1], np.argwhere(np.diff(self.time) > np.diff(self.time).min()).flatten(), [len(self.time) - 1]])
+        segs = [(start + 1, end + 1) for start, end in zip(gaps[:-1], gaps[1:]) if (end-start)>=min_segment]
 
-        lc_seg = [LightCurve(t=self.time[start:end], r=self.rate[start:end], e=self.error[start:end]) for start, end in segs]
+        lc_seg = [self._return_lightcurve(t=self.time[start:end], r=self.rate[start:end], e=self.error[start:end]) for start, end in segs]
+        return lc_seg
 
     def bin_by_gaps(self):
         gaps = np.concatenate([[-1], np.argwhere(np.diff(self.time) > np.diff(self.time).min()).flatten(), [len(self.time) - 1]])
         segs = [(start + 1, end + 1) for start, end in zip(gaps[:-1], gaps[1:])]
 
         t = np.array([0.5*(self.time[start] + self.time[end-1]) for start, end in segs])
         new_dt = np.array([(self.time[end-1] - self.time[start]) for start, end in segs])
 
         dt = np.diff(self.time).min()
         cts = np.array([np.sum(self.rate[start:end]) * dt for start, end in segs])
         r = cts / new_dt
 
         e = np.sqrt(r) / np.sqrt(new_dt)
 
-        lc = LightCurve(t=t, r=r, e=e)
+        lc = self._return_lightcurve(t=t, r=r, e=e)
         lc.time_error = new_dt / 2
         return lc
 
     def split_on_nan(self, min_segment=0):
         """
         lclist = pylag.LightCurve.split_on_gaps(min_segment=0)
 
@@ -589,32 +619,28 @@
 
         if to_self:
             self.time = t
             self.rate = r
             self.error = e
 
         else:
-            lc = LightCurve(t=t, r=r, e=e)
-            lc.__class__ = self.__class__
-            return lc
+            return self._return_lightcurve(t=t, r=r, e=e)
 
     def remove_gaps(self, to_self=False):
         t = self.time[self.rate>0]
         r = self.rate[self.rate>0]
         e = self.error[self.rate>0]
 
         if to_self:
             self.time = t
             self.rate = r
             self.error = e
 
         else:
-            lc = LightCurve(t=t,r=r, e=e)
-            lc.__class__ = self.__class__
-            return lc
+            return self._return_lightcurve(t=t, r=r, e=e)
 
     def rebin_slow(self, tbin):
         """
         rebin_lc = pylag.LightCurve.rebin(tbin)
 
         Rebin the light curve by summing together counts from the old bins into
         new larger bins and return the rebinned light curve as a new LightCurve
@@ -652,18 +678,15 @@
                 counts[-1] *= (float(tbin) / float(max(time_slice) - min(time_slice)))
 
         counts = np.array(counts)
         rate = counts / tbin
         # calculate the sqrt(N) error from the total counts
         err = rate * np.sqrt(counts) / counts
 
-        binlc = LightCurve(t=time[:-1], r=rate, e=err)
-        # make sure the returned object has the right class (if this is called from a derived class)
-        binlc.__class__ = self.__class__
-        return binlc
+        return self._return_lightcurve(t=time[:-1], r=rate, e=err)
 
     def rebin2(self, tbin):
         """
         rebin_lc = pylag.LightCurve.rebin2(tbin)
 
         Rebin the light curve by summing together counts from the old bins into
         new larger bins and return the rebinned light curve as a new LightCurve
@@ -694,18 +717,15 @@
 
         # digitize returns an array stating which bin each element falls into
         digitized = np.digitize(self.time, time)
         counts = np.array([ np.sum(self.dt*self.rate[digitized==i]) for i in range(1,len(time))])
         rate = counts / tbin
         err = rate * np.sqrt(counts) / counts
 
-        binlc = LightCurve(t=time[:-1], r=rate, e=err)
-        # make sure the returned object has the right class (if this is called from a derived class)
-        binlc.__class__ = self.__class__
-        return binlc
+        return self._return_lightcurve(t=time[:-1], r=rate, e=err)
 
     def rebin(self, tbin=None, time=None):
         """
         rebin_lc = pylag.LightCurve.rebin3(tbin)
 
         Rebin the light curve by summing together counts from the old bins into
         new larger bins and return the rebinned light curve as a new LightCurve
@@ -740,35 +760,29 @@
 
         # count the number of original time bins in each new time bin for the efefctive exposure
         num_in_bin = np.array([np.sum(binid == (i + 1)) for i in range(len(time) - 1)])
 
         rate = counts / (self.dt*num_in_bin)
         err = rate * np.sqrt(counts) / counts
 
-        binlc = LightCurve(t=time[:-1], r=rate, e=err)
-        # make sure the returned object has the right class (if this is called from a derived class)
-        binlc.__class__ = self.__class__
-        return binlc
+        return self._return_lightcurve(t=time[:-1], r=rate, e=err)
 
     # TODO: Counts binning based on accumulated count over previous time window
 
     def interpolate(self, tbin=None, time=None, interp_kind='nearest'):
         if time is None:
             time = np.arange(min(self.time), max(self.time)+tbin, tbin)
         rate_interp = interp1d(self.time, self.rate, kind=interp_kind, fill_value='extrapolate')
         tdiff = np.diff(time)
         dt = np.hstack([tdiff, tdiff[-1]])
         rate = rate_interp(time)
         counts = rate * dt
         err = rate * np.sqrt(counts) / counts
 
-        interp_lc = LightCurve(t=time, r=rate, e=err)
-        # make sure the returned object has the right class (if this is called from a derived class)
-        interp_lc.__class__ = self.__class__
-        return interp_lc
+        return self._return_lightcurve(t=time, r=rate, e=err)
 
     def mean(self):
         """
         mean = pylag.LightCurve.mean()
 
         Returns the mean count rate over the light curve
 
@@ -975,66 +989,55 @@
         if not isinstance(other, list):
             raise ValueError("pylag LightCurve Concatenate ERROR: Expected a list of LightCurves to append")
 
         newtime = np.concatenate([self.time] + [lc.time for lc in other])
         newrate = np.concatenate([self.rate] + [lc.rate for lc in other])
         newerr = np.concatenate([self.error] + [lc.error for lc in other])
 
-        newlc = LightCurve(t=newtime, r=newrate, e=newerr)
-        newlc.__class__ = self.__class__
-        return newlc
+        return self._return_lightcurve(t=newtime, r=newrate, e=newerr)
 
     def sort_time(self):
         """
         Sort the light curve points in time order
         """
         t, r, e = zip(*sorted(zip(self.time, self.rate, self.error)))
-        return LightCurve(t=np.array(t), r=np.array(r), e=np.array(e))
+        return self._return_lightcurve(t=np.array(t), r=np.array(r), e=np.array(e))
 
     def log(self):
         """
         Return the logarithm of the count rate
         """
         r = np.log(self.rate)
         e = self.error / self.rate
-        return LightCurve(t=self.time, r=r, e=e)
+        return self._return_lightcurve(t=self.time, r=r, e=e)
 
     def rescale_time(self, mult=None, mass=None):
         """
         Rescale the time axis of the light curve, multiplying by a constant
         e.g. for GM/c^3 to s conversion
         """
         if mass is not None:
             mult = 6.67E-11 * mass * 2E30 / (3E8)**3
         t = self.time * mult
-        lc = LightCurve(t=t, r=self.rate, e=self.error)
-        lc.__class__ = self.__class__
-        return lc
+        return self._return_lightcurve(t=t, r=self.rate, e=self.error)
 
     def convert_time(self, conv_to, conv_from=None):
         """
         Convert the time between different missions or astropy time formats
         conv_to can be any of the string representations for astropy formats, including xmmsec and nustarsec which are
         defined here
         """
         if conv_from is None:
-            if self.telescope == 'XMM':
-                conv_from = 'xmmsec'
-            elif self.telescope == 'CHANDRA':
-                conv_from = 'cxcsec'
-            elif self.telescope == 'NuSTAR':
-                conv_from = 'nustarsec'
-            else:
+            if self.time_format is None:
                 raise ValueError("Can't work out what time the LightCurve is starting in, and conv_from not specified")
+            conv_from = self.time_format
 
         time_obj = astropy.time.Time(self.time, format=conv_from)
         new_time = getattr(time_obj, conv_to)
-        newtime_lc = LightCurve(t=new_time, r=self.rate, e=self.error)
-        newtime_lc.__class__ = self.__class__
-        return newtime_lc
+        return self._return_lightcurve(t=new_time, r=self.rate, e=self.error, time_format=conv_to)
 
     def first_deriv(self):
         """
         Return the first derivative of the light curve
         """
         dt = np.diff(self.time)
         dr = self.rate[1:] - self.rate[:-1]
@@ -1061,48 +1064,93 @@
         # draw the counts in each time bin from a Poisson distribution
         # with the mean set according to the original number of counts in the bin
         rnd_counts = np.random.poisson(counts)
         rate = rnd_counts.astype(float) / self.dt
         # sqrt(N) errors again as if we're making a measurement
         error = np.sqrt(self.rate / self.dt)
 
-        resample_lc = LightCurve(t=self.time, r=rate, e=error)
-        resample_lc.__class__ = self.__class__
-        return resample_lc
+        return self._return_lightcurve(t=self.time, r=rate, e=error)
 
     def moving_average(self, window_size=3):
         window = np.ones(int(window_size)) / float(window_size)
         r_avg = np.convolve(self.rate, window, 'same')
-        lc_avg = LightCurve(t=self.time, r=r_avg, e=np.zeros(self.time.shape))
-        lc_avg.__class__ = self.__class__
-        return lc_avg
+        return self._return_lightcurve(t=self.time, r=r_avg, e=np.zeros(self.time.shape))
 
     def resample_moving_average(self, window_size=3, num_resamples=10000):
         resamples = []
         for n in range(num_resamples):
             resamples.append(self.resample_noise().moving_average(window_size))
         r = self.moving_average(window_size).rate
         e = np.std(np.array([l.rate for l in resamples]), axis=0)
-        resample_lc = LightCurve(t=self.time, r=r, e=e)
-        resample_lc.__class__ = self.__class__
-        return resample_lc
+        return self._return_lightcurve(t=self.time, r=r, e=e)
 
     def find_nearest(self, other, time_mode='matches'):
         if isinstance(other, LightCurve):
             idx = [np.abs(self.time - t).argmin() for t in other.time]
             if time_mode == 'matches':
                 t = self.time[idx]
             elif time_mode == 'orig':
                 t = other.time
-            match_lc = LightCurve(t=t, r=self.rate[idx], e=self.error[idx])
-            match_lc.__class__ = self.__class__
-            return match_lc
+            return self._return_lightcurve(t=t, r=self.rate[idx], e=self.error[idx])
         else:
             return NotImplemented
 
+    def fill_time(self, start=None, end=None, dt=None, exact=False, nan_fill=False):
+        """
+        fill_lc = pylag.LightCurve.fill_time(start=None, end=None, dt=None, exact=False, nan_fill=False)
+
+        Fill the time axis so it is a continuous set of evenly spaced data points
+
+        Arguments
+        ---------
+        start :    float, optional (default=None)
+                   start time of the new time bins. If None, use the start of the current light curve
+        end :      float, optional (default=None)
+                   end time of the new time bins. If None, use the end of the current light curve
+        dt :       float, optional (default=None)
+                   time bin size. If None, use the current time bin size
+        exact :    bool, optional (default=False)
+                   if True, require an exact match between the time values of the old and new light curve, otherwise
+                   find the nearest time bin (within 0.5 times the bin width)
+        nan_fill : bool, optional (default=False)
+                   fill the empty time bins with NaN instead of zeros
+
+        Returns
+        -------
+        fill_lc : LightCurve with filled time bins
+        """
+        if start is None:
+            start = self.time.min()
+        if end is None:
+            end = self.time.max()
+        if dt is None:
+            dt = self.dt
+
+        new_time = np.arange(start, end+dt, dt)
+        new_rate = np.zeros_like(new_time)
+        new_error = np.zeros_like(new_time)
+
+        if nan_fill:
+            new_rate = np.nan * new_rate
+            new_error = np.nan * new_error
+
+        if exact:
+            new_rate[np.isin(new_time, self.time)] = self.rate[np.isin(self.time, new_time)]
+            new_error[np.isin(new_time, self.time)] = self.error[np.isin(self.time, new_time)]
+        else:
+            # for each of the new time bins, find the nearest in the original light curve, but only those within
+            # half a time bin
+            idx = [np.abs(self.time - t).argmin() for t in new_time if np.abs(self.time - t).min() < 0.5*self.dt]
+            # find indices in new array where we have a match
+            matches = [np.min(np.abs(self.time - t)) < 0.5*self.dt for t in new_time]
+            new_rate[matches] = self.rate[idx]
+            new_error[matches] = self.error[idx]
+
+        return self._return_lightcurve(t=new_time, r=new_rate, e=new_error)
+
     def background(self):
         """
         Return the background time series as a LightCurve
         :return:
         """
         if self.bkg_rate is not None:
             return LightCurve(t=self.time, r=self.bkg_rate, e=self.bkg_error)
@@ -1119,15 +1167,15 @@
         """
         rsum = self.rate + self.bkg_rate
         esum = np.sqrt(self.error**2 + self.bkg_error**2)
         if to_self:
             self.rate = rsum
             self.error = esum
         else:
-            return LightCurve(t=self.time, r=rsum, e=esum)
+            return self._return_lightcurve(t=self.time, r=rsum, e=esum)
 
     def to_df(self, errors=False):
         import pandas as pd
         cols = {'time':self.time, 'rate':self.rate}
         if errors:
             cols['error'] = self.error
         df = pd.DataFrame(cols).set_index('time')
@@ -1155,17 +1203,15 @@
                     newbkg = self.bkg_rate + other.bkg_rate
                     newbkgerr = np.sqrt(self.bkg_error ** 2 + other.bkg_error ** 2)
             except:
                 pass
 
             # construct a new Lidnf repoquery --extras --exclude=kernel,kernel-\*ghtCurve with the result and make sure it has the right class
             # (if calling from a derived class)
-            newlc = LightCurve(t=self.time, r=newrate, e=newerr, b=newbkg, be=newbkgerr)
-            newlc.__class__ = self.__class__
-            return newlc
+            return self._return_lightcurve(t=self.time, r=newrate, e=newerr, b=newbkg, be=newbkgerr)
 
         elif isinstance(other, (float, int)):
             newrate = self.rate + other
             newerr = np.sqrt(newrate*self.dt) / self.dt
             newlc = LightCurve(t=self.time, r=newrate, e=newerr)
             newlc.__class__ = self.__class__
             return newlc
@@ -1219,17 +1265,15 @@
                     newbkg = self.bkg_rate - other.bkg_rate
                     newbkgerr = np.sqrt(self.bkg_error ** 2 + other.bkg_error ** 2)
             except:
                 pass
 
             # construct a new LightCurve with the result and make sure it has the right class
             # (if calling from a derived class)
-            newlc = LightCurve(t=self.time, r=newrate, e=newerr, b=newbkg, be=newbkgerr)
-            newlc.__class__ = self.__class__
-            return newlc
+            return self._return_lightcurve(t=self.time, r=newrate, e=newerr, b=newbkg, be=newbkgerr)
 
         else:
             return NotImplemented
 
     def __isub__(self, other):
         """
         Overloaded -= operator to subtract a LightCurve object from this one in
@@ -1264,17 +1308,15 @@
         """
         if isinstance(other, (float, int)):
             newrate = self.rate * other
             # add the fractional errors in quadrature
             newerr = newrate * (self.error / self.rate)
             # construct a new LightCurve with the result and make sure it has the right class
             # (if calling from a derived class)
-            newlc = LightCurve(t=self.time, r=newrate, e=newerr)
-            newlc.__class__ = self.__class__
-            return newlc
+            return self._return_lightcurve(t=self.time, r=newrate, e=newerr)
 
         else:
             return NotImplemented
 
     def __div__(self, other):
         """
         Overloaded / operator to divide this LightCurve object by another and
@@ -1287,27 +1329,23 @@
                 raise AssertionError("pyLag LightCurve ERROR: Cannot divide light curves of different lengths")
             # subtract the count rate
             newrate = self.rate / other.rate
             # add the fractional errors in quadrature
             newerr = newrate * np.sqrt((self.error / self.rate) ** 2 + (other.error / other.rate) ** 2)
             # construct a new LightCurve with the result and make sure it has the right class
             # (if calling from a derived class)
-            newlc = LightCurve(t=self.time, r=newrate, e=newerr)
-            newlc.__class__ = self.__class__
-            return newlc
+            return self._return_lightcurve(t=self.time, r=newrate, e=newerr)
 
         elif isinstance(other, (float, int)):
             newrate = self.rate / other
             # add the fractional errors in quadrature
             newerr = newrate * (self.error / self.rate)
             # construct a new LightCurve with the result and make sure it has the right class
             # (if calling from a derived class)
-            newlc = LightCurve(t=self.time, r=newrate, e=newerr)
-            newlc.__class__ = self.__class__
-            return newlc
+            return self._return_lightcurve(t=self.time, r=newrate, e=newerr)
 
         else:
             return NotImplemented
 
     def __truediv__(self, other):
         """
         Overloaded / operator to divide this LightCurve object by another and
@@ -1320,27 +1358,23 @@
                 raise AssertionError("pyLag LightCurve ERROR: Cannot divide light curves of different lengths")
             # subtract the count rate
             newrate = self.rate / other.rate
             # add the fractional errors in quadrature
             newerr = newrate * np.sqrt((self.error / self.rate) ** 2 + (other.error / other.rate) ** 2)
             # construct a new LightCurve with the result and make sure it has the right class
             # (if calling from a derived class)
-            newlc = LightCurve(t=self.time, r=newrate, e=newerr)
-            newlc.__class__ = self.__class__
-            return newlc
+            return self._return_lightcurve(t=self.time, r=newrate, e=newerr)
 
         elif isinstance(other, (float, int)):
             newrate = self.rate / other
             # add the fractional errors in quadrature
             newerr = newrate * (self.error / self.rate)
             # construct a new LightCurve with the result and make sure it has the right class
             # (if calling from a derived class)
-            newlc = LightCurve(t=self.time, r=newrate, e=newerr)
-            newlc.__class__ = self.__class__
-            return newlc
+            return self._return_lightcurve(t=self.time, r=newrate, e=newerr)
 
         else:
             return NotImplemented
 
     def __eq__(self, other):
         """
         Overloaded == operator to check light curve lengths and time binning are
@@ -1374,40 +1408,50 @@
         return len(self.rate)
 
     def __getitem__(self, index):
         """
         Overloaded operator to access count rate via [] operator
         """
         if isinstance(index, slice):
-            lcslice = LightCurve(t=self.time[index], r=self.rate[index], e=self.error[index])
-            lcslice.__class__ = self.__class__
-            return lcslice
+            return self._return_lightcurve(t=self.time[index], r=self.rate[index], e=self.error[index])
         else:
             return self.rate[index]
 
     def __getslice__(self, start, end):
         """
         Overloaded operator to extract a portion of the light curve using
         [start:end] operator and return as a new LightCurve object
         """
-        slice = LightCurve(t=self.time[start:end], r=self.rate[start:end], e=self.error[start:end])
-        slice.__class__ = self.__class__
-        return slice
+        return self._return_lightcurve(t=self.time[start:end], r=self.rate[start:end], e=self.error[start:end])
 
     def __str__(self):
         return "<pylag.lightcurve.LightCurve: %d time bins, dt = %g%s>" % (len(self), self.dt, ", loaded from: %s" % self.filename if self.filename is not None else "")
 
     def __repr__(self):
         return "<pylag.lightcurve.LightCurve: %d time bins, dt = %g%s>" % (len(self), self.dt, ", loaded from: %s" % self.filename if self.filename is not None else "")
 
     def _getplotdata(self):
         return self.time, (self.rate, self.error)
 
     def _getplotaxes(self):
-        return 'Time / s', 'linear', 'Count Rate / ct s$^{-1}$', 'linear'
+        unit = ''
+        if self.time_format is not None:
+            if 'sec' in self.time_format:
+                unit = ' / s'
+            elif 'mjd' in self.time_format:
+                unit = ' / MJD'
+        return 'Time%s' % unit, 'linear', 'Count Rate / ct s$^{-1}$', 'linear'
+
+    def _return_lightcurve(self, t, r, e, b=[], be=[], time_format=None):
+        lc = LightCurve(t=t, r=r, e=e, b=b, be=be, time_format=time_format if time_format is not None else self.time_format)
+        lc.__class__ = self.__class__
+        lc.telescope = self.telescope
+        lc.instrument = self.instrument
+        return lc
+
 
 
 class VariableBinLightCurve(LightCurve):
     """
     pylag.VariableBinLightCurve
 
     LightCurve class for storing and plotting light curves with variable bin sizes (encoded as the central time of each
@@ -1987,14 +2031,17 @@
             for n, a in enumerate(arr):
                 t = self.lclist[0][n].time
                 np.savetxt('%s_%02d.dat' % (filename, n), np.vstack([t, a]).T, fmt=fmt, delimiter=delimiter)
         else:
             t = self.lclist[0].time
             np.savetxt(filename, np.vstack([t, arr]).T, fmt=fmt, delimiter=delimiter)
 
+    def split(self):
+        split_lclist = [segment_lclist for segment_lclist in zip(*self.lclist)]
+        return [EnergyLCList(enmin=self.enmin, enmax=self.enmax, lclist=l) for l in split_lclist]
 
     def __getitem__(self, index):
         return self.lclist[index]
 
     def __getslice__(self, start, end):
         """
         new_lclist = pylag.extract_lclist_time_segment(lclist, tstart, tend)
```

### Comparing `pylag-2.1/pylag/math_functions.py` & `pylag-2.2/pylag/math_functions.py`

 * *Files identical despite different names*

### Comparing `pylag-2.1/pylag/mlcovariance.py` & `pylag-2.2/pylag/mlcovariance.py`

 * *Files identical despite different names*

### Comparing `pylag-2.1/pylag/mlfit.py` & `pylag-2.2/pylag/mlfit.py`

 * *Files identical despite different names*

### Comparing `pylag-2.1/pylag/model.py` & `pylag-2.2/pylag/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,14 +28,23 @@
         for p, v in zip([p for p in out_params if out_params[p].vary], values):
             out_params[p].value = v
     else:
         for p, v in zip(params, values):
             out_params[p].value = v
     return out_params
 
+def get_param_names(params, variable_only=False):
+    """
+    Return a list of the parameter names
+    """
+    if variable_only:
+        return [k for k in params if params[k].vary]
+    else:
+        return [k for k in params]
+
 
 class Model(object):
     """
     pylag.model.Model
 
     Base class for deriving models that can be fit to data. Models are defined as a class that inhertis from this class.
     The model class contains definitions of all the model parameters, and the means to evaluate the model for some set
@@ -57,27 +66,39 @@
     def __init__(self, component_name=None, **kwargs):
         self.prefix = component_name + "_" if component_name is not None else ''
         self.params = self.get_params(**kwargs)
 
     def get_params(self):
         raise AssertionError("I should be overridden!")
 
+    def get_param_names(self, par=None, variable_only=False):
+        if par is None:
+            par = self.get_params()
+        if variable_only:
+            return [k for k in par if par[k].vary]
+        else:
+            return [k for k in par]
+
     def eval(self, params, x):
         raise AssertionError("I should be overriden")
 
     def eval_gradient(self, params, x):
         raise AssertionError("I should be overriden")
 
     def __call__(self, *args):
         return self.eval(*args)
 
 
 class AdditiveModel(Model):
     def __init__(self, components):
-        self.components = [c(component_name='add%0d'%n) for n, c in enumerate(components)]
+        self.component_names = [c.__name__ for c in components]
+        for i in range(len(self.component_names)):
+            if self.component_names[i] in self.component_names[:i]:
+                self.component_names[i] += '_%0d' % i
+        self.components = [c(component_name=n) for c, n in zip(components, self.component_names)]
 
     def get_params(self):
         params = lmfit.Parameters()
         for c in self.components:
             params = params + c.get_params()
         return params
 
@@ -141,21 +162,21 @@
         norm = np.exp(params['%snorm' % self.prefix].value)
         slope = params['%sslope' % self.prefix].value
 
         return np.stack([norm * x**slope, norm * x**slope * np.log(x)], axis=-1)
 
 
 class BendingPowerLaw(Model):
-    def get_params(self, norm=1., slope=1.):
+    def get_params(self, norm=1., slope1=0., fbend=-5., slope2=-2.):
         params = lmfit.Parameters()
 
         params.add('%snorm' % self.prefix, value=norm, min=-50, max=50)
-        params.add('%sslope1' % self.prefix, value=slope, min=-10, max=10)
-        params.add('%sfbend' % self.prefix, value=slope, min=-6, max=-2)
-        params.add('%sslope2' % self.prefix, value=slope, min=-10, max=10)
+        params.add('%sslope1' % self.prefix, value=slope1, min=-2, max=-0)
+        params.add('%sfbend' % self.prefix, value=fbend, min=-6, max=-2)
+        params.add('%sslope2' % self.prefix, value=slope2, min=-10, max=0)
 
         return params
 
     def eval(self, params, x):
         norm = np.exp(params['%snorm' % self.prefix].value)
         slope1 = params['%sslope1' % self.prefix].value
         fbend = 10. ** params['%sfbend' % self.prefix].value
@@ -181,34 +202,34 @@
 
 class Lorentzian(Model):
     def get_params(self, norm=1., centre=-4, width=1e-3):
         params = lmfit.Parameters()
 
         params.add('%snorm' % self.prefix, value=norm, min=-50, max=50)
         params.add('%scentre' % self.prefix, value=centre, min=-6, max=-2)
-        params.add('%swidth' % self.prefix, value=width, min=1e-6, max=100)
+        params.add('%swidth' % self.prefix, value=width, min=-10, max=-3)
 
         return params
 
     def eval(self, params, x):
         norm = np.exp(params['%snorm' % self.prefix].value)
         centre = 10. ** params['%scentre' % self.prefix].value
-        width = params['%swidth' % self.prefix].value
+        width = 10. ** params['%swidth' % self.prefix].value
 
         return norm * (1./np.pi) * 0.5 * width / ((x - centre)**2 + 0.25*width**2)
 
     def eval_gradient(self, params, x):
         norm = np.exp(params['%snorm' % self.prefix].value)
         centre = 10. ** params['%scentre' % self.prefix].value
-        width = params['%swidth' % self.prefix].value
+        width = 10. ** params['%swidth' % self.prefix].value
 
         return np.stack([norm * (1. / np.pi) * 0.5 * width / ((x - centre) ** 2 + 0.25 * width ** 2),
                          centre * np.log(10) * (norm * width / np.pi) * (x - centre) / (
                                      (x - centre) ** 2 + 0.25 * width ** 2) ** 2,
-                         norm * (1. / (2. * np.pi)) * (((x - centre) ** 2 + 0.25 * width ** 2) - width ** 2) / (
+                         width * np.log(10) * norm * (1. / (2. * np.pi)) * (((x - centre) ** 2 + 0.25 * width ** 2) - width ** 2) / (
                                      (x - centre) ** 2 + 0.25 * width ** 2) ** 2
                          ], axis=-1)
 
 
 class Constant(Model):
     def get_params(self, slope=1., intercept=0.):
         params = lmfit.Parameters()
@@ -220,7 +241,26 @@
     def eval(self, params, x):
         constant = params['%sconstant' % self.prefix].value
 
         return constant * np.ones_like(x)
 
     def eval_gradient(self, params, x):
         return np.ones_like(x)[:, np.newaxis]   # add a dimension to match the shape of gradients from other models
+
+
+class LogConstant(Model):
+    def get_params(self, slope=1., intercept=0.):
+        params = lmfit.Parameters()
+
+        params.add('%slgconstant' % self.prefix, value=slope, min=-10, max=10)
+
+        return params
+
+    def eval(self, params, x):
+        constant = 10. ** params['%slgconstant' % self.prefix].value
+
+        return constant * np.ones_like(x)
+
+    def eval_gradient(self, params, x):
+        constant = 10. ** params['%slgconstant' % self.prefix].value
+
+        return constant * np.log(10) * np.ones_like(x)[:, np.newaxis]   # add a dimension to match the shape of gradients from other models
```

### Comparing `pylag-2.1/pylag/periodogram.py` & `pylag-2.2/pylag/periodogram.py`

 * *Files 11% similar despite different names*

```diff
@@ -71,14 +71,19 @@
         if lc is not None:
             if not isinstance(lc, LightCurve):
                 raise ValueError(
                     "pyLag CrossSpectrum ERROR: Can only compute cross spectrum between two LightCurve objects")
 
             self.freq, self.periodogram = self.calculate(lc, norm, **kwargs)
 
+            # capture some useful statistics about the light curve
+            self.lcmean = lc.rate.mean()
+            self.dt = lc.dt
+            self.Nt = lc.length
+
         else:
             self.freq = np.array(f)
             self.periodogram = np.array(per)
 
         # these will only be set once the periodogram is binned
         self.freq_error = ferr
         self.error = err
@@ -215,14 +220,56 @@
         per_avg : float
                   The average value of the periodogram over the frequency range
         """
         bin_edges = [fmin, fmax]
         per_mean, _, _ = binned_statistic(self.freq, self.periodogram, statistic='mean', bins=bin_edges)
         return per_mean[0]
 
+    def num_freq_in_bins(self, bins):
+        """
+        numfreq = pylag.Periodogram.num_freq_in_bins(bins)
+
+        Returns the number of sample frequencies that fall into bins specified
+        in a pyLag Binning object
+
+        Arguments
+        ---------
+        bins : Binning
+               pyLag Binning object defining the bins into which sample frequencies
+               are to be counted
+
+        Returns
+        -------
+        numfreq : ndarray
+                  The number of frequencies falling into each bin
+        """
+        return bins.num_points_in_bins(self.freq)
+
+    def num_freq_in_range(self, fmin, fmax):
+        """
+        num_freq = pylag.Periodogram.num_freq_in_range(fmin, fmax)
+
+        Return the number of FFT frequency points that fall in a specified frequency
+        interval.
+
+        Arguments
+        ---------
+        fmin : float
+               Lower bound of frequency range
+        fmax : float
+               Upper bound of frequency range
+
+        Returns
+        -------
+        num_freq : int
+                   Number of frequency points in ranhe
+
+        """
+        return np.sum(np.logical_and(self.freq>=fmin, self.freq<fmax))
+
     def points_in_freqrange(self, fmin, fmax):
         """
         range_points = pylag.Periodogram.points_in_freqrange(fmin, fmax)
 
         Return the list of periodogram points that fall in a specified frequency
         interval.
 
@@ -237,14 +284,44 @@
         -------
         range_points : list
                        List of periodogram points (complex) in the frequency range
 
         """
         return [p for f, p in zip(self.freq, self.periodogram) if fmin <= f < fmax]
 
+    def moving_average(self, window_size):
+        """
+        per_avg = pylag.Periodogram.moving_average(window_size)
+
+        Calculate the moving average of the periodogram across frequency bins.
+        The error at each frequency is the standard deviation of the periodogram points that went into the bin
+
+        Arguments
+        ---------
+        window_size : int
+                      number of points in moving average
+
+        Returns
+        -------
+        per_avg : Periodogram
+                  pyLag Periodogram object storing the moving average periodogram
+
+        """
+        window = np.ones(int(window_size)) / float(window_size)
+        per_mean = np.convolve(self.periodogram, window, 'same')
+        per_meansq = np.convolve(self.periodogram**2, window, 'same')
+        per_std = np.sqrt(per_meansq - per_mean**2)
+        return Periodogram(f=self.freq, per=per_mean, err=per_std, ferr=self.freq_error)
+
+    def noise_level(self, bkg=0.):
+        """
+        Calculate the theoretical Poisson noise level from the light curve
+        """
+        return 2.*(self.lcmean + bkg) / self.lcmean**2
+
     def _getplotdata(self):
         return (self.freq, self.freq_error), (self.periodogram, self.error)
 
     def _getplotaxes(self):
         return 'Frequency / Hz', 'log', 'Periodogram', 'log'
 
 
@@ -382,41 +459,46 @@
         if calc_error:
             error = self.bins.std_error(freq_list, per_list)
         else:
             error = None
 
         return self.bins.bin(freq_list, per_list), error
 
-    def freq_average_slow(self, fmin, fmax):
+    def bin(self, bins, calc_error=True):
         """
-        per_avg = pylag.StackedPeriodogram.freq_average(fmin, fmax)
+        per, err = pylag.StackedPeriodogram.calculate_binned()
 
-        calculate the average value of the periodogram over a specified
-        frequency interval. The final periodogram is the average over all of
-        the individual frequency points from all of the light curves that fall
-        into the range.
+        Calculates the average periodogram in each frequency bin. The final
+        periodogram in each bin is the average over all of the individual
+        frequency points from all of the light curves that fall into that bin.
 
         Arguments
         ---------
-        fmin : float
-               Lower bound of frequency range
-        fmax : float
-               Upper bound of frequency range
+        bins : Binning
+               Binning object describing the bins into which the stacked periodograms
+               are to be averaged
 
         Returns
         -------
-        per_avg : complex
-                  The average value of the cross spectrum over the frequency range
-
+        per : Peridogram
+              The binned periodogram
+        err : ndarray
+              The standard error of the periodogram in each bin
         """
-        per_points = []
-        for per in self.periodograms:
-            per_points += per.points_in_freqrange(fmin, fmax)
+        freq_list = np.hstack([p.freq for p in self.periodograms])
+        per_list = np.hstack([p.periodogram for p in self.periodograms])
+
+        per_bin = bins.bin(freq_list, per_list)
+
+        if calc_error:
+            error = bins.std_error(freq_list, per_list)
+        else:
+            error = None
 
-        return np.mean(per_points)
+        return Periodogram(f=bins.bin_cent, per=per_bin, err=error, ferr=bins.x_error())
 
     def freq_average(self, fmin, fmax):
         """
         per_avg = pylag.StackedPeriodogram.freq_average(fmin, fmax)
 
         calculate the average value of the periodogram over a specified
         frequency interval. The final periodogram is the average over all of
@@ -438,7 +520,50 @@
         """
         freq_list = np.hstack([p.freq for p in self.periodograms])
         per_list = np.hstack([p.periodogram for p in self.periodograms])
 
         bin_edges = [fmin, fmax]
         per_mean, _, _ = binned_statistic(freq_list, per_list, statistic='mean', bins=bin_edges)
         return per_mean[0]
+
+    def num_freq_in_range(self, fmin, fmax):
+        """
+        num_freq = pylag.Periodogram.num_freq_in_range(fmin, fmax)
+
+        Return the number of FFT frequency points that fall in a specified frequency
+        interval.
+
+        Arguments
+        ---------
+        fmin : float
+               Lower bound of frequency range
+        fmax : float
+               Upper bound of frequency range
+
+        Returns
+        -------
+        num_freq : int
+                   Number of frequency points in ranhe
+
+        """
+        return np.sum([np.sum(np.logical_and(p.freq>=fmin, p.freq<fmax)) for p in self.periodograms])
+
+    def num_freq_in_bins(self, bins):
+        """
+        num_freq = pylag.Periodogram.num_freq_in_range(fmin, fmax)
+
+        Return the number of FFT frequency points that fall in specified bins.
+
+        Arguments
+        ---------
+        fmin : float
+               Lower bound of frequency range
+        fmax : float
+               Upper bound of frequency range
+
+        Returns
+        -------
+        num_freq : int
+                   Number of frequency points in ranhe
+
+        """
+        return np.sum(np.vstack([p.num_freq_in_bins(bins) for p in self.periodograms]), axis=0)
```

### Comparing `pylag-2.1/pylag/plotter.py` & `pylag-2.2/pylag/plotter.py`

 * *Files 17% similar despite different names*

```diff
@@ -90,20 +90,20 @@
     legend        : boolean
                     If True, a legend is shown on the plot. By default, set
                     to True if series labels are provided
     legend_loc    : string (default='upper right')
                     The matplotlib string specifying the location the legend
                     should be placed ('best', 'upper right', 'center right',
                     'lower left' etc.)
-    colour_series : list of strings (default=['k', 'b', 'g', 'r', 'c', 'm'])
+    colours       : list of strings (default=['k', 'b', 'g', 'r', 'c', 'm'])
                     The repeating sequence of matplotlib colour specifiers
                     setting the order in which colours are assigned to plot
                     series. The sequence is repeated as many times as necessary
                     to cover all the series
-    marker_series : list of strings (default=['+', 'x', 'o', 's'])
+    markers       : list of strings (default=['+', 'x', 'o', 's'])
                     The repeating sequence of matplotlib plot marker specifiers
                     setting the order in which they are applied to data series.
                     To plot all series as lines, use a single entry ['-']
     font_face     : string (default=None)
                     Specify the font face. If None, use the matplotlub default
     font_size     : integer (default=None)
                     Specify the font size. If None, use the matplotlub default
@@ -148,19 +148,22 @@
     show_plot     : boolean, optional (default=True)
                     display the plot window on screen automatically when the plot
                     is created or updated. If False, the plot can be displayed
                     by calling the show method()
     """
 
     def __init__(self, data_object=None, xdata=None, ydata=None, xscale='', yscale='', xlabel='',
-                 ylabel='', title='', series_labels=[], grid='minor', lines=False, marker_series=None, colour_series=None,
-                 errorbar=True, preset=None, figsize=None, show_plot=True):
+                 ylabel='', title='', series_labels=[], grid='minor', lines=False, markers=None, colours=None,
+                 errorbar=True, preset=None, figsize=None, show_plot=True, nested=False, parent=None):
         self._fig = None
         self._ax = None
 
+        self.nested = nested
+        self.parent = parent
+
         self._labels = list(series_labels)
 
         self._xlabel = ''
         self._ylabel = ''
 
         self._title = title
 
@@ -171,36 +174,38 @@
         self._ytickformat = None
 
         self.errorbar = errorbar
 
         self._figsize = figsize
 
         # variables to set plot formatting
-        if colour_series is not None:
-            self._colour_series = colour_series
+        if colours is not None:
+            self._colour_series = colours
         else:
             self._colour_series = ['k', 'tab:blue', 'tab:orange', 'tab:green', 'tab:red', 'tab:purple']
 
-        if marker_series is not None:
-            self._marker_series = marker_series
+        if markers is not None:
+            self._marker_series = markers
+        elif lines == 'step':
+            self._marker_series = ['step']
         elif lines:
             self._marker_series = ['-']
         else:
             self._marker_series = ['+', 'x', 'o', 's']
 
         self._font_face = None
         self._font_size = None
         self._tick_scale = 0.88
         self._grid = grid
         self._legend_location = 'upper right'
         self._xlim = None
         self._ylim = None
 
         # do we display the plot on screen automatically when calling plot()?
-        self.show_plot = show_plot
+        self.show_plot = show_plot and not self.nested
 
         self._legend = (len(self._labels) > 0)
 
         if data_object is not None:
             self.xdata = []
             self.xerror = []
             self.ydata = []
@@ -276,30 +281,32 @@
             self._ylabel = ylabel
         # if we're passed axis log/linear scaling, these override the scaling set in data_object
         if xscale != '':
             self._xscale = xscale
         if yscale != '':
             self._yscale = yscale
 
-        self.plot()
-        all_plots.append(self)
+        if not self.nested:
+            self.plot()
+            all_plots.append(self)
 
     def _setup_axes(self):
         """
         pylag.plot._setup_axes()
 
         close and recreate the figure and axes, applying the updated settings.
         This function is called automatically by plot()
         """
-        # close the old figure (if already plotted)
-        if self._fig is not None:
-            self.close()
+        if not self.nested:
+            # close the old figure (if already plotted)
+            if self._fig is not None:
+                self.close()
 
-        # create a new figure window and axes
-        self._fig, self._ax = plt.subplots(figsize=self._figsize)
+            # create a new figure window and axes
+            self._fig, self._ax = plt.subplots(figsize=self._figsize)
 
         # set log or linear scaling
         self._ax.set_xscale(self._xscale)
         self._ax.set_yscale(self._yscale)
 
         # set axis labels
         self._ax.set_xlabel(self._xlabel)
@@ -342,17 +349,61 @@
         # plot the data series in turn
         for xd, yd, yerr, xerr, marker, colour, label in zip(self.xdata, self.ydata, self.yerror, self.xerror, markers,
                                                              colours, self._labels):
             if not isinstance(xerr, (np.ndarray, list)):
                 xerr = np.zeros(len(xd))
             if not isinstance(yerr, (np.ndarray, list)):
                 yerr = np.zeros(len(yd))
-            if self.errorbar:
+
+            if marker == 'stair':
+                edges = np.concatenate([xd[np.isfinite(yd)] - xerr[np.isfinite(yd)], [xd[np.isfinite(yd)][-1] + xerr[np.isfinite(yd)][-1]]])
+                self._ax.stairs(yd[np.isfinite(yd)], edges, color=colour, label=label)
+
+            elif marker == 'step':
+                self._ax.step(xd[np.isfinite(yd)], yd[np.isfinite(yd)], where='mid', color=colour, label=label)
+
+            elif marker == 'region':
+                if xerr is not None:
+                    # if we're including the x error points, we need to put in the co-ordinates for the left
+                    # and right hand sides of each error box
+                    high_bound = []
+                    low_bound = []
+                    xpoints = []
+                    if yerr.ndim == 1:
+                        for x, y, xe, ye in zip(xd, yd, xerr, yerr):
+                            high_bound.append(y + ye)
+                            high_bound.append(y + ye)
+                            low_bound.append(y - ye)
+                            low_bound.append(y - ye)
+                            xpoints.append(x - xe)
+                            xpoints.append(x + xe)
+                    else:
+                        for x, y, xe, yem, yep in zip(xd, yd, xerr, yerr[0,:], yerr[1,:]):
+                            high_bound.append(y + yep)
+                            high_bound.append(y + yep)
+                            low_bound.append(y - yem)
+                            low_bound.append(y - yem)
+                            xpoints.append(x - xe)
+                            xpoints.append(x + xe)
+                    self._ax.plot(xd, yd, '-', color=colour, label=label)
+                    self._ax.fill_between(xpoints, low_bound, high_bound, facecolor=colour, alpha=0.5)
+                else:
+                    if yerr.ndim == 1:
+                        high_bound = np.array(yd) + np.array(yerr)
+                        low_bound = np.array(yd) - np.array(yerr)
+                    else:
+                        high_bound = np.array(yd) + np.array(yerr[1,:])
+                        low_bound = np.array(yd) - np.array(yerr[0,:])
+                    self._ax.plot(xd, yd, '-', color=colour, label=label)
+                    self._ax.fill_between(xd, low_bound, high_bound, facecolor=colour, alpha=0.5)
+
+            elif self.errorbar:
                 self._ax.errorbar(xd[np.isfinite(yd)], yd[np.isfinite(yd)], yerr=yerr[np.isfinite(yd)] if yerr.ndim==1 else np.vstack([ye[np.isfinite(yd)] for ye in yerr]),
                               xerr=xerr[np.isfinite(yd)], fmt=marker, color=colour, label=label)
+
             else:
                 if marker != '-':
                     mk = marker
                 else:
                     mk = None
                 self._ax.plot(xd[np.isfinite(yd)], yd[np.isfinite(yd)], marker=mk, color=colour, label=label)
 
@@ -370,15 +421,15 @@
 
     def show(self, **kwargs):
         """
         pylag.plot.show()
 
         show the plot window on the screen
         """
-        if 'inline' not in matplotlib.get_backend():
+        if not self.nested and 'inline' not in matplotlib.get_backend() and 'ipympl' not in matplotlib.get_backend():
             self._fig.show(**kwargs)
 
     def plot(self, **kwargs):
         """
         pylag.plot.plot()
 
         Wrapper function to perform all steps necessary to create/update the plot.
@@ -395,15 +446,16 @@
             self._set_fonts()
         if self.legend:
             if self._font_face is not None:
                 font_prop = font_manager.FontProperties(family=self._font_face, size=self._font_size)
             else:
                 font_prop = None
             self._ax.legend(loc=self._legend_location, prop=font_prop)
-        self._fig.tight_layout()
+        if not self.nested:
+            self._fig.tight_layout()
         if self.show_plot:
             self.show()
 
     def close(self):
         """
         pylag.plot.show()
 
@@ -450,15 +502,18 @@
         -------
         setter : function
                  The setter function
         """
 
         def setter(self, value):
             setattr(self, attr, value)
-            self.plot()
+            if not self.nested:
+                self.plot()
+            else:
+                self.parent.plot()
 
         return setter
 
     def _get_getter(attr):
         """
         getter = pylag.plot._get_getter(attr)
 
@@ -1236,7 +1291,176 @@
         else:
             return self.bins.bin_cent, self.hist
 
     def _getplotaxes(self):
         return self.xlabel, self.xscale, self.ylabel, self.yscale
 
 
+class MultiPlot(Plot):
+    def __init__(self, data_objects=[], title='', series_labels=None, grid='minor', lines=False, marker_series=None, colour_series=None,
+                 preset=None, figsize=None, show_plot=True, dim=None, cols=False, sharex=True, sharey=False, wspace=0.05, hspace=0.05, wratio=None, hratio=None, pargs=None):
+        self._fig = None
+        self._ax = None
+
+        self._figsize = figsize
+
+        # variables to set plot formatting
+        if colour_series is not None:
+            self._colour_series = colour_series
+        else:
+            self._colour_series = ['k', 'tab:blue', 'tab:orange', 'tab:green', 'tab:red', 'tab:purple']
+
+        if marker_series is not None:
+            self._marker_series = marker_series
+        elif lines:
+            self._marker_series = ['-']
+        else:
+            self._marker_series = ['+', 'x', 'o', 's']
+
+        self._font_face = None
+        self._font_size = None
+        self._tick_scale = 0.88
+        self._grid = grid
+        self._legend_location = 'upper right'
+        self._xlim = None
+        self._ylim = None
+
+        # do we display the plot on screen automatically when calling plot()?
+        self.show_plot = show_plot
+
+        self.data_objects = data_objects
+        self.series_labels = series_labels if series_labels is not None else [[]]*len(self.data_objects)
+        plot_kwargs = pargs if pargs is not None else [{}]*len(self.data_objects)
+        self.plots = [Plot(d, series_labels=l, nested=True, parent=self, **k) for d, l, k in zip(self.data_objects, self.series_labels, plot_kwargs)]
+
+        if dim is not None:
+            self.dim = dim
+        elif cols:
+            self.dim = (1, len(self.data_objects))
+        else:
+            self.dim = (len(self.data_objects), 1)
+
+        self.sharex = sharex
+        self.sharey = sharey
+        self.wspace = wspace
+        self.hspace = hspace
+
+        self.gridspec = {}
+        if wratio is not None:
+            self.gridspec['width_ratios'] = wratio
+        if hratio is not None:
+            self.gridspec['height_ratios'] = hratio
+
+        if sharex:
+            for p in self.plots[:-1]:
+                p.xlabel = None
+
+        if sharey:
+            for p in self.plots[:-1]:
+                p.ylabel = None
+
+        self.plot()
+        all_plots.append(self)
+
+
+    def plot(self):
+        if self._fig is not None:
+            self.close()
+
+        self._fig, self._ax = plt.subplots(self.dim[0], self.dim[1], figsize=self.figsize, sharex=self.sharex, sharey=self.sharey, gridspec_kw=self.gridspec)
+        plt.subplots_adjust(left=0.1, bottom=0.1, right=0.95, top=0.95, wspace=self.wspace, hspace=self.hspace)
+        if len(self._ax.shape) == 1:
+            for n, p in enumerate(self.plots):
+                p._ax = self._ax[n]
+        else:
+            for n, p in enumerate(self.plots):
+                p._ax = self._ax[n//self.dim[0]][n % self.dim[0]]
+        for p in self.plots:
+            p.plot()
+
+    def paper_format(self):
+        self._font_face = 'Liberation Serif'
+        self._font_size = 18
+        self._tick_scale = 0.88
+        for p in self.plots:
+            p._font_face = self._font_face
+            p._font_size = self._font_size
+            p._tick_scale = self._tick_scale
+        self.plot()
+
+    def _get_getter(attr):
+        """
+        getter = pylag.plot._get_getter(attr)
+
+        Returns a getter function for plot attribute attr.
+
+        A re-usable getter functions for all properties
+
+        Note this needs to be re-implemented here for the attributes defined in the derived class.
+
+        Arguments
+        ---------
+        attr : string
+             : The name of the member variable to get
+
+        Returns
+        -------
+        getter : function
+                 The get function
+        """
+
+        def getter(self):
+            return getattr(self, attr)
+
+        return getter
+
+    def _get_multi_setter(attr):
+        """
+        setter = pylag.plot._get_setter(attr)
+
+        Returns a setter function for plot attribute attr which updates the
+        member variable for all of the subplots
+
+        A re-usable setter functions for all properties that need the plot to
+        update
+
+        Arguments
+        ---------
+        attr : string
+             : The name of the member variable to be set
+
+        Returns
+        -------
+        setter : function
+                 The setter function
+        """
+
+        def setter(self, value):
+            setattr(self, attr, value)
+            for p in self.plots:
+                setattr(p, attr, value)
+            self.plot()
+
+        return setter
+
+    labels = property(_get_getter('_labels'), _get_multi_setter('_labels'))
+    xlabel = property(_get_getter('_xlabel'), _get_multi_setter('_xlabel'))
+    ylabel = property(_get_getter('_ylabel'), _get_multi_setter('_ylabel'))
+    xscale = property(_get_getter('_xscale'), _get_multi_setter('_xscale'))
+    yscale = property(_get_getter('_yscale'), _get_multi_setter('_yscale'))
+    xlim = property(_get_getter('_xlim'), _get_multi_setter('_xlim'))
+    ylim = property(_get_getter('_ylim'), _get_multi_setter('_ylim'))
+    grid = property(_get_getter('_grid'), _get_multi_setter('_grid'))
+    legend = property(_get_getter('_legend'), _get_multi_setter('_legend'))
+    legend_location = property(_get_getter('_legend_location'), _get_multi_setter('_legend_location'))
+    colour_series = property(_get_getter('_colour_series'), _get_multi_setter('_colour_series'))
+    marker_series = property(_get_getter('_marker_series'), _get_multi_setter('_marker_series'))
+    font_face = property(_get_getter('_font_face'), _get_multi_setter('_font_face'))
+    font_size = property(_get_getter('_font_size'), _get_multi_setter('_font_size'))
+    tick_scale = property(_get_getter('_tick_scale'), _get_multi_setter('_tick_scale'))
+    xtickformat = property(_get_getter('_xtickformat'), _get_multi_setter('_xtickformat'))
+    ytickformat = property(_get_getter('_ytickformat'), _get_multi_setter('_ytickformat'))
+
+    def __getitem__(self, item):
+        return self.plots[item]
+
+
```

### Comparing `pylag-2.1/pylag/response.py` & `pylag-2.2/pylag/response.py`

 * *Files identical despite different names*

### Comparing `pylag-2.1/pylag/simulator.py` & `pylag-2.2/pylag/simulator.py`

 * *Files identical despite different names*

### Comparing `pylag-2.1/pylag/time.py` & `pylag-2.2/pylag/time.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,7 +25,19 @@
     """
     name = "nustarsec"
     unit = 1.0 / erfa.DAYSEC  # in days (1 day == 86400 seconds)
     epoch_val = "2010-01-01 00:00:00"
     epoch_val2 = None
     epoch_scale = "tt"
     epoch_format = "iso"
+
+
+class TimeNicerSec(astropy.time.TimeFromEpoch):
+    """
+    NuSTAR seconds from 2010-01-01 00:00:00 TT.
+    """
+    name = "nicersec"
+    unit = 1.0 / erfa.DAYSEC  # in days (1 day == 86400 seconds)
+    epoch_val = "2014-01-01 00:00:00"
+    epoch_val2 = None
+    epoch_scale = "tt"
+    epoch_format = "iso"
```

### Comparing `pylag-2.1/pylag.egg-info/SOURCES.txt` & `pylag-2.2/pylag.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-.gitignore
 LICENSE.md
 README.md
-changelog.md
 setup.cfg
 setup.py
 pylag/__init__.py
 pylag/absorber.py
 pylag/binning.py
 pylag/bispectrum.py
 pylag/cepstrum.py
@@ -31,14 +29,15 @@
 pylag/mlcovariance.py
 pylag/mlfit.py
 pylag/model.py
 pylag/periodogram.py
 pylag/plotter.py
 pylag/response.py
 pylag/reverb_model.py
+pylag/rms.py
 pylag/simulator.py
 pylag/time.py
 pylag/util.py
 pylag.egg-info/PKG-INFO
 pylag.egg-info/SOURCES.txt
 pylag.egg-info/dependency_links.txt
 pylag.egg-info/requires.txt
```

