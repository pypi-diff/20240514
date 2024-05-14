# Comparing `tmp/bigstream-1.3.0.tar.gz` & `tmp/bigstream-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigstream-1.3.0.tar", last modified: Tue Apr 16 14:40:05 2024, max compression
+gzip compressed data, was "bigstream-1.4.0.tar", last modified: Tue May 14 19:01:39 2024, max compression
```

## Comparing `bigstream-1.3.0.tar` & `bigstream-1.4.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2024-04-16 14:40:05.925942 bigstream-1.3.0/
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     1518 2023-10-02 19:28:02.000000 bigstream-1.3.0/LICENSE.md
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      270 2024-04-16 14:40:05.924454 bigstream-1.3.0/PKG-INFO
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     8731 2023-07-11 16:34:08.000000 bigstream-1.3.0/README.md
-drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2024-04-16 14:40:05.899900 bigstream-1.3.0/bigstream/
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)        5 2023-07-11 16:34:08.000000 bigstream-1.3.0/bigstream/__init__.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    46332 2024-04-10 16:12:30.000000 bigstream-1.3.0/bigstream/align.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     9265 2024-01-16 21:48:49.000000 bigstream-1.3.0/bigstream/application_pipelines.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7793 2024-04-10 16:12:30.000000 bigstream-1.3.0/bigstream/configure_irm.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    21545 2024-04-10 16:12:30.000000 bigstream-1.3.0/bigstream/distributed_align.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     6148 2024-04-10 16:12:30.000000 bigstream-1.3.0/bigstream/distributed_io_utility.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    22766 2024-04-10 16:12:30.000000 bigstream-1.3.0/bigstream/distributed_transform.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7403 2024-04-10 16:12:30.000000 bigstream-1.3.0/bigstream/features.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     6665 2024-04-10 16:12:30.000000 bigstream-1.3.0/bigstream/io_utility.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     6554 2024-01-22 19:55:56.000000 bigstream-1.3.0/bigstream/level_set.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    10153 2023-11-08 19:06:20.000000 bigstream-1.3.0/bigstream/metrics.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    25553 2024-04-10 16:12:30.000000 bigstream-1.3.0/bigstream/motion_correct.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    24297 2024-04-10 16:12:30.000000 bigstream-1.3.0/bigstream/piecewise_align.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    19357 2024-04-11 20:49:31.000000 bigstream-1.3.0/bigstream/piecewise_transform.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16188 2023-11-08 19:06:20.000000 bigstream-1.3.0/bigstream/stitch.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    18807 2024-04-11 20:49:47.000000 bigstream-1.3.0/bigstream/transform.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16649 2024-04-10 16:12:30.000000 bigstream-1.3.0/bigstream/utility.py
-drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2024-04-16 14:40:05.918426 bigstream-1.3.0/bigstream.egg-info/
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      270 2024-04-16 14:40:05.000000 bigstream-1.3.0/bigstream.egg-info/PKG-INFO
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      642 2024-04-16 14:40:05.000000 bigstream-1.3.0/bigstream.egg-info/SOURCES.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)        1 2024-04-16 14:40:05.000000 bigstream-1.3.0/bigstream.egg-info/dependency_links.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      275 2024-04-16 14:40:05.000000 bigstream-1.3.0/bigstream.egg-info/requires.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)       10 2024-04-16 14:40:05.000000 bigstream-1.3.0/bigstream.egg-info/top_level.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)       38 2024-04-16 14:40:05.927498 bigstream-1.3.0/setup.cfg
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      854 2024-04-16 14:39:31.000000 bigstream-1.3.0/setup.py
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2024-05-14 19:01:39.537896 bigstream-1.4.0/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     1518 2023-10-02 19:28:02.000000 bigstream-1.4.0/LICENSE.md
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      270 2024-05-14 19:01:39.536670 bigstream-1.4.0/PKG-INFO
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     8733 2024-05-10 21:22:22.000000 bigstream-1.4.0/README.md
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2024-05-14 19:01:39.514257 bigstream-1.4.0/bigstream/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)        5 2023-07-11 16:34:08.000000 bigstream-1.4.0/bigstream/__init__.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    54608 2024-05-14 16:40:17.000000 bigstream-1.4.0/bigstream/align.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     9265 2024-01-16 21:48:49.000000 bigstream-1.4.0/bigstream/application_pipelines.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     8716 2024-05-10 21:28:19.000000 bigstream-1.4.0/bigstream/configure_irm.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    21545 2024-04-10 16:12:30.000000 bigstream-1.4.0/bigstream/distributed_align.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     6148 2024-04-10 16:12:30.000000 bigstream-1.4.0/bigstream/distributed_io_utility.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    22766 2024-04-10 16:12:30.000000 bigstream-1.4.0/bigstream/distributed_transform.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7403 2024-04-10 16:12:30.000000 bigstream-1.4.0/bigstream/features.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     6665 2024-04-10 16:12:30.000000 bigstream-1.4.0/bigstream/io_utility.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     6554 2024-01-22 19:55:56.000000 bigstream-1.4.0/bigstream/level_set.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    10153 2023-11-08 19:06:20.000000 bigstream-1.4.0/bigstream/metrics.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    25553 2024-04-10 16:12:30.000000 bigstream-1.4.0/bigstream/motion_correct.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    25608 2024-05-14 16:57:53.000000 bigstream-1.4.0/bigstream/piecewise_align.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    19357 2024-04-11 20:49:31.000000 bigstream-1.4.0/bigstream/piecewise_transform.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16188 2023-11-08 19:06:20.000000 bigstream-1.4.0/bigstream/stitch.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    18807 2024-05-13 21:42:32.000000 bigstream-1.4.0/bigstream/transform.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16649 2024-04-10 16:12:30.000000 bigstream-1.4.0/bigstream/utility.py
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2024-05-14 19:01:39.531901 bigstream-1.4.0/bigstream.egg-info/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      270 2024-05-14 19:01:39.000000 bigstream-1.4.0/bigstream.egg-info/PKG-INFO
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      642 2024-05-14 19:01:39.000000 bigstream-1.4.0/bigstream.egg-info/SOURCES.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)        1 2024-05-14 19:01:39.000000 bigstream-1.4.0/bigstream.egg-info/dependency_links.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      275 2024-05-14 19:01:39.000000 bigstream-1.4.0/bigstream.egg-info/requires.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)       10 2024-05-14 19:01:39.000000 bigstream-1.4.0/bigstream.egg-info/top_level.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)       38 2024-05-14 19:01:39.539302 bigstream-1.4.0/setup.cfg
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      854 2024-05-14 18:51:50.000000 bigstream-1.4.0/setup.py
```

### Comparing `bigstream-1.3.0/LICENSE.md` & `bigstream-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bigstream-1.3.0/README.md` & `bigstream-1.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     blocksize=blocksize,
     static_transform_list=[global_transform,]
     write_path='./deform.zarr',
     cluster_kwargs={## params to control your cluster},
 )
 
 # apply the transforms
