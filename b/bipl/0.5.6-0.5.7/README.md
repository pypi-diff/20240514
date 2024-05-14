# Comparing `tmp/bipl-0.5.6.tar.gz` & `tmp/bipl-0.5.7.tar.gz`

## Comparing `bipl-0.5.6.tar` & `bipl-0.5.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/__init__.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/_env.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/py.typed
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/io/__init__.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/io/_dzi.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/io/_gdal.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/io/_libs.py
--rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/io/_openslide.py
--rw-r--r--   0        0        0     9637 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/io/_slide.py
--rw-r--r--   0        0        0     7027 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/io/_slide_bases.py
--rw-r--r--   0        0        0    18547 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/io/_tiff.py
--rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/io/_util.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/ops/__init__.py
--rw-r--r--   0        0        0    15085 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/ops/_mosaic.py
--rw-r--r--   0        0        0     8556 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/ops/_tile.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/ops/_types.py
--rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/ops/_util.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.5.6/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.5.6/LICENSE
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 bipl-0.5.6/README.md
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 bipl-0.5.6/hatch_build.py
--rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 bipl-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     5504 2020-02-02 00:00:00.000000 bipl-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 bipl-0.5.7/src/bipl/__init__.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 bipl-0.5.7/src/bipl/_env.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.5.7/src/bipl/py.typed
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.5.7/src/bipl/io/__init__.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 bipl-0.5.7/src/bipl/io/_dzi.py
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 bipl-0.5.7/src/bipl/io/_gdal.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.5.7/src/bipl/io/_libs.py
+-rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bipl-0.5.7/src/bipl/io/_openslide.py
+-rw-r--r--   0        0        0     9795 2020-02-02 00:00:00.000000 bipl-0.5.7/src/bipl/io/_slide.py
+-rw-r--r--   0        0        0     7317 2020-02-02 00:00:00.000000 bipl-0.5.7/src/bipl/io/_slide_bases.py
+-rw-r--r--   0        0        0    20960 2020-02-02 00:00:00.000000 bipl-0.5.7/src/bipl/io/_tiff.py
+-rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 bipl-0.5.7/src/bipl/io/_util.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 bipl-0.5.7/src/bipl/ops/__init__.py
+-rw-r--r--   0        0        0    15085 2020-02-02 00:00:00.000000 bipl-0.5.7/src/bipl/ops/_mosaic.py
+-rw-r--r--   0        0        0     8556 2020-02-02 00:00:00.000000 bipl-0.5.7/src/bipl/ops/_tile.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 bipl-0.5.7/src/bipl/ops/_types.py
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 bipl-0.5.7/src/bipl/ops/_util.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.5.7/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.5.7/LICENSE
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 bipl-0.5.7/README.md
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 bipl-0.5.7/hatch_build.py
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 bipl-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     6285 2020-02-02 00:00:00.000000 bipl-0.5.7/PKG-INFO
```

### Comparing `bipl-0.5.6/src/bipl/_env.py` & `bipl-0.5.7/src/bipl/_env.py`

 * *Files 24% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     # - Each step effectively filters image with [1 4 6 4 1] window,
     #   keeping 1/4 of pixels.
     # + No aliasing.
     # + Middle-ground in perf.
     # - Shifts image by 1/2 of pixel on each step.
     # TODO: implement [1 3 3 1] filtering
     BIPL_DOWN: Literal['area', 'box', 'gauss'] = 'gauss'  # Downsampling mode
+    BIPL_SUBPIX: bool = False  # Subpixel downsampling
 
     BIPL_TILE_POOL_SIZE: int = 64_000_000  # Min resolution for tiled pooling
     BIPL_ICC: bool = False  # Apply image color correction
     BIPL_CLAHE: bool = False
 
 
 env = Env()
```

### Comparing `bipl-0.5.6/src/bipl/io/__init__.py` & `bipl-0.5.7/src/bipl/io/__init__.py`

 * *Files identical despite different names*

### Comparing `bipl-0.5.6/src/bipl/io/_dzi.py` & `bipl-0.5.7/src/bipl/io/_dzi.py`

 * *Files identical despite different names*

### Comparing `bipl-0.5.6/src/bipl/io/_gdal.py` & `bipl-0.5.7/src/bipl/io/_gdal.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 
 
 # TODO: handle associated images via `base.Image`
 
 
 @dataclass(frozen=True)
 class _Level(ImageLevel):
-    index: int
     g: 'Gdal'
     bands: tuple[gdal.Band, ...]
 
     def crop(self, *loc: slice) -> np.ndarray:
         box, valid_box, shape = self._unpack_2d_loc(*loc)
 
         (y0, y1), (x0, x1) = valid_box.tolist()
@@ -59,15 +58,15 @@
             return np.broadcast_to(self.g.bg_color, (*shape, 3))
 
         h, w = y1 - y0, x1 - x0
         c = self.g.num_channels
         chw = np.empty((c, h, w), 'u1')
 
         with self.g.lock:
-            for b, hw in zip(self.bands, np.split(chw, c, 0)):
+            for b, hw in zip(self.bands, chw[:, None, :, :]):
                 gdal_array.BandReadAsArray(b, x0, y0, w, h, buf_obj=hw)
 
         # TODO: add pad if necessary
         rgb = chw.transpose(1, 2, 0)
         return self._expand(rgb, valid_box, box, self.g.bg_color)
 
 
@@ -108,12 +107,11 @@
         return 1 + self.ds.GetRasterBand(1).GetOverviewCount()
 
     def __getitem__(self, index: int) -> _Level:
         bands: tuple[gdal.Band, ...] = tuple(
             b if index == 0 else b.GetOverview(index - 1) for b in self._bands)
 
         shape = (bands[0].YSize, bands[0].XSize, self.num_channels)
-        mpp = self.mpp if index == 0 else None
-        return _Level(shape, mpp, index, self, bands)
+        return _Level(shape, self, bands)
 
     def keys(self) -> list[str]:
         return []  # TODO: fill if GDAL can detect auxilary images
```

### Comparing `bipl-0.5.6/src/bipl/io/_libs.py` & `bipl-0.5.7/src/bipl/io/_libs.py`

 * *Files identical despite different names*

### Comparing `bipl-0.5.6/src/bipl/io/_openslide.py` & `bipl-0.5.7/src/bipl/io/_openslide.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,32 +241,35 @@
         return None
 
     def __repr__(self) -> str:
         return f'{type(self).__name__}({addressof(self.ptr.contents):0x})'
 
     def _get_metadata(self) -> dict[str, str]:
         names = OSD.openslide_get_property_names(self.ptr)
-        return {
-            name.decode(): value.decode() for name in _ntas_to_iter(names)
-            if (value := OSD.openslide_get_property_value(self.ptr, name))
-        }
+        r = {}
+        for name in _ntas_to_iter(names):
+            if (value := OSD.openslide_get_property_value(self.ptr, name)):
+                try:
+                    r[name.decode()] = value.decode()
+                except UnicodeDecodeError:
+                    continue
+        return r
 
     def __len__(self) -> int:
         return OSD.openslide_get_level_count(self.ptr)
 
     def __getitem__(self, index: int) -> _Level:
         h, w = c_int64(), c_int64()
         OSD.openslide_get_level_dimensions(self.ptr, index, byref(w), byref(h))
         downsample = OSD.openslide_get_level_downsample(self.ptr, index)
         if downsample <= 0:
             raise ValueError(f'Invalid level downsample: {downsample}')
 
-        mpp = self.mpp if index == 0 else None
         downsample = round2(downsample)
-        return _Level((h.value, w.value, 3), mpp, downsample, index, self)
+        return _Level((h.value, w.value, 3), downsample, index, self)
 
     def keys(self) -> list[str]:
         names = OSD.openslide_get_associated_image_names(self.ptr)
         return [name.decode() for name in _ntas_to_iter(names)]
 
     def get(self, key: str) -> _Image:
         name = key.encode()
