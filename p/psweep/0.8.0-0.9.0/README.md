# Comparing `tmp/psweep-0.8.0.tar.gz` & `tmp/psweep-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psweep-0.8.0.tar", last modified: Tue Aug 23 20:10:56 2022, max compression
+gzip compressed data, was "psweep-0.9.0.tar", last modified: Tue Sep 13 20:44:25 2022, max compression
```

## Comparing `psweep-0.8.0.tar` & `psweep-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-----   0 elcorto   (1001) elcorto   (1001)        0 2022-08-23 20:10:56.859413 psweep-0.8.0/
--rw-r-----   0 elcorto   (1001) elcorto   (1001)     1519 2022-08-16 07:12:11.000000 psweep-0.8.0/LICENSE
--rw-r-----   0 elcorto   (1001) elcorto   (1001)    35524 2022-08-23 20:10:56.859413 psweep-0.8.0/PKG-INFO
--rw-r-----   0 elcorto   (1001) elcorto   (1001)    35102 2022-08-20 22:01:12.000000 psweep-0.8.0/README.md
-drwxr-----   0 elcorto   (1001) elcorto   (1001)        0 2022-08-23 20:10:56.859413 psweep-0.8.0/bin/
--rwxr-----   0 elcorto   (1001) elcorto   (1001)     1783 2022-01-14 10:07:40.000000 psweep-0.8.0/bin/psweep-db2json
--rwxr-----   0 elcorto   (1001) elcorto   (1001)     1663 2022-01-14 10:07:40.000000 psweep-0.8.0/bin/psweep-db2table
--rwxr-----   0 elcorto   (1001) elcorto   (1001)      197 2021-11-30 21:18:08.000000 psweep-0.8.0/bin/psweep-pull
--rwxr-----   0 elcorto   (1001) elcorto   (1001)      228 2021-11-30 21:18:08.000000 psweep-0.8.0/bin/psweep-push
--rw-r-----   0 elcorto   (1001) elcorto   (1001)       38 2022-08-23 20:10:56.859413 psweep-0.8.0/setup.cfg
--rw-r-----   0 elcorto   (1001) elcorto   (1001)     1032 2022-08-23 20:06:41.000000 psweep-0.8.0/setup.py
-drwxr-----   0 elcorto   (1001) elcorto   (1001)        0 2022-08-23 20:10:56.859413 psweep-0.8.0/src/
-drwxr-----   0 elcorto   (1001) elcorto   (1001)        0 2022-08-23 20:10:56.859413 psweep-0.8.0/src/psweep/
--rw-r-----   0 elcorto   (1001) elcorto   (1001)       22 2021-11-30 21:18:08.000000 psweep-0.8.0/src/psweep/__init__.py
--rw-r-----   0 elcorto   (1001) elcorto   (1001)      652 2022-01-14 16:17:00.000000 psweep-0.8.0/src/psweep/cli.py
--rw-r-----   0 elcorto   (1001) elcorto   (1001)    32111 2022-08-20 22:01:12.000000 psweep-0.8.0/src/psweep/psweep.py
-drwxr-----   0 elcorto   (1001) elcorto   (1001)        0 2022-08-23 20:10:56.859413 psweep-0.8.0/src/psweep.egg-info/
--rw-r-----   0 elcorto   (1001) elcorto   (1001)    35524 2022-08-23 20:10:56.000000 psweep-0.8.0/src/psweep.egg-info/PKG-INFO
--rw-r-----   0 elcorto   (1001) elcorto   (1001)      365 2022-08-23 20:10:56.000000 psweep-0.8.0/src/psweep.egg-info/SOURCES.txt
--rw-r-----   0 elcorto   (1001) elcorto   (1001)        1 2022-08-23 20:10:56.000000 psweep-0.8.0/src/psweep.egg-info/dependency_links.txt
--rw-r-----   0 elcorto   (1001) elcorto   (1001)       63 2022-08-23 20:10:56.000000 psweep-0.8.0/src/psweep.egg-info/entry_points.txt
--rw-r-----   0 elcorto   (1001) elcorto   (1001)       52 2022-08-23 20:10:56.000000 psweep-0.8.0/src/psweep.egg-info/requires.txt
--rw-r-----   0 elcorto   (1001) elcorto   (1001)        7 2022-08-23 20:10:56.000000 psweep-0.8.0/src/psweep.egg-info/top_level.txt
+drwxr-----   0 elcorto   (1001) elcorto   (1001)        0 2022-09-13 20:44:25.078275 psweep-0.9.0/
+-rw-r-----   0 elcorto   (1001) elcorto   (1001)     1519 2022-08-16 07:12:11.000000 psweep-0.9.0/LICENSE
+-rw-r-----   0 elcorto   (1001) elcorto   (1001)    35547 2022-09-13 20:44:25.078275 psweep-0.9.0/PKG-INFO
+-rw-r-----   0 elcorto   (1001) elcorto   (1001)    35102 2022-08-20 22:01:12.000000 psweep-0.9.0/README.md
+drwxr-----   0 elcorto   (1001) elcorto   (1001)        0 2022-09-13 20:44:25.078275 psweep-0.9.0/bin/
+-rwxr-----   0 elcorto   (1001) elcorto   (1001)     1783 2022-01-14 10:07:40.000000 psweep-0.9.0/bin/psweep-db2json
+-rwxr-----   0 elcorto   (1001) elcorto   (1001)     1663 2022-01-14 10:07:40.000000 psweep-0.9.0/bin/psweep-db2table
+-rwxr-----   0 elcorto   (1001) elcorto   (1001)      197 2021-11-30 21:18:08.000000 psweep-0.9.0/bin/psweep-pull
+-rwxr-----   0 elcorto   (1001) elcorto   (1001)      228 2021-11-30 21:18:08.000000 psweep-0.9.0/bin/psweep-push
+-rw-r-----   0 elcorto   (1001) elcorto   (1001)       38 2022-09-13 20:44:25.078275 psweep-0.9.0/setup.cfg
+-rw-r-----   0 elcorto   (1001) elcorto   (1001)     1061 2022-09-13 20:43:23.000000 psweep-0.9.0/setup.py
+drwxr-----   0 elcorto   (1001) elcorto   (1001)        0 2022-09-13 20:44:25.078275 psweep-0.9.0/src/
+drwxr-----   0 elcorto   (1001) elcorto   (1001)        0 2022-09-13 20:44:25.078275 psweep-0.9.0/src/psweep/
+-rw-r-----   0 elcorto   (1001) elcorto   (1001)       22 2021-11-30 21:18:08.000000 psweep-0.9.0/src/psweep/__init__.py
+-rw-r-----   0 elcorto   (1001) elcorto   (1001)      652 2022-01-14 16:17:00.000000 psweep-0.9.0/src/psweep/cli.py
+-rw-r-----   0 elcorto   (1001) elcorto   (1001)    34319 2022-09-13 20:12:47.000000 psweep-0.9.0/src/psweep/psweep.py
+drwxr-----   0 elcorto   (1001) elcorto   (1001)        0 2022-09-13 20:44:25.078275 psweep-0.9.0/src/psweep.egg-info/
+-rw-r-----   0 elcorto   (1001) elcorto   (1001)    35547 2022-09-13 20:44:25.000000 psweep-0.9.0/src/psweep.egg-info/PKG-INFO
+-rw-r-----   0 elcorto   (1001) elcorto   (1001)      365 2022-09-13 20:44:25.000000 psweep-0.9.0/src/psweep.egg-info/SOURCES.txt
+-rw-r-----   0 elcorto   (1001) elcorto   (1001)        1 2022-09-13 20:44:25.000000 psweep-0.9.0/src/psweep.egg-info/dependency_links.txt
+-rw-r-----   0 elcorto   (1001) elcorto   (1001)       63 2022-09-13 20:44:25.000000 psweep-0.9.0/src/psweep.egg-info/entry_points.txt
+-rw-r-----   0 elcorto   (1001) elcorto   (1001)       52 2022-09-13 20:44:25.000000 psweep-0.9.0/src/psweep.egg-info/requires.txt
+-rw-r-----   0 elcorto   (1001) elcorto   (1001)        7 2022-09-13 20:44:25.000000 psweep-0.9.0/src/psweep.egg-info/top_level.txt
```

### Comparing `psweep-0.8.0/LICENSE` & `psweep-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psweep-0.8.0/PKG-INFO` & `psweep-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: psweep
-Version: 0.8.0
+Version: 0.9.0
 Summary: loop like a pro, make parameter studies fun: set up and run a parameter study/sweep/scan, save a database
 Home-page: https://github.com/elcorto/psweep
 Author: Steve Schmerler
 Author-email: git@elcorto.com
 License: BSD 3-Clause
 Keywords: parameter study sweep scan database pandas
 Platform: UNKNOWN
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![pypi](https://img.shields.io/pypi/v/psweep?color=blue)
 ![GitHub Workflow Status](https://img.shields.io/github/workflow/status/elcorto/psweep/tests?label=tests)
 [![DOI](https://zenodo.org/badge/92956212.svg)](https://zenodo.org/badge/latestdoi/92956212)
```

### Comparing `psweep-0.8.0/README.md` & `psweep-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `psweep-0.8.0/bin/psweep-db2json` & `psweep-0.9.0/bin/psweep-db2json`

 * *Files identical despite different names*

### Comparing `psweep-0.8.0/bin/psweep-db2table` & `psweep-0.9.0/bin/psweep-db2table`

 * *Files identical despite different names*

### Comparing `psweep-0.8.0/setup.py` & `psweep-0.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 here = os.path.abspath(os.path.dirname(__file__))
 bindir = "bin"
 with open(os.path.join(here, "README.md")) as fd:
     long_description = fd.read()
 
 setup(
     name="psweep",
-    version="0.8.0",
+    version="0.9.0",
     description=(
         "loop like a pro, make parameter studies fun: set up and "
         "run a parameter study/sweep/scan, save a database"
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/elcorto/psweep",
     author="Steve Schmerler",
     author_email="git@elcorto.com",
     license="BSD 3-Clause",
     keywords="parameter study sweep scan database pandas",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     install_requires=open("requirements.txt").read().splitlines(),
+    python_requires=">=3.8",
     scripts=["{}/{}".format(bindir, script) for script in os.listdir(bindir)],
     entry_points={
         "console_scripts": [
             "psweep-checkdir=psweep.cli:check_calc_dir",
         ],
     },
 )
```

### Comparing `psweep-0.8.0/src/psweep/cli.py` & `psweep-0.9.0/src/psweep/cli.py`

 * *Files identical despite different names*

### Comparing `psweep-0.8.0/src/psweep/psweep.py` & `psweep-0.9.0/src/psweep/psweep.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,34 +164,46 @@
     # The same observations have been also made elsewhere [1,2]. Esp. [2]
     # points to [3] which in turn mentions joblib.hashing.hash(). It's code
     # shows how complex the problem is, but so far this is our best bet.
     #
     # [1] https://death.andgravity.com/stable-hashing
     # [2] https://ourpython.com/python/deterministic-recursive-hashing-in-python
     # [3] https://stackoverflow.com/a/52175075
-    try:
-        if skip_special_cols:
-            keys = [x for x in dct.keys() if not x.startswith("_")]
-            _dct = {kk: dct[kk] for kk in keys}
-        else:
-            _dct = dct
-        return joblib.hash(_dct, hash_name=method)
+    if skip_special_cols:
+        _dct = {
+            key: val for key, val in dct.items() if not key.startswith("_")
+        }
+    else:
+        _dct = dct
     # joblib can hash "anything" so we didn't come up with an input that
     # actually fails to hash. As such, TypeError is just a guess here. But
     # still we don't catch ValueError raised when an invalid hash_name is
     # passed (anything other than md5 or sha1).
+    try:
+        return joblib.hash(_dct, hash_name=method)
     except TypeError as ex:
         if raise_error:
             raise PsweepHashError(
                 f"Error in hash calculation of: {dct}"
             ) from ex
         else:
             return np.nan
 
 
+def add_hashes(params: Sequence[dict]) -> Sequence[dict]:
+    """Calculate hash for each pset and set pset["_pset_hash"]. Return new
+    params list.
+    """
+    new_params = []
+    for pset in params:
+        pset["_pset_hash"] = pset_hash(pset)
+        new_params.append(pset)
+    return new_params
+
+
 def check_calc_dir(calc_dir: str, df: pd.DataFrame):
     """Check calc dir for consistency with database.
 
     Assuming dirs are named::
 
         <calc_dir>/<pset_id1>
         <calc_dir>/<pset_id2>
@@ -656,47 +668,75 @@
     [{'a': 1, 'b': 77, 'c': 'const'},
      {'a': 2, 'b': 88, 'c': 'const'}]
     """
     assert is_seq(plists), f"input {plists=} is no sequence"
     return itr2params(itertools.product(*plists))
 
 
-def filter_same_hash(params: Sequence[dict], **kwds) -> Sequence[dict]:
+def filter_params_unique(params: Sequence[dict], **kwds) -> Sequence[dict]:
     """Reduce params to unique psets.
 
+    Use pset["_pset_hash"]  if present, else calculate hash on the fly.
+
     Parameters
     ----------
-    params :
-    kwds :
+    params
+    kwds
         passed to :func:`pset_hash`
     """
-    msk = np.unique(
-        [pset_hash(dct, **kwds) for dct in params], return_index=True
-    )[1]
+    get_hash = lambda pset: pset.get("_pset_hash", pset_hash(pset, **kwds))
+    msk = np.unique([get_hash(pset) for pset in params], return_index=True)[1]
     return [params[ii] for ii in np.sort(msk)]
 
 
+def filter_same_hash(*args, **kwds):
+    warnings.warn(
+        "filter_same_hash() was renamed to filter_params_unique()",
+        DeprecationWarning,
+    )
+    return filter_params_unique(*args, **kwds)
+
+
+def filter_params_dup_hash(
+    params: Sequence[dict], hashes: Sequence[str], **kwds
+) -> Sequence[dict]:
+    """Return params with psets whose hash is not in `hashes`.
+
+    Use pset["_pset_hash"]  if present, else calculate hash on the fly.
+
+    Parameters
+    ----------
+    params
+    hashes
+    kwds
+        passed to :func:`pset_hash`
+    """
+    get_hash = lambda pset: pset.get("_pset_hash", pset_hash(pset, **kwds))
+    return [pset for pset in params if not get_hash(pset) in hashes]
+
+
 def stargrid(
     const: dict,
     vary: Sequence[dict],
     vary_labels: Sequence[str] = None,
     vary_label_col: str = "_vary",
-    filter_dups=True,
+    filter_dups=None,
+    skip_dups=True,
 ) -> Sequence[dict]:
     """
     Helper to create a specific param sampling pattern.
 
     Vary params in a "star" pattern (and not a full pgrid) around constant
     values (middle of the "star").
 
     When doing that, duplicate psets can occur. By default try to filter them
-    out (use filter_same_hash()) but ignore hash calculation errors and return
+    out (use filter_params_unique()) but ignore hash calculation errors and return
     non-reduced params in that case. If you want to fail at hash errors, use
 
-    >>> filter_same_hash(stargrid(..., filter_dups=False), raise_error=True)
+    >>> filter_params_unique(stargrid(..., skip_dups=False), raise_error=True)
 
     Examples
     --------
     >>> from psweep import psweep as ps
     >>> const=dict(a=1, b=77, c=11)
     >>> a=ps.plist("a", [1,2,3,4])
     >>> b=ps.plist("b", [77,88,99])
@@ -706,15 +746,15 @@
     [{'a': 1, 'b': 77, 'c': 11},
      {'a': 2, 'b': 77, 'c': 11},
      {'a': 3, 'b': 77, 'c': 11},
      {'a': 4, 'b': 77, 'c': 11},
      {'a': 1, 'b': 88, 'c': 11},
      {'a': 1, 'b': 99, 'c': 11}]
 
-    >>> ps.stargrid(const, vary=[a, b], filter_dups=False)
+    >>> ps.stargrid(const, vary=[a, b], skip_dups=False)
     [{'a': 1, 'b': 77, 'c': 11},
      {'a': 2, 'b': 77, 'c': 11},
      {'a': 3, 'b': 77, 'c': 11},
      {'a': 4, 'b': 77, 'c': 11},
      {'a': 1, 'b': 77, 'c': 11},
      {'a': 1, 'b': 88, 'c': 11},
      {'a': 1, 'b': 99, 'c': 11}]
@@ -745,17 +785,22 @@
             if vary_labels is not None:
                 label = {vary_label_col: vary_labels[ii]}
                 _dct = merge_dicts(dct, label)
             else:
                 _dct = dct
             params.append(merge_dicts(const, _dct))
 
-    if filter_dups:
+    if filter_dups is not None:
+        skip_dups = filter_dups
+        warnings.warn(
+            "filter_dups was renamed to skip_dups", DeprecationWarning
+        )
+    if skip_dups:
         try:
-            return filter_same_hash(
+            return filter_params_unique(
                 params, raise_error=True, skip_special_cols=True
             )
         except PsweepHashError:
             return params
     else:
         return params
 
@@ -778,25 +823,28 @@
     verbose: Union[bool, Sequence[str]] = None,
     run_id: str = None,
     calc_dir: str = None,
     simulate: bool = False,
     pset_seq=np.nan,
     run_seq: int = None,
 ):
+    """
+    Add special fields to pset. Call worker on exactly one pset. Return
+    DataFrame row built from ``pset.update(worker(pset))``.
+    """
     assert run_id is not None
     assert calc_dir is not None
     pset_id = str(uuid.uuid4())
     _pset = copy.deepcopy(pset)
     time_start = pd.Timestamp(time.time(), unit=PANDAS_TIME_UNIT)
     update = {
         "_run_id": run_id,
         "_pset_id": pset_id,
         "_calc_dir": calc_dir,
         "_time_utc": time_start,
-        "_pset_hash": pset_hash(pset, PSET_HASH_ALG, raise_error=False),
         "_pset_seq": pset_seq,
         "_run_seq": run_seq,
     }
     _pset.update(update)
     if verbose is not None:
         df_row_print = pd.DataFrame([_pset], index=[time_start])
         if isinstance(verbose, bool) and verbose:
@@ -824,16 +872,20 @@
     verbose: Union[bool, Sequence[str]] = False,
     calc_dir="calc",
     simulate=False,
     database_dir: str = None,
     database_basename="database.pk",
     backup=False,
     git=False,
+    skip_dups=False,
 ) -> pd.DataFrame:
     """
+    Call `worker` for each `pset` in `params`. Populate a DataFrame with rows
+    from each call ``worker(pset)``.
+
     Parameters
     ----------
     worker : Callable
         must accept one parameter: `pset` (a dict ``{'a': 1, 'b': 'foo',
         ...}``), return either an update to `pset` or a new dict, result will
         be processes as ``pset.update(worker(pset))``
     params : seq of dicts
@@ -841,37 +893,45 @@
     df : DataFrame
         append rows to this DataFrame, if None then either create new one or
         read existing database file from disk if found
     poolsize : {None, int}
         * None : use serial execution
         * int : use multiprocessing.Pool (even for ``poolsize=1``)
     save : bool
-        save final DataFrame to ``<calc_dir>/database.pk`` (pickle format only)
+        save final DataFrame to ``<database_dir>/<database_basename>`` (pickle
+        format only), default: "calc/database.pk", see also `database_dir`,
+        `calc_dir` and `database_basename`
     tmpsave : bool
         save results from each `pset` in `params` (the current DataFrame row) to
         ``<calc_dir>/tmpsave/<run_id>/<pset_id>.pk`` (pickle format only)
     verbose : {bool, sequence of str}
         * bool : print the current DataFrame row
         * sequence : list of DataFrame column names, print the row but only
           those columns
     calc_dir : str
+        Dir where calculation artifacts can be saved if needed, such as dirs
+        per pset ``<calc_dir>/<pset>``. Will be added to the database in
+        ``_calc_dir`` field.
     simulate : bool
         run everything in ``<calc_dir>.simulate``, don't call `worker`, i.e. save
         what the run would create, but without the results from `worker`,
         useful to check if `params` are correct before starting a production run
     database_dir : str
         Path for the database. Default is ``<calc_dir>``.
     database_basename : str
-        ``<database_dir>/<database_basename>``
+        ``<database_dir>/<database_basename>``, default: "database.pk"
     backup : bool
         Make backup of ``<calc_dir>`` to ``<calc_dir>.bak_<timestamp>_run_id_<_run_id>``
     git : bool
         Use ``git`` to commit all files written and changed by the current run
         (``_run_id``). Make sure to create a ``.gitignore`` manually before if
         needed.
+    skip_dups : bool
+        Skip psets whose hash is already present in `df`. Useful when repeating
+        (parts of) a study.
     """
 
     database_dir = calc_dir if database_dir is None else database_dir
 
     git_enter(git)
 
     if simulate:
@@ -912,14 +972,19 @@
             "backup destination {dst} exists, seems like there has been no new "
             "data in {calc_dir} since the last backup".format(
                 dst=dst, calc_dir=calc_dir
             )
         )
         shutil.copytree(calc_dir, dst)
 
+    params = add_hashes(params)
+
+    if skip_dups and len(df) > 0:
+        params = filter_params_dup_hash(params, df._pset_hash.values)
+
     run_id = str(uuid.uuid4())
 
     worker_wrapper_partial = partial(
         worker_wrapper,
         worker=worker,
         tmpsave=tmpsave,
         verbose=verbose,
@@ -1033,14 +1098,15 @@
     params: Sequence[dict],
     calc_dir: str = "calc",
     calc_templ_dir: str = "templates/calc",
     machine_templ_dir: str = "templates/machines",
     git: bool = False,
     backup: bool = False,
     write_pset: bool = False,
+    skip_dups: bool = False,
 ) -> pd.DataFrame:
 
     """
     Write files based on templates.
     """
     git_enter(git)
 
@@ -1054,15 +1120,22 @@
                 pj(calc_dir, pset["_pset_id"], template.targetname),
                 template.fill(pset),
             )
             if write_pset:
                 pickle_write(pj(calc_dir, pset["_pset_id"], "pset.pk"), pset)
         return {}
 
-    df = run_local(worker, params, calc_dir=calc_dir, backup=backup, git=False)
+    df = run_local(
+        worker,
+        params,
+        calc_dir=calc_dir,
+        backup=backup,
+        skip_dups=skip_dups,
+        git=False,
+    )
 
     msk_latest = df._run_seq == df._run_seq.values.max()
     msk_old = df._run_seq < df._run_seq.values.max()
     for machine in machines:
         txt = ""
         for pfx, msk in [("# ", msk_old), ("", msk_latest)]:
             if msk.any():
```

### Comparing `psweep-0.8.0/src/psweep.egg-info/PKG-INFO` & `psweep-0.9.0/src/psweep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: psweep
-Version: 0.8.0
+Version: 0.9.0
 Summary: loop like a pro, make parameter studies fun: set up and run a parameter study/sweep/scan, save a database
 Home-page: https://github.com/elcorto/psweep
 Author: Steve Schmerler
 Author-email: git@elcorto.com
 License: BSD 3-Clause
 Keywords: parameter study sweep scan database pandas
 Platform: UNKNOWN
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![pypi](https://img.shields.io/pypi/v/psweep?color=blue)
 ![GitHub Workflow Status](https://img.shields.io/github/workflow/status/elcorto/psweep/tests?label=tests)
 [![DOI](https://zenodo.org/badge/92956212.svg)](https://zenodo.org/badge/latestdoi/92956212)
```

