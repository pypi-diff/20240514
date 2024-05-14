# Comparing `tmp/scores-0.72.tar.gz` & `tmp/scores-0.8.tar.gz`

## Comparing `scores-0.72.tar` & `scores-0.8.tar`

### file list

```diff
@@ -1,52 +1,51 @@
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 scores-0.72/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 scores-0.72/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 scores-0.72/environment.yml
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scores-0.72/mkdocs.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.72/py.typed
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scores-0.72/readthedocs.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.72/setup.cfg
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 scores-0.72/.binder/postBuild
--rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 scores-0.72/.binder/requirements.txt
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scores-0.72/.github/pull_request_template.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 scores-0.72/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 scores-0.72/.github/ISSUE_TEMPLATE/new_score.md
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scores-0.72/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 scores-0.72/.github/workflows/python-app.yml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 scores-0.72/.github/workflows/run-pre-commit.yml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 scores-0.72/src/scores/__init__.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 scores-0.72/src/scores/functions.py
--rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 scores-0.72/src/scores/sample_data.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 scores-0.72/src/scores/typing.py
--rw-r--r--   0        0        0    15729 2020-02-02 00:00:00.000000 scores-0.72/src/scores/utils.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 scores-0.72/src/scores/categorical/__init__.py
--rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 scores-0.72/src/scores/categorical/binary_impl.py
--rw-r--r--   0        0        0    14019 2020-02-02 00:00:00.000000 scores-0.72/src/scores/categorical/contingency_impl.py
--rw-r--r--   0        0        0    11009 2020-02-02 00:00:00.000000 scores-0.72/src/scores/categorical/multicategorical_impl.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 scores-0.72/src/scores/continuous/__init__.py
--rw-r--r--   0        0        0    18015 2020-02-02 00:00:00.000000 scores-0.72/src/scores/continuous/flip_flop_impl.py
--rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 scores-0.72/src/scores/continuous/murphy_impl.py
--rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 scores-0.72/src/scores/continuous/quantile_loss_impl.py
--rw-r--r--   0        0        0    16768 2020-02-02 00:00:00.000000 scores-0.72/src/scores/continuous/standard_impl.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 scores-0.72/src/scores/pandas/__init__.py
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 scores-0.72/src/scores/pandas/continuous.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 scores-0.72/src/scores/pandas/typing.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 scores-0.72/src/scores/probability/__init__.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 scores-0.72/src/scores/probability/brier_impl.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 scores-0.72/src/scores/probability/checks.py
--rw-r--r--   0        0        0    37852 2020-02-02 00:00:00.000000 scores-0.72/src/scores/probability/crps_impl.py
--rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 scores-0.72/src/scores/probability/roc_impl.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 scores-0.72/src/scores/processing/__init__.py
--rw-r--r--   0        0        0    12458 2020-02-02 00:00:00.000000 scores-0.72/src/scores/processing/discretise.py
--rw-r--r--   0        0        0    29482 2020-02-02 00:00:00.000000 scores-0.72/src/scores/processing/isoreg_impl.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 scores-0.72/src/scores/processing/matching.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 scores-0.72/src/scores/processing/cdf/__init__.py
--rw-r--r--   0        0        0    16430 2020-02-02 00:00:00.000000 scores-0.72/src/scores/processing/cdf/cdf_functions.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 scores-0.72/src/scores/stats/__init__.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scores-0.72/src/scores/stats/statistical_tests/__init__.py
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 scores-0.72/src/scores/stats/statistical_tests/acovf.py
--rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 scores-0.72/src/scores/stats/statistical_tests/diebold_mariano_impl.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 scores-0.72/.gitignore
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 scores-0.72/LICENSE
--rw-r--r--   0        0        0     6130 2020-02-02 00:00:00.000000 scores-0.72/README.md
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 scores-0.72/pyproject.toml
--rw-r--r--   0        0        0     8853 2020-02-02 00:00:00.000000 scores-0.72/PKG-INFO
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 scores-0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 scores-0.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 scores-0.8/environment.yml
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scores-0.8/mkdocs.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.8/py.typed
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scores-0.8/readthedocs.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.8/setup.cfg
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 scores-0.8/.binder/postBuild
+-rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 scores-0.8/.binder/requirements.txt
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 scores-0.8/.github/pull_request_template.md
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 scores-0.8/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 scores-0.8/.github/ISSUE_TEMPLATE/new_score.md
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 scores-0.8/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 scores-0.8/.github/workflows/run-pre-commit.yml
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 scores-0.8/src/scores/__init__.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 scores-0.8/src/scores/functions.py
+-rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 scores-0.8/src/scores/sample_data.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 scores-0.8/src/scores/typing.py
+-rw-r--r--   0        0        0    12735 2020-02-02 00:00:00.000000 scores-0.8/src/scores/utils.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 scores-0.8/src/scores/categorical/__init__.py
+-rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 scores-0.8/src/scores/categorical/binary_impl.py
+-rw-r--r--   0        0        0    21466 2020-02-02 00:00:00.000000 scores-0.8/src/scores/categorical/contingency_impl.py
+-rw-r--r--   0        0        0    11009 2020-02-02 00:00:00.000000 scores-0.8/src/scores/categorical/multicategorical_impl.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 scores-0.8/src/scores/continuous/__init__.py
+-rw-r--r--   0        0        0    18015 2020-02-02 00:00:00.000000 scores-0.8/src/scores/continuous/flip_flop_impl.py
+-rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 scores-0.8/src/scores/continuous/murphy_impl.py
+-rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 scores-0.8/src/scores/continuous/quantile_loss_impl.py
+-rw-r--r--   0        0        0    16768 2020-02-02 00:00:00.000000 scores-0.8/src/scores/continuous/standard_impl.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 scores-0.8/src/scores/pandas/__init__.py
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 scores-0.8/src/scores/pandas/continuous.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 scores-0.8/src/scores/pandas/typing.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 scores-0.8/src/scores/probability/__init__.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 scores-0.8/src/scores/probability/brier_impl.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 scores-0.8/src/scores/probability/checks.py
+-rw-r--r--   0        0        0    37967 2020-02-02 00:00:00.000000 scores-0.8/src/scores/probability/crps_impl.py
+-rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 scores-0.8/src/scores/probability/roc_impl.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 scores-0.8/src/scores/processing/__init__.py
+-rw-r--r--   0        0        0    12458 2020-02-02 00:00:00.000000 scores-0.8/src/scores/processing/discretise.py
+-rw-r--r--   0        0        0    29482 2020-02-02 00:00:00.000000 scores-0.8/src/scores/processing/isoreg_impl.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 scores-0.8/src/scores/processing/matching.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 scores-0.8/src/scores/processing/cdf/__init__.py
+-rw-r--r--   0        0        0    16430 2020-02-02 00:00:00.000000 scores-0.8/src/scores/processing/cdf/cdf_functions.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 scores-0.8/src/scores/stats/__init__.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scores-0.8/src/scores/stats/statistical_tests/__init__.py
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 scores-0.8/src/scores/stats/statistical_tests/acovf.py
+-rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 scores-0.8/src/scores/stats/statistical_tests/diebold_mariano_impl.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 scores-0.8/.gitignore
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 scores-0.8/LICENSE
+-rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 scores-0.8/README.md
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 scores-0.8/pyproject.toml
+-rw-r--r--   0        0        0     9392 2020-02-02 00:00:00.000000 scores-0.8/PKG-INFO
```