```

### Comparing `bipl-0.5.6/src/bipl/io/_slide.py` & `bipl-0.5.7/src/bipl/io/_slide.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 __all__ = ['Slide']
 
 import os
 import warnings
 from bisect import bisect_right
 from collections.abc import Callable, Mapping, Sequence
 from dataclasses import dataclass, field, replace
-from math import ceil
 from pathlib import Path
 from typing import final, overload
 from warnings import warn
 
 import numpy as np
 from glow import memoize, shared_call, weak_memoize
 
 from bipl import env
-from bipl.ops import normalize_loc, resize
+from bipl.ops import normalize_loc, rescale_crop
 
 from ._openslide import Openslide
 from ._slide_bases import REGISTRY, Driver, Image, ImageLevel
 from ._tiff import Tiff
 from ._util import clahe, round2
 
 # TODO: inside Slide.open import ._slide.registry,
@@ -43,15 +42,15 @@
         env.BIPL_DRIVERS.discard('gdal')
         os.environ['BIPL_DRIVERS'] = str([*env.BIPL_DRIVERS]).replace("'", '"')
 
 _drv: type[Driver] | None
 for _drv, _regex in [  # LIFO, last driver takes priority
     (Gdal, r'^.*\.(tif|tiff)$'),
     (Openslide, r'^.*\.(bif|mrxs|ndpi|scn|svs|svsslide|tif|tiff|vms|vmu)$'),
-    (Tiff, r'^.*\.(svs|tif|tiff)$'),
+    (Tiff, r'^.*\.(bif|svs|tif|tiff)$'),
     (Gdal, r'^(/vsicurl.*|(http|https|ftp)://.*)$'),
 ]:
     if _drv is not None and _drv.__name__.lower() in env.BIPL_DRIVERS:
         _drv.register(_regex)
 
 
 @shared_call  # merge duplicate calls
@@ -107,34 +106,35 @@
     ) -> 'Slide':
         driver = driver_fn(path)
 
         num_images = len(driver)
         if num_images == 0:
             raise ValueError('Empty file')
 
-        im_0, *images = (driver[idx] for idx in range(num_images))
-        if not isinstance(im_0, ImageLevel):
-            raise TypeError('First pyramid layer is not tiled')
-
         # Retrieve all sub-images
-        levels: dict[int, ImageLevel] = {1: im_0}
+        levels: dict[int, ImageLevel] = {}
         extras: dict[str, Image] = {}
-        for im in images:
-            if isinstance(im, ImageLevel):
-                downsample = round2(im_0.shape[0] / im.shape[0])
-                levels[downsample] = im
-            elif key := im.key:
-                extras[key] = im
+        for idx in range(num_images):
+            match driver[idx]:
+                case ImageLevel(shape=shape) as im:
+                    levels[round2(levels[1].shape[0]
+                                  / shape[0]) if levels else 1] = im
+                case Image(key=str(key)) as im:
+                    extras[key] = im
+                case _:
+                    continue
+
         extras |= driver.named_items()
+        if not levels:
+            raise TypeError('No tiled layers present')
 
         level_downsamples = *sorted(levels.keys()),
-        # TODO: make virtual levels if downsamples are too distant (ProxyLevel)
 
         if mpp is None:  # If no override is passed, use native if present
-            mpp = levels[1].mpp
+            mpp = driver.mpp
 
         return Slide(
             path=path,
             shape=levels[1].shape,
             mpp=mpp,
             downsamples=level_downsamples,
             driver=type(driver).__name__,
@@ -200,15 +200,22 @@
         /,
         *,
         tol: float = 0.01,
     ) -> tuple[int, ImageLevel]:
         """Gives the most detailed LOD below `downsample`"""
         downsample = downsample * max(1, 1 + tol)
         idx = max(bisect_right(self.downsamples, downsample) - 1, 0)
-        return self.downsamples[idx], self.levels[idx]
+        ds = self.downsamples[idx]
+        lv = self.levels[idx]
+
+        # Make octave level as close as possible to target
+        while (ds_ := ds * 2) < downsample and (lv_ := lv.octave()):
+            ds, lv = ds_, lv_
+
+        return ds, lv
 
     def resample(self, mpp: float, *, tol: float = 0.01) -> ImageLevel:
         """Resample slide to specific resolution"""
         downsample = mpp / self.mpp_or_error()
         return self.pool(downsample, tol=tol)
 
     def pool(self, downsample: float, /, *, tol: float = 0.01) -> ImageLevel:
@@ -262,18 +269,18 @@
 
         if scale is None:
             if mpp is None:
                 raise ValueError('Only one of zoom/mpp should be None')
             scale = self.mpp_or_error() / mpp
 
         ds, lvl = self.best_level_for(1 / scale, tol=tol)
-        loc = *(slice(int(c / ds), int((c + size / scale) / ds))
-                for c, size in zip(z0_yx_offset, dsize)),
-        image = lvl.crop(*loc)
-        return resize(image, dsize)
+
+        yx_offset = *(int(c * scale) for c in z0_yx_offset),
+        loc = *(slice(c, c + size) for c, size in zip(yx_offset, dsize)),
+        return rescale_crop(lvl, *loc, scale=1 / ds / scale, interpolation=3)
 
     def extra(self, name: str) -> np.ndarray | None:
         if im := self.extras.get(name):
             return im.numpy()
         return None
 
     def thumbnail(self) -> np.ndarray:
```

### Comparing `bipl-0.5.6/src/bipl/io/_slide_bases.py` & `bipl-0.5.7/src/bipl/io/_slide_bases.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from math import ceil
 from typing import TYPE_CHECKING, final
 
 import cv2
 import numpy as np
 
 from bipl import env
-from bipl.ops import Tile, get_fusion, normalize_loc, resize
+from bipl.ops import Tile, get_fusion, normalize_loc, rescale_crop, resize
 
 if TYPE_CHECKING:
     from ._util import Icc
 
 REGISTRY: dict[re.Pattern, list[type['Driver']]] = {}
 _MIN_TILE = 256
 
@@ -43,16 +43,14 @@
     @property
     def icc(self) -> 'Icc | None':
         return None
 
 
 @dataclass(frozen=True)
 class ImageLevel(Image):
-    mpp: float | None
-
     @final
     @property
     def key(self) -> None:
         return None
 
     def crop(self, *loc: slice) -> np.ndarray:
         """Reads crop of LOD. Overridable"""
@@ -83,21 +81,33 @@
         base = self
         if isinstance(base, ProxyLevel):
             scale = base.scale * scale
             base = base.base
 
         h, w, c = base.shape
         h, w = (round(h * scale), round(w * scale))  # TODO: round/ceil/floor ?
