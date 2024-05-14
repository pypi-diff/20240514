# Comparing `tmp/pandorapsf-0.2.7.tar.gz` & `tmp/pandorapsf-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandorapsf-0.2.7.tar", max compression
+gzip compressed data, was "pandorapsf-0.2.8.tar", max compression
```

## Comparing `pandorapsf-0.2.7.tar` & `pandorapsf-0.2.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1071 2023-09-22 21:06:08.416872 pandorapsf-0.2.7/LICENSE
--rw-r--r--   0        0        0       15 2023-09-21 17:07:25.661702 pandorapsf-0.2.7/README.md
--rw-r--r--   0        0        0      363 2024-05-09 17:18:16.649829 pandorapsf-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     1734 2024-05-09 17:18:08.933079 pandorapsf-0.2.7/src/pandorapsf/__init__.py
--rw-r--r--   0        0        0    14579 2023-10-11 00:00:22.516507 pandorapsf-0.2.7/src/pandorapsf/data/dichroic-transmission.csv
--rw-r--r--   0        0        0   100800 2024-05-03 14:35:17.450737 pandorapsf-0.2.7/src/pandorapsf/data/nirda-wav-solution.fits
--rw-r--r--   0        0        0     2777 2023-09-21 16:57:33.816212 pandorapsf-0.2.7/src/pandorapsf/data/pandora.mplstyle
--rw-r--r--   0        0        0     6452 2023-10-10 23:55:05.530892 pandorapsf-0.2.7/src/pandorapsf/data/pandora_visible_qe.csv
--rw-r--r--   0        0        0    25577 2023-09-22 16:23:38.985186 pandorapsf-0.2.7/src/pandorapsf/data/pixel_vs_wavelength.csv
--rw-r--r--   0        0        0    14400 2024-05-03 14:35:17.463147 pandorapsf-0.2.7/src/pandorapsf/data/visda-wav-solution.fits
--rw-r--r--   0        0        0     7461 2024-05-08 14:32:10.310103 pandorapsf-0.2.7/src/pandorapsf/plotting.py
--rw-r--r--   0        0        0    29360 2024-05-09 15:29:04.711409 pandorapsf-0.2.7/src/pandorapsf/psf.py
--rw-r--r--   0        0        0    30154 2024-05-08 15:43:00.159415 pandorapsf-0.2.7/src/pandorapsf/scene.py
--rw-r--r--   0        0        0     8506 2024-05-08 19:29:04.935549 pandorapsf-0.2.7/src/pandorapsf/sparsewarp.py
--rw-r--r--   0        0        0    22754 2024-05-08 19:05:42.377580 pandorapsf-0.2.7/src/pandorapsf/utils.py
--rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 pandorapsf-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-09-22 21:06:08.416872 pandorapsf-0.2.8/LICENSE
+-rw-r--r--   0        0        0       15 2023-09-21 17:07:25.661702 pandorapsf-0.2.8/README.md
+-rw-r--r--   0        0        0      363 2024-05-14 16:18:10.298135 pandorapsf-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     1734 2024-05-14 16:18:01.139705 pandorapsf-0.2.8/src/pandorapsf/__init__.py
+-rw-r--r--   0        0        0    14579 2023-10-11 00:00:22.516507 pandorapsf-0.2.8/src/pandorapsf/data/dichroic-transmission.csv
+-rw-r--r--   0        0        0   100800 2024-05-03 14:35:17.450737 pandorapsf-0.2.8/src/pandorapsf/data/nirda-wav-solution.fits
+-rw-r--r--   0        0        0     2777 2023-09-21 16:57:33.816212 pandorapsf-0.2.8/src/pandorapsf/data/pandora.mplstyle
+-rw-r--r--   0        0        0     6452 2023-10-10 23:55:05.530892 pandorapsf-0.2.8/src/pandorapsf/data/pandora_visible_qe.csv
+-rw-r--r--   0        0        0    25577 2023-09-22 16:23:38.985186 pandorapsf-0.2.8/src/pandorapsf/data/pixel_vs_wavelength.csv
+-rw-r--r--   0        0        0    14400 2024-05-03 14:35:17.463147 pandorapsf-0.2.8/src/pandorapsf/data/visda-wav-solution.fits
+-rw-r--r--   0        0        0     7516 2024-05-14 16:17:43.677921 pandorapsf-0.2.8/src/pandorapsf/plotting.py
+-rw-r--r--   0        0        0    27926 2024-05-14 16:11:07.177571 pandorapsf-0.2.8/src/pandorapsf/psf.py
+-rw-r--r--   0        0        0    30154 2024-05-08 15:43:00.159415 pandorapsf-0.2.8/src/pandorapsf/scene.py
+-rw-r--r--   0        0        0     8506 2024-05-08 19:29:04.935549 pandorapsf-0.2.8/src/pandorapsf/sparsewarp.py
+-rw-r--r--   0        0        0    22790 2024-05-14 15:37:42.622494 pandorapsf-0.2.8/src/pandorapsf/utils.py
+-rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 pandorapsf-0.2.8/PKG-INFO
```

### Comparing `pandorapsf-0.2.7/LICENSE` & `pandorapsf-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.7/src/pandorapsf/__init__.py` & `pandorapsf-0.2.8/src/pandorapsf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.7"
+__version__ = "0.2.8"
 # Standard library
 import os  # noqa
 
 PACKAGEDIR = os.path.abspath(os.path.dirname(__file__))
 TESTDIR = "/".join(PACKAGEDIR.split("/")[:-2]) + "/tests/"
 PANDORASTYLE = "{}/data/pandora.mplstyle".format(PACKAGEDIR)