### Comparing `scores-0.72/.pre-commit-config.yaml` & `scores-0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scores-0.72/CODE_OF_CONDUCT.md` & `scores-0.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scores-0.72/readthedocs.yaml` & `scores-0.8/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `scores-0.72/.binder/requirements.txt` & `scores-0.8/.binder/requirements.txt`

 * *Files identical despite different names*

### Comparing `scores-0.72/.github/ISSUE_TEMPLATE/feature_request.md` & `scores-0.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ---
-name: Feature request
+name: Request a feature, improvement or correction
 about: Suggest an idea for this project
 title: ''
 labels: ''
 assignees: ''
 
 ---
```

### Comparing `scores-0.72/.github/workflows/python-app.yml` & `scores-0.8/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `scores-0.72/.github/workflows/run-pre-commit.yml` & `scores-0.8/.github/workflows/run-pre-commit.yml`

 * *Files identical despite different names*

### Comparing `scores-0.72/src/scores/__init__.py` & `scores-0.8/src/scores/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import scores.functions
 import scores.pandas
 import scores.probability
 import scores.processing
 import scores.sample_data
 import scores.stats.statistical_tests  # noqa: F401
 
-__version__ = "v0.72"
+__version__ = "0.8"
 
 __all__ = [
     "scores.categorical",
     "scores.contingency",
     "scores.continuous",
     "scores.functions",
     "scores.pandas",
```

### Comparing `scores-0.72/src/scores/functions.py` & `scores-0.8/src/scores/functions.py`

 * *Files identical despite different names*

### Comparing `scores-0.72/src/scores/sample_data.py` & `scores-0.8/src/scores/sample_data.py`

 * *Files identical despite different names*

### Comparing `scores-0.72/src/scores/typing.py` & `scores-0.8/src/scores/typing.py`

 * *Files identical despite different names*

### Comparing `scores-0.72/src/scores/utils.py` & `scores-0.8/src/scores/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,31 +16,22 @@
 You are requesting to reduce or preserve every dimension by specifying the string 'all'.
 In this case, 'all' is also a named dimension in your data, leading to an ambiguity.
 In order to reduce or preserve the named data dimension, specify ['all'] as a list item
 rather than relying on string interpretation. The program will continue to interpret the
 string as an instruction to reduce or preserve every dimension.
 """
 
-ERROR_SPECIFIED_NONPRESENT_PRESERVE_DIMENSION = """
-You are requesting to preserve a dimension which does not appear in your data (fcst or obs).
-It is ambiguous how to proceed therefore an exception has been raised instead.
-"""
 
-ERROR_SPECIFIED_NONPRESENT_PRESERVE_DIMENSION2 = """
+ERROR_SPECIFIED_NONPRESENT_PRESERVE_DIMENSION = """
 You are requesting to preserve a dimension which does not appear in your data 
 (fcst, obs or weights). It is ambiguous how to proceed therefore an exception has been
 raised instead.
 """
 
 ERROR_SPECIFIED_NONPRESENT_REDUCE_DIMENSION = """
-You are requesting to reduce a dimension which does not appear in your data (fcst or obs).
-It is ambiguous how to proceed therefore an exception has been raised instead.
-"""
-
-ERROR_SPECIFIED_NONPRESENT_REDUCE_DIMENSION2 = """
 You are requesting to reduce a dimension which does not appear in your data
 (fcst, obs or weights). It is ambiguous how to proceed therefore an exception has been 
 raised instead.
 """
 
 ERROR_OVERSPECIFIED_PRESERVE_REDUCE = """
 You have specified both preserve_dims and reduce_dims. This method doesn't know how
@@ -55,188 +46,119 @@
     """
 
 
 def gather_dimensions(  # pylint: disable=too-many-branches
     fcst_dims: Iterable[Hashable],
     obs_dims: Iterable[Hashable],
     *,  # Force keywords arguments to be keyword-only
+    weights_dims: Optional[Iterable[Hashable]] = None,
     reduce_dims: Optional[FlexibleDimensionTypes] = None,
     preserve_dims: Optional[FlexibleDimensionTypes] = None,
+    score_specific_fcst_dims: Optional[FlexibleDimensionTypes] = None,
 ) -> set[Hashable]:
     """
     Establish which dimensions to reduce when calculating errors but before taking means.
 
-    Note: `scores.utils.gather_dimensions` and `scores.utils.gather_dimensions2` will be
-    integrated at some point in the future. `scores.utils.gather_dimensions2` offers
-    more comprehensive and less restrictive dimension checking and should be preferred in
-    the meantime. See `scores.probability.crps_cdf` for an example of
-    `scores.utils.gather_dimensions2` usage.
-
-    Args:
-        fcst_dims: Forecast dimensions inputs
-        obs_dims: Observation dimensions inputs.
-        reduce_dims: Dimensions to reduce.
-        preserve_dims: Dimensions to preserve.
-
-    Returns:
-        Dimensions based on optional args.
-    Raises:
-        ValueError: When `preserve_dims and `reduce_dims` are both specified.
-
-    See also:
-        `scores.utils.gather_dimensions2`
-    """
-
-    all_dims = set(fcst_dims).union(set(obs_dims))
-
-    # Handle error conditions related to specified dimensions
-    if preserve_dims is not None and reduce_dims is not None:
-        raise ValueError(ERROR_OVERSPECIFIED_PRESERVE_REDUCE)
-
-    # Handle error conditions related to specified dimensions
-    specified = preserve_dims or reduce_dims
-    if specified == "all":
-        if "all" in all_dims:
-            warnings.warn(WARN_ALL_DATA_CONFLICT_MSG)
-    elif specified is not None:
-        if isinstance(specified, str):
-            specified = [specified]
-
-        if not set(specified).issubset(all_dims):
-            if preserve_dims is not None:
-                raise ValueError(ERROR_SPECIFIED_NONPRESENT_PRESERVE_DIMENSION)
-            raise ValueError(ERROR_SPECIFIED_NONPRESENT_REDUCE_DIMENSION)
-
-    # Handle preserve_dims case
-    if preserve_dims is not None:
-        if preserve_dims == "all":
-            return set([])
-
-        if isinstance(preserve_dims, str):
-            preserve_dims = [preserve_dims]
-
-        reduce_dims = set(all_dims).difference(preserve_dims)
-
-    # Handle reduce all
-    elif reduce_dims == "all":
-        reduce_dims = set(all_dims)
-
-    # Handle is reduce_dims and preserve_dims are both None
-    if reduce_dims is None and preserve_dims is None:
-        reduce_dims = set(all_dims)
-
-    # Handle reduce by string
-    elif isinstance(reduce_dims, str):
-        reduce_dims = set([reduce_dims])
-
-    # Turn into a set if needed
-    assert reduce_dims is not None  # nosec - this is just to modify type hinting
-    reduce_dims = set(reduce_dims)
-
-    # Reduce by list is the default so no handling needed
-    return reduce_dims
-
-
-def gather_dimensions2(  # pylint: disable=too-many-branches
-    fcst: xr.DataArray,
-    obs: xr.DataArray,
-    *,  # Force keywords arguments to be keyword-only
-    weights: Optional[xr.DataArray] = None,
-    reduce_dims: Optional[FlexibleDimensionTypes] = None,
-    preserve_dims: Optional[FlexibleDimensionTypes] = None,
-    special_fcst_dims: Optional[FlexibleDimensionTypes] = None,
-) -> set[Hashable]:
-    """
-    Performs standard dimensions checks for inputs of functions that calculate (mean) scores.
-    Returns a set of the dimensions to reduce.
-
-    Note: `scores.utils.gather_dimensions` and `scores.utils.gather_dimensions2` will be
-    integrated at some point in the future. `scores.utils.gather_dimensions2` offers
-    more comprehensive and less restrictive dimension checking and should be preferred in
-    the meantime. See `scores.probability.crps_cdf` for an example of
-    `scores.utils.gather_dimensions2` usage.
-
     Args:
         fcst: Forecast data
         obs: Observation data
         weights: Weights for calculating a weighted mean of scores
         reduce_dims: Dimensions to reduce. Can be "all" to reduce all dimensions.
         preserve_dims: Dimensions to preserve. Can be "all" to preserve all dimensions.
-        special_fcst_dims: Dimension(s) in `fcst` that are reduced to calculate individual scores.
+        score_specific_fcst_dims: Dimension(s) in `fcst` that are reduced to calculate individual scores.
             Must not appear as a dimension in `obs`, `weights`, `reduce_dims` or `preserve_dims`.
             e.g. the ensemble member dimension if calculating CRPS for ensembles, or the
             threshold dimension of calculating CRPS for CDFs.
 
     Returns:
         Set of dimensions over which to take the mean once the checks are passed.
 
     Raises:
         ValueError: when `preserve_dims and `reduce_dims` are both specified.
-        ValueError: when `special_fcst_dims` is not a subset of `fcst.dims`.
+        ValueError: when `score_specific_fcst_dims` is not a subset of `fcst.dims`.
         ValueError: when `obs.dims`, `weights.dims`, `reduce_dims` or `preserve_dims`
-            contains elements from `special_fcst_dims`.
+            contains elements from `score_specific_fcst_dims`.
         ValueError: when `preserve_dims and `reduce_dims` contain elements not among dimensions
             of the data (`fcst`, `obs` or `weights`).
 
-    See also:
-        `scores.utils.gather_dimensions`
     """
-    all_data_dims = set(fcst.dims).union(set(obs.dims))
-    if weights is not None:
-        all_data_dims = all_data_dims.union(set(weights.dims))
 
-    # all_scoring_dims is the set of dims remaining after individual scores are computed.
-    all_scoring_dims = all_data_dims.copy()
+    all_data_dims = set(fcst_dims).union(set(obs_dims))
+    if weights_dims is not None:
+        all_data_dims = all_data_dims.union(set(weights_dims))
 
     # Handle error conditions related to specified dimensions
     if preserve_dims is not None and reduce_dims is not None:
         raise ValueError(ERROR_OVERSPECIFIED_PRESERVE_REDUCE)
 
+    # all_scoring_dims is the set of dims remaining after individual scores are computed.
+    all_scoring_dims = all_data_dims.copy()
+
+    # Handle error conditions related to specified dimensions
     specified_dims = preserve_dims or reduce_dims
 
     if specified_dims == "all":
         if "all" in all_data_dims:
             warnings.warn(WARN_ALL_DATA_CONFLICT_MSG)
     elif specified_dims is not None:
         if isinstance(specified_dims, str):
             specified_dims = [specified_dims]
 
-    # check that special_fcst_dims are in fcst.dims only
-    if special_fcst_dims is not None:
-        if isinstance(special_fcst_dims, str):
-            special_fcst_dims = [special_fcst_dims]
-        if not set(special_fcst_dims).issubset(set(fcst.dims)):
-            raise ValueError("`special_fcst_dims` must be a subset of `fcst` dimensions")
-        if len(set(obs.dims).intersection(set(special_fcst_dims))) > 0:
-            raise ValueError("`obs.dims` must not contain any `special_fcst_dims`")
-        if weights is not None:
-            if len(set(weights.dims).intersection(set(special_fcst_dims))) > 0:
-                raise ValueError("`weights.dims` must not contain any `special_fcst_dims`")
+    # Raise errors unless score_specific_fcst_dims are in fcst.dims only
+    if score_specific_fcst_dims is not None:
+        if isinstance(score_specific_fcst_dims, str):
+            score_specific_fcst_dims = [score_specific_fcst_dims]
+        if not set(score_specific_fcst_dims).issubset(set(fcst_dims)):
+            raise ValueError("`score_specific_fcst_dims` must be a subset of `fcst` dimensions")
+        if len(set(obs_dims).intersection(set(score_specific_fcst_dims))) > 0:
+            raise ValueError("`obs.dims` must not contain any `score_specific_fcst_dims`")
+        if weights_dims is not None:
+            if len(set(weights_dims).intersection(set(score_specific_fcst_dims))) > 0:
+                raise ValueError("`weights.dims` must not contain any `score_specific_fcst_dims`")
         if specified_dims is not None and specified_dims != "all":
-            if len(set(specified_dims).intersection(set(special_fcst_dims))) > 0:
-                raise ValueError("`reduce_dims` and `preserve_dims` must not contain any `special_fcst_dims`")
-        # remove special_fcst_dims from all_scoring_dims
-        all_scoring_dims = all_scoring_dims.difference(set(special_fcst_dims))
+            if len(set(specified_dims).intersection(set(score_specific_fcst_dims))) > 0:
+                raise ValueError("`reduce_dims` and `preserve_dims` must not contain any `score_specific_fcst_dims`")
+
+        # Finally, remove score_specific_fcst_dims from all_scoring_dims
+        all_scoring_dims = all_data_dims.difference(set(score_specific_fcst_dims))
 
     if specified_dims is not None and specified_dims != "all":
-        if not set(specified_dims).issubset(all_scoring_dims):
+        if not set(specified_dims).issubset(all_data_dims):
             if preserve_dims is not None:
-                raise ValueError(ERROR_SPECIFIED_NONPRESENT_PRESERVE_DIMENSION2)
-            raise ValueError(ERROR_SPECIFIED_NONPRESENT_REDUCE_DIMENSION2)
+                raise ValueError(ERROR_SPECIFIED_NONPRESENT_PRESERVE_DIMENSION)
+            raise ValueError(ERROR_SPECIFIED_NONPRESENT_REDUCE_DIMENSION)
 
-    # all errors have been captured, so now return list of dims to reduce
-    if specified_dims is None:
-        return all_scoring_dims
-    if reduce_dims is not None:
-        if reduce_dims == "all":
-            return all_scoring_dims
-        return set(specified_dims)
-    if preserve_dims == "all":
-        return set([])
-    return all_scoring_dims.difference(set(specified_dims))
+    # Turn preserve dims into reduce dims, if needed
+    if preserve_dims is not None:
+        if preserve_dims == "all":
+            return set([])
+
+        if isinstance(preserve_dims, str):
+            preserve_dims = [preserve_dims]
+
+        reduce_dims = set(all_scoring_dims).difference(preserve_dims)
+
+    # Handle reduction of all dimensions by string "all""
+    elif reduce_dims == "all":
+        reduce_dims = set(all_scoring_dims)
+
+    # Handle reduction of a single dim by string name
+    elif isinstance(reduce_dims, str):
+        reduce_dims = set([reduce_dims])
+
+    # Handle when reduce_dims and preserve_dims are both None
+    elif reduce_dims is None and preserve_dims is None:
+        reduce_dims = set(all_scoring_dims)
+
+    # Turn into a set if needed
+    assert reduce_dims is not None  # nosec - this is just to modify type hinting
+    reduce_dims = set(reduce_dims)
+
+    # Reduce by list is the default so no handling needed
+    return reduce_dims
 
 
 def dims_complement(data, *, dims=None) -> list[str]:
     """Returns the complement of data.dims and dims
 
     Args:
         data: Input xarray object
```

### Comparing `scores-0.72/src/scores/categorical/__init__.py` & `scores-0.8/src/scores/categorical/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.72/src/scores/categorical/binary_impl.py` & `scores-0.8/src/scores/categorical/binary_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.72/src/scores/categorical/multicategorical_impl.py` & `scores-0.8/src/scores/categorical/multicategorical_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.72/src/scores/continuous/__init__.py` & `scores-0.8/src/scores/continuous/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.72/src/scores/continuous/flip_flop_impl.py` & `scores-0.8/src/scores/continuous/flip_flop_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.72/src/scores/continuous/murphy_impl.py` & `scores-0.8/src/scores/continuous/murphy_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.72/src/scores/continuous/quantile_loss_impl.py` & `scores-0.8/src/scores/continuous/quantile_loss_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.72/src/scores/continuous/standard_impl.py` & `scores-0.8/src/scores/continuous/standard_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.72/src/scores/pandas/continuous.py` & `scores-0.8/src/scores/pandas/continuous.py`

 * *Files identical despite different names*

### Comparing `scores-0.72/src/scores/probability/__init__.py` & `scores-0.8/src/scores/probability/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.72/src/scores/probability/brier_impl.py` & `scores-0.8/src/scores/probability/brier_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.72/src/scores/probability/checks.py` & `scores-0.8/src/scores/probability/checks.py`

 * *Files identical despite different names*

### Comparing `scores-0.72/src/scores/probability/crps_impl.py` & `scores-0.8/src/scores/probability/crps_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -810,21 +810,25 @@
         - M. Zamo and P. Naveau (2018), "Estimation of the Continuous Ranked Probability
             Score with Limited Information and Applications to Ensemble Weather Forecasts",
             Math Geosci 50:209-234, https://doi.org/10.1007/s11004-017-9709-7
     """
     if method not in ["ecdf", "fair"]:
         raise ValueError("`method` must be one of 'ecdf' or 'fair'")
 
-    dims_for_mean = scores.utils.gather_dimensions2(
-        fcst,
-        obs,
-        weights=weights,
+    weights_dims = None
+    if weights is not None:
+        weights_dims = weights.dims
+
+    dims_for_mean = scores.utils.gather_dimensions(
+        fcst.dims,
+        obs.dims,
+        weights_dims=weights_dims,
         reduce_dims=reduce_dims,
         preserve_dims=preserve_dims,
-        special_fcst_dims=ensemble_member_dim,
+        score_specific_fcst_dims=ensemble_member_dim,
     )
 
     ensemble_member_dim1 = scores.utils.tmp_coord_name(fcst)
 
     # calculate forecast spread contribution
     fcst_copy = fcst.rename({ensemble_member_dim: ensemble_member_dim1})  # type: ignore
```

### Comparing `scores-0.72/src/scores/probability/roc_impl.py` & `scores-0.8/src/scores/probability/roc_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.72/src/scores/processing/__init__.py` & `scores-0.8/src/scores/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.72/src/scores/processing/discretise.py` & `scores-0.8/src/scores/processing/discretise.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,17 +185,17 @@
 ):
     """
     Calculates the proportion of `data` equal to or exceeding `thresholds`.
 
     Args:
         data (xarray.Dataset or xarray.DataArray): The data from which
             to calculate the proportion exceeding `thresholds`
-        thresholds (iterable): The proportion of Flip-Flop index results
+        thresholds (iterable): The proportion of Flip-Flop Index results
             equal to or exceeding these thresholds will be calculated.
-            the flip-flop index.
+            the Flip-Flop Index.
         reduce_dims: Dimensions to reduce.
         preserve_dims: Dimensions to preserve.
 
     Returns:
         An xarray data object with the type of `data` and dimensions
         `dims` + 'threshold'. The values are the proportion of `data`
         that are greater than or equal to the corresponding threshold.
@@ -219,17 +219,17 @@
     defined by the relationship of data to threshold as specified by
     the operation `mode`.
 
     Args:
         data: The data to convert
            into 0 and 1 according the thresholds before calculating the
            proportion.
-        thresholds: The proportion of Flip-Flop index results
+        thresholds: The proportion of Flip-Flop Index results
             equal to or exceeding these thresholds will be calculated.
-            the flip-flop index.
+            the Flip-Flop Index.
         mode: Specifies the required relation of `data` to `thresholds`
             for a value to fall in the 'event' category (i.e. assigned to 1).
             Allowed modes are:
 
             - '>=' values in `data` greater than or equal to the
               corresponding threshold are assigned as 1.
             - '>' values in `data` greater than the corresponding threshold
```

### Comparing `scores-0.72/src/scores/processing/isoreg_impl.py` & `scores-0.8/src/scores/processing/isoreg_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.72/src/scores/processing/matching.py` & `scores-0.8/src/scores/processing/matching.py`

 * *Files identical despite different names*

### Comparing `scores-0.72/src/scores/processing/cdf/cdf_functions.py` & `scores-0.8/src/scores/processing/cdf/cdf_functions.py`

 * *Files identical despite different names*

### Comparing `scores-0.72/src/scores/stats/statistical_tests/acovf.py` & `scores-0.8/src/scores/stats/statistical_tests/acovf.py`

 * *Files identical despite different names*

### Comparing `scores-0.72/src/scores/stats/statistical_tests/diebold_mariano_impl.py` & `scores-0.8/src/scores/stats/statistical_tests/diebold_mariano_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.72/.gitignore` & `scores-0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `scores-0.72/LICENSE` & `scores-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scores-0.72/README.md` & `scores-0.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-# About the Scores Project
+# Scores: Forecast and Model Verification and Evaluation Software
+> 
+> **A list of over 50 metrics, statistical techniques and data processing tools contained in `scores` is [available here](https://scores.readthedocs.io/en/latest/included.html).**
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nci/scores/HEAD?labpath=tutorials%2FExplanation.ipynb)
-
-One-line intro: xarray based verification scores and tools that can scale with Dask if needed. Pandas supported where possible.
-Why use it: trusted implementations, novel metrics, performance, one-stop-shop.
-
-A **complete list** of the 47 included Metrics, Statistical Techniques and Data Processing Tools is: [available here](https://scores.readthedocs.io/en/latest/included.html).
-
-Here is a **curated selection** of the Metrics and Tools included in `scores`:
-
-| continuous                      | probability | categorical      | statistical tests |
-| ----------                      | ----------- | -----------      | ----------------- |
-| MAE, MSE, RMSE, Flip-Flop Index, Quantile Score, Murphy score, Pearson's Correlation Coefficient, Additive Bias, Multiplicative Bias  | CRPS for CDF, CRPS for ensemble, ROC, Brier Score, Isotonic Regression (reliability diagrams)   | FIRM, Hit Rate, Probability of False Detection, Success Ratio, Peirce's Skill Score  |  Diebold Mariano (with the Harvey et al. 1997 and the Hering and Genton 2011 modifications) |
+`scores` is a Python package containing mathematical functions for the verification, evaluation, and optimisation of forecasts, predictions or models. It primarily supports the meteorological, climatological and geoscience communities. In addition to supporting the Earth system science communities, it also has wide potential application in machine learning and other domains.
 
 **Notice -- This repository is currently undergoing initial construction and maintenance. It is getting much closer to our goals for version one, but there are a few more things to add. This notice will be removed after the first feature release. In the meantime, please feel free to look around, and don't hesitate to get in touch with any questions (see the contributing guide for how).**
 
 Documentation is hosted at [scores.readthedocs.io](https://scores.readthedocs.io).  
 Source code is hosted at [github.com/nci/scores](https://github.com/nci/scores).  
 The tutorial gallery is hosted at [as part of the documentation, here](https://scores.readthedocs.io/en/latest/tutorials/Explanation.html).
 
-`scores` is a Python package containing mathematical functions for the verification, evaluation, and optimisation of forecasts, predictions or models. It primarily supports the geoscience and earth system science communities. It also has wide potential application in machine learning, and in domains other than meteorology, geoscience and weather.
+## Overview
+Here is a **curated selection** of the metrics, tools and statistical tests included in `scores`:
 
-`scores` includes novel scores not commonly found elsewhere (e.g. FIRM, Flip-Flop Index), complex scores (e.g. threshold weighted CRPS), more common scores (e.g. MAE, RMSE) and statistical tests (such as the Diebold Mariano test). Additionally, it provides pre-processing tools for preparing data for scores in a variety of formats including Cumulative Density Functions (CDF). `scores` provides its own implementations where relevant to avoid extensive dependencies.
+|                       	| **Description** 	| **Selection of Included Functions** 	|
+|-----------------------	|-----------------	|--------------	|
+| **[Continuous](https://scores.readthedocs.io/en/latest/included.html#continuous)**        	|Scores for evaluating single-valued continuous forecasts.                  	|Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), Additive Bias, Multiplicative Bias, Pearson's Correlation Coefficient, Flip-Flop Index, Quantile loss, Murphy score.              	|
+| **[Probability](https://scores.readthedocs.io/en/latest/included.html#probability)**       	|Scores for evaluating forecasts that are expressed as predictive distributions, ensembles, and probabilities of binary events.                 	|Brier Score, Continuous Ranked Probability Score (CRPS) for Cumulative Density Function (CDF), Threshold weighted CRPS for CDF, CRPS for ensemble, Receiver Operating Characteristic (ROC), Isotonic Regression (reliability diagrams).              	|
+| **[Categorical](https://scores.readthedocs.io/en/latest/included.html#categorical)**       	|Scores for evaluating forecasts based on categories.                	|Probability of Detection (POD), False Alarm Rate (FAR), Probability of False Detection (POFD), Success Ratio, Accuracy, Peirce's Skill Score, Critical Success Index (CSI), Gilbert Skill Score, Heidke Skill Score, Odds Ratio, Odds Ratio Skill Score, F1 score, FIxed Risk Multicategorical (FIRM) Score.               	|
+| **[Statistical Tests](https://scores.readthedocs.io/en/latest/included.html#statistical-tests)** 	|Tools to conduct statistical tests and generate confidence intervals.                 	|Diebold Mariano.              	|
+| **[Processing tools](https://scores.readthedocs.io/en/latest/included.html#processing-tools-for-preparing-data)**        	|Tools to pre-process data.                 	|Data matching, Discretization, Cumulative Density Function Manipulation.              	|
 
-`scores` is focused on supporting xarray datatypes for earth system data. It also aims to be compatible with pandas, geopandas, pangeo and work with NetCDF4, hdf5, Zarr and GRIB data sources among others. `scores` is designed to use Dask for scaling and performance.
 
-All of the scores and metrics in this package have undergone a thorough statistical and scientific review. Every score has a companion Jupyter Notebook tutorial demonstrating its use in practice.
+`scores` not only includes common scores (e.g. MAE, RMSE), it includes novel scores not commonly found elsewhere (e.g. FIRM, Flip-Flop Index), complex scores (e.g. threshold weighted CRPS), and statistical tests (such as the Diebold Mariano test). Additionally, it provides pre-processing tools for preparing data for scores in a variety of formats including cumulative distribution functions (CDF). `scores` provides its own implementations where relevant to avoid extensive dependencies.
+
+`scores` primarily supports xarray datatypes for Earth system data allowing it to work with NetCDF4, hdf5, Zarr and GRIB data sources among others. `scores` uses Dask for scaling and performance. Some metrics work with pandas and we will aim to expand this capability. 
+
+All of the scores and metrics in this package have undergone a thorough scientific review. Every score has a companion Jupyter Notebook tutorial that demonstrates its use in practice.
 
 ## Contributing
 To find out more about contributing, see our [contributor's guide](https://github.com/nci/scores/blob/main/docs/contributing.md).
 
-All interactions in discussions, issues, emails and code (e.g. merge requests, code comments) will be managed according to the expectations outlined in the [ code of conduct ](https://github.com/nci/scores/blob/main/CODE_OF_CONDUCT.md) and in accordance with all relevant laws and obligations. This project is an inclusive, respectful and open project with high standards for respectful behaviour and language. The code of conduct is the Contributor Covenant, adopted by over 40, 000 open source projects. Any concerns will be dealt with fairly and respectfully, with the processes described in the code of conduct.
+All interactions in discussions, issues, emails and code (e.g. merge requests, code comments) will be managed according to the expectations outlined in the [ code of conduct ](https://github.com/nci/scores/blob/main/CODE_OF_CONDUCT.md) and in accordance with all relevant laws and obligations. This project is an inclusive, respectful and open project with high standards for respectful behaviour and language. The code of conduct is the Contributor Covenant, adopted by over 40,000 open source projects. Any concerns will be dealt with fairly and respectfully, with the processes described in the code of conduct.
 
 ## Using This Package
 
 The [installation guide](https://scores.readthedocs.io/en/latest/installation.html) describes four different use cases for installing, using and working with this package.
 
 Most users currently want the *all* installation option. This includes the mathematical functions (scores, metrics, statistical tests etc.), the tutorial notebooks and development libraries.
 
@@ -58,18 +59,14 @@
 
 To install the mathematical functions ONLY (no tutorial notebooks, no developer libraries), use the *minimal* installation option. *minimal* is a stable version with limited dependencies and can be installed from the Python Package Index.
 
 ```bash
 > pip install scores
 ```
 
-## Related Packages
-
-There are similar packages which should be acknowledged, in particular [xskillscore](https://xskillscore.readthedocs.io/en/stable/) and [climpred](https://github.com/pangeo-data/climpred). These packages both provide overlapping and similar functionality. `scores` provides an additional option to the community and has additional metrics which are not found in those other packages. `scores` seeks to be self-contained with few dependencies, and so re-implements various metrics which are found in other libraries, so that it can be a simple one-stop-shop for the metrics of interest to its userbase.
-
 ## Finding and Downloading Data
 
 Other than very small files to support automated testing, this repository does not contain significant data for tutorials and demonstrations. The tutorials demonstrate how to easily download sample data and generate synthetic data.
 
 ## Acknowledging This Work
 
-If you find this work useful, please consider a citation or acknowledgment of it. A citable DOI is coming soon. This section will be updated in the coming weeks to include the correct citation.
+If you find this work useful, please consider citing or acknowledging it. A citable DOI is coming soon. This section will be updated in the coming weeks to include the correct citation.
```

### Comparing `scores-0.72/pyproject.toml` & `scores-0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scores-0.72/PKG-INFO` & `scores-0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scores
-Version: 0.72
+Version: 0.8
 Summary: Scores is a package containing mathematical functions for the verification, evaluation and optimisation of model outputs and predictions.
 Project-URL: Homepage, http://www.bom.gov.au
 Author-email: Tennessee Leeuwenburg <tennessee.leeuwenburg@bom.gov.au>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -61,47 +61,48 @@
 Requires-Dist: jupyterlab; extra == 'tutorial'
 Requires-Dist: matplotlib; extra == 'tutorial'
 Requires-Dist: plotly; extra == 'tutorial'
 Requires-Dist: rasterio; extra == 'tutorial'
 Requires-Dist: rioxarray; extra == 'tutorial'
 Description-Content-Type: text/markdown
 
-# About the Scores Project
+# Scores: Forecast and Model Verification and Evaluation Software
+> 
+> **A list of over 50 metrics, statistical techniques and data processing tools contained in `scores` is [available here](https://scores.readthedocs.io/en/latest/included.html).**
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nci/scores/HEAD?labpath=tutorials%2FExplanation.ipynb)
-
-One-line intro: xarray based verification scores and tools that can scale with Dask if needed. Pandas supported where possible.
-Why use it: trusted implementations, novel metrics, performance, one-stop-shop.
-
-A **complete list** of the 47 included Metrics, Statistical Techniques and Data Processing Tools is: [available here](https://scores.readthedocs.io/en/latest/included.html).
-
-Here is a **curated selection** of the Metrics and Tools included in `scores`:
-
-| continuous                      | probability | categorical      | statistical tests |
-| ----------                      | ----------- | -----------      | ----------------- |
-| MAE, MSE, RMSE, Flip-Flop Index, Quantile Score, Murphy score, Pearson's Correlation Coefficient, Additive Bias, Multiplicative Bias  | CRPS for CDF, CRPS for ensemble, ROC, Brier Score, Isotonic Regression (reliability diagrams)   | FIRM, Hit Rate, Probability of False Detection, Success Ratio, Peirce's Skill Score  |  Diebold Mariano (with the Harvey et al. 1997 and the Hering and Genton 2011 modifications) |
+`scores` is a Python package containing mathematical functions for the verification, evaluation, and optimisation of forecasts, predictions or models. It primarily supports the meteorological, climatological and geoscience communities. In addition to supporting the Earth system science communities, it also has wide potential application in machine learning and other domains.
 
 **Notice -- This repository is currently undergoing initial construction and maintenance. It is getting much closer to our goals for version one, but there are a few more things to add. This notice will be removed after the first feature release. In the meantime, please feel free to look around, and don't hesitate to get in touch with any questions (see the contributing guide for how).**
 
 Documentation is hosted at [scores.readthedocs.io](https://scores.readthedocs.io).  
 Source code is hosted at [github.com/nci/scores](https://github.com/nci/scores).  
 The tutorial gallery is hosted at [as part of the documentation, here](https://scores.readthedocs.io/en/latest/tutorials/Explanation.html).
 
-`scores` is a Python package containing mathematical functions for the verification, evaluation, and optimisation of forecasts, predictions or models. It primarily supports the geoscience and earth system science communities. It also has wide potential application in machine learning, and in domains other than meteorology, geoscience and weather.
+## Overview
+Here is a **curated selection** of the metrics, tools and statistical tests included in `scores`:
 
-`scores` includes novel scores not commonly found elsewhere (e.g. FIRM, Flip-Flop Index), complex scores (e.g. threshold weighted CRPS), more common scores (e.g. MAE, RMSE) and statistical tests (such as the Diebold Mariano test). Additionally, it provides pre-processing tools for preparing data for scores in a variety of formats including Cumulative Density Functions (CDF). `scores` provides its own implementations where relevant to avoid extensive dependencies.
+|                       	| **Description** 	| **Selection of Included Functions** 	|
+|-----------------------	|-----------------	|--------------	|
+| **[Continuous](https://scores.readthedocs.io/en/latest/included.html#continuous)**        	|Scores for evaluating single-valued continuous forecasts.                  	|Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), Additive Bias, Multiplicative Bias, Pearson's Correlation Coefficient, Flip-Flop Index, Quantile loss, Murphy score.              	|
+| **[Probability](https://scores.readthedocs.io/en/latest/included.html#probability)**       	|Scores for evaluating forecasts that are expressed as predictive distributions, ensembles, and probabilities of binary events.                 	|Brier Score, Continuous Ranked Probability Score (CRPS) for Cumulative Density Function (CDF), Threshold weighted CRPS for CDF, CRPS for ensemble, Receiver Operating Characteristic (ROC), Isotonic Regression (reliability diagrams).              	|
+| **[Categorical](https://scores.readthedocs.io/en/latest/included.html#categorical)**       	|Scores for evaluating forecasts based on categories.                	|Probability of Detection (POD), False Alarm Rate (FAR), Probability of False Detection (POFD), Success Ratio, Accuracy, Peirce's Skill Score, Critical Success Index (CSI), Gilbert Skill Score, Heidke Skill Score, Odds Ratio, Odds Ratio Skill Score, F1 score, FIxed Risk Multicategorical (FIRM) Score.               	|
+| **[Statistical Tests](https://scores.readthedocs.io/en/latest/included.html#statistical-tests)** 	|Tools to conduct statistical tests and generate confidence intervals.                 	|Diebold Mariano.              	|
+| **[Processing tools](https://scores.readthedocs.io/en/latest/included.html#processing-tools-for-preparing-data)**        	|Tools to pre-process data.                 	|Data matching, Discretization, Cumulative Density Function Manipulation.              	|
 
-`scores` is focused on supporting xarray datatypes for earth system data. It also aims to be compatible with pandas, geopandas, pangeo and work with NetCDF4, hdf5, Zarr and GRIB data sources among others. `scores` is designed to use Dask for scaling and performance.
 
-All of the scores and metrics in this package have undergone a thorough statistical and scientific review. Every score has a companion Jupyter Notebook tutorial demonstrating its use in practice.
+`scores` not only includes common scores (e.g. MAE, RMSE), it includes novel scores not commonly found elsewhere (e.g. FIRM, Flip-Flop Index), complex scores (e.g. threshold weighted CRPS), and statistical tests (such as the Diebold Mariano test). Additionally, it provides pre-processing tools for preparing data for scores in a variety of formats including cumulative distribution functions (CDF). `scores` provides its own implementations where relevant to avoid extensive dependencies.
+
+`scores` primarily supports xarray datatypes for Earth system data allowing it to work with NetCDF4, hdf5, Zarr and GRIB data sources among others. `scores` uses Dask for scaling and performance. Some metrics work with pandas and we will aim to expand this capability. 
+
+All of the scores and metrics in this package have undergone a thorough scientific review. Every score has a companion Jupyter Notebook tutorial that demonstrates its use in practice.
 
 ## Contributing
 To find out more about contributing, see our [contributor's guide](https://github.com/nci/scores/blob/main/docs/contributing.md).
 
-All interactions in discussions, issues, emails and code (e.g. merge requests, code comments) will be managed according to the expectations outlined in the [ code of conduct ](https://github.com/nci/scores/blob/main/CODE_OF_CONDUCT.md) and in accordance with all relevant laws and obligations. This project is an inclusive, respectful and open project with high standards for respectful behaviour and language. The code of conduct is the Contributor Covenant, adopted by over 40, 000 open source projects. Any concerns will be dealt with fairly and respectfully, with the processes described in the code of conduct.
+All interactions in discussions, issues, emails and code (e.g. merge requests, code comments) will be managed according to the expectations outlined in the [ code of conduct ](https://github.com/nci/scores/blob/main/CODE_OF_CONDUCT.md) and in accordance with all relevant laws and obligations. This project is an inclusive, respectful and open project with high standards for respectful behaviour and language. The code of conduct is the Contributor Covenant, adopted by over 40,000 open source projects. Any concerns will be dealt with fairly and respectfully, with the processes described in the code of conduct.
 
 ## Using This Package
 
 The [installation guide](https://scores.readthedocs.io/en/latest/installation.html) describes four different use cases for installing, using and working with this package.
 
 Most users currently want the *all* installation option. This includes the mathematical functions (scores, metrics, statistical tests etc.), the tutorial notebooks and development libraries.
 
@@ -125,18 +126,14 @@
 
 To install the mathematical functions ONLY (no tutorial notebooks, no developer libraries), use the *minimal* installation option. *minimal* is a stable version with limited dependencies and can be installed from the Python Package Index.
 
 ```bash
 > pip install scores
 ```
 
-## Related Packages
-
-There are similar packages which should be acknowledged, in particular [xskillscore](https://xskillscore.readthedocs.io/en/stable/) and [climpred](https://github.com/pangeo-data/climpred). These packages both provide overlapping and similar functionality. `scores` provides an additional option to the community and has additional metrics which are not found in those other packages. `scores` seeks to be self-contained with few dependencies, and so re-implements various metrics which are found in other libraries, so that it can be a simple one-stop-shop for the metrics of interest to its userbase.
-
 ## Finding and Downloading Data
 
 Other than very small files to support automated testing, this repository does not contain significant data for tutorials and demonstrations. The tutorials demonstrate how to easily download sample data and generate synthetic data.
 
 ## Acknowledging This Work
 
-If you find this work useful, please consider a citation or acknowledgment of it. A citable DOI is coming soon. This section will be updated in the coming weeks to include the correct citation.
+If you find this work useful, please consider citing or acknowledging it. A citable DOI is coming soon. This section will be updated in the coming weeks to include the correct citation.
```