-        mpp = base.mpp / scale if base.mpp else None
-        if scale > 0.5:  # Downscale to less then 2x, or upsample
-            return ProxyLevel((h, w, c), mpp, scale, base)
-
-        downsample = 2 ** (int(1 / scale).bit_length() - 1)
-        r_tile = max(_MIN_TILE // downsample, 1)
-        return TiledProxyLevel((h, w, c), mpp, scale, base, downsample, r_tile)
+        if scale <= 0.5:  # Downscale to more then 2x
+
+            # NOTE: to use this datapath we must
+            # - have 4^k downsamples (seen only in SVS)
+            # - fail `octave()` call - always succedes unless SVS is choked
+            #   (0s in tile sizes)
+            downsample = 2 ** (int(1 / scale).bit_length() - 1)
+            r_tile = max(_MIN_TILE // downsample, 1)
+            bh, bw, bc = base.shape
+            bh, bw = ((bh + downsample - 1) // downsample,
+                      (bw + downsample - 1) // downsample)
+
+            scale *= downsample
+            base = TiledProxyLevel((bh, bw, bc), base, downsample, r_tile)
+
+        return ProxyLevel((h, w, c), scale, base)
+
+    def octave(self) -> 'ImageLevel | None':
+        return None
 
     def _unpack_2d_loc(
         self,
         *slices: slice,
     ) -> tuple[np.ndarray, np.ndarray, list[int]]:
         # box[axis, {start, stop}]
         box = np.array([(s.start, s.stop) for s in slices])
@@ -106,15 +116,16 @@
         h, w = self.shape[:2]
         valid_box = box.clip(0, [[h], [w]])
 
         # Full output shape
         out_shape = (box @ [-1, 1]).tolist()
         return box, valid_box, out_shape
 
-    def _expand(self, rgb: np.ndarray, valid_box: np.ndarray, box: np.ndarray,
+    @staticmethod
+    def _expand(rgb: np.ndarray, valid_box: np.ndarray, box: np.ndarray,
                 bg_color: np.ndarray) -> np.ndarray:
         offsets = np.abs(valid_box - box)
         if offsets.any():
             tp, bm, lt, rt = offsets.ravel().tolist()
             rgb = cv2.copyMakeBorder(rgb, tp, bm, lt, rt, cv2.BORDER_CONSTANT,
                                      None, bg_color.tolist())
         return np.ascontiguousarray(rgb)
@@ -122,15 +133,15 @@
     @final
     def apply(  # type: ignore[override]
         self,
         fn: Callable[[np.ndarray], np.ndarray],
         pad: int = 0,
     ) -> '_LambdaLevel':
         # _LambdaLevel is not subclass of _LambdaImage
-        return _LambdaLevel(self.shape, self.mpp, self, fn, pad)
+        return _LambdaLevel(self.shape, self, fn, pad)
 
 
 @dataclass(frozen=True)
 class _LambdaImage(Image):
     base: Image
     fn: Callable[[np.ndarray], np.ndarray]
 
@@ -156,41 +167,35 @@
 
 
 @dataclass(frozen=True)
 class ProxyLevel(ImageLevel):
     scale: float
     base: ImageLevel
 
-    def _get_loc(self, *src_loc: slice) -> np.ndarray:
-        return self.base[src_loc]
-
     def crop(self, *loc: slice) -> np.ndarray:
-        src_loc = *[
-            # TODO: round/ceil/floor ?
-            slice(round(s.start / self.scale), round(s.stop / self.scale))
-            for s in loc
-        ],
-        image = self._get_loc(*src_loc)
-
-        h, w = ((s.stop - s.start) for s in loc)
-        return resize(image, (h, w))
+        return rescale_crop(
+            self.base, *loc, scale=1 / self.scale, interpolation=3)
 
 
 @dataclass(frozen=True)
-class TiledProxyLevel(ProxyLevel):
+class TiledProxyLevel(ImageLevel):
+    base: ImageLevel
     downsample: int
     r_tile: int
 
-    def _get_loc(self, *src_loc: slice) -> np.ndarray:
-        s_start = [s.start for s in src_loc]
-        s_shape = *(s.stop - s.start for s in src_loc),
+    def crop(self, *loc: slice) -> np.ndarray:
+        s_start = [s.start * self.downsample for s in loc]
+
+        r_shape = *(s.stop - s.start for s in loc),
+        s_shape = *(size * self.downsample for size in r_shape),
         if np.prod(s_shape) < env.BIPL_TILE_POOL_SIZE:
-            return super()._get_loc(*src_loc)
+            s_loc = *(slice(s.start * self.downsample,
+                            s.stop * self.downsample) for s in loc),
+            return resize(self.base.crop(*s_loc), r_shape[:2])
 
-        r_shape = *(ceil(size / self.downsample) for size in s_shape),
         r_tile = self.r_tile
         s_tile = r_tile * self.downsample
 
         ty, tx = (ceil(size / s_tile) for size in s_shape)
         tgrid = np.mgrid[:ty, :tx].reshape(2, -1).T
 
         t_shape = (r_tile, r_tile)
@@ -203,28 +208,30 @@
         )
         image = get_fusion(r_tiles, r_shape)
         assert image is not None
         return image
 
 
 class Driver:
+    mpp: float | None
+
     @final
     @classmethod
     def register(cls, regex: str):
         """Registers type builder for extensions. Last call takes precedence"""
         REGISTRY.setdefault(re.compile(regex), []).append(cls)
 
     def __init__(self, path: str) -> None:
         raise NotImplementedError
 
     def __len__(self) -> int:
         """Count of indexed images, usually resolution images"""
         return 0
 
-    def __getitem__(self, index: int) -> Image:
+    def __getitem__(self, index: int) -> Image | None:
         """Gives indexed image"""
         raise NotImplementedError
 
     def named_items(self) -> dict[str, Image]:
         keys = self.keys()
         return {k: self.get(k) for k in keys}
```

### Comparing `bipl-0.5.6/src/bipl/io/_tiff.py` & `bipl-0.5.7/src/bipl/io/_tiff.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,77 +4,78 @@
 - not thread safe (internally)
 - compatible with TIFF and its flavours
 """
 
 __all__ = ['Tiff']
 
 import ctypes
+import mmap
 import sys
 import warnings
 import weakref
-from collections.abc import Iterator
+from collections.abc import Callable, Iterator
 from contextlib import contextmanager
 from ctypes import (POINTER, addressof, byref, c_char_p, c_float, c_int,
-                    c_ubyte, c_uint16, c_uint32, c_uint64, c_void_p,
-                    create_string_buffer, string_at)
-from dataclasses import dataclass, field
+                    c_ubyte, c_uint16, c_uint32, c_uint64, c_void_p, string_at)
+from dataclasses import dataclass, field, replace
 from enum import Enum
-from functools import cached_property
+from heapq import heappop, heappush
 from itertools import product
 from threading import Lock
-from typing import NamedTuple, Protocol, TypeVar
+from typing import TypeVar
 
 import cv2
 import imagecodecs
 import numpy as np
-from glow import sizeof
+import numpy.typing as npt
+from glow import shared_call, si_bin, sizeof
 from numpy.lib.stride_tricks import as_strided
 
 from bipl._env import env
 
 from ._libs import load_library
 from ._slide_bases import Driver, Image, ImageLevel
-from ._util import (Icc, is_aperio, parse_aperio_description, parse_xml,
-                    unflatten)
+from ._util import (Icc, get_aperio_properties, get_ventana_properties,
+                    parse_xml, unflatten)
 
 _T = TypeVar('_T')
+_U8 = npt.NDArray[np.uint8]
 
 TIFF = load_library('libtiff', 6, 5)
 # _TIFF.TIFFSetErrorHandler(None)
 
 (TIFF.TIFFOpenW if sys.platform == 'win32' else TIFF.TIFFOpen).restype \
     = POINTER(c_ubyte)
 
+_RESOLUTION_UNITS = {2: 25400, 3: 10000}
+
 
 # ---------------------------- TIFF tags mappings ----------------------------
 class _ColorSpace(Enum):
     MINISBLACK = 1
     RGB = 2
     YCBCR = 6
 
 
-class _ColorInfo(NamedTuple):
-    space: _ColorSpace
-    subsampling: tuple[int, int]
-
-    def to_rgb(self, x: np.ndarray) -> np.ndarray:
-        if self.space is not _ColorSpace.YCBCR or self.subsampling != (2, 2):
-            return x
-
-        h, w = x.shape[:2]
-        assert h % 2 == w % 2 == 0
-
-        # (2 h/2) w 3 -> h/2 w 3
-        # h/2 (w/2 2) 3 -> h/2 w/2 2 3 -> h/2 w/2 (2 3) -> h/2 w/2 6
-        hw6 = x[:h // 2, :, :].reshape(h // 2, w // 2, 6)
-
-        # y00, y01, y10, y11, cb, cr
-        y = hw6[:, :, [[0, 1], [2, 3]]].transpose(0, 2, 1, 3).reshape(h, w)
-        cb_cr = hw6[:, :, [4, 5]]
-        return cv2.cvtColorTwoPlane(y, cb_cr, cv2.COLOR_YUV2RGB_NV12)
+def nv12_to_rgb(x: _U8) -> _U8:
+    w = x.shape[1]
+    assert w % 2 == 0
+    w2 = w // 2
+
+    # h/2 w 3 -> h/2 w/2 6
+    # 6 channels are [Y-Y-Y-Y-Cb-Cr] of 2x2 pixel block
+    hw6 = x.reshape(-1, w2, 6)
+
+    # -> h/2 w/2 4 -> h/2 w/2 2 2 -> h/2 2 w/2 2 -> h w
+    y = hw6[..., :4].reshape(-1, w2, 2, 2).transpose(0, 2, 1, 3).reshape(-1, w)
+    # -> h/2 w/2 2
+    cb_cr = hw6[:, :, 4:]
+
+    r = cv2.cvtColorTwoPlane(y, cb_cr, cv2.COLOR_YUV2RGB_NV12)
+    return np.asarray(r)
 
 
 class _Compression(Enum):
     RAW = 1
     CCITT = 2
     CCITTFAX3 = 3
     CCITTFAX4 = 4
@@ -94,49 +95,58 @@
     SGILOG24 = 34677
     JPEG2000 = 34712
     LZMA = 34925
     ZSTD = 50000
     WEBP = 50001
 
 
+class _Planarity(Enum):
+    CONTIG = 1  # Single buffer for all image planes
+    # SEPARATE = 2  # Separate buffers for each R/G/B plane. TODO: support
+
+
 class _Tag:  # noqa: PIE795,RUF100
-    JPEG_TABLES = 347
+    DESCRIPTION = 270
+    MAKE = 271
+    TILE_OFFSETS = 324
     TILE_BYTE_COUNTS = 325
+    JPEG_TABLES = 347
     BACKGROUND_COLOR = 434
+    XMP = 700
+    ICC_PROFILE = 34675
+    JPEGCOLORMODE = 65538
 
 
 class _Tags:
     def __init__(self, ptr):
         self._ptr = ptr
+
         compression, = self._get(c_uint16, 259)
         self.compression = _Compression(compression)
 
+        planarity, = self._get(c_uint16, 284)
+        self.planarity = _Planarity(planarity)  # TODO: use later
+
         self.spp, = self._get(c_uint16, 277)
-        self.is_planar, = self._get(c_uint16, 284)
-        self.image_size = self._get(c_uint32, 257, 256)
-        self.tile_size = self._get(c_uint32, 323, 322)
-        self.description = self._get_str(270)
-        self.resolution = self._get(c_float, 283, 282)
 
         # ! crashes, but should work according to openslide docs
         # self.is_hamamatsu = bool(self._get(c_uint16, 65420))
-        self.make = self._get_str(271)
 
         self.bps, = self._get(c_uint16, 339) or [1]
 
         ics, = self._get(c_uint16, 262)
-        colorspace = _ColorSpace(ics)
-        subsampling = (1, 1)
+        self.color = _ColorSpace(ics)
+        self.subsampling = (1, 1)
 
         # TODO: use this in YCbCr conversion
         self.gray = np.array([], 'f4')  # Luma coefficients
         self.yuv_centered = True
         self.yuv_bw = np.array([], 'f4')  # BW pairs, per channel
 
-        if colorspace is _ColorSpace.YCBCR:
+        if self.color is _ColorSpace.YCBCR:
             self.gray = np.array([.299, .587, .114], 'f4')
             gray_ptr = POINTER(c_float)()
             if TIFF.TIFFGetField(self._ptr, 529, byref(gray_ptr)):
                 self.gray = np.ctypeslib.as_array(gray_ptr, [3]).copy()
 
             # YCbCr subsampling H/W, i.e:
             # 24bps:
@@ -146,29 +156,29 @@
             #  (2 1) = 4:4:0 (cccc/____), 50% H, 100% W
             # 12bps:
             #  (1 4) = 4:1:1 (c___/c___), 100% H, 25% W
             #  (2 2) = 4:2:0 (c_c_/____), 50% H, 50% W - a.k.a. YUV-NV12
             # 10bps:
             #  (2 4) = 4:1:0 (c___/____), 50% H, 25% W
             ss_w, ss_h = self._get_varargs((c_uint16, c_uint16), 530) or (2, 2)
-            subsampling = ss_h, ss_w
+            self.subsampling = ss_h, ss_w
 
             self.yuv_centered = 2 not in self._get(c_uint16, 531)
 
             bw_ptr = POINTER(c_float)()
             if TIFF.TIFFGetField(self._ptr, 532, byref(bw_ptr)):
                 self.yuv_bw = np.ctypeslib.as_array(bw_ptr, [3, 2])
 
-        self.color = _ColorInfo(colorspace, subsampling)
+            self.jpcm, = self._get(c_int, _Tag.JPEGCOLORMODE)
 
         self.icc = None
         icc_size = c_int()
         icc_ptr = c_char_p()
-        if (TIFF.TIFFGetField(self._ptr, 34675, byref(icc_size),
-                              byref(icc_ptr)) and icc_size.value > 0):
+        if TIFF.TIFFGetField(self._ptr, _Tag.ICC_PROFILE, byref(icc_size),
+                             byref(icc_ptr)) and icc_size.value > 0:
             self.icc = Icc(string_at(icc_ptr, icc_size.value))
 
     def _get(
         self,
         tp: type['ctypes._SimpleCData[_T]'],
         *tags: int,
     ) -> tuple[_T, ...]:
@@ -188,277 +198,350 @@
     def _get_varargs(self, tps: tuple[type['ctypes._SimpleCData[_T]'], ...],
                      tag: int) -> tuple[_T, ...]:
         cvs = *(tp() for tp in tps),
         if TIFF.TIFFGetField(self._ptr, c_uint32(tag), *map(byref, cvs)):
             return *(cv.value for cv in cvs),
         return ()
 
-
-# -------------------------- lazy decoding proxies ---------------------------
-class SupportsArray(Protocol):
-    def __array__(self) -> np.ndarray:
-        ...
-
-    def __getitem__(self, key) -> np.ndarray:
-        ...
-
-
-class _ProxyArray:
     @property
-    def numpy(self) -> np.ndarray:
-        raise NotImplementedError
-
-    def __array__(self) -> np.ndarray:
-        return self.numpy
-
-    def __getitem__(self, key) -> np.ndarray:
-        return self.numpy[key]
+    def image_shape(self) -> tuple[int, int, int]:
+        shape = *self._get(c_uint32, 257, 256), self.spp
+        if len(shape) != 3:
+            raise ValueError(f'TIFF: Bad image shape - {shape}')
+        return shape
 
+    @property
+    def tile_shape(self) -> tuple[int, int, int] | None:
+        if not TIFF.TIFFIsTiled(self._ptr):
+            return None
+        tile = *self._get(c_uint32, 323, 322), self.spp
+        if len(tile) != 3:
+            raise ValueError(f'TIFF: Bad tile shape - {tile}')
+        return tile
 
-class _CachedArray(_ProxyArray):
-    @cached_property
-    def numpy(self) -> np.ndarray:
-        return self._numpy_impl()
+    def tile_spans(self, shape: tuple[int, ...],
+                   tile: tuple[int, ...]) -> npt.NDArray[np.uint64]:
+        """Returns (h w d 2) tensor of start:stop of each tile w.r.t file."""
+        grid_shape = *(len(range(0, s, t)) for s, t in zip(shape, tile)),
+
+        ptr = POINTER(c_uint64)()
+        if not TIFF.TIFFGetField(self._ptr, _Tag.TILE_OFFSETS, byref(ptr)):
+            raise ValueError('TIFF has tiled image, but no '
+                             'tile offsets table present')
+        tbs = np.ctypeslib.as_array(ptr, grid_shape).copy()
+        # TIFF._TIFFfree(tbc_ptr)  # TODO: ensure no segfault
+
+        ptr = POINTER(c_uint64)()
+        if not TIFF.TIFFGetField(self._ptr, _Tag.TILE_BYTE_COUNTS, byref(ptr)):
+            raise ValueError('TIFF has tiled image, but no '
+                             'tile size table present')
+        tbc = np.ctypeslib.as_array(ptr, grid_shape).copy()
+        # TIFF._TIFFfree(tbc_ptr)  # TODO: ensure no segfault
+
+        return np.stack((tbs, tbs + tbc), -1)
+
+    def get_decoder(self) -> Callable[[bytes], _U8]:
+        match self.compression:
+            case _Compression.JPEG:
+                jpt = None
+                size = c_int()
+                ptr = c_char_p()
+                if (TIFF.TIFFGetField(self._ptr, _Tag.JPEG_TABLES, byref(size),
+                                      byref(ptr)) and size.value > 4):
+                    jpt = string_at(ptr, size.value)
+                    # TIFF._TIFFfree(ptr)  # TODO: ensure no segfault
+                return _JpegDecoder(jpt, self.color.name)
+
+            case _Compression.JPEG2000_RGB | _Compression.JPEG2000_YUV:
+                return imagecodecs.jpeg2k_decode
+
+            case _:
+                return imagecodecs.imread  # type: ignore
+
+    def _bg_color(self, meta: dict) -> _U8:
+        if c := meta.get('ScanWhitePoint'):
+            return np.array(int(c), 'u1')
 
-    def _numpy_impl(self) -> np.ndarray:
-        raise NotImplementedError
+        bg_hex = b'FFFFFF'
+        bg_color_ptr = c_char_p()
+        # TODO: find sample file to test this path. Never reached
+        if TIFF.TIFFGetField(self._ptr, _Tag.BACKGROUND_COLOR,
+                             byref(bg_color_ptr)):
+            bg_hex = string_at(bg_color_ptr, 3)
+            # TIFF._TIFFfree(bg_color_ptr)  # TODO: ensure no segfault
+        return np.frombuffer(bytes.fromhex(bg_hex.decode()), 'u1').copy()
 
+    def vendor_props(
+        self,
+        vendor: str,
+        index: int = 0,
+        description: str | None = None,
+    ) -> tuple[str, dict[str, str]] | None:
+        if description is None:
+            description = self._get_str(_Tag.DESCRIPTION)
+
+        match vendor:
+            case 'ventana':  # BIF of Roche
+                xmp_size = c_int()
+                xmp_ptr = c_char_p()
+                if TIFF.TIFFGetField(self._ptr, _Tag.XMP, byref(xmp_size),
+                                     byref(xmp_ptr)) and xmp_size.value > 0:
+                    xmp = string_at(xmp_ptr, xmp_size.value)
+                    if meta := get_ventana_properties(xmp, index):
+                        return description, meta
+                if index != 0:
+                    return description, {}
+
+            case 'aperio':  # SVS
+                return get_aperio_properties(description, index)
+
+            case 'hamamatsu':  # NDPI
+                if self._get_str(_Tag.MAKE) == 'Hamamatsu':
+                    raise ValueError('TIFF: Hamamatsu is not yet supported')
+
+            case 'generic':  # TIFF
+                try:
+                    meta = unflatten(parse_xml(description))
+                except Exception:  # noqa: BLE001
+                    return description, {}
+                else:
+                    return '', meta
 
-@dataclass
-class CompressedArray(_CachedArray):
-    data: object
+        return None
 
-    def _numpy_impl(self) -> np.ndarray:
-        return imagecodecs.imread(self.data)
+    def vendor_properties(self) -> tuple[str, str, dict[str, str]]:
+        description = self._get_str(_Tag.DESCRIPTION)
 
+        for vendor in ('ventana', 'aperio', 'hamamatsu', 'generic'):
+            if r := self.vendor_props(vendor, 0, description):
+                header, meta = r
+                return vendor, header, meta
+
+        raise ValueError('Unknown vendor')
+
+    def _get_mpp(self, vendor: str, meta: dict) -> float | None:
+        """Extract MPP, um/pixel, phisical pixel size"""
+        if vendor == 'ventana':
+            # Ventana messes with TIFF tag XResolution, YResolution
+            return float(mpp_s) if (mpp_s := meta.get('ScanRes')) else None
+
+        if pixels_per_unit := self._get(c_float, 283, 282):
+            res_unit_kind, = self._get(c_uint16, 296)
+            if res_unit := _RESOLUTION_UNITS.get(res_unit_kind):
+                mpp_xy = [res_unit / ppu for ppu in pixels_per_unit if ppu]
+                if mpp_xy and (mpp := float(np.mean(mpp_xy))):
+                    return mpp
 
-@dataclass
-class JpegArray(_CachedArray):
-    data: object
-    jpt: bytes
-    colorspace: int
+        if mpp_s := meta.get('MPP'):
+            return float(mpp_s)
+        return None
 
-    def _numpy_impl(self) -> np.ndarray:
-        return imagecodecs.jpeg_decode(
-            self.data, tables=self.jpt, colorspace=self.colorspace)
+    def properties(self) -> tuple[str, str, dict[str, str], float | None, _U8]:
+        """Extracts: (vendor, header, metadata, mpp)"""
+        vendor, header, meta = self.vendor_properties()
+        mpp = self._get_mpp(vendor, meta)
+        bg_color = self._bg_color(meta)
+        return vendor, header, meta, mpp, bg_color
 
 
 # ------------------ image, level & opener implementations -------------------
 
 
 @dataclass(frozen=True)
 class _BaseImage(Image):
-    index: int
     icc_impl: Icc | None
-    tiff: 'Tiff'
 
     @property
     def icc(self) -> Icc | None:
         return self.icc_impl
 
 
 @dataclass(frozen=True)
 class _Image(_BaseImage):
-    head: list[str]
-    vendor: str
+    tiff: 'Tiff'
+    head: str
+    index: int
 
     @property
     def key(self) -> str | None:
-        if self.vendor == 'aperio' and self.index == 1:
+        if self.tiff.vendor == 'aperio' and self.index == 1:
             return 'thumbnail'
+        if self.tiff.vendor == 'ventana':
+            match self.head:
+                case 'Thumbnail':
+                    return 'thumbnail'
+                case 'Label Image' | 'Label_Image':
+                    return 'macro'
+            return None
         for key in ('label', 'macro'):
-            if any(key in s for s in self.head):
+            if any(key in s for s in self.head.splitlines()):
                 return key
         return None
 
-    def numpy(self) -> np.ndarray:
+    def numpy(self) -> _U8:
         h, w = self.shape[:2]
         rgba = np.empty((h, w, 4), dtype='u1')
 
+        # TODO: find offset & size of such images
         with self.tiff.ifd(self.index) as ptr:
             ok = TIFF.TIFFReadRGBAImageOriented(ptr, w, h,
                                                 c_void_p(rgba.ctypes.data), 1,
                                                 0)
             if not ok:
                 raise ValueError('TIFF image read failed')
 
         rgba = cv2.cvtColor(rgba, cv2.COLOR_mRGBA2RGBA)
         # TODO: do we need to use bg_color to fill points where alpha = 0 ?
-        return rgba[..., :3]
+        return np.asarray(rgba[..., :3])
+
+
+@dataclass(frozen=True, slots=True)
+class _JpegDecoder:
+    jpt: bytes | None = field(repr=False)
+    color: str | None
+
+    def __call__(self, buf: bytes) -> _U8:
+        return imagecodecs.jpeg_decode(
+            buf, tables=self.jpt, colorspace=self.color, outcolorspace='RGB')
 
 
 @dataclass(frozen=True)
 class _Level(ImageLevel, _BaseImage):
-    color: _ColorInfo
-    bg_color: np.ndarray
-    compression: _Compression
-    jpt: bytes = field(repr=False)
+    memo: mmap.mmap
+    spans: npt.NDArray[np.uint64] = field(repr=False)
     tile: tuple[int, ...]
-    tile_sizes: np.ndarray = field(repr=False)
+    decode: Callable[[bytes], _U8]
+    cache: '_CacheZYXC'
+    fill: _U8
+    pool: int = 1
+
+    def octave(self) -> '_Level | None':
+        th, tw, tc = self.tile
+        if th % 2 or tw % 2:
+            return None
+
+        h, w, c = self.shape
+        return replace(
+            self,
+            shape=((h + 1) // 2, (w + 1) // 2, c),
+            tile=(th // 2, tw // 2, tc),
+            pool=self.pool * 2,
+        )
+
+    def __eq__(self, rhs) -> bool:
+        return (type(rhs) is _Level and self.memo is rhs.memo
+                and self.shape == rhs.shape)
 
-    def _read_tile(self, iy, ix, ptr) -> SupportsArray:
-        nbytes = int(self.tile_sizes[iy, ix])
+    def __hash__(self) -> int:
+        return hash(self.memo) & hash(self.shape)
 
-        if not nbytes:  # If nothing to read, don't read
-            raise ValueError('File has corrupted tiles with zero size')
-            # TODO: read from previous level
-            # * If tile is empty on level N,
-            # * then all tiles on levels >N are invalid, whether empty or not
-            return np.broadcast_to(self.bg_color, self.tile)
-
-        offset = iy * self.tile_sizes.shape[1] + ix
-
-        # if not self.compression.name.startswith('JPEG2000'):
-        if self.compression not in {
-                _Compression.JPEG2000_RGB, _Compression.JPEG2000_YUV
-        }:
-            image = np.empty(self.tile, dtype='u1')
-            isok = TIFF.TIFFReadEncodedTile(ptr, offset,
-                                            c_void_p(image.ctypes.data),
-                                            image.size)
-            if isok == -1:
-                raise ValueError('TIFF tile read failed')
-            return self.color.to_rgb(image)
-
-        data = create_string_buffer(nbytes)
-        TIFF.TIFFReadRawTile(ptr, offset, data, len(data))
-
-        if self.jpt:
-            return JpegArray(data, self.jpt, self.color.space.value)
-        return CompressedArray(data)
-
-    def _get_tile(self, iy: int, ix: int, ptr, skip: bool) -> SupportsArray:
-        # NOTE: like any op using TIFF pointer, this must be called under lock.
+    @shared_call  # Thread safety
+    def _get_tile(self, *loc: int) -> _U8 | None:
         # NOTE:
         # Like OpenSlide does we use private cache for each slide
-        # with (level, y, x) key.
-        # But:
-        # - we store compressed data instead of pixel data to cache more tiles.
-        # - we cache opened slides to not waste time on re-opening
+        #   with (level, y, x) key to cache decoded pixels.
+        # But we also cache opened slides to not waste time on re-opening
         #   (that can lead to multiple caches existing at the same moment).
-        # NOTE:
-        # If tile becomes uncompressed we don't evict old compressed data.
-        #   (but we should, that CAN LEAD TO HIGH MEMORY USAGE).
-        # TODO: adjust cache size when tile is decoded.
-        # TODO: cache pixel data
-        tiff = self.tiff
-        key = (self.index, iy, ix)
-        cache = tiff.cache
-
-        # Cache hit, move to the end
-        if (entry := cache.pop(key, None)) is not None:
-            _, obj = cache[key] = entry
-            return obj
-
-        # Cache miss
-        obj = self._read_tile(iy, ix, ptr)
-
-        # Non-cacheable object or no cache at all
-        if skip or not (cache_cap := env.BIPL_TILE_CACHE):
-            return obj
-        if (size := sizeof(obj)) > cache_cap:
-            warnings.warn(
-                f'Rejecting overlarge cache entry of size {size} bytes',
-                stacklevel=3)
-            return obj
+        lo, hi = self.spans[loc].tolist()
+        if lo == hi:  # If nothing to read, don't read
+            return None
+
+        key = (*self.shape, *loc)
+        if (im := self.cache[key]) is None:  # Cache miss
+
+            # Read tile from disk
+            im = self.decode(self.memo[lo:hi])
+
+            # Resize if level is pooled
+            th, tw = self.tile[:2]
+            if im.shape[:2] != (th, tw):
+                if self.pool > 2:
+                    im = cv2.resize(im, (tw, th), interpolation=cv2.INTER_AREA)
+                else:
+                    im = cv2.resize(im, (tw, th))
 
-        # Remove least recently used entries and put new one
-        tiff.cache_size += size
-        while tiff.cache_size > cache_cap:
-            tiff.cache_size -= cache.pop(next(iter(cache)))[0]
-        cache[key] = (size, obj)
-        return obj
+            self.cache[key] = im  # type: ignore
+        return im  # type: ignore
 
-    def crop(self, *loc: slice) -> np.ndarray:
+    def crop(self, *loc: slice) -> _U8:
         *tile, spp = self.tile
 
         # (y/x lo/hi)
         box = np.array([(s.start, s.stop) for s in loc])
         out_shape = np.r_[box[:, 1] - box[:, 0], spp]
 
         if not out_shape.all():
             return np.empty(out_shape, self.dtype)
 
         bmin, bmax = box.T.clip(0, self.shape[:2])  # (y/x)
         if (bmin == bmax).any():  # Crop is outside of image
-            return np.broadcast_to(self.bg_color, out_shape)
+            return np.broadcast_to(self.fill, out_shape)
 
-        iloc, masks, t_crops, o_crops, ((y0, y1), (x0, x1)) = zip(
+        iloc, t_crops, o_crops, ((y0, y1), (x0, x1)) = zip(
             *map(self._make_index, box[:, 0], bmin, bmax, tile))
 
-        with self.tiff.ifd(self.index) as ptr:
-            parts = self._get_n_tiles(iloc, masks, ptr)
+        parts = [
+            self._get_tile(y, x, 0)
+            for y, x in product(*(ids.tolist() for ids in iloc))
+        ]
 
         out = np.empty(out_shape, self.dtype)
-        out[:y0] = self.bg_color
-        out[y0:y1, :x0] = self.bg_color
-        out[y0:y1, x1:] = self.bg_color
-        out[y1:] = self.bg_color
-
-        self._fill_result(out, parts, o_crops, t_crops)
-
+        out[:y0] = self.fill
+        out[y0:y1, :x0] = self.fill
+        out[y0:y1, x1:] = self.fill
+        out[y1:] = self.fill
+        for part, (oy, ox), (ty, tx) in zip(parts, product(*o_crops),
+                                            product(*t_crops)):
+            if part is None:
+                out[slice(*oy), slice(*ox)] = self.fill
+            else:
+                out[slice(*oy), slice(*ox)] = part[slice(*ty), slice(*tx)]
         return out
 
     def _make_index(
-        self, min_: int, vmin: int, vmax: int, tile: int
-    ) -> tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
+            self, min_: int, vmin: int, vmax: int,
+            tile: int) -> tuple[np.ndarray, np.ndarray, np.ndarray, list]:
         # (n + 1)
         ids1 = np.arange(vmin // tile, 1 - (-vmax // tile))
         n = ids1.size - 1
         ts = ids1 * tile
         vsep = ts.clip(vmin, vmax)
 
         # (n lo/hi), source & target slices
         u = vsep.itemsize
         o_crops = as_strided(vsep - min_, (n, 2), (u, u))
         t_crops = as_strided(vsep, (n, 2), (u, u)) - ts[:-1, None]
 
         # (lo/hi), region of `out` to fill
         o_span = o_crops[[0, -1], [0, 1]].tolist()
 
-        # Cache only edges
-        # Increases cache usage for linear reads (such as in `ops.Mosaic`)
-        mask = np.zeros(n, np.bool_)
-        mask[1:-1] = True
-
-        return ids1[:-1], mask, t_crops, o_crops, o_span
-
-    def _get_n_tiles(self, iloc, masks, ptr):
-        parts = [
-            self._get_tile(y, x, ptr, skip_cache)
-            for (y, x), skip_cache in zip(
-                product(*(ids.tolist() for ids in iloc)),
-                np.bitwise_and.outer(*masks).ravel().tolist(),
-            )
-        ]
-        return parts
-
-    def _fill_result(self, out, parts, o_crops, t_crops):
-        for part, (oy, ox), (ty, tx) in zip(parts, product(*o_crops),
-                                            product(*t_crops)):
-            # NOTE: This call does decoding and caching of pixel data
-            #       sequentially, but can be done in parallel.
-            out[slice(*oy), slice(*ox)] = part[slice(*ty), slice(*tx)]
+        return ids1[:-1], t_crops, o_crops, o_span
 
 
 # FIXME: Get around slides from choked SVS encoder
 class Tiff(Driver):
     def __init__(self, path: str):
-        # TODO: use memmap instead of libtiff
         self._ptr = (
             TIFF.TIFFOpenW(path, b'rm') if sys.platform == 'win32' else
             TIFF.TIFFOpen(path.encode(), b'rm'))
         if not self._ptr:
             raise ValueError(f'File {path} cannot be opened')
 
         weakref.finalize(self, TIFF.TIFFClose, self._ptr)
         self._dir = 0
         self._lock = Lock()
-        self.cache: dict[tuple, tuple[int, SupportsArray]] = {}
-        self.cache_size = 0
+        self.cache = _CacheZYXC()
+
+        # Initially directory 0 is active
+        self._tags = _Tags(self._ptr)
+        self.vendor, self._head, self._meta, self.mpp, self._bg_color \
+            = self._tags.properties()
+
+        with open(path, 'rb') as f:
+            self._memo = mmap.mmap(f.fileno(), 0, access=mmap.ACCESS_READ)
 
     def __repr__(self) -> str:
         return f'{type(self).__name__}({addressof(self._ptr.contents):0x})'
 
     @contextmanager
     def ifd(self, index: int) -> Iterator:
         with self._lock:
@@ -466,99 +549,82 @@
                 self._dir = index
                 TIFF.TIFFSetDirectory(self._ptr, index)
             yield self._ptr
 
     def __len__(self) -> int:
         return TIFF.TIFFNumberOfDirectories(self._ptr)
 
-    def _bg_color(self) -> np.ndarray:
-        bg_hex = b'FFFFFF'
-        bg_color_ptr = c_char_p()
-        # TODO: find sample file to test this path. Never reached
-        if TIFF.TIFFGetField(self._ptr, _Tag.BACKGROUND_COLOR,
-                             byref(bg_color_ptr)):
-            bg_hex = string_at(bg_color_ptr, 3)
-            # TIFF._TIFFfree(bg_color_ptr)  # TODO: ensure no segfault
-        return np.frombuffer(bytes.fromhex(bg_hex.decode()), 'u1').copy()
+    def _get(self, index: int) -> Image | None:
+        if index == 0:
+            tags = self._tags
+            head = self._head
+        else:
+            tags = _Tags(self._ptr)
+            r = tags.vendor_props(self.vendor, index)
+            if not r:
+                raise ValueError('File directories are from different vendors')
+            head, _ = r
 
-    def _parse_description(self, desc: str,
-                           make: str) -> tuple[str, list[str], dict[str, str]]:
-        vendor = ''
-        if is_aperio(desc):
-            vendor = 'aperio'
-            head, meta = parse_aperio_description(desc)
+        if tags.color is _ColorSpace.YCBCR and tags.subsampling != (2, 2):
+            raise ValueError('Unsupported YUV subsampling: '
+                             f'{tags.subsampling}')
 
-        else:
-            if make == 'Hamamatsu':
-                raise ValueError('Hamamatsu is not yet supported via libtiff')
-            try:
-                head = []
-                meta = unflatten(parse_xml(desc))
-            except Exception:  # noqa: BLE001
-                head = [desc]
-                meta = {}
-
-        return vendor, head, meta
-
-    def _mpp(self, resolution: tuple[float, ...],
-             meta: dict[str, str]) -> float | None:
-        if s := [(10_000 / v) for v in resolution if v]:
-            return float(np.mean(s))
-        if mpp := meta.get('MPP'):
-            return float(mpp)
-        return None
+        shape = tags.image_shape
+        tile = tags.tile_shape
 
-    def _get(self, index: int) -> Image:
-        tags = _Tags(self._ptr)
+        if tile is None:  # Not tiled
+            return _Image(shape, tags.icc, self, head, index)
 
-        if tags.is_planar != 1:
-            raise TypeError(f'Level {index} is not contiguous!')
+        spans = tags.tile_spans(shape, tile)
 
-        bg_color = self._bg_color()
-        vendor, head, meta = self._parse_description(tags.description,
-                                                     tags.make)
-        mpp = self._mpp(tags.resolution, meta) if index == 0 else None
+        # Aperio can choke on non-L0 levels. Read those from L0 to fix.
+        # `openslide` does this for us, delegate to it.
+        if self.vendor == 'aperio' and (spans[..., 0] == spans[..., 1]).any():
+            raise ValueError('Found 0s in tile size table')
 
-        if (tags.color.space is _ColorSpace.YCBCR
-                and tags.color.subsampling != (2, 2)):
-            raise ValueError('Unsupported YUV subsampling: '
-                             f'{tags.color.subsampling}')
+        return _Level(shape, tags.icc, self._memo, spans, tile,
+                      tags.get_decoder(), self.cache, self._bg_color)
 
-        # Compression and JPEG tables
-        jpt = b''
-        if tags.compression is _Compression.JPEG:
-            count = c_int()
-            jpt_ptr = c_char_p()
-            if TIFF.TIFFGetField(self._ptr, _Tag.JPEG_TABLES, byref(count),
-                                 byref(jpt_ptr)) and count.value > 4:
-                jpt = string_at(jpt_ptr, count.value)
-                # TIFF._TIFFfree(jpt_ptr)  # TODO: ensure no segfault
+    def __getitem__(self, index: int) -> Image | None:
+        with self.ifd(index):
+            return self._get(index)
 
-        # Whole level shape
-        shape = (*tags.image_size, tags.spp)
-        if len(shape) != 3:
-            raise ValueError(f'Bad shape in TIFF: {shape}')
 
-        # Tile shape, if applicable
-        if not TIFF.TIFFIsTiled(self._ptr):  # Not yet supported
-            return _Image(shape, index, tags.icc, self, head, vendor)
+# ------------------------------- tile caching -------------------------------
 
-        # Tile sizes
-        tile = (*tags.tile_size, tags.spp)
-        if len(tile) != 3:
-            raise ValueError(f'Bad tile shape in TIFF: {tile}')
 
-        tbc = np.empty([], 'u8')
-        tbc_ptr = POINTER(c_uint64)()
-        if TIFF.TIFFGetField(self._ptr, _Tag.TILE_BYTE_COUNTS, byref(tbc_ptr)):
-            num_tiles = *(len(range(0, s, t)) for s, t in zip(shape, tile)),
-            tbc = np.ctypeslib.as_array(tbc_ptr, num_tiles).copy()
-            # TIFF._TIFFfree(tbc_ptr)  # TODO: ensure no segfault
-            if (tbc == 0).any():
-                raise ValueError('Found 0s in tile size table')
+@dataclass(repr=False, slots=True)
+class _CacheZYXC:
+    lock: Lock = field(default_factory=Lock, repr=False)
+    used: int = 0
+    keys: list[tuple] = field(default_factory=list, repr=False)
+    # IYXC -> (size, buf)
+    buf: dict[tuple, tuple[int, _U8]] = field(default_factory=dict, repr=False)
 
-        return _Level(shape, index, tags.icc, self, mpp, tags.color, bg_color,
-                      tags.compression, jpt, tile, tbc)
+    def __repr__(self) -> str:
+        return (f'{type(self).__name__}'
+                f'(used={si_bin(self.used)}, items={len(self.buf)})')
 
-    def __getitem__(self, index: int) -> Image:
-        with self.ifd(index):
-            return self._get(index)
+    def __getitem__(self, key: tuple) -> _U8 | None:
+        with self.lock:
+            if e := self.buf.get(key):
+                return e[1]
+        return None
+
+    def __setitem__(self, key: tuple, obj: _U8) -> None:
+        if not (capacity := env.BIPL_TILE_CACHE):
+            return
+        if (size := sizeof(obj)) > capacity:
+            warnings.warn(
+                f'Rejecting overlarge cache entry of size {size} bytes',
+                stacklevel=3)
+            return
+        max_size = capacity - size
+
+        with self.lock:
+            while self.keys and self.used > max_size:
+                self.used -= self.buf.pop(heappop(self.keys))[0]
+
+            if self.used <= max_size:
+                heappush(self.keys, key)
+                self.buf[key] = (size, obj)
+                self.used += size
```

### Comparing `bipl-0.5.6/src/bipl/io/_util.py` & `bipl-0.5.7/src/bipl/io/_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,37 +48,48 @@
     parts = s.translate(tab).split('.')
     return tuple(int(word) if word.isdigit() else word for word in parts)
 
 
 # ---------------------------- aperio description ----------------------------
 
 
-def is_aperio(s: str) -> bool:
-    return s.startswith('Aperio')
+def get_aperio_properties(description: str,
+                          index: int = 0) -> tuple[str, dict[str, str]] | None:
+    if index == 0 and not description.startswith('Aperio'):
+        return None
+    header, *kv_pairs = description.split('|')
 
-
-def parse_aperio_description(s: str) -> tuple[list[str], dict[str, str]]:
-    header, *kv_pairs = s.split('|')
-
-    head = [s.strip() for s in header.splitlines()]
+    header = '\n'.join(s.strip() for s in header.splitlines())
 
     meta = {}
-    for s in kv_pairs:
-        tags = s.split('=', 1)
-        if len(tags) == 2:
-            meta[tags[0].strip()] = tags[1].strip()
-        else:
-            raise ValueError(f'Unparseable line in description: {s!r}')
+    for i, kv in enumerate(kv_pairs):
+        match kv.split('=', 1):
+            case [str(k), str(v)]:
+                meta[k.strip()] = v.strip()
+            case ['']:
+                continue
+            case _:
+                raise ValueError(f'Cannot parse TIFF description line #{i}: '
+                                 f'{kv!r}, {description!r}')
 
-    return head, meta
+    return header, meta
 
 
 # ----------------------------- xml description ------------------------------
 
 
+def get_ventana_properties(s: bytes, index: int = 0) -> dict[str, str]:
+    t = fromstring(s, XMLParser(resolve_entities=False, no_network=True))
+    if index == 0:
+        if (root := t.find('iScan')) is not None:
+            return dict(root.items())
+        return {}
+    return {'xmp': s.decode()}
+
+
 def parse_xml(s: str,
               /,
               *,
               group: str = 'property',
               name: str = 'name',
               value: str = 'value') -> dict[str, str]:
     t = fromstring(s, XMLParser(resolve_entities=False, no_network=True))
@@ -97,15 +108,15 @@
 # ----------------------------------------------------------------------------
 
 
 def _gdal_parse_description(meta: Mapping[str, str]) -> dict[str, Any]:
     desc = meta.get('TIFFTAG_IMAGEDESCRIPTION')
     if not desc:
         return {}
-    if is_aperio(desc):
+    if get_aperio_properties(desc):
         raise ValueError('Aperio is not yet supported by GDAL driver')
     try:
         props = parse_xml(desc)
     except Exception:  # noqa: BLE001
         return {}
     return unflatten(props)
```

### Comparing `bipl-0.5.6/src/bipl/ops/_mosaic.py` & `bipl-0.5.7/src/bipl/ops/_mosaic.py`

 * *Files identical despite different names*

### Comparing `bipl-0.5.6/src/bipl/ops/_tile.py` & `bipl-0.5.7/src/bipl/ops/_tile.py`

 * *Files identical despite different names*

### Comparing `bipl-0.5.6/src/bipl/ops/_types.py` & `bipl-0.5.7/src/bipl/ops/_types.py`

 * *Files identical despite different names*

### Comparing `bipl-0.5.6/src/bipl/ops/_util.py` & `bipl-0.5.7/src/bipl/ops/_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     """Converts probability array of (H W C) shape to (H W 3) RGB image"""
     if prob.ndim != 3:
         raise ValueError(f'prob should be 3d, got: {prob.shape}')
     h, w, c = prob.shape
     if not prob.size:
         return np.empty((h, w, 3), dtype='u1')
 
-    hue = prob.argmax(-1).astype('u1')
+    hue = prob.argmax(-1).astype('u1')  # NOTE: valid only for simple Indexer
     value = prob.max(-1)
     if value.dtype != 'u1':
         value *= 255
         value = value.round().astype('u1')
 
     hue_lut = np.zeros(256, 'u1')
     hue_lut[:c] = np.linspace(0, 127, c, endpoint=False, dtype='u1')
@@ -39,16 +39,23 @@
     return cv2.cvtColor(hsv, cv2.COLOR_HSV2RGB)
 
 
 def get_trapz(step: int, overlap: int) -> np.ndarray:
     """Returns trapezional window kernel to apply stiching"""
     if overlap == 0:
         raise ValueError('not applicable for overlap 0')
-    pad = np.linspace(0, 1, overlap + 2)[1:-1]  # strip initial 0 and final 1
-    return np.r_[pad, np.ones(step - overlap), pad[::-1]].astype('f4')
+
+    ramp = np.arange(1, overlap + 1).astype('f4')
+    ramp /= overlap + 1
+
+    r = np.empty(step + overlap, dtype='f4')
+    r[:overlap] = ramp
+    r[overlap:step] = 1
+    r[step:] = ramp[::-1]
+    return r
 
 
 def normalize_loc(loc: Sequence[slice] | slice,
                   shape: Sequence[int]) -> tuple[slice, ...]:
     """Ensures slices match ndim and have noo `None` endpoints"""
     if isinstance(loc, slice):
         loc = loc,
@@ -196,24 +203,27 @@
     box = np.array([[s.start, s.stop] for s in loc], 'i4')  # (y/x, start/stop)
     h, w = (box[:, 1] - box[:, 0]).tolist()
     if not h or not w:  # 0-size output
         return np.empty((h, w, *a.shape[2:]), a.dtype)
 
     lo_f, hi_f = np.multiply(box, scale, dtype='f4').T
 
+    loc = *(slice(floor(lo_), ceil(hi_)) for lo_, hi_ in zip(lo_f, hi_f)),
+    if not env.BIPL_SUBPIX:
+        return resize(padslice(a, *loc), (h, w))
+
     # Extra margin to accomodate interpolation kernel
     # 2x2 (0 extra) - nearest (0), bilinear (1), area (3)
     # 4x4 (1 extra) - bicubic (2)
     # 8x8 (3 extra) - lanczos4 (4)
     eps = (0, 0, 1, 0, 3)[interpolation]
 
     # Tight slice to have all necessary pixels
-    loc = tuple(
-        slice(*np.clip([floor(lo_) - eps, ceil(hi_) + eps], 0, size))
-        for lo_, hi_, size in zip(lo_f, hi_f, a.shape))
+    loc = *(slice(*np.clip([s.start - eps, s.stop + eps], 0, size))
+            for s, size in zip(loc, a.shape)),
     r = a[loc]
     if not r.size:  # 0-size tight slice
         return np.zeros((h, w, *a.shape[2:]), a.dtype)
 
     # Resample image crop to destination grid
     dy, dx = (lo_ - s.start + (scale - 1) / 2 for lo_, s in zip(lo_f, loc))
     return cv2.warpAffine(
```

### Comparing `bipl-0.5.6/LICENSE` & `bipl-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bipl-0.5.6/README.md` & `bipl-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `bipl-0.5.6/hatch_build.py` & `bipl-0.5.7/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bipl-0.5.6/pyproject.toml` & `bipl-0.5.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [tool.hatch.build.targets.wheel]
 artifacts = ["*.dll"]  # only wheel keeps DLLs
 
 [tool.hatch.build.hooks.custom]  # enable "custom" hook
 
 [project]
 name = "bipl"
-version = "0.5.6"
+version = "0.5.7"
 description = "Openslide/libtiff/GDAL ndarray-like interface and lazy parallel tile-based processing"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = [
     "medical", "images", "pathology", "whole-slide", "wsi", "pyramid", "slide",
     "libtiff", "openslide", "osgeo", "gdal",  # backends
@@ -30,15 +30,14 @@
     {name = "Paul Maevskikh", email = "arquolo@gmail.com"},
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 
 dependencies = [
     "glow~=0.13.5",
```