```

### Comparing `pandorapsf-0.2.7/src/pandorapsf/data/dichroic-transmission.csv` & `pandorapsf-0.2.8/src/pandorapsf/data/dichroic-transmission.csv`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.7/src/pandorapsf/data/nirda-wav-solution.fits` & `pandorapsf-0.2.8/src/pandorapsf/data/nirda-wav-solution.fits`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.7/src/pandorapsf/data/pandora.mplstyle` & `pandorapsf-0.2.8/src/pandorapsf/data/pandora.mplstyle`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.7/src/pandorapsf/data/pandora_visible_qe.csv` & `pandorapsf-0.2.8/src/pandorapsf/data/pandora_visible_qe.csv`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.7/src/pandorapsf/data/pixel_vs_wavelength.csv` & `pandorapsf-0.2.8/src/pandorapsf/data/pixel_vs_wavelength.csv`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.7/src/pandorapsf/data/visda-wav-solution.fits` & `pandorapsf-0.2.8/src/pandorapsf/data/visda-wav-solution.fits`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.7/src/pandorapsf/plotting.py` & `pandorapsf-0.2.8/src/pandorapsf/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,21 +89,19 @@
     # ax[n // 2, 0].set(ylabel="Y Pixel")
     # ax[n - 1, n // 2].set(xlabel="X Pixel")
     ax[0, n // 2].set(title=image_type.upper())
     plt.subplots_adjust(hspace=0.051, wspace=0.051)
     return fig
 
 
-def plot_spectral(
-    psf,
-    var="wavelength",
-    n=5,
-    npixels=20,
-    image_type="psf",
-):
+def plot_spectral(psf, var="wavelength", n=5, npixels=20, image_type="psf", **kwargs):
+
+    vmin, vmax = _get_v(kwargs, image_type)
+    cmap = kwargs.pop("cmap", "viridis")
+
     wavs = np.linspace(
         getattr(psf, var + "1d").min(), getattr(psf, var + "1d").max(), n
     )
     m = npixels // 2
     fig, ax = plt.subplots(
         1,
         n,
@@ -131,16 +129,17 @@
             y, x, f = psf.prf(
                 row=kwargs.pop("row", 0), column=kwargs.pop("column", 0), **kwargs
             )
         im = ax[ndx].pcolormesh(
             x,
             y,
             f,
-            vmin=0,
-            vmax=[0.1 if image_type.lower() == "prf" else 0.01][0],
+            vmin=vmin,
+            vmax=vmax,
+            cmap=cmap,
         )
         ax[ndx].set(
             xlim=(-m, m),
             ylim=(-m, m),
             xticks=np.arange(-(m - 1), m, 2),
             yticks=np.arange(-(m - 1), m, 2),
             title=f"{wavs[ndx]:0.2} $\mu$m",
```

### Comparing `pandorapsf-0.2.7/src/pandorapsf/psf.py` & `pandorapsf-0.2.8/src/pandorapsf/psf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Defines the PSF class"""
 
 # Standard library
-import os
 from typing import Dict, List, Union
 
 # Third-party
 import astropy.units as u
-import matplotlib.pyplot as plt
 import numpy as np
 import numpy.typing as npt
+import pandorasat as ps
 from astropy.io import fits
 from pandorasat.utils import get_phoenix_model
 
-from . import PACKAGEDIR, PANDORASTYLE
+from . import PACKAGEDIR
 from .utils import bin_prf
 
 __all__ = ["PSF"]
 
 
 class PSF(object):
     """Class to use PSFs"""
@@ -403,43 +402,14 @@
             freeze_dictionary=kwargs.copy(),
             #            blur_value=self.blur_value,
             extrapolate=self.extrapolate,
             scale=self.scale,
         )
         return psf2
 
-    def plot_sensitivity(self, ax=None):
-        if ax is None:
-            _, ax = plt.subplots()
-        with plt.style.context(PANDORASTYLE):
-            ax.plot(self.trace_wavelength.value, self.trace_sensitivity.value, c="k")
-            ax.set(
-                xticks=np.linspace(*ax.get_xlim(), 9),
-                xlabel=f"Wavelength [{self.trace_wavelength.unit.to_string('latex')}]",
-                ylabel=f"Sensitivity [{self.trace_sensitivity.unit.to_string('latex')}]",
-                title=self.name.upper(),
-            )
-            ax.spines[["right", "top"]].set_visible(True)
-            if (self.trace_pixel.value != 0).any():
-                ax_p = ax.twiny()
-                ax_p.set(xticks=ax.get_xticks(), xlim=ax.get_xlim())
-                ax_p.set_xlabel(xlabel="$\delta$ Pixel Position", color="grey")
-                ax_p.set_xticklabels(
-                    labels=list(
-                        np.interp(
-                            ax.get_xticks(),
-                            self.trace_wavelength.value,
-                            self.trace_pixel.value,
-                        ).astype(int)
-                    ),
-                    rotation=45,
-                    color="grey",
-                )
-        return ax
-
     def __repr__(self):
         freeze_dictionary = (
             f" (Frozen: {', '.join([f'{key}: {item:.3f}' for key, item in self.freeze_dictionary.items()])})"
             if len(self.freeze_dictionary) != 0
             else ""
         )
         return f"{self.ndims}D PSF Model [{', '.join(self.dimension_names)}]{freeze_dictionary}"
@@ -493,23 +463,24 @@
             #            p.blur_value = blur_value
             #            p._blur(blur_value=p.blur_value)
             return p
         else:
             raise ValueError(f"No such PSF as `{name}`")
 
     def _add_trace_params(self):
-        fname = f"{PACKAGEDIR}/data/{self.name.lower()}-wav-solution.fits"
-        if not os.path.isfile(fname):
-            raise ValueError(f"No wavelength solutions for `{self.name}`.")
-        hdu = fits.open(fname)
-        for idx in np.arange(1, hdu[1].header["TFIELDS"] + 1):
-            name, unit = hdu[1].header[f"TTYPE{idx}"], hdu[1].header[f"TUNIT{idx}"]
-            setattr(self, f"_trace_{name}", hdu[1].data[name] * u.Quantity(1, unit))
-        self._trace_sensitivity *= hdu[1].header["SENSCORR"] * u.Quantity(
-            1, hdu[1].header["CORRUNIT"]
+        if self.name == "visda":
+            detector = ps.VisibleDetector()
+        elif self.name == "nirda":
+            detector = ps.NIRDetector()
+        else:
+            raise ValueError(f"Can not parse name {self.name}.")
+        self._trace_sensitivity, self._trace_pixel, self._trace_wavelength = (
+            detector.trace_sensitivity,
+            detector.trace_pixel,
+            detector.trace_wavelength,
         )
 
     @property
     def trace_sensitivity(self):
         if not hasattr(self, "_trace_sensitivity"):
             self._add_trace_params()
         return self._trace_sensitivity
```

### Comparing `pandorapsf-0.2.7/src/pandorapsf/scene.py` & `pandorapsf-0.2.8/src/pandorapsf/scene.py`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.7/src/pandorapsf/sparsewarp.py` & `pandorapsf-0.2.8/src/pandorapsf/sparsewarp.py`

 * *Files identical despite different names*

### Comparing `pandorapsf-0.2.7/src/pandorapsf/utils.py` & `pandorapsf-0.2.8/src/pandorapsf/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,14 +252,15 @@
                     for idx in range(n)
                     for jdx in range(n)
                 ],
                 axis=0,
             )
             * subpixel_row.unit
         )
+        subpixel_size *= downsample
 
     if trim is not None:
         PSF = PSF[trim:-trim, trim:-trim]
         subpixel_column = subpixel_column[trim:-trim, trim:-trim]
         subpixel_row = subpixel_row[trim:-trim, trim:-trim]
 
     return (
```