-local_aligned = piecewise_apply_transform(
+local_aligned = distributed_apply_transform(
     fix_highres, mov_highres,
     fix_highres_spacing, mov_highres_spacing,
     transform_list=[global_transform, local_transform],
     blocksize=blocksize,
     write_path='./deformed.zarr',
     cluster_kwargs={## params to control your cluster},
 )
```

### Comparing `bigstream-1.3.0/bigstream/align.py` & `bigstream-1.4.0/bigstream/align.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,44 @@
 from bigstream.configure_irm import configure_irm
 from bigstream.transform import apply_transform, compose_transform_list, compress_transform_list
 from bigstream.metrics import patch_mutual_information
 from bigstream import features
 import cv2
 
 
+def realize_mask(image, mask):
+    """
+    Ensure that mask is an ndarray
+
+    Parameters
+    ----------
+    image : nd-array
+        The image from which mask is derived
+
+    mask : None, nd-array, tuple of floats, or function
+        The mask data. If None, return None.
+        If an nd-array, threshold at zero.
+        If a tuple of floats, mask specified values.
+        If a function, apply it.
+
+    Returns
+    -------
+    A mask for image, which is either None or a binary nd-array
+    dtype is always uint8
+    """
+
+    if mask is None: return None
+    if isinstance(mask, np.ndarray):
+        return (mask > 0).astype(np.uint8)
+    if isinstance(mask, (tuple, list)):
+        return np.isin(image, mask, invert=True).astype(np.uint8)
+    if callable(mask):
+        return mask(image).astype(np.uint8)
+
+
 def apply_alignment_spacing(
     fix,
     mov,
     fix_mask,
     mov_mask,
     fix_spacing,
     mov_spacing,
@@ -208,14 +238,15 @@
 
 
 def feature_point_ransac_affine_align(
     fix, mov,
     fix_spacing,
     mov_spacing,
     blob_sizes,
+    safeguard_exceptions=True,
     alignment_spacing=None,
     num_sigma_max=15,
     cc_radius=12,
     nspots=5000,
     match_threshold=0.7,
     max_spot_match_distance=None,
     point_matches_threshold=50,
@@ -240,24 +271,20 @@
 
     Compute an affine alignment from feature points and ransac.
     A blob detector finds feature points in fix and mov. Correspondence
     between the fix and mov point sets is estimated using neighborhood
     correlation. A ransac filter determines the affine transform that brings
     the largest number of corresponding points to the same locations.
 
-    At least 100 spots must be found in the fixed image and 100 spots
-    in the moving image, otherwise default is returned. At least 50
-    correspondence pairs must be found, otherwise default is returned.
-    These constraints are required for reasonable performance from the
-    ransac affine alignment algorithm.
-
-    If insufficient points are found modify fix_spot_detection_kwargs
-    and/or mov_spot_detection_kwargs. See bigstream.features.
-
-    If insufficient point matches are found, modify match_threshold.
+    Several safeguards are implemented to ensure degenerate or poorly behaved
+    affines won't be returned. If your alignment is returning a ValueError,
+    then likely one of the safeguards is being triggered. See the
+    safeguard_exceptions parameter description below for more information.
+    When running this function as part of the distributed pipeline,
+    safeguard_exceptions is set to False automatically.
 
     Parameters
     ----------
     fix : ndarray
         the fixed image
 
     mov : ndarray
@@ -270,54 +297,97 @@
 
     mov_spacing : 1d array
         The spacing in physical units (e.g. mm or um) between voxels
         of the moving image.
         Length must equal `mov.ndim`
 
     blob_sizes : list of two floats
-        The [minimum, maximum] size of feature point objects in voxel units
+        The [minimum, maximum] size of feature point objects in voxel units.
+        These are radii; so if your data contains features that are 10 voxels
+        diameter on average, a reasonable value for this parameter would be
+        [3, 7] (symmetric about a radius of 5).
+
+    safeguard_exceptions : bool (default: True)
+        When this value is True, a failed safeguard test will return a
+        ValueError and a message indicating which safeguard failed.
+        This behavior is desired when working with one image at a time.
+
+        When this value if False, a failed safeguard test will print
+        a warning message, but return the identity transform without
+        throwing an exception. This behavior is desired when working
+        with many images (or tiles/blocks) at the same time.
+
+        Feature point detection and correspondence estimation are noisy
+        algorithms. Even with ransac, it is possible that insufficient
+        point detections or poor correspondence estimation will result
+        in a poor affine. Several safeguards are on by default to prevent
+        the return of a bad affine transform. These include:
+
+            * too few spots found in fix or moving image
+            * too few correspondences are identified between fix and moving spots
+            * an affine that is too far from identity is produced
+
+        These safeguards can all be relaxed through parameters described
+        below.
+
+    alignment_spacing : float (default: None)
+        Fixed and moving images are skip sampled to a voxel spacing
+        as close as possible to this value. Many alignments can be solved
+        at far lower resolution than the collected data. This parameter
+        can significantly speed up computation.
 
     num_sigma_max : scalar int (default: 15)
         The maximum number of laplacians to use in the feature point LoG detector
 
     cc_radius : scalar int (default: 12)
         The halfwidth of neighborhoods around feature points used to determine
         correlation and correspondence
 
     nspots : scalar int (default: 5000)
         The maximum number of feature point spots to use in each image
         If more spots are found the brightest ones are used.
 
     match_threshold : scalar float in range [0, 1] (default: 0.7)
         The minimum correlation two feature point neighborhoods must have to
-        consider them corresponding points
+        consider them corresponding points. This number can vary significantly
+        with input data quality. Consider lowering this before lowering
+        point_matches_threshold.
 
     max_spot_match_distance : scalar float (default: None)
         The maximum distance a fix and mov spot can be before alignment
         to still be considered matching spots; in microns. This helps
         prevent false positive correspondences.
 
     point_matches_threshold : scalar int (default: 50)
-        Minimum number of matching points for a valid alignment
+        Minimum number of matching points to proceed with alignment
+        Finding fewer matching point pairs than this threshold is a
+        safeguard test failure.
 
     align_threshold : scalar float (default: 2.0)
         The maximum distance two points can be to be considered aligned
         by the affine transform; in microns.
 
     diagonal_constraint : scalar float (default: 0.25)
         Diagonal entries of the affine matrix cannot be lower than
-        1 - diagonal_contraint or higher than 1 + diagonal_contraint. 
-        If this condition is violated the default transform is returned.
-        This helps prevent bad alignments.
+        1 - diagonal_contraint or higher than 1 + diagonal_contraint.
+        Failing this condition is a safeguard test failure. Raising this
+        value will allow increasingly extreme affine transforms to be
+        returned.
 
     fix_spot_detection_kwargs : dict (default {})
         Arguments passed to bigstream.features.blob_detection for fixed image
+        See docstring for that function for valid arguments.
+        You may need to modify these in order to pass the spot count threshold
+        safeguards, consider doing that before lowering fix_spots_count_threshold.
 
     mov_spot_detection_kwargs : dict (default {})
         Arguments passed to bigstream.features.blob_detection for moving image
+        See docstring for that function for valid arguments.
+        You may need to modify these in order to pass the spot count threshold
+        safeguards, consider doing that before lowering mov_spots_count_threshold.
 
     fix_spots : nd-array Nx3 (default: None)
         Skip the spot detection for the fixed image and provide your own spot coordinate
 
     fix_spots_count_threshold : scalar int (default: 100)
         Minimum number of fixed spots that need to exist for a valid alignment.
         Note that many times in order to have a better alignment it is better to tweak
@@ -327,19 +397,29 @@
         Skip the spot detection for the moving image and provide your own spot coordinate
 
     mov_spots_count_threshold : scalar int (default: 100)
         Minimum number of fixed spots that need to exist for a valid alignment.
         Note that many times in order to have a better alignment it is better to tweak
         threshold and/or threshold_rel in mov_spot_detection_kwargs then to lower this value
 
-    fix_mask : binary nd-array (default: None)
-        Spots from fixed image can only be found in the foreground of this mask
-
-    mov_mask : binary nd-array (default: None)
-        Spots from moving image can only be found in the foreground of this mask
+    fix_mask : nd-array, tuple of floats, or function (default: None)
+        Spots from fixed image can only be found in the foreground of this mask.
+        If an nd-array, any non-zero value is considered foreground and any
+        zero value is considered background. If a tuple of floats, any voxel
+        with value in the tuple is considered background. If a function, it
+        must take a single nd-array argument as input and return an array
+        of the same shape as the input but with dtype bool.
+
+    mov_mask : nd-array (default: None)
+        Spots from moving image can only be found in the foreground of this mask.
+        If an nd-array, any non-zero value is considered foreground and any
+        zero value is considered background. If a tuple of floats, any voxel
+        with value in the tuple is considered background. If a function, it
+        must take a single nd-array argument as input and return an array
+        of the same shape as the input but with dtype bool.
 
     fix_origin : 1d array (default: all zeros)
         The origin of the fixed image in physical units
 
     mov_origin : 1d array (default: all zeros)
         The origin of the moving image in physical units
 
@@ -360,14 +440,18 @@
     affine_matrix : 2d array 4x4
         An affine matrix matching the moving image to the fixed image
     """
 
     # establish default
     if default is None: default = np.eye(fix.ndim + 1)
 
+    # realize masks
+    fix_mask = realize_mask(fix, fix_mask)
+    mov_mask = realize_mask(mov, mov_mask)
+
     # apply static transforms
     if static_transform_list:
         mov = apply_transform(
             fix, mov, fix_spacing, mov_spacing,
             transform_list=static_transform_list,
             fix_origin=fix_origin,
             mov_origin=mov_origin,
@@ -416,17 +500,21 @@
             mask=fix_mask,
             **fix_kwargs,
         )
     print(f'{time.ctime(time.time())} found {len(fix_spots)} fixed spots',
           flush=True)
     if len(fix_spots) < fix_spots_count_threshold:
         print(f'{time.ctime(time.time())}',
-              'insufficient fixed spots found, returning default',
+              'insufficient fixed spots found',
               flush=True)
-        return default
+        if safeguard_exceptions:
+            raise ValueError('fix spot detection safeguard failed')
+        else:
+            print('returning default', flush=True)
+            return default
 
     # get mov spots
     print(f'{time.ctime(time.time())} computing moving spots', flush=True)
     if mov_spots is None:
         mov_kwargs = {
             'num_sigma':num_sigma,
             'exclude_border':cc_radius,
@@ -435,22 +523,25 @@
         print(f'{time.ctime(time.time())} moving spots detection using',
               mov_kwargs, flush=True)
         mov_spots = features.blob_detection(
             mov, blob_sizes[0], blob_sizes[1],
             mask=mov_mask,
             **mov_kwargs,
         )
-
     print(f'{time.ctime(time.time())} found {len(mov_spots)} moving spots',
           flush=True)
     if len(mov_spots) < mov_spots_count_threshold:
         print(f'{time.ctime(time.time())}',
-              'insufficient moving spots found, returning default',
+              'insufficient moving spots found',
               flush=True)
-        return default
+        if safeguard_exceptions:
+            raise ValueError('mov spot detection safeguard failed')
+        else:
+            print('returning default', flush=True)
+            return default
 
     # sort
     print(f'{time.ctime(time.time())} sorting spots', flush=True)
     sort_idx = np.argsort(fix_spots[:, 3])[::-1]
     fix_spots = fix_spots[sort_idx, :3][:nspots]
     sort_idx = np.argsort(mov_spots[:, 3])[::-1]
     mov_spots = mov_spots[sort_idx, :3][:nspots]
@@ -477,17 +568,21 @@
         correlations, match_threshold,
         max_distance=max_spot_match_distance,
     )
     print(f'{time.ctime(time.time())} {len(fix_spots)} - {len(mov_spots)} matched spots',
           flush=True)
     if len(fix_spots) < point_matches_threshold or len(mov_spots) < point_matches_threshold:
         print(f'{time.ctime(time.time())}',
-              'insufficient point matches found, returning default',
+              'insufficient point matches found',
               flush=True)
-        return default
+        if safeguard_exceptions:
+            raise ValueError('point matches safeguard failed')
+        else:
+            print('returning default', flush=True)
+            return default
 
     # align
     print(f'{time.ctime(time.time())}',
           'Found enough spots to estimate the affine',
           'fix:', len(fix_spots), ',',
           'moving:', len(mov_spots),
           flush=True)
@@ -497,17 +592,21 @@
         confidence=0.999,
         **kwargs,
     )
 
     # ensure affine is sensible
     if np.any( np.abs(np.diag(Aff) - 1) > diagonal_constraint ):
         print(f'{time.ctime(time.time())}',
-              'Degenerate affine produced, returning default',
+              'Degenerate affine produced',
               flush=True)
-        return default
+        if safeguard_exceptions:
+            raise ValueError('diagonal_constraint safeguard failed')
+        else:
+            print('returning default', flush=True)
+            return default
 
     # augment matrix and return
     affine = np.eye(fix.ndim + 1)
     affine[:fix.ndim, :] = Aff
     return affine
 
 
@@ -581,25 +680,39 @@
         Can be specified per axis.
 
     alignment_spacing : float (default: None)
         Fixed and moving images are skip sampled to a voxel spacing
         as close as possible to this value. Intended for very fast
         simple alignments (e.g. low amplitude motion correction)
 
-    fix_mask : binary ndarray (default: None)
+    fix_mask : ndarray, tuple of floats, or function (default: None)
         A mask limiting metric evaluation region of the fixed image
-        Assumed to have the same domain as the fixed image, though sampling
-        can be different. I.e. the origin and span are the same (in phyiscal
-        units) but the number of voxels can be different.
+        If an nd-array, any non-zero value is considered foreground and any
+        zero value is considered background. If a tuple of floats, any voxel
+        with value in the tuple is considered background. If a function, it
+        must take a single nd-array argument as input and return an array
+        of the same shape as the input but with dtype bool.
+
+        If an nd-array, it is assumed to have the same domain as the fixed
+        image, though sampling can be different. I.e. the origin and span
+        are the same (in phyiscal units) but the number of voxels can
+        be different.
 
-    mov_mask : binary ndarray (default: None)
+    mov_mask : ndarray, tuple of floats, or function (default: None)
         A mask limiting metric evaluation region of the moving image
-        Assumed to have the same domain as the moving image, though sampling
-        can be different. I.e. the origin and span are the same (in phyiscal
-        units) but the number of voxels can be different.
+        If an nd-array, any non-zero value is considered foreground and any
+        zero value is considered background. If a tuple of floats, any voxel
+        with value in the tuple is considered background. If a function, it
+        must take a single nd-array argument as input and return an array
+        of the same shape as the input but with dtype bool.
+
+        If an nd-array, it is assumed to have the same domain as the fixed
+        image, though sampling can be different. I.e. the origin and span
+        are the same (in phyiscal units) but the number of voxels can
+        be different.
 
     fix_origin : 1d array (default: None)
         Origin of the fixed image.
         Length must equal `fix.ndim`
 
     mov_origin : 1d array (default: None)
         Origin of the moving image.
@@ -666,14 +779,18 @@
     # format static transform data explicitly
     a, b = format_static_transform_data(
         static_transform_list, fix, fix_spacing, fix_origin,
     )
     static_transform_spacing = a
     static_transform_origin = b
 
+    # realize masks as arrays
+    fix_mask = realize_mask(fix, fix_mask)
+    mov_mask = realize_mask(mov, mov_mask)
+
     # skip sample and determine mask spacings
     X = apply_alignment_spacing(
         fix, mov,
         fix_mask, mov_mask,
         fix_spacing, mov_spacing,
         alignment_spacing,
     )
@@ -820,25 +937,39 @@
         is initialized with that transform.
 
     alignment_spacing : float (default: None)
         Fixed and moving images are skip sampled to a voxel spacing
         as close as possible to this value. Intended for very fast
         simple alignments (e.g. low amplitude motion correction)
 
-    fix_mask : binary ndarray (default: None)
+    fix_mask : ndarray, tuple of floats, or function (default: None)
         A mask limiting metric evaluation region of the fixed image
-        Assumed to have the same domain as the fixed image, though sampling
-        can be different. I.e. the origin and span are the same (in phyiscal
-        units) but the number of voxels can be different.
+        If an nd-array, any non-zero value is considered foreground and any
+        zero value is considered background. If a tuple of floats, any voxel
+        with value in the tuple is considered background. If a function, it
+        must take a single nd-array argument as input and return an array
+        of the same shape as the input but with dtype bool.
+
+        If an nd-array, it is assumed to have the same domain as the fixed
+        image, though sampling can be different. I.e. the origin and span
+        are the same (in phyiscal units) but the number of voxels can
+        be different.
 
-    mov_mask : binary ndarray (default: None)
+    mov_mask : ndarray, tuple of floats, or function (default: None)
         A mask limiting metric evaluation region of the moving image
-        Assumed to have the same domain as the moving image, though sampling
-        can be different. I.e. the origin and span are the same (in phyiscal
-        units) but the number of voxels can be different.
+        If an nd-array, any non-zero value is considered foreground and any
+        zero value is considered background. If a tuple of floats, any voxel
+        with value in the tuple is considered background. If a function, it
+        must take a single nd-array argument as input and return an array
+        of the same shape as the input but with dtype bool.
+
+        If an nd-array, it is assumed to have the same domain as the fixed
+        image, though sampling can be different. I.e. the origin and span
+        are the same (in phyiscal units) but the number of voxels can
+        be different.
 
     fix_origin : 1d array (default: None)
         Origin of the fixed image.
         Length must equal `fix.ndim`
 
     mov_origin : 1d array (default: None)
         Origin of the moving image.
@@ -873,14 +1004,18 @@
     # format static transform data explicitly
     a, b = format_static_transform_data(
         static_transform_list, fix, fix_spacing, fix_origin,
     )
     static_transform_spacing = a
     static_transform_origin = b
 
+    # realize masks
+    fix_mask = realize_mask(fix, fix_mask)
+    mov_mask = realize_mask(mov, mov_mask)
+
     # skip sample and convert inputs to sitk images
     X = apply_alignment_spacing(
         fix, mov,
         fix_mask, mov_mask,
         fix_spacing, mov_spacing,
         alignment_spacing,
     )
@@ -1011,25 +1146,39 @@
         at the requested 100.0 units control point spacing.
     
     alignment_spacing : float (default: None)
         Fixed and moving images are skip sampled to a voxel spacing
         as close as possible to this value. Intended for very fast
         simple alignments (e.g. low amplitude motion correction)
 
-    fix_mask : binary ndarray (default: None)
+    fix_mask : ndarray, tuple of floats, or function (default: None)
         A mask limiting metric evaluation region of the fixed image
-        Assumed to have the same domain as the fixed image, though sampling
-        can be different. I.e. the origin and span are the same (in phyiscal
-        units) but the number of voxels can be different.
+        If an nd-array, any non-zero value is considered foreground and any
+        zero value is considered background. If a tuple of floats, any voxel
+        with value in the tuple is considered background. If a function, it
+        must take a single nd-array argument as input and return an array
+        of the same shape as the input but with dtype bool.
+
+        If an nd-array, it is assumed to have the same domain as the fixed
+        image, though sampling can be different. I.e. the origin and span
+        are the same (in phyiscal units) but the number of voxels can
+        be different.
 
-    mov_mask : binary ndarray (default: None)
+    mov_mask : ndarray, tuple of floats, or function (default: None)
         A mask limiting metric evaluation region of the moving image
-        Assumed to have the same domain as the moving image, though sampling
-        can be different. I.e. the origin and span are the same (in phyiscal
-        units) but the number of voxels can be different.
+        If an nd-array, any non-zero value is considered foreground and any
+        zero value is considered background. If a tuple of floats, any voxel
+        with value in the tuple is considered background. If a function, it
+        must take a single nd-array argument as input and return an array
+        of the same shape as the input but with dtype bool.
+
+        If an nd-array, it is assumed to have the same domain as the fixed
+        image, though sampling can be different. I.e. the origin and span
+        are the same (in phyiscal units) but the number of voxels can
+        be different.
 
     fix_origin : 1d array (default: None)
         Origin of the fixed image.
         Length must equal `fix.ndim`
 
     mov_origin : 1d array (default: None)
         Origin of the moving image.
@@ -1070,14 +1219,18 @@
     # format static transform data explicitly
     a, b = format_static_transform_data(
         static_transform_list, fix, fix_spacing, fix_origin,
     )
     static_transform_spacing = a
     static_transform_origin = b
 
+    # realize masks
+    fix_mask = realize_mask(fix, fix_mask)
+    mov_mask = realize_mask(mov, mov_mask)
+
     # skip sample and convert inputs to sitk images
     X = apply_alignment_spacing(
         fix, mov,
         fix_mask, mov_mask,
         fix_spacing, mov_spacing,
         alignment_spacing,
     )
@@ -1201,25 +1354,39 @@
         'rigid' : run `affine_align` with `rigid=True`
         'affine' : run `affine_align`
         'deform' : run `deformable_align`
         For each tuple, the dict specifies the arguments to that alignment function
         Arguments specified here override any global arguments given through kwargs
         for their specific step only.
 
-    fix_mask : binary ndarray (default: None)
+    fix_mask : ndarray, tuple of floats, or function (default: None)
         A mask limiting metric evaluation region of the fixed image
-        Assumed to have the same domain as the fixed image, though sampling
-        can be different. I.e. the origin and span are the same (in phyiscal
-        units) but the number of voxels can be different.
+        If an nd-array, any non-zero value is considered foreground and any
+        zero value is considered background. If a tuple of floats, any voxel
+        with value in the tuple is considered background. If a function, it
+        must take a single nd-array argument as input and return an array
+        of the same shape as the input but with dtype bool.
+
+        If an nd-array, it is assumed to have the same domain as the fixed
+        image, though sampling can be different. I.e. the origin and span
+        are the same (in phyiscal units) but the number of voxels can
+        be different.
 
-    mov_mask : binary ndarray (default: None)
+    mov_mask : ndarray, tuple of floats, or function (default: None)
         A mask limiting metric evaluation region of the moving image
-        Assumed to have the same domain as the moving image, though sampling
-        can be different. I.e. the origin and span are the same (in phyiscal
-        units) but the number of voxels can be different.
+        If an nd-array, any non-zero value is considered foreground and any
+        zero value is considered background. If a tuple of floats, any voxel
+        with value in the tuple is considered background. If a function, it
+        must take a single nd-array argument as input and return an array
+        of the same shape as the input but with dtype bool.
+
+        If an nd-array, it is assumed to have the same domain as the fixed
+        image, though sampling can be different. I.e. the origin and span
+        are the same (in phyiscal units) but the number of voxels can
+        be different.
 
     fix_origin : 1d array (default: None)
         Origin of the fixed image.
         Length must equal `fix.ndim`
 
     mov_origin : 1d array (default: None)
         Origin of the moving image.
```

### Comparing `bigstream-1.3.0/bigstream/application_pipelines.py` & `bigstream-1.4.0/bigstream/application_pipelines.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.3.0/bigstream/configure_irm.py` & `bigstream-1.4.0/bigstream/configure_irm.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,43 @@
     'CWS':sitk.sitkCosineWindowedSinc,
     'WWS':sitk.sitkWelchWindowedSinc,
     'LWS':sitk.sitkLanczosWindowedSinc,
     'BWS':sitk.sitkBlackmanWindowedSinc,
 }
 
 
+# default optimizer args
+default_its = 100
+default_step = 0.25
+default_optimizer_args = {
+    'A':{'simplexDelta':1., 'numberOfIterations':default_its},
+    'CGLS':{'learningRate':default_step, 'numberOfIterations':default_its},
+    'E':{'numberOfSteps':default_its},
+    'GD':{'learningRate':default_step, 'numberOfIterations':default_its},
+    'GDLS':{'learningRate':default_step, 'numberOfIterations':default_its},
+    'LBFGS2':{},
+    'LBFGSB':{},
+    'OPOE':{},
+    'P':{},
+    'RSGD':{'learningRate':default_step, 'minStep':0., 'numberOfIterations':default_its},
+}
+
+
+# default metric args
+# only one metric has a required parameter, so this is a bit silly
+default_metric_args = {
+    'ANC':{'radius':12},
+    'C':{},
+    'D':{},
+    'JHMI':{},
+    'MMI':{},
+    'MS':{},
+}
+
+
 def configure_irm(
     metric='MMI',
     optimizer='RSGD',
     sampling='NONE',
     interpolator='1',
     shrink_factors=(1,),
     smooth_sigmas=(0,),
@@ -153,14 +182,15 @@
         'ANC':irm.SetMetricAsANTSNeighborhoodCorrelation,
         'C':irm.SetMetricAsCorrelation,
         'D':irm.SetMetricAsDemons,
         'JHMI':irm.SetMetricAsJointHistogramMutualInformation,
         'MMI':irm.SetMetricAsMattesMutualInformation,
         'MS':irm.SetMetricAsMeanSquares,
     }
+    metric_args = {**default_metric_args[metric], **metric_args}
     metric_switch[metric](**metric_args)
 
     # sampling switch
     sampling_switch = {
         'NONE':irm.NONE,
         'REGULAR':irm.REGULAR,
         'RANDOM':irm.RANDOM,
@@ -178,14 +208,15 @@
         'GDLS':irm.SetOptimizerAsGradientDescentLineSearch,
         'LBFGS2':irm.SetOptimizerAsLBFGS2,
         'LBFGSB':irm.SetOptimizerAsLBFGSB,
         'OPOE':irm.SetOptimizerAsOnePlusOneEvolutionary,
         'P':irm.SetOptimizerAsPowell,
         'RSGD':irm.SetOptimizerAsRegularStepGradientDescent,
     }
+    optimizer_args = {**default_optimizer_args[optimizer], **optimizer_args}
     optimizer_switch[optimizer](**optimizer_args)
     irm.SetOptimizerScalesFromPhysicalShift()
     if optimizer == 'E':
         irm.SetOptimizerScales(exhaustive_step_sizes)
 
     # set pyramid
     irm.SetShrinkFactorsPerLevel(shrink_factors)
```

### Comparing `bigstream-1.3.0/bigstream/distributed_align.py` & `bigstream-1.4.0/bigstream/distributed_align.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.3.0/bigstream/distributed_io_utility.py` & `bigstream-1.4.0/bigstream/distributed_io_utility.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.3.0/bigstream/distributed_transform.py` & `bigstream-1.4.0/bigstream/distributed_transform.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.3.0/bigstream/features.py` & `bigstream-1.4.0/bigstream/features.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.3.0/bigstream/io_utility.py` & `bigstream-1.4.0/bigstream/io_utility.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.3.0/bigstream/level_set.py` & `bigstream-1.4.0/bigstream/level_set.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.3.0/bigstream/metrics.py` & `bigstream-1.4.0/bigstream/metrics.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.3.0/bigstream/motion_correct.py` & `bigstream-1.4.0/bigstream/motion_correct.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.3.0/bigstream/piecewise_align.py` & `bigstream-1.4.0/bigstream/piecewise_align.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import numpy as np
 import time
 from itertools import product
 from scipy.interpolate import LinearNDInterpolator
 from dask.distributed import as_completed, wait
 from ClusterWrap.decorator import cluster
 import bigstream.utility as ut
+from bigstream.align import realize_mask
 from bigstream.align import alignment_pipeline
 from bigstream.transform import apply_transform, compose_transform_list
 from bigstream.transform import apply_transform_to_coordinates
 from bigstream.transform import compose_transforms
 from distributed import Lock, MultiLock
 
 
@@ -73,25 +74,39 @@
 
     blocksize : iterable
         The shape of blocks in voxels
 
     overlap : float in range [0, 1] (default: 0.5)
         Block overlap size as a percentage of block size
 
-    fix_mask : binary ndarray (default: None)
+    fix_mask : ndarray, tuple of floats, or function (default: None)
         A mask limiting metric evaluation region of the fixed image
-        Assumed to have the same domain as the fixed image, though sampling
-        can be different. I.e. the origin and span are the same (in physical
-        units) but the number of voxels can be different.
+        If an nd-array, any non-zero value is considered foreground and any
+        zero value is considered background. If a tuple of floats, any voxel
+        with value in the tuple is considered background. If a function, it
+        must take a single nd-array argument as input and return an array
+        of the same shape as the input but with dtype bool.
+
+        If an nd-array, it is assumed to have the same domain as the fixed
+        image, though sampling can be different. I.e. the origin and span
+        are the same (in phyiscal units) but the number of voxels can
+        be different.
 
-    mov_mask : binary ndarray (default: None)
+    mov_mask : ndarray, tuple of floats, or function (default: None)
         A mask limiting metric evaluation region of the moving image
-        Assumed to have the same domain as the moving image, though sampling
-        can be different. I.e. the origin and span are the same (in physical
-        units) but the number of voxels can be different.
+        If an nd-array, any non-zero value is considered foreground and any
+        zero value is considered background. If a tuple of floats, any voxel
+        with value in the tuple is considered background. If a function, it
+        must take a single nd-array argument as input and return an array
+        of the same shape as the input but with dtype bool.
+
+        If an nd-array, it is assumed to have the same domain as the fixed
+        image, though sampling can be different. I.e. the origin and span
+        are the same (in phyiscal units) but the number of voxels can
+        be different.
 
     static_transform_list : list of numpy arrays (default: [])
         Transforms applied to moving image before applying query transform
         Assumed to have the same domain as the fixed image, though sampling
         can be different. I.e. the origin and span are the same (in physical
         units) but the number of voxels can be different.
 
@@ -149,19 +164,19 @@
     zarr_blocks = (128,) * fix.ndim
     fix_zarr_path = temporary_directory.name + '/fix.zarr'
     mov_zarr_path = temporary_directory.name + '/mov.zarr'
     fix_mask_zarr_path = temporary_directory.name + '/fix_mask.zarr'
     mov_mask_zarr_path = temporary_directory.name + '/mov_mask.zarr'
     fix_zarr = ut.numpy_to_zarr(fix, zarr_blocks, fix_zarr_path)
     mov_zarr = ut.numpy_to_zarr(mov, zarr_blocks, mov_zarr_path)
-    fix_mask_zarr = None
-    if fix_mask is not None:
+    fix_mask_zarr = fix_mask
+    if isinstance(fix_mask, np.ndarray):
         fix_mask_zarr = ut.numpy_to_zarr(fix_mask, zarr_blocks, fix_mask_zarr_path)
-    mov_mask_zarr = None
-    if mov_mask is not None:
+    mov_mask_zarr = mov_mask
+    if isinstance(mov_mask, np.ndarray):
         mov_mask_zarr = ut.numpy_to_zarr(mov_mask, zarr_blocks, mov_mask_zarr_path)
 
     # zarr files for initial deformations
     new_list = []
     zarr_blocks = (128,) * fix.ndim + (fix.ndim,)
     for iii, transform in enumerate(static_transform_list):
         if len(transform.shape) > fix.ndim:  # fields are always fix.ndim + 1
@@ -196,15 +211,15 @@
         start = blocksize * (i, j, k) - overlaps
         stop = start + blocksize + 2 * overlaps
         start = np.maximum(0, start)
         stop = np.minimum(fix.shape, stop)
         coords = tuple(slice(x, y) for x, y in zip(start, stop))
 
         foreground = True
-        if fix_mask is not None:
+        if isinstance(fix_mask, np.ndarray):
             start = blocksize * (i, j, k)
             stop = start + blocksize
             ratio = np.array(fix_mask.shape) / fix.shape
             start = np.round( ratio * start ).astype(int)
             stop = np.round( ratio * stop ).astype(int)
             mask_crop = fix_mask[tuple(slice(a, b) for a, b in zip(start, stop))]
             if not np.sum(mask_crop) / np.prod(mask_crop.shape) >= foreground_percentage:
@@ -279,29 +294,37 @@
         mov_origin = mov_start * mov_spacing - fix_block_coords_phys[0]
         ##################################################################
 
 
         ################ Read fix and moving data ########################
         fix = fix_zarr[fix_slices]
         mov = mov_zarr[mov_slices]
-        fix_mask, mov_mask = None, None
-        if fix_mask_zarr is not None:
+        fix_mask, mov_mask = fix_mask_zarr, mov_mask_zarr
+        if isinstance(fix_mask_zarr, zarr.core.Array):
             ratio = np.array(fix_mask_zarr.shape) / fix_zarr.shape
             start = np.round( ratio * fix_block_coords[0] ).astype(int)
             stop = np.round( ratio * (fix_block_coords[-1] + 1) ).astype(int)
             fix_mask_slices = tuple(slice(a, b) for a, b in zip(start, stop))
             fix_mask = fix_mask_zarr[fix_mask_slices]
-        if mov_mask_zarr is not None:
+        if isinstance(mov_mask_zarr, zarr.core.Array):
             ratio = np.array(mov_mask_zarr.shape) / mov_zarr.shape
             start = np.round( ratio * mov_start ).astype(int)
             stop = np.round( ratio * mov_stop ).astype(int)
             mov_mask_slices = tuple(slice(a, b) for a, b in zip(start, stop))
             mov_mask = mov_mask_zarr[mov_mask_slices]
         ##################################################################
 
+        
+        ################ Parse steps #####################################
+        # we don't want exceptions in the distributed context
+        for step in steps:
+            if step[0] == 'ransac':
+                step[1]['safeguard_exceptions'] = False
+        ##################################################################
+
 
         ############################ Align ###############################
         # run alignment pipeline
         transform = alignment_pipeline(
             fix, mov, fix_spacing, mov_spacing, steps,
             fix_mask=fix_mask, mov_mask=mov_mask,
             mov_origin=mov_origin,
```

### Comparing `bigstream-1.3.0/bigstream/piecewise_transform.py` & `bigstream-1.4.0/bigstream/piecewise_transform.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.3.0/bigstream/stitch.py` & `bigstream-1.4.0/bigstream/stitch.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.3.0/bigstream/transform.py` & `bigstream-1.4.0/bigstream/transform.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.3.0/bigstream/utility.py` & `bigstream-1.4.0/bigstream/utility.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.3.0/bigstream.egg-info/SOURCES.txt` & `bigstream-1.4.0/bigstream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigstream-1.3.0/setup.py` & `bigstream-1.4.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="bigstream",
-    version="1.3.0",
+    version="1.4.0",
     author="Greg M. Fleishman",
     author_email="greg.nli10me@gmail.com",
     description="Tools for distributed alignment of massive images",
     url="https://github.com/JaneliaScicomp/bigstream",
     license="BSD-3",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

