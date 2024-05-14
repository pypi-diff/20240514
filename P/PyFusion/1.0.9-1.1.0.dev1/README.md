# Comparing `tmp/pyfusion-1.0.9.tar.gz` & `tmp/PyFusion-1.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfusion-1.0.9.tar", max compression
+gzip compressed data
```

## Comparing `pyfusion-1.0.9.tar` & `PyFusion-1.1.0.dev1.tar`

### file list

```diff
@@ -1,15 +1,43 @@
--rw-r--r--   0        0        0      575 2023-01-25 12:50:19.599452 pyfusion-1.0.9/LICENSE
--rw-r--r--   0        0        0      897 2023-01-25 12:50:19.599452 pyfusion-1.0.9/README.md
--rw-r--r--   0        0        0      188 2023-01-25 12:50:19.603452 pyfusion-1.0.9/fusion/__init__.py
--rw-r--r--   0        0        0    18351 2023-01-25 12:50:19.603452 pyfusion-1.0.9/fusion/authentication.py
--rw-r--r--   0        0        0      960 2023-01-25 12:50:19.603452 pyfusion-1.0.9/fusion/exceptions.py
--rw-r--r--   0        0        0    10005 2023-01-25 12:50:19.603452 pyfusion-1.0.9/fusion/fs_sync.py
--rwxr-xr-x   0        0        0    32117 2023-01-25 12:50:19.603452 pyfusion-1.0.9/fusion/fusion.py
--rw-r--r--   0        0        0    13986 2023-01-25 12:50:19.603452 pyfusion-1.0.9/fusion/fusion_filesystem.py
--rw-r--r--   0        0        0    18532 2023-01-25 12:50:19.603452 pyfusion-1.0.9/fusion/utils.py
--rw-r--r--   0        0        0     3473 2023-01-25 12:50:19.603452 pyfusion-1.0.9/pyproject.toml
--rw-r--r--   0        0        0       36 2023-01-25 12:50:19.603452 pyfusion-1.0.9/tests/__init__.py
--rw-r--r--   0        0        0     3675 2023-01-25 12:50:19.603452 pyfusion-1.0.9/tests/conftest.py
--rw-r--r--   0        0        0     4793 2023-01-25 12:50:19.603452 pyfusion-1.0.9/tests/test_fusion.py
--rw-r--r--   0        0        0     2827 1970-01-01 00:00:00.000000 pyfusion-1.0.9/setup.py
--rw-r--r--   0        0        0     4007 1970-01-01 00:00:00.000000 pyfusion-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0      292 1970-01-01 00:00:00.000000 PyFusion-1.1.0.dev1/Cargo.toml
+-rw-r--r--   0     1001      127      326 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0     1001      127     9838 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/.github/workflows/dev.yml
+-rw-r--r--   0     1001      127     4939 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/.github/workflows/release.yml
+-rw-r--r--   0     1001      127     1328 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/.gitignore
+-rw-r--r--   0     1001      127      668 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127      235 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/BUILD.md
+-rw-r--r--   0     1001      127     2559 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/CHANGELOG.md
+-rw-r--r--   0     1001      127      575 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/LICENSE
+-rw-r--r--   0     1001      127     1386 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/README.md
+-rw-r--r--   0     1001      127       35 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/docs/api.md
+-rw-r--r--   0     1001      127       43 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/docs/changelog.md
+-rw-r--r--   0     1001      127     3532 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/docs/contributing.md
+-rw-r--r--   0     1001      127    86597 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/docs/get_started.ipynb
+-rw-r--r--   0     1001      127       42 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/docs/index.md
+-rw-r--r--   0     1001      127      930 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/docs/installation.md
+-rw-r--r--   0     1001      127      106 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/docs/usage.md
+-rw-r--r--   0     1001      127      373 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/fusion/__init__.py
+-rw-r--r--   0     1001      127     1597 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/fusion/__main__.py
+-rw-r--r--   0     1001      127    25755 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/fusion/authentication.py
+-rw-r--r--   0     1001      127      910 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/fusion/exceptions.py
+-rw-r--r--   0     1001      127    13730 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/fusion/fs_sync.py
+-rw-r--r--   0     1001      127    53307 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/fusion/fusion.py
+-rw-r--r--   0     1001      127    24428 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/fusion/fusion_filesystem.py
+-rw-r--r--   0     1001      127        0 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/fusion/test_fusion_filesystem.py
+-rw-r--r--   0     1001      127      163 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/fusion/types.py
+-rw-r--r--   0     1001      127    35946 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/fusion/utils.py
+-rw-r--r--   0     1001      127      473 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/makefile
+-rw-r--r--   0     1001      127     1783 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/mkdocs.yml
+-rw-r--r--   0     1001      127       36 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/py_tests/__init__.py
+-rw-r--r--   0     1001      127     5857 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/py_tests/conftest.py
+-rw-r--r--   0     1001      127    25811 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/py_tests/test_authentication.py
+-rw-r--r--   0     1001      127     4258 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/py_tests/test_filesystem.py
+-rw-r--r--   0     1001      127      525 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/py_tests/test_fsync.py
+-rw-r--r--   0     1001      127    28808 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/py_tests/test_fusion.py
+-rw-r--r--   0     1001      127    38800 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/py_tests/test_utils.py
+-rw-r--r--   0     1001      127    16095 2024-05-14 19:28:45.000000 PyFusion-1.1.0.dev1/requirements-dev.lock
+-rw-r--r--   0     1001      127    12643 2024-05-14 19:28:37.000000 PyFusion-1.1.0.dev1/requirements.lock
+-rw-r--r--   0     1001      127     1042 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/src/lib.rs
+-rw-r--r--   0     1001      127     1201 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/tox.ini
+-rw-r--r--   0     1001      127     8095 2024-05-14 19:28:17.000000 PyFusion-1.1.0.dev1/Cargo.lock
+-rw-r--r--   0     1001      127     5677 2024-05-14 19:28:21.000000 PyFusion-1.1.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     3450 1970-01-01 00:00:00.000000 PyFusion-1.1.0.dev1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pyfusion-1.0.9/LICENSE` & `PyFusion-1.1.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfusion-1.0.9/fusion/exceptions.py` & `PyFusion-1.1.0.dev1/fusion/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,48 +4,38 @@
 class APIResponseError(Exception):
     """APIResponseError exception wrapper to handle API response errors.
 
     Args:
         Exception : Exception to wrap.
     """
 
-    pass
-
 
 class APIRequestError(Exception):
     """APIRequestError exception wrapper to handle API request erorrs.
 
     Args:
         Exception : Exception to wrap.
     """
 
-    pass
-
 
 class APIConnectError(Exception):
     """APIConnectError exception wrapper to handle API connection errors.
 
     Args:
         Exception : Exception to wrap.
     """
 
-    pass
-
 
 class UnrecognizedFormatError(Exception):
     """UnrecognizedFormatError exception wrapper to handle format errors.
 
     Args:
         Exception : Exception to wrap.
     """
 
-    pass
-
 
 class CredentialError(Exception):
     """CredentialError exception wrapper to handle errors in credentials provided for authentication.
 
     Args:
         Exception : Exception to wrap.
     """
-
-    pass
```

### Comparing `pyfusion-1.0.9/fusion/fs_sync.py` & `PyFusion-1.1.0.dev1/fusion/fs_sync.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,302 +1,381 @@
 """Fusion fsync."""
 
 import base64
 import hashlib
 import json
 import logging
-import os
 import sys
 import time
+import warnings
 from os.path import relpath
 from pathlib import Path
+from typing import Any, Optional
 
 import fsspec
 import pandas as pd
 from joblib import Parallel, delayed
-from tqdm.auto import tqdm
+from tqdm import tqdm
 
 from .utils import (
     cpu_count,
     distribution_to_filename,
+    is_dataset_raw,
     path_to_url,
+    tqdm_joblib,
     upload_files,
     validate_file_names,
 )
 
 logger = logging.getLogger(__name__)
 VERBOSE_LVL = 25
 DEFAULT_CHUNK_SIZE = 2**16
 
 
-def _get_loop(df, show_progress):
-    if show_progress:
-        loop = tqdm(df.iterrows(), total=len(df))
-    else:
-        loop = df.iterrows()
-    return loop
-
-
-def _url_to_path(x):
-    file_name = distribution_to_filename(
-        "", x.split("/")[2], x.split("/")[4], x.split("/")[6], x.split("/")[0]
-    )
+def _url_to_path(x: str) -> str:
+    file_name = distribution_to_filename("", x.split("/")[2], x.split("/")[4], x.split("/")[6], x.split("/")[0])
     return f"{x.split('/')[0]}/{x.split('/')[2]}/{x.split('/')[4]}/{file_name}"
 
 
-def _download(fs_fusion, fs_local, df, n_par, show_progress=True):
-    def _download_files(row):
-        p_path = row["path_fusion"]
+def _download(
+    fs_fusion: fsspec.filesystem,
+    fs_local: fsspec.filesystem,
+    df: pd.DataFrame,
+    n_par: int,
+    show_progress: bool = True,
+    local_path: str = "",
+) -> list[tuple[bool, str, Optional[str]]]:
+    def _download_files(row: pd.Series[Any]) -> tuple[bool, str, Optional[str]]:
+        p_path = local_path + row["path_fusion"]
         if not fs_local.exists(p_path):
-            try:
-                fs_local.mkdir(Path(p_path).parent, exist_ok=True, create_parents=True)
-            except Exception as ex:
-                logger.info(f"Path {p_path} exists already", ex)
+            fs_local.mkdir(Path(p_path).parent, exist_ok=True, create_parents=True)
         try:
             fs_fusion.get(row["url"], p_path, chunk_size=DEFAULT_CHUNK_SIZE)
-            return True, p_path, None
-        except Exception as ex:
-            logger.log(
+            return (True, p_path, None)
+        except BaseException as ex:
+            logger.exception(
                 VERBOSE_LVL,
                 f"Failed to write to {p_path}. ex - {ex}",
             )
             msg = str(ex)
 
-            return False, p_path, msg
+            return (False, p_path, msg)
 
-    loop = _get_loop(df, show_progress)
-    if len(df) > 1:
-        res = Parallel(n_jobs=n_par)(
-            delayed(_download_files)(row) for index, row in loop
-        )
+    if n_par > 1 and len(df) > 0:
+        if show_progress:
+            with tqdm_joblib(tqdm(total=len(df))) as _:
+                res = Parallel(n_jobs=n_par)(delayed(_download_files)(row) for _, row in df.iterrows())
+        else:
+            res = Parallel(n_jobs=n_par)(delayed(_download_files)(row) for _, row in df.iterrows())
+    elif len(df) > 0:
+        if show_progress:
+            res = [None] * len(df)
+            with tqdm(total=len(df)) as p:
+                for i, row in df.iterrows():
+                    r = _download_files(row)
+                    res[i] = r
+                    if r[0] is True:
+                        p.update(1)
+        else:
+            res = [_download_files(row) for _, row in df.iterrows()]
     else:
-        res = [_download_files(row) for index, row in loop]
+        return []
 
-    return res
+    return  # type: ignore
 
 
-def _upload(fs_fusion, fs_local, df, n_par, show_progress=True):
-    df.rename(columns={"path_local": "path"}, inplace=True)
-    loop = _get_loop(df, show_progress)
-    parallel = True if len(df) > 1 else False
+def _upload(
+    fs_fusion: fsspec.filesystem,
+    fs_local: fsspec.filesystem,
+    df: pd.DataFrame,
+    n_par: int,
+    show_progress: bool = True,
+    local_path: str = "",
+) -> list[tuple[bool, str, Optional[str]]]:
+    upload_df = df.rename(columns={"path_local": "path"})
+    upload_df["path"] = local_path + upload_df["path"]
+    parallel = len(df) > 1
     res = upload_files(
-        fs_fusion, fs_local, loop, parallel=parallel, n_par=n_par, multipart=True
+        fs_fusion,
+        fs_local,
+        upload_df,
+        parallel=parallel,
+        n_par=n_par,
+        multipart=True,
+        show_progress=show_progress,
     )
 
     return res
 
 
-def _generate_md5_token(path, fs):
-    hash_md5 = hashlib.md5()
+def _generate_sha256_token(path: str, fs: fsspec.filesystem, chunk_size: int = 5 * 2**20) -> str:
+    hash_sha256 = hashlib.sha256()
+    chunk_count = 0
     with fs.open(path, "rb") as file:
-        for chunk in iter(lambda: file.read(4096), b""):
-            hash_md5_chunk = hashlib.md5()
-            hash_md5_chunk.update(chunk)
-            hash_md5.update(chunk)
+        for chunk in iter(lambda: file.read(chunk_size), b""):
+            hash_sha256_chunk = hashlib.sha256()
+            hash_sha256_chunk.update(chunk)
+            hash_sha256.update(hash_sha256_chunk.digest())
+            chunk_count += 1
 
-    return base64.b64encode(hash_md5.digest()).decode()
+    if chunk_count > 1:
+        return base64.b64encode(hash_sha256.digest()).decode()
+    else:
+        return base64.b64encode(hash_sha256_chunk.digest()).decode()
 
 
 def _get_fusion_df(
-    fs_fusion, datasets_lst, catalog, flatten=False, dataset_format=None
-):
+    fs_fusion: fsspec.filesystem,
+    datasets_lst: list[str],
+    catalog: str,
+    flatten: bool = False,
+    dataset_format: Optional[str] = None,
+) -> pd.DataFrame:
     df_lst = []
     for dataset in datasets_lst:
         changes = fs_fusion.info(f"{catalog}/datasets/{dataset}")["changes"]["datasets"]
         if len(changes) > 0:
             changes = changes[0]["distributions"]
-            urls = [
-                catalog + "/datasets/" + "/".join(i["key"].split(".")) for i in changes
-            ]
+            keys = [i["key"].replace(".", "/").split("/") for i in changes]
+            keys = ["/".join([k[0], k[1], k[2], k[-1]]) for k in keys]
+            urls = [catalog + "/datasets/" + k for k in keys]
             urls = [i.replace("distribution", "distributions") for i in urls]
             urls = [
-                "/".join(i.split("/")[:3] + ["datasetseries"] + i.split("/")[3:])
-                if "datasetseries" not in i
-                else i
+                ("/".join(i.split("/")[:3] + ["datasetseries"] + i.split("/")[3:]) if "datasetseries" not in i else i)
                 for i in urls
             ]
-            # ts = [pd.Timestamp(i["values"][0]).timestamp() for i in changes]
             sz = [int(i["values"][1]) for i in changes]
-            md = [i["values"][2].split("md5=")[-1] for i in changes]
+            md = [i["values"][2].split("SHA-256=")[-1][:44] for i in changes]
             keys = [_url_to_path(i) for i in urls]
 
             if flatten:
                 keys = ["/".join(k.split("/")[:2] + k.split("/")[-1:]) for k in keys]
 
-            df = pd.DataFrame([keys, urls, sz, md]).T
-            df.columns = ["path", "url", "size", "md5"]
-            if dataset_format and len(df) > 0:
-                df = df[df.url.str.split("/").str[-1] == dataset_format]
-            df_lst.append(df)
+            info_df = pd.DataFrame([keys, urls, sz, md]).T
+            info_df.columns = pd.Index(["path", "url", "size", "sha256"])
+            if dataset_format and len(info_df) > 0:
+                info_df = info_df[info_df.url.str.split("/").str[-1] == dataset_format]
+            df_lst.append(info_df)
         else:
-            df_lst.append(pd.DataFrame(columns=["path", "url", "size", "md5"]))
+            df_lst.append(pd.DataFrame(columns=["path", "url", "size", "sha256"]))
 
     return pd.concat(df_lst)
 
 
-def _get_local_state(fs_local, fs_fusion, datasets, catalog, dataset_format=None):
+def _get_local_state(
+    fs_local: fsspec.filesystem,
+    fs_fusion: fsspec.filesystem,
+    datasets: list[str],
+    catalog: str,
+    dataset_format: Optional[str] = None,
+    local_state: Optional[pd.DataFrame] = None,
+    local_path: str = "",
+) -> pd.DataFrame:
     local_files = []
     local_files_rel = []
-    local_dirs = (
-        [f"{catalog}/{i}" for i in datasets] if len(datasets) > 0 else [catalog]
-    )
+    local_dirs = [f"{local_path}{catalog}/{i}" for i in datasets] if len(datasets) > 0 else [local_path + catalog]
 
     for local_dir in local_dirs:
         if not fs_local.exists(local_dir):
             fs_local.mkdir(local_dir, exist_ok=True, create_parents=True)
 
-        local_files = fs_local.find(local_dir)
-        local_rel_path = [i[i.find(local_dir) :] for i in local_files]
+        local_files_temp = fs_local.find(local_dir)
+        local_rel_path = [i[i.find(local_dir) :] for i in local_files_temp]
         local_file_validation = validate_file_names(local_rel_path, fs_fusion)
-        local_files += [
-            f for flag, f in zip(local_file_validation, local_files) if flag
-        ]
+        local_files += [f for flag, f in zip(local_file_validation, local_files_temp) if flag]
         local_files_rel += [
-            os.path.join(local_dir, relpath(i, local_dir)).replace("\\", "/")
-            for i in local_files
+            Path(local_dir, relpath(loc_file, local_dir).replace("\\", "/").replace(local_path, ""))
+            for loc_file in local_files_temp
         ]
 
-    # local_mtime = [fs_local.info(x)["mtime"] for x in local_files]
-    local_md5 = [_generate_md5_token(x, fs_local) for x in local_files]
-    local_url_eqiv = [path_to_url(i) for i in local_files]
-    df_local = pd.DataFrame([local_files_rel, local_url_eqiv, local_md5]).T
-    df_local.columns = ["path", "url", "md5"]
+    local_mtime = [fs_local.info(x)["mtime"] for x in local_files]
+    is_raw_lst = is_dataset_raw(local_files, fs_fusion)
+    local_url_eqiv = [path_to_url(i, r) for i, r in zip(local_files, is_raw_lst)]
+    df_local = pd.DataFrame([local_files_rel, local_url_eqiv, local_mtime, local_files]).T
+    df_local = df_local[["path", "url", "mtime", "local_path"]]
+
+    if local_state is not None and len(local_state) > 0:
+        df_join = df_local.merge(local_state, on="path", how="left", suffixes=("", "_prev"))
+        df_join.loc[df_join["mtime"] != df_join["mtime_prev"], "sha256"] = [
+            _generate_sha256_token(x, fs_local) for x in df_join[df_join["mtime"] != df_join["mtime_prev"]].local_path
+        ]
+        df_local.columns = pd.Index(["path", "url", "mtime", "sha256"])
+    else:
+        df_local["sha256"] = [_generate_sha256_token(x, fs_local) for x in local_files]
 
     if dataset_format and len(df_local) > 0:
         df_local = df_local[df_local.url.str.split("/").str[-1] == dataset_format]
 
     df_local = df_local.sort_values("path").drop_duplicates()
     return df_local
 
 
-def _synchronize(
+def _synchronize(  # noqa: PLR0913
     fs_fusion: fsspec.filesystem,
     fs_local: fsspec.filesystem,
     df_local: pd.DataFrame,
     df_fusion: pd.DataFrame,
     direction: str = "upload",
-    n_par: int = None,
+    n_par: Optional[int] = None,
     show_progress: bool = True,
-):
+    local_path: str = "",
+) -> list[tuple[bool, str, Optional[str]]]:
     """Synchronize two filesystems."""
 
     n_par = cpu_count(n_par)
     if direction == "upload":
-        join_df = df_local.merge(
-            df_fusion, on="url", suffixes=("_local", "_fusion"), how="left"
-        )
-        join_df = join_df[join_df["md5_local"] != join_df["md5_fusion"]]
-        res = _upload(fs_fusion, fs_local, join_df, n_par, show_progress=show_progress)
+        if len(df_local) == 0:
+            msg = "No dataset members available for upload for your dataset selection."
+            logger.warning(msg)
+            warnings.warn(msg, stacklevel=2)
+            res = []
+        else:
+            join_df = df_local.merge(df_fusion, on="url", suffixes=("_local", "_fusion"), how="left")
+            join_df = join_df[join_df["sha256_local"] != join_df["sha256_fusion"]]
+            res = _upload(
+                fs_fusion,
+                fs_local,
+                join_df,
+                n_par,
+                show_progress=show_progress,
+                local_path=local_path,
+            )
     elif direction == "download":
-        join_df = df_local.merge(
-            df_fusion, on="url", suffixes=("_local", "_fusion"), how="right"
-        )
-        join_df = join_df[join_df["md5_local"] != join_df["md5_fusion"]]
-        res = _download(
-            fs_fusion, fs_local, join_df, n_par, show_progress=show_progress
-        )
+        if len(df_fusion) == 0:
+            msg = "No dataset members available for download for your dataset selection."
+            logger.warning(msg)
+            warnings.warn(msg, stacklevel=2)
+            res = []
+        else:
+            join_df = df_local.merge(df_fusion, on="url", suffixes=("_local", "_fusion"), how="right")
+            join_df = join_df[join_df["sha256_local"] != join_df["sha256_fusion"]]
+            res = _download(
+                fs_fusion,
+                fs_local,
+                join_df,
+                n_par,
+                show_progress=show_progress,
+                local_path=local_path,
+            )
     else:
         raise ValueError("Unknown direction of operation.")
     return res
 
 
-def fsync(
+def fsync(  # noqa: PLR0913
     fs_fusion: fsspec.filesystem,
     fs_local: fsspec.filesystem,
-    products: list = None,
-    datasets: list = None,
-    catalog: str = None,
+    products: Optional[list[str]] = None,
+    datasets: Optional[list[str]] = None,
+    catalog: Optional[str] = None,
     direction: str = "upload",
-    flatten=False,
-    dataset_format=None,
-    n_par=None,
-    show_progress=True,
-    log_level=logging.ERROR,
+    flatten: bool = False,
+    dataset_format: Optional[str] = None,
+    n_par: Optional[int] = None,
+    show_progress: bool = True,
+    local_path: str = "",
+    log_level: int = logging.ERROR,
     log_path: str = ".",
-):
+) -> None:
     """Synchronisation between the local filesystem and Fusion.
 
     Args:
         fs_fusion (fsspec.filesystem): Fusion filesystem.
         fs_local (fsspec.filesystem): Local filesystem.
-        datasets (list): List of products.
+        products (list): List of products.
         datasets (list): List of datasets.
         catalog (str): Fusion catalog.
         direction (str): Direction of synchronisation: upload/download.
         flatten (bool): Flatten the folder structure.
         dataset_format (str): Dataset format for upload/download.
         n_par (int, optional): Specify how many distributions to download in parallel. Defaults to all.
-        show_progress (bool, optional): Display a progress bar during data download Defaults to True.
-        log_level: Logging level. Error level by default.
-        log_path (str, optional): The folder path where the log is stored.
+        show_progress (bool): Display a progress bar during data download Defaults to True.
+        local_path (str): path to files in the local filesystem, e.g., "s3a://my_bucket/"
+        log_level (int): Logging level. Error level by default.
+        log_path (str): The folder path where the log is stored. Defaults to ".".
 
     Returns:
 
     """
 
     if logger.hasHandlers():
         logger.handlers.clear()
-    file_handler = logging.FileHandler(
-        filename="{0}/{1}".format(log_path, "fusion_fsync.log")
-    )
+    file_handler = logging.FileHandler(filename="{}/{}".format(log_path, "fusion_fsync.log"))
     logging.addLevelName(VERBOSE_LVL, "VERBOSE")
     stdout_handler = logging.StreamHandler(sys.stdout)
     formatter = logging.Formatter(
         "%(asctime)s.%(msecs)03d %(name)s:%(levelname)s %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
     )
     stdout_handler.setFormatter(formatter)
     logger.addHandler(stdout_handler)
     logger.addHandler(file_handler)
     logger.setLevel(log_level)
 
-    catalog = "common" if not catalog else catalog
-    datasets = [] if not datasets else datasets
-    products = [] if not products else products
-
-    assert (
-        len(products) > 0 or len(datasets) > 0
-    ), "At least one list products or datasets should be non-empty."
+    catalog = catalog if catalog else "common"
+    datasets = datasets if datasets else []
+    products = products if products else []
+
+    assert len(products) > 0 or len(datasets) > 0, "At least one list products or datasets should be non-empty."
     assert direction in [
         "upload",
         "download",
     ], "The direction must be either upload or download."
 
+    if len(local_path) > 0 and local_path[-1] != "/":
+        local_path += "/"
+
     for product in products:
-        res = json.loads(fs_fusion.cat(f"common/products/{product}").decode())
+        res = json.loads(fs_fusion.cat(f"{catalog}/products/{product}").decode())
         datasets += [r["identifier"] for r in res["resources"]]
 
     assert len(datasets) > 0, "The supplied products did not contain any datasets."
 
     local_state = pd.DataFrame()
+    fusion_state = pd.DataFrame()
     while True:
         try:
             local_state_temp = _get_local_state(
-                fs_local, fs_fusion, datasets, catalog, dataset_format
+                fs_local,
+                fs_fusion,
+                datasets,
+                catalog,
+                dataset_format,
+                local_state,
+                local_path,
             )
-            if not local_state_temp.equals(local_state):
-                fusion_state = _get_fusion_df(
-                    fs_fusion, datasets, catalog, flatten, dataset_format
-                )
+            fusion_state_temp = _get_fusion_df(fs_fusion, datasets, catalog, flatten, dataset_format)
+            if not local_state_temp.equals(local_state) or not fusion_state_temp.equals(fusion_state):
                 res = _synchronize(
                     fs_fusion,
                     fs_local,
                     local_state_temp,
-                    fusion_state,
+                    fusion_state_temp,
                     direction,
                     n_par,
                     show_progress,
+                    local_path,
                 )
-                if len(res) == 0 or all((i[0] for i in res)):
+                if len(res) == 0 or all(i[0] for i in res):
                     local_state = local_state_temp
+                    fusion_state = fusion_state_temp
+
+                if not all(r[0] for r in res):
+                    failed_res = [r for r in res if not r[0]]
+                    msg = f"Not all {direction}s were successfully completed. The following failed:\n{failed_res}"
+                    errs = [r for r in res if not r[2]]
+                    logger.warning(msg)
+                    logger.warning(errs)
+                    warnings.warn(msg, stacklevel=2)
+
             else:
                 logger.info("All synced, sleeping")
                 time.sleep(10)
 
-        except KeyboardInterrupt:
+        except KeyboardInterrupt:  # noqa: PERF203
             if input("Type exit to exit: ") != "exit":
                 continue
             break
 
-        except Exception as ex:
-            logger.error("%s Issue occurred: %s", type(ex), ex)
+        except Exception as _:
+            logger.error("Exception thrown", exc_info=True)
             continue
```

### Comparing `pyfusion-1.0.9/fusion/fusion.py` & `PyFusion-1.1.0.dev1/fusion/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,834 +1,1059 @@
-"""Main Fusion module."""
+"""Fusion utilities."""
 
+import contextlib
+import json as js
 import logging
-import sys
-import warnings
+import math
+import multiprocessing as mp
+import os
+import re
+import threading
+from collections.abc import Generator
+from contextlib import nullcontext
+from datetime import date, datetime, timedelta, timezone
+from io import BytesIO
 from pathlib import Path
-from typing import Dict, List, Union
-from zipfile import ZipFile
-
+from queue import Queue
+from threading import Lock, Thread
+from typing import Any, Optional, Union
+from urllib.parse import urlparse, urlunparse
+
+import aiohttp
+import fsspec
+import joblib
 import pandas as pd
+import pyarrow as pa
+import pyarrow.parquet as pq
 import requests
 from joblib import Parallel, delayed
-from tabulate import tabulate
+from pyarrow import csv, json, unify_schemas
+from pyarrow.parquet import filters_to_expression
 from tqdm import tqdm
+from urllib3.util.retry import Retry
 
-from .authentication import FusionCredentials, get_default_fs
-from .exceptions import APIResponseError
-from .fusion_filesystem import FusionHTTPFileSystem
-from .utils import (
-    cpu_count,
-    distribution_to_filename,
-    distribution_to_url,
-    get_session,
-    normalise_dt_param_str,
-    path_to_url,
-    read_csv,
-    read_json,
-    read_parquet,
-    stream_single_file_new_session,
-    upload_files,
-    validate_file_names,
-)
+from . import __version__ as version
+from .authentication import FusionAiohttpSession, FusionCredentials, FusionOAuthAdapter
+from .types import PyArrowFilterT, WorkerQueueT
 
 logger = logging.getLogger(__name__)
 VERBOSE_LVL = 25
+DT_YYYYMMDD_RE = re.compile(r"^(\d{4})(\d{2})(\d{2})$")
+DT_YYYYMMDDTHHMM_RE = re.compile(r"(\d{4})(\d{2})(\d{2})T(\d{4})$")
+DT_YYYY_MM_DD_RE = re.compile(r"^(\d{4})-(\d{1,2})-(\d{1,2})$")
+DEFAULT_CHUNK_SIZE = 2**16
+DEFAULT_THREAD_POOL_SIZE = 5
+
+
+@contextlib.contextmanager
+def tqdm_joblib(tqdm_object: tqdm) -> Generator[tqdm, None, None]:  # type: ignore
+    # pragma: no cover
+    """Progress bar sensitive to exceptions during the batch processing.
+
+    Args:
+        tqdm_object (tqdm.tqdm): tqdm object.
+
+    Yields: tqdm.tqdm object
+
+    """
+
+    class TqdmBatchCompletionCallback(joblib.parallel.BatchCompletionCallBack):  # type: ignore
+        """Tqdm execution wrapper."""
+
+        def __call__(self, *args: Any, **kwargs: Any) -> Any:
+            n = 0
+            for i in args[0]._result:
+                try:
+                    if i[0] is True:
+                        n += 1
+                except Exception as _:  # noqa: F841, PERF203, BLE001
+                    n += 1
+            tqdm_object.update(n=n)
+            return super().__call__(*args, **kwargs)
+
+    old_batch_callback: type[joblib.parallel.BatchCompletionCallBack] = joblib.parallel.BatchCompletionCallBack
+    joblib.parallel.BatchCompletionCallBack = TqdmBatchCompletionCallback
+    try:
+        yield tqdm_object
+    finally:
+        joblib.parallel.BatchCompletionCallBack = old_batch_callback
+        tqdm_object.close()
+
+
+def cpu_count(thread_pool_size: Optional[int] = None, is_threading: bool = False) -> int:
+    """Determine the number of cpus/threads for parallelization.
+
+    Args:
+        thread_pool_size (int): override argument for number of cpus/threads.
+        is_threading: use threads instead of CPUs
+
+    Returns: number of cpus/threads to use.
+
+    """
+    if os.environ.get("NUM_THREADS") is not None:
+        return int(os.environ["NUM_THREADS"])
+    if thread_pool_size:
+        return thread_pool_size
+    if is_threading:
+        return 10
+
+    thread_pool_size = mp.cpu_count() if mp.cpu_count() else DEFAULT_THREAD_POOL_SIZE
+    return thread_pool_size
+
+
+def csv_to_table(
+    path: str,
+    fs: Optional[fsspec.filesystem] = None,
+    columns: Optional[list[str]] = None,
+    filters: Optional[PyArrowFilterT] = None,
+) -> pa.Table:
+    """Reads csv data to pyarrow table.
+
+    Args:
+        path (str): path to the file.
+        fs: filesystem object.
+        columns: columns to read.
+        filters: arrow filters.
+
+    Returns:
+        class:`pyarrow.Table` pyarrow table with the data.
+    """
+    filters = filters_to_expression(filters) if filters else filters
+    with fs.open(path) if fs else nullcontext(path) as f:
+        tbl = csv.read_csv(f)
+        if filters is not None:
+            tbl = tbl.filter(filters)
+        if columns is not None:
+            tbl = tbl.select(columns)
+        return tbl
+
+
+def json_to_table(
+    path: str,
+    fs: Optional[fsspec.filesystem] = None,
+    columns: Optional[list[str]] = None,
+    filters: Optional[PyArrowFilterT] = None,
+) -> pa.Table:
+    """Reads json data to pyarrow table.
+
+    Args:
+        path: path to json file.
+        fs: filesystem.
+        columns: columns to read.
+        filters: arrow filters.
+
+    Returns:
+        class:`pyarrow.Table` pyarrow table with the data.
+    """
+    filters = filters_to_expression(filters) if filters else filters
+    with fs.open(path) if fs else nullcontext(path) as f:
+        tbl = json.read_json(f)
+        if filters is not None:
+            tbl = tbl.filter(filters)
+        if columns is not None:
+            tbl = tbl.select(columns)
+        return tbl
+
+
+PathLikeT = Union[str, Path]
+
+
+def parquet_to_table(
+    path: Union[PathLikeT, list[PathLikeT]],
+    fs: Optional[fsspec.filesystem] = None,
+    columns: Optional[list[str]] = None,
+    filters: Optional[PyArrowFilterT] = None,
+) -> pa.Table:
+    """Reads parquet data to pyarrow table.
+
+    Args:
+        path: path to parquet file.
+        fs: filesystem.
+        columns: columns to read.
+        filters: arrow filters.
+
+    Returns:
+        class:`pyarrow.Table` pyarrow table with the data.
+    """
+
+    if isinstance(path, list):
+        schemas = [
+            pq.ParquetDataset(
+                p,
+                use_legacy_dataset=False,
+                filters=filters,
+                filesystem=fs,
+                memory_map=True,
+            ).schema
+            for p in path
+        ]
+    else:
+        schemas = [
+            pq.ParquetDataset(
+                path,
+                use_legacy_dataset=False,
+                filters=filters,
+                filesystem=fs,
+                memory_map=True,
+            ).schema
+        ]
 
+    schema = unify_schemas(schemas)
+    return pq.ParquetDataset(
+        path,
+        use_legacy_dataset=False,
+        filters=filters,
+        filesystem=fs,
+        memory_map=True,
+        schema=schema,
+    ).read(columns=columns)
+
+
+def read_csv(
+    path: str,
+    columns: Optional[list[str]] = None,
+    filters: Optional[PyArrowFilterT] = None,
+    fs: Optional[fsspec.filesystem] = None,
+    dataframe_type: str = "pandas",
+) -> Union[pd.DataFrame, pa.Table]:
+    """Reads csv with possibility of selecting columns and filtering the data.
+
+    Args:
+        path (str): path to the csv file.
+        columns: list of selected fields.
+        filters: filters.
+        fs: filesystem object.
+        dataframe_type (str, optional): Datafame type pandas or polars
+
+    Returns:
+        Union[pandas.DataFrame, polars.DataFrame]: a dataframe containing the data.
+
+    """
+    try:
+        try:
+            res = csv_to_table(path, fs, columns=columns, filters=filters)
+
+            if dataframe_type == "pandas":
+                res = res.to_pandas()
+            elif dataframe_type == "polars":
+                import polars as pl
 
-class Fusion:
-    """Core Fusion class for API access."""
+                res = pl.from_arrow(res)
+            else:
+                raise ValueError(f"Unknown DataFrame type {dataframe_type}")
+        except Exception as err:
+            logger.log(
+                VERBOSE_LVL,
+                f"Failed to read {path}, with comma delimiter.",
+                exc_info=True,
+            )
+            raise Exception from err
 
-    @staticmethod
-    def _call_for_dataframe(url: str, session: requests.Session) -> pd.DataFrame:
-        """Private function that calls an API endpoint and returns the data as a pandas dataframe.
-
-        Args:
-            url (Union[FusionCredentials, Union[str, dict]): URL for an API endpoint with valid parameters.
-            session (requests.Session): Specify a proxy if required to access the authentication server. Defaults to {}.
-
-        Returns:
-            pandas.DataFrame: a dataframe containing the requested data.
-        """
-        response = session.get(url)
-        response.raise_for_status()
-        table = response.json()["resources"]
-        df = pd.DataFrame(table).reset_index(drop=True)
-        return df
-
-    def __init__(
-        self,
-        credentials: Union[str, dict] = "config/client_credentials.json",
-        root_url: str = "https://fusion-api.jpmorgan.com/fusion/v1/",
-        download_folder: str = "downloads",
-        log_level: int = logging.ERROR,
-        fs=None,
-        log_path: str = ".",
-    ) -> None:
-        """Constructor to instantiate a new Fusion object.
-
-        Args:
-            credentials (Union[str, dict], optional): A path to a credentials file or
-                a dictionary containing the required keys.
-                Defaults to 'config/client_credentials.json'.
-            root_url (_type_, optional): The API root URL.
-                Defaults to "https://fusion-api.jpmorgan.com/fusion/v1/".
-            download_folder (str, optional): The folder path where downloaded data files
-                are saved. Defaults to "downloads".
-            log_level (int, optional): Set the logging level. Defaults to logging.ERROR.
-            fs (fsspec.filesystem): filesystem.
-            log_path (str, optional): The folder path where the log is stored.
-        """
-        self._default_catalog = "common"
-
-        self.root_url = root_url
-        self.download_folder = download_folder
-        Path(download_folder).mkdir(parents=True, exist_ok=True)
-
-        if logger.hasHandlers():
-            logger.handlers.clear()
-        file_handler = logging.FileHandler(
-            filename="{0}/{1}".format(log_path, "fusion_sdk.log")
-        )
-        logging.addLevelName(VERBOSE_LVL, "VERBOSE")
-        stdout_handler = logging.StreamHandler(sys.stdout)
-        formatter = logging.Formatter(
-            "%(asctime)s.%(msecs)03d %(name)s:%(levelname)s %(message)s",
-            datefmt="%Y-%m-%d %H:%M:%S",
+    except Exception:  # noqa: BLE001
+        logger.log(
+            VERBOSE_LVL,
+            f"Could not parse {path} properly. Trying with pandas csv reader.",
+            exc_info=True,
         )
-        stdout_handler.setFormatter(formatter)
-        logger.addHandler(stdout_handler)
-        logger.addHandler(file_handler)
-        logger.setLevel(log_level)
-
-        if isinstance(credentials, FusionCredentials):
-            self.credentials = credentials
-        else:
-            self.credentials = FusionCredentials.from_object(credentials)
+        try:  # pragma: no cover
+            with fs.open(path) if fs else nullcontext(path) as f:
+                if dataframe_type == "pandas":
+                    res = pd.read_csv(f, usecols=columns, index_col=False)
+                elif dataframe_type == "polars":
+                    import polars as pl
+
+                    res = pl.read_csv(f, columns=columns)
+                else:
+                    raise ValueError(f"Unknown DataFrame type {dataframe_type}")
+
+        except Exception as err:  # noqa: BLE001
+            logger.log(
+                VERBOSE_LVL,
+                f"Could not parse {path} properly. " f"Trying with pandas csv reader pandas engine.",
+                exc_info=True,
+            )
+            with fs.open(path) if fs else nullcontext(path) as f:
+                if dataframe_type == "pandas":
+                    res = pd.read_table(  # pragma: no cover
+                        f,
+                        usecols=columns,
+                        index_col=False,
+                        engine="python",
+                        delimiter=None,
+                    )
+                else:
+                    raise ValueError(f"Unknown DataFrame type {dataframe_type}") from err
+    return res
+
+
+def read_json(
+    path: str,
+    columns: Optional[list[str]] = None,
+    filters: Optional[PyArrowFilterT] = None,
+    fs: Optional[fsspec.filesystem] = None,
+    dataframe_type: str = "pandas",
+) -> Union[pd.DataFrame, pa.Table]:
+    """Read json files(s) to pandas.
+
+    Args:
+        path (str): path or a list of paths to parquet files.
+        columns (list): list of selected fields.
+        filters (list): filters.
+        fs: filesystem object.
+        dataframe_type (str, optional): Datafame type pandas or polars
+
+    Returns:
+        Union[pandas.DataFrame, polars.DataFrame]: a dataframe containing the data.
+    """
+
+    try:
+        try:
+            res = json_to_table(path, fs, columns=columns, filters=filters)
+            if dataframe_type == "pandas":
+                res = res.to_pandas()
+            elif dataframe_type == "polars":
+                import polars as pl
 
-        self.session = get_session(self.credentials, self.root_url)
-        self.fs = fs if fs else get_default_fs()
+                res = pl.from_arrow(res)
+            else:
+                raise ValueError(f"Unknown DataFrame type {dataframe_type}")
+        except Exception as err:
+            logger.log(
+                VERBOSE_LVL,
+                f"Failed to read {path}, with arrow reader. {err}",
+            )
+            raise err
 
-    def __repr__(self):
-        """Object representation to list all available methods."""
-        return "Fusion object \nAvailable methods:\n" + tabulate(
-            pd.DataFrame(
-                [
-                    [
-                        method_name
-                        for method_name in dir(Fusion)
-                        if callable(getattr(Fusion, method_name))
-                        and not method_name.startswith("_")
-                    ]
-                    + [
-                        p
-                        for p in dir(Fusion)
-                        if isinstance(getattr(Fusion, p), property)
-                    ]
-                ]
-            ).T.set_index(0),
-            tablefmt="psql",
+    except Exception:  # noqa: BLE001
+        logger.log(
+            VERBOSE_LVL,
+            f"Could not parse {path} properly. " f"Trying with pandas json reader.",
+            exc_info=True,
         )
-
-    @property
-    def default_catalog(self) -> str:
-        """Returns the default catalog.
-
-        Returns:
-            None
-        """
-        return self._default_catalog
-
-    @default_catalog.setter
-    def default_catalog(self, catalog) -> None:
-        """Allow the default catalog, which is "common" to be overridden.
-
-        Args:
-            catalog (str): The catalog to use as the default
-
-        Returns:
-            None
-        """
-        self._default_catalog = catalog
-
-    def __use_catalog(self, catalog):
-        """Determine which catalog to use in an API call.
-
-        Args:
-            catalog (str): The catalog value passed as an argument to an API function wrapper.
-
-        Returns:
-            str: The catalog to use
-        """
-        if catalog is None:
-            return self.default_catalog
-        else:
-            return catalog
-
-    def get_fusion_filesystem(self):
-        """Creates Fusion Filesystem.
-
-        Returns: Fusion Filesystem
-
-        """
-        return FusionHTTPFileSystem(
-            client_kwargs={"root_url": self.root_url, "credentials": self.credentials}
+        try:  # pragma: no cover
+            with fs.open(path) if fs else nullcontext(path) as f:
+                if dataframe_type == "pandas":
+                    res = pd.read_json(f)
+                elif dataframe_type == "polars":
+                    import polars as pl
+
+                    res = pl.read_json(f)
+                else:
+                    raise ValueError(f"Unknown DataFrame type {dataframe_type}")
+
+        except Exception as err:
+            logger.log(VERBOSE_LVL, f"Could not parse {path} properly. ", exc_info=True)
+            raise err  # pragma: no cover
+    return res
+
+
+def read_parquet(
+    path: PathLikeT,
+    columns: Optional[list[str]] = None,
+    filters: Optional[PyArrowFilterT] = None,
+    fs: Optional[fsspec.filesystem] = None,
+    dataframe_type: str = "pandas",
+) -> Union[pd.DataFrame, pa.Table]:
+    """Read parquet files(s) to pandas.
+
+    Args:
+        path (PathLikeT): path or a list of paths to parquet files.
+        columns (list): list of selected fields.
+        filters (list): filters.
+        fs: filesystem object.
+        dataframe_type (str, optional): Datafame type pandas or polars
+
+    Returns:
+        Union[pandas.DataFrame, polars.DataFrame]: a dataframe containing the data.
+
+    """
+
+    tbl = parquet_to_table(path, columns=columns, filters=filters, fs=fs)
+    if dataframe_type == "pandas":
+        return tbl.to_pandas()
+    if dataframe_type == "polars":
+        import polars as pl
+
+        return pl.from_arrow(tbl)
+    else:
+        raise ValueError(f"Unknown DataFrame type {dataframe_type}")
+
+
+def _normalise_dt_param(dt: Union[str, int, datetime, date]) -> str:
+    """Convert dates into a normalised string representation.
+
+    Args:
+        dt (Union[str, int, datetime, date]): A date represented in various types.
+
+    Returns:
+        str: A normalized date string.
+    """
+    if isinstance(dt, (date, datetime)):
+        return dt.strftime("%Y-%m-%d")
+
+    if isinstance(dt, int):
+        dt = str(dt)
+
+    if not isinstance(dt, str):
+        raise ValueError(f"{dt} is not in a recognised data format")
+
+    matches = DT_YYYY_MM_DD_RE.match(dt)
+    if matches:
+        yr = matches.group(1)
+        mth = matches.group(2).zfill(2)
+        day = matches.group(3).zfill(2)
+        return f"{yr}-{mth}-{day}"
+
+    matches = DT_YYYYMMDD_RE.match(dt)
+
+    if matches:
+        return "-".join(matches.groups())
+
+    matches = DT_YYYYMMDDTHHMM_RE.match(dt)
+
+    if matches:
+        return "-".join(matches.groups())
+
+    raise ValueError(f"{dt} is not in a recognised data format")
+
+
+def normalise_dt_param_str(dt: str) -> tuple[str, ...]:
+    """Convert a date parameter which may be a single date or a date range into a tuple.
+
+    Args:
+        dt (str): Either a single date or a date range separated by a ":".
+
+    Returns:
+        tuple: A tuple of dates.
+    """
+    date_parts = dt.split(":")
+    max_date_seg_cnt = 2
+    if not date_parts or len(date_parts) > max_date_seg_cnt:
+        raise ValueError(f"Unable to parse {dt} as either a date or an interval")
+
+    return tuple(_normalise_dt_param(dt_part) if dt_part else dt_part for dt_part in date_parts)
+
+
+def distribution_to_filename(
+    root_folder: str,
+    dataset: str,
+    datasetseries: str,
+    file_format: str,
+    catalog: str = "common",
+    partitioning: Optional[str] = None,
+) -> str:
+    """Returns a filename representing a dataset distribution.
+
+    Args:
+        root_folder (str): The root folder path.
+        dataset (str): The dataset identifier.
+        datasetseries (str): The datasetseries instance identifier.
+        file_format (str): The file type, e.g. CSV or Parquet
+        catalog (str, optional): The data catalog containing the dataset. Defaults to "common".
+        partitioning (str, optional): Partitioning specification.
+
+    Returns:
+        str: FQ distro file name
+    """
+    if datasetseries[-1] == "/" or datasetseries[-1] == "\\":
+        datasetseries = datasetseries[0:-1]
+
+    if partitioning == "hive":
+        file_name = f"{dataset}.{file_format}"
+    else:
+        file_name = f"{dataset}__{catalog}__{datasetseries}.{file_format}"
+
+    sep = "/"
+    if "\\" in root_folder:
+        sep = "\\"
+    return f"{root_folder}{sep}{file_name}"
+
+
+def _filename_to_distribution(file_name: str) -> tuple[str, str, str, str]:
+    """Breaks a filename down into the components that represent a dataset distribution in the catalog.
+
+    Args:
+        file_name (str): The filename to decompose.
+
+    Returns:
+        tuple: A tuple consisting of catalog id, dataset id, datasetseries instane id, and file format (e.g. CSV).
+    """
+    dataset, catalog, series_format = Path(file_name).name.split("__")
+    datasetseries, file_format = series_format.split(".")
+    return catalog, dataset, datasetseries, file_format
+
+
+def distribution_to_url(
+    root_url: str,
+    dataset: str,
+    datasetseries: str,
+    file_format: str,
+    catalog: str = "common",
+    is_download: bool = False,
+) -> str:
+    """Returns the API URL to download a dataset distribution.
+
+    Args:
+        root_url (str): The base url for the API.
+        dataset (str): The dataset identifier.
+        datasetseries (str): The datasetseries instance identifier.
+        file_format (str): The file type, e.g. CSV or Parquet
+        catalog (str, optional): The data catalog containing the dataset. Defaults to "common".
+        is_download (bool, optional): Is url for download
+
+    Returns:
+        str: A URL for the API distribution endpoint.
+    """
+    if datasetseries[-1] == "/" or datasetseries[-1] == "\\":
+        datasetseries = datasetseries[0:-1]
+
+    if datasetseries == "sample":
+        return f"{root_url}catalogs/{catalog}/datasets/{dataset}/sample/distributions/csv"
+    if is_download:
+        return (
+            f"{root_url}catalogs/{catalog}/datasets/{dataset}/datasetseries/"
+            f"{datasetseries}/distributions/{file_format}/operationType/download"
         )
+    return (
+        f"{root_url}catalogs/{catalog}/datasets/{dataset}/datasetseries/" f"{datasetseries}/distributions/{file_format}"
+    )
+
+
+def _get_canonical_root_url(any_url: str) -> str:
+    """Get the full URL for the API endpoint.
+
+    Args:
+        any_url (str): A valid URL or URL part
+
+    Returns:
+        str: A complete root URL
+
+    """
+    url_parts = urlparse(any_url)
+    root_url = urlunparse((url_parts[0], url_parts[1], "", "", "", ""))
+    return root_url
+
+
+async def get_client(credentials: FusionCredentials, **kwargs: Any) -> FusionAiohttpSession:  # noqa: PLR0915
+    """Gets session for async.
+
+    Args:
+        credentials: Credentials.
+        **kwargs: Kwargs.
+
+    Returns:
+
+    """
+
+    async def on_request_start_token(session: Any, _trace_config_ctx: Any, params: Any) -> None:
+        async def _refresh_token_data() -> tuple[str, str]:
+            payload = (
+                {
+                    "grant_type": "client_credentials",
+                    "client_id": credentials.client_id,
+                    "client_secret": credentials.client_secret,
+                    "aud": credentials.resource,
+                }
+                if credentials.grant_type == "client_credentials"
+                else {
+                    "grant_type": "password",
+                    "client_id": credentials.client_id,
+                    "username": credentials.username,
+                    "password": credentials.password,
+                    "resource": credentials.resource,
+                }
+            )
+            async with aiohttp.ClientSession(trust_env=True) as session:
+                if not credentials.auth_url:
+                    raise ValueError("Auth URL is required for token refresh")
+                if credentials.proxies:
+                    response = await session.post(credentials.auth_url, data=payload, proxy=http_proxy)
+                else:
+                    response = await session.post(credentials.auth_url, data=payload)
+                response_data = await response.json()
+
+            access_token = response_data["access_token"]
+            expiry = response_data["expires_in"]
+            return access_token, expiry
+
+        token_expires_in = (session.credentials.bearer_token_expiry - datetime.now(tz=timezone.utc)).total_seconds()
+        if session.credentials.is_bearer_token_expirable and token_expires_in < session.refresh_within_seconds:
+            token, expiry = await _refresh_token_data()
+            session.credentials.bearer_token = token
+            session.credentials.bearer_token_expiry = datetime.now(tz=timezone.utc) + timedelta(seconds=int(expiry))
+            session.number_token_refreshes += 1
 
-    def list_catalogs(self, output: bool = False) -> pd.DataFrame:
-        """Lists the catalogs available to the API account.
-
-        Args:
-            output (bool, optional): If True then print the dataframe. Defaults to False.
+        params.headers.update(
+            {
+                "Authorization": f"Bearer {session.credentials.bearer_token}",
+                "User-Agent": f"fusion-python-sdk {version}",
+            }
+        )
 
-        Returns:
-            class:`pandas.DataFrame`: A dataframe with a row for each catalog
-        """
-        url = f"{self.root_url}catalogs/"
-        df = Fusion._call_for_dataframe(url, self.session)
-
-        if output:
-            print(tabulate(df, headers="keys", tablefmt="psql"))
-
-        return df
-
-    def catalog_resources(
-        self, catalog: str = None, output: bool = False
-    ) -> pd.DataFrame:
-        """List the resources contained within the catalog, for example products and datasets.
-
-        Args:
-            catalog (str, optional): A catalog identifier. Defaults to 'common'.
-            output (bool, optional): If True then print the dataframe. Defaults to False.
-
-        Returns:
-           class:`pandas.DataFrame`: A dataframe with a row for each resource within the catalog
-        """
-        catalog = self.__use_catalog(catalog)
-
-        url = f"{self.root_url}catalogs/{catalog}"
-        df = Fusion._call_for_dataframe(url, self.session)
-
-        if output:
-            print(tabulate(df, headers="keys", tablefmt="psql", maxcolwidths=30))
-
-        return df
-
-    def list_products(
-        self,
-        contains: Union[str, list] = None,
-        id_contains: bool = False,
-        catalog: str = None,
-        output: bool = False,
-        max_results: int = -1,
-        display_all_columns: bool = False,
-    ) -> pd.DataFrame:
-        """Get the products contained in a catalog. A product is a grouping of datasets.
-
-        Args:
-            contains (Union[str, list], optional): A string or a list of strings that are product
-                identifiers to filter the products list. If a list is provided then it will return
-                products whose identifier matches any of the strings. Defaults to None.
-            id_contains (bool): Filter datasets only where the string(s) are contained in the identifier,
-                ignoring description.
-            catalog (str, optional): A catalog identifier. Defaults to 'common'.
-            output (bool, optional): If True then print the dataframe. Defaults to False.
-            max_results (int, optional): Limit the number of rows returned in the dataframe.
-                Defaults to -1 which returns all results.
-            display_all_columns (bool, optional): If True displays all columns returned by the API,
-                otherwise only the key columns are displayed
-
-        Returns:
-            class:`pandas.DataFrame`: a dataframe with a row for each product
-        """
-        catalog = self.__use_catalog(catalog)
-
-        url = f"{self.root_url}catalogs/{catalog}/products"
-        df = Fusion._call_for_dataframe(url, self.session)
-
-        if contains:
-            if isinstance(contains, list):
-                contains = "|".join(f"{s}" for s in contains)
-            if id_contains:
-                df = df[df["identifier"].str.contains(contains, case=False)]
+    async def on_request_start_fusion_token(session: Any, _trace_config_ctx: Any, params: Any) -> None:
+        async def _refresh_fusion_token_data() -> tuple[str, str]:
+            full_url_lst = str(params.url).split("/")
+            url = "/".join(full_url_lst[: full_url_lst.index("datasets") + 2]) + "/authorize/token"
+            if credentials.proxies:
+                async with session.get(url, proxy=http_proxy) as response:
+                    response_data = await response.json()
             else:
-                df = df[
-                    df["identifier"].str.contains(contains, case=False)
-                    | df["description"].str.contains(contains, case=False)
-                ]
-
-        df["category"] = df.category.str.join(", ")
-        df["region"] = df.region.str.join(", ")
-        if not display_all_columns:
-            df = df[
-                ["identifier", "title", "region", "category", "status", "description"]
-            ]
-
-        if max_results > -1:
-            df = df[0:max_results]
-
-        if output:
-            print(tabulate(df, headers="keys", tablefmt="psql", maxcolwidths=30))
-
-        return df
-
-    def list_datasets(
-        self,
-        contains: Union[str, list] = None,
-        id_contains: bool = False,
-        catalog: str = None,
-        output: bool = False,
-        max_results: int = -1,
-        display_all_columns: bool = False,
-    ) -> pd.DataFrame:
-        """_summary_.
-
-        Args:
-            contains (Union[str, list], optional): A string or a list of strings that are dataset
-                identifiers to filter the datasets list. If a list is provided then it will return
-                datasets whose identifier matches any of the strings. Defaults to None.
-            id_contains (bool): Filter datasets only where the string(s) are contained in the identifier,
-                ignoring description.
-            catalog (str, optional): A catalog identifier. Defaults to 'common'.
-            output (bool, optional): If True then print the dataframe. Defaults to False.
-            max_results (int, optional): Limit the number of rows returned in the dataframe.
-                Defaults to -1 which returns all results.
-            display_all_columns (bool, optional): If True displays all columns returned by the API,
-                otherwise only the key columns are displayed
-
-        Returns:
-            class:`pandas.DataFrame`: a dataframe with a row for each dataset.
-        """
-        catalog = self.__use_catalog(catalog)
-
-        url = f"{self.root_url}catalogs/{catalog}/datasets"
-        df = Fusion._call_for_dataframe(url, self.session)
-
-        if contains:
-            if isinstance(contains, list):
-                contains = "|".join(f"{s}" for s in contains)
-            if id_contains:
-                df = df[df["identifier"].str.contains(contains, case=False)]
+                async with session.get(url) as response:
+                    response_data = await response.json()
+            access_token = response_data["access_token"]
+            expiry = response_data["expires_in"]
+            return access_token, expiry
+
+        url_lst = params.url.path.split("/")
+        fusion_auth_req = "distributions" in url_lst
+        if fusion_auth_req:
+            catalog = url_lst[url_lst.index("catalogs") + 1]
+            dataset = url_lst[url_lst.index("datasets") + 1]
+            fusion_token_key = catalog + "_" + dataset
+            if fusion_token_key not in session.fusion_token_dict:
+                fusion_token, fusion_token_expiry = await _refresh_fusion_token_data()
+                session.fusion_token_dict[fusion_token_key] = fusion_token
+                session.fusion_token_expiry_dict[fusion_token_key] = datetime.now(tz=timezone.utc) + timedelta(
+                    seconds=int(fusion_token_expiry)
+                )
+                logger.log(VERBOSE_LVL, "Refreshed fusion token")
             else:
-                df = df[
-                    df["identifier"].str.contains(contains, case=False)
-                    | df["description"].str.contains(contains, case=False)
-                ]
-
-        if max_results > -1:
-            df = df[0:max_results]
-
-        df["category"] = df.category.str.join(", ")
-        df["region"] = df.region.str.join(", ")
-        if not display_all_columns:
-            df = df[
-                [
-                    "identifier",
-                    "title",
-                    "region",
-                    "category",
-                    "coverageStartDate",
-                    "coverageEndDate",
-                    "description",
-                ]
-            ]
-
-        if output:
-            print(tabulate(df, headers="keys", tablefmt="psql", maxcolwidths=30))
-
-        return df
-
-    def dataset_resources(
-        self, dataset: str, catalog: str = None, output: bool = False
-    ) -> pd.DataFrame:
-        """List the resources available for a dataset, currently this will always be a datasetseries.
-
-        Args:
-            dataset (str): A dataset identifier
-            catalog (str, optional): A catalog identifier. Defaults to 'common'.
-            output (bool, optional): If True then print the dataframe. Defaults to False.
-
-        Returns:
-            class:`pandas.DataFrame`: A dataframe with a row for each resource
-        """
-        catalog = self.__use_catalog(catalog)
-
-        url = f"{self.root_url}catalogs/{catalog}/datasets/{dataset}"
-        df = Fusion._call_for_dataframe(url, self.session)
-
-        if output:
-            print(tabulate(df, headers="keys", tablefmt="psql"))
-
-        return df
-
-    def list_dataset_attributes(
-        self,
-        dataset: str,
-        catalog: str = None,
-        output: bool = False,
-        display_all_columns: bool = False,
-    ) -> pd.DataFrame:
-        """Returns the list of attributes that are in the dataset.
-
-        Args:
-            dataset (str): A dataset identifier
-            catalog (str, optional): A catalog identifier. Defaults to 'common'.
-            output (bool, optional): If True then print the dataframe. Defaults to False.
-            display_all_columns (bool, optional): If True displays all columns returned by the API,
-                otherwise only the key columns are displayed
-
-        Returns:
-            class:`pandas.DataFrame`: A dataframe with a row for each attribute
-        """
-        catalog = self.__use_catalog(catalog)
-
-        url = f"{self.root_url}catalogs/{catalog}/datasets/{dataset}/attributes"
-        df = (
-            Fusion._call_for_dataframe(url, self.session)
-            .sort_values(by="index")
-            .reset_index(drop=True)
-        )
-
-        if not display_all_columns:
-            df = df[["identifier", "dataType", "isDatasetKey", "description"]]
-
-        if output:
-            print(tabulate(df, headers="keys", tablefmt="psql", maxcolwidths=30))
-
-        return df
-
-    def list_datasetmembers(
-        self,
-        dataset: str,
-        catalog: str = None,
-        output: bool = False,
-        max_results: int = -1,
-    ) -> pd.DataFrame:
-        """List the available members in the dataset series.
-
-        Args:
-            dataset (str): A dataset identifier
-            catalog (str, optional): A catalog identifier. Defaults to 'common'.
-            output (bool, optional): If True then print the dataframe. Defaults to False.
-            max_results (int, optional): Limit the number of rows returned in the dataframe.
-                Defaults to -1 which returns all results.
-
-        Returns:
-            class:`pandas.DataFrame`: a dataframe with a row for each dataset member.
-        """
-        catalog = self.__use_catalog(catalog)
-
-        url = f"{self.root_url}catalogs/{catalog}/datasets/{dataset}/datasetseries"
-        df = Fusion._call_for_dataframe(url, self.session)
-
-        if max_results > -1:
-            df = df[0:max_results]
-
-        if output:
-            print(tabulate(df, headers="keys", tablefmt="psql"))
-
-        return df
-
-    def datasetmember_resources(
-        self, dataset: str, series: str, catalog: str = None, output: bool = False
-    ) -> pd.DataFrame:
-        """List the available resources for a datasetseries member.
-
-        Args:
-            dataset (str): A dataset identifier
-            series (str): The datasetseries identifier
-            catalog (str, optional): A catalog identifier. Defaults to 'common'.
-            output (bool, optional): If True then print the dataframe. Defaults to False.
-
-        Returns:
-            class:`pandas.DataFrame`: A dataframe with a row for each datasetseries member resource.
-                Currently, this will always be distributions.
-        """
-        catalog = self.__use_catalog(catalog)
-
-        url = f"{self.root_url}catalogs/{catalog}/datasets/{dataset}/datasetseries/{series}"
-        df = Fusion._call_for_dataframe(url, self.session)
-
-        if output:
-            print(tabulate(df, headers="keys", tablefmt="psql"))
-
-        return df
-
-    def list_distributions(
-        self, dataset: str, series: str, catalog: str = None, output: bool = False
-    ) -> pd.DataFrame:
-        """List the available distributions (downloadable instances of the dataset with a format type).
-
-        Args:
-            dataset (str): A dataset identifier
-            series (str): The datasetseries identifier
-            catalog (str, optional): A catalog identifier. Defaults to 'common'.
-            output (bool, optional): If True then print the dataframe. Defaults to False.
-
-        Returns:
-            class:`pandas.DataFrame`: A dataframe with a row for each distribution.
-        """
-        catalog = self.__use_catalog(catalog)
-
-        url = f"{self.root_url}catalogs/{catalog}/datasets/{dataset}/datasetseries/{series}/distributions"
-        df = Fusion._call_for_dataframe(url, self.session)
-
-        if output:
-            print(tabulate(df, headers="keys", tablefmt="psql"))
-
-        return df
-
-    def _resolve_distro_tuples(
-        self,
-        dataset: str,
-        dt_str: str = "latest",
-        dataset_format: str = "parquet",
-        catalog: str = None,
-    ):
-        """Resolve distribution tuples given specification params.
-
-        A private utility function to generate a list of distribution tuples.
-        Each tuple is a distribution, identified by catalog, dataset id,
-        datasetseries member id, and the file format.
-
-        Args:
-            dataset (str): A dataset identifier
-            dt_str (str, optional): Either a single date or a range identified by a start or end date,
-                or both separated with a ":". Defaults to 'latest' which will return the most recent
-                instance of the dataset.
-            dataset_format (str, optional): The file format, e.g. CSV or Parquet. Defaults to 'parquet'.
-            catalog (str, optional): A catalog identifier. Defaults to 'common'.
-
-        Returns:
-            list: a list of tuples, one for each distribution
-        """
-        catalog = self.__use_catalog(catalog)
-
-        datasetseries_list = self.list_datasetmembers(dataset, catalog)
-
-        if datasetseries_list.empty:
-            raise APIResponseError(
-                f"No data available for dataset {dataset}. "
-                f"Check that a valid dataset identifier and date/date range has been set."
-            )
+                fusion_token_expires_in = (
+                    session.fusion_token_expiry_dict[fusion_token_key] - datetime.now(tz=timezone.utc)
+                ).total_seconds()
+                if fusion_token_expires_in < session.refresh_within_seconds:
+                    (
+                        fusion_token,
+                        fusion_token_expiry,
+                    ) = await _refresh_fusion_token_data()
+                    session.fusion_token_dict[fusion_token_key] = fusion_token
+                    session.fusion_token_expiry_dict[fusion_token_key] = datetime.now(tz=timezone.utc) + timedelta(
+                        seconds=int(fusion_token_expiry)
+                    )
+                    logger.log(VERBOSE_LVL, "Refreshed fusion token")
 
-        if dt_str == "latest":
-            dt_str = datasetseries_list.iloc[
-                datasetseries_list["createdDate"].values.argmax()
-            ]["identifier"]
-
-        parsed_dates = normalise_dt_param_str(dt_str)
-        if len(parsed_dates) == 1:
-            parsed_dates = (parsed_dates[0], parsed_dates[0])
-
-        if parsed_dates[0]:
-            datasetseries_list = datasetseries_list[
-                datasetseries_list["fromDate"] >= parsed_dates[0]
-            ]
-
-        if parsed_dates[1]:
-            datasetseries_list = datasetseries_list[
-                datasetseries_list["toDate"] <= parsed_dates[1]
-            ]
-
-        required_series = list(datasetseries_list["@id"])
-        tups = [
-            (catalog, dataset, series, dataset_format) for series in required_series
-        ]
+            params.headers.update({"Fusion-Authorization": f"Bearer {session.fusion_token_dict[fusion_token_key]}"})
 
-        return tups
+    if credentials.proxies:
+        http_proxy: Optional[str] = None
+        if "http" in credentials.proxies:
+            http_proxy = credentials.proxies["http"]
+        elif "https" in credentials.proxies:
+            http_proxy = credentials.proxies["https"]
+
+    trace_config = aiohttp.TraceConfig()
+    trace_config.on_request_start.append(on_request_start_token)
+    trace_config.on_request_start.append(on_request_start_fusion_token)
+
+    if "timeout" in kwargs:
+        timeout = aiohttp.ClientTimeout(total=kwargs["timeout"])
+    else:
+        timeout = aiohttp.ClientTimeout(total=60 * 60)  # default 60min timeout
+    session = FusionAiohttpSession(trace_configs=[trace_config], trust_env=True, timeout=timeout)
+    session.post_init(credentials=credentials)
+    return session
+
+
+def get_session(
+    credentials: FusionCredentials, root_url: str, get_retries: Optional[Union[int, Retry]] = None
+) -> requests.Session:
+    """Create a new http session and set parameters.
+
+    Args:
+        credentials (FusionCredentials): Valid user credentials to provide an acces token
+        root_url (str): The URL to call.
+
+    Returns:
+        requests.Session(): A HTTP Session object
+
+    """
+    if not get_retries:
+        get_retries = Retry(total=5, backoff_factor=0.1, status_forcelist=[429, 500, 502, 503, 504])
+    else:
+        get_retries = Retry.from_int(get_retries)
+    session = requests.Session()
+    if credentials.proxies:
+        session.proxies.update(credentials.proxies)
+    try:
+        mount_url = _get_canonical_root_url(root_url)
+    except Exception:  # noqa: BLE001
+        mount_url = "https://"
+    auth_handler = FusionOAuthAdapter(credentials, max_retries=get_retries, mount_url=mount_url)
+    session.mount(mount_url, auth_handler)
+    return session
+
+
+def _stream_single_file_new_session_dry_run(
+    credentials: FusionCredentials, url: str, output_file: str
+) -> tuple[bool, str, Optional[str]]:
+    """Function to test that a distribution is available without downloading.
+
+    Args:
+        credentials (FusionCredentials): Valid user credentials to provide an acces token
+        root_url (str): The URL to call.
+        output_file: The filename that the data will be saved into.
+
+    Returns:
+        requests.Session(): A HTTP Session object
+
+    """
+    try:
+        resp = get_session(credentials, url).head(url)
+        resp.raise_for_status()
+        return (True, output_file, None)
+    except BaseException as ex:  # noqa: BLE001
+        logger.log(VERBOSE_LVL, f"Failed to download url {url} to {output_file}", exc_info=True)
+        return (False, output_file, str(ex))
+
+
+def stream_single_file_new_session_chunks(  # noqa: PLR0913
+    session: requests.Session,
+    url: str,
+    output_file: fsspec.spec.AbstractBufferedFile,
+    start: int,
+    end: int,
+    lock: threading.Lock,
+    results: list[tuple[bool, str, Optional[str]]],
+    idx: int,
+    overwrite: bool = True,
+    fs: Optional[fsspec.AbstractFileSystem] = None,
+) -> int:
+    """Function to stream a single file from the API to a file on disk.
+
+    Args:
+        session (class `requests.Session`): HTTP session.
+        url (str): The URL to call.
+        output_file: The file handle for the target write file.
+        start (int): Start byte.
+        end(int): End byte.
+        lock (Threading.Lock): Lock.
+        results (list): Results list.
+        idx (int): Results list index.
+        overwrite (bool, optional): True if previously downloaded files should be overwritten. Defaults to True.
+        fs (fsspec.filesystem): Filesystem.
+
+    Returns:
+        int: Exit status
+
+    """
+    if fs is None:
+        fs = fsspec.filesystem("file")
+    if not overwrite and fs.exists(output_file):
+        results[idx] = True, output_file, None
+        return 0
+
+    try:
+        url = url + f"?downloadRange=bytes={start}-{end-1}"
+        with session.get(url, stream=False) as r:
+            r.raise_for_status()
+            with lock:
+                output_file.seek(start)
+                output_file.write(r.content)
 
-    def download(
-        self,
-        dataset: str,
-        dt_str: str = "latest",
-        dataset_format: str = "parquet",
-        catalog: str = None,
-        n_par: int = None,
-        show_progress: bool = True,
-        force_download: bool = False,
-        download_folder: str = None,
-        return_paths: bool = False,
-    ):
-        """Downloads the requested distributions of a dataset to disk.
-
-        Args:
-            dataset (str): A dataset identifier
-            dt_str (str, optional): Either a single date or a range identified by a start or end date,
-                or both separated with a ":". Defaults to 'latest' which will return the most recent
-                instance of the dataset.
-            dataset_format (str, optional): The file format, e.g. CSV or Parquet. Defaults to 'parquet'.
-            catalog (str, optional): A catalog identifier. Defaults to 'common'.
-            n_par (int, optional): Specify how many distributions to download in parallel.
-                Defaults to all cpus available.
-            show_progress (bool, optional): Display a progress bar during data download Defaults to True.
-            force_download (bool, optional): If True then will always download a file even
-                if it is already on disk. Defaults to True.
-            download_folder (str, optional): The path, absolute or relative, where downloaded files are saved.
-                Defaults to download_folder as set in __init__
-            return_paths (bool, optional): Return paths and success statuses of the downloaded files.
-
-        Returns:
-
-        """
-        catalog = self.__use_catalog(catalog)
-
-        n_par = cpu_count(n_par)
-        required_series = self._resolve_distro_tuples(
-            dataset, dt_str, dataset_format, catalog
+        logger.log(
+            VERBOSE_LVL,
+            f"Wrote {start} - {end} bytes to {output_file}",
         )
+        results[idx] = (True, output_file, None)
+        return 0
+    except Exception as ex:  # noqa: BLE001
+        logger.log(
+            VERBOSE_LVL,
+            f"Failed to write to {output_file}.",
+            exc_info=True,
+        )
+        results[idx] = (False, output_file, str(ex))
+        return 1
 
-        if not download_folder:
-            download_folder = self.download_folder
 
-        if not self.fs.exists(download_folder):
-            self.fs.mkdir(download_folder, create_parents=True)
-        download_spec = [
-            {
-                "credentials": self.credentials,
-                "url": distribution_to_url(
-                    self.root_url, series[1], series[2], series[3], series[0]
-                ),
-                "output_file": distribution_to_filename(
-                    download_folder, series[1], series[2], series[3], series[0]
-                ),
-                "overwrite": force_download,
-                "fs": self.fs,
-            }
-            for series in required_series
-        ]
-
-        if show_progress:
-            loop = tqdm(download_spec)
-        else:
-            loop = download_spec
+def _worker(
+    queue: WorkerQueueT,
+    session: requests.Session,
+    url: str,
+    output_file: str,
+    lock: threading.Lock,
+    results: list[tuple[bool, str, Optional[str]]],
+) -> None:
+    while True:
+        idx, start, end = queue.get()
+        if idx == -1 and start == -1 and end == -1:
+            break
+        stream_single_file_new_session_chunks(session, url, output_file, start, end, lock, results, idx)
+        queue.task_done()
+
+
+def download_single_file_threading(
+    credentials: FusionCredentials,
+    url: str,
+    output_file: fsspec.spec.AbstractBufferedFile,
+    chunk_size: int = 5 * 2**20,
+    fs: Optional[fsspec.AbstractFileSystem] = None,
+    max_threads: int = 10,
+) -> list[tuple[bool, str, Optional[str]]]:
+    """Download single file using range requests.
+
+    Args:
+        credentials (FusionCredentials): Valid user credentials to provide an access token
+        url (str): The URL to call.
+        output_file (str): The filename that the data will be saved into.
+        chunk_size (int): Chunk size for parallelization.
+        fs (fsspec.filesystem): Filesystem.
+        max_threads (int, optional): Number of threads to use. Defaults to 10.
+
+    Returns: List[Tuple]
+
+    """
+    if fs is None:
+        fs = fsspec.filesystem("file")
+    session = get_session(credentials, url)
+    header = session.head(url).headers
+    content_length = int(header["Content-Length"])
+    n_chunks = int(math.ceil(content_length / chunk_size))
+    starts = [i * chunk_size for i in range(n_chunks)]
+    ends = [min((i + 1) * chunk_size, content_length) for i in range(n_chunks)]
+    lock = Lock()
+    output_file_h: fsspec.spec.AbstractBufferedFile = fs.open(output_file, "wb")
+    results = [None] * n_chunks
+    queue: WorkerQueueT = Queue(max_threads)
+    threads = []
+    for _ in range(max_threads):
+        t = Thread(target=_worker, args=(queue, session, url, output_file_h, lock, results))
+        t.start()
+        threads.append(t)
+
+    for idx, (start, end) in enumerate(zip(starts, ends)):
+        queue.put((idx, start, end))
+
+    queue.join()
+
+    for _ in range(max_threads):
+        queue.put((-1, -1, -1))
+    for t in threads:
+        t.join()
+
+    output_file_h.close()
+    return results  # type: ignore
+
+
+def stream_single_file_new_session(
+    credentials: FusionCredentials,
+    url: str,
+    output_file: str,
+    overwrite: bool = True,
+    block_size: int = DEFAULT_CHUNK_SIZE,
+    dry_run: bool = False,
+    fs: Optional[fsspec.AbstractFileSystem] = None,
+) -> tuple[bool, str, Optional[str]]:
+    """Function to stream a single file from the API to a file on disk.
+
+    Args:
+        credentials (FusionCredentials): Valid user credentials to provide an access token
+        url (str): The URL to call.
+        output_file (str): The filename that the data will be saved into.
+        overwrite (bool, optional): True if previously downloaded files should be overwritten. Defaults to True.
+        block_size (int, optional): The chunk size to download data. Defaults to DEFAULT_CHUNK_SIZE
+        dry_run (bool, optional): Test that a file can be downloaded and return the filename without
+            downloading the data. Defaults to False.
+        fs (fsspec.filesystem): Filesystem.
+
+    Returns:
+        tuple: A tuple
+
+    """
+    if fs is None:
+        fs = fsspec.filesystem("file")
+    if dry_run:
+        return _stream_single_file_new_session_dry_run(credentials, url, output_file)
+
+    if not overwrite and fs.exists(output_file):
+        return True, output_file, None
+
+    try:
+        with get_session(credentials, url).get(url, stream=True) as r:
+            r.raise_for_status()
+            byte_cnt = 0
+            with fs.open(output_file, "wb") as outfile:
+                for chunk in r.iter_content(block_size):
+                    byte_cnt += len(chunk)
+                    outfile.write(chunk)
         logger.log(
             VERBOSE_LVL,
-            f"Beginning {len(loop)} downloads in batches of {n_par}",
-        )
-        res = Parallel(n_jobs=n_par)(
-            delayed(stream_single_file_new_session)(**spec) for spec in loop
+            f"Wrote {byte_cnt:,} bytes to {output_file}",
         )
-        if (len(res) > 0) and (not all((r[0] for r in res))):
-            for r in res:
-                if not r[0]:
-                    warnings.warn(f"The download of {r[1]} was not successful")
-        return res if return_paths else None
-
-    def to_df(
-        self,
-        dataset: str,
-        dt_str: str = "latest",
-        dataset_format: str = "parquet",
-        catalog: str = None,
-        n_par: int = None,
-        show_progress: bool = True,
-        columns: List = None,
-        filters: List = None,
-        force_download: bool = False,
-        download_folder: str = None,
-        **kwargs,
-    ) -> pd.DataFrame:
-        """Gets distributions for a specified date or date range and returns the data as a dataframe.
-
-        Args:
-            dataset (str): A dataset identifier
-            dt_str (str, optional): Either a single date or a range identified by a start or end date,
-                or both separated with a ":". Defaults to 'latest' which will return the most recent
-                instance of the dataset.
-            dataset_format (str, optional): The file format, e.g. CSV or Parquet. Defaults to 'parquet'.
-            catalog (str, optional): A catalog identifier. Defaults to 'common'.
-            n_par (int, optional): Specify how many distributions to download in parallel.
-                Defaults to all cpus available.
-            show_progress (bool, optional): Display a progress bar during data download Defaults to True.
-            columns (List, optional): A list of columns to return from a parquet file. Defaults to None
-            filters (List, optional): List[Tuple] or List[List[Tuple]] or None (default)
-                Rows which do not match the filter predicate will be removed from scanned data.
-                Partition keys embedded in a nested directory structure will be exploited to avoid
-                loading files at all if they contain no matching rows. If use_legacy_dataset is True,
-                filters can only reference partition keys and only a hive-style directory structure
-                is supported. When setting use_legacy_dataset to False, also within-file level filtering
-                and different partitioning schemes are supported.
-                More on https://arrow.apache.org/docs/python/generated/pyarrow.parquet.ParquetDataset.html
-            force_download (bool, optional): If True then will always download a file even
-                if it is already on disk. Defaults to False.
-            download_folder (str, optional): The path, absolute or relative, where downloaded files are saved.
-                Defaults to download_folder as set in __init__
-        Returns:
-            class:`pandas.DataFrame`: a dataframe containing the requested data.
-                If multiple dataset instances are retrieved then these are concatenated first.
-        """
-        catalog = self.__use_catalog(catalog)
-
-        n_par = cpu_count(n_par)
-        if not download_folder:
-            download_folder = self.download_folder
-        download_res = self.download(
-            dataset,
-            dt_str,
-            dataset_format,
-            catalog,
-            n_par,
-            show_progress,
-            force_download,
-            download_folder,
-            return_paths=True,
+        return (True, output_file, None)
+    except Exception as ex:  # noqa: BLE001
+        logger.log(
+            VERBOSE_LVL,
+            f"Failed to write to {output_file}.",
+            exc_info=True,
         )
+        return (False, output_file, str(ex))
 
-        if not all(res[0] for res in download_res):
-            failed_res = [res for res in download_res if not res[0]]
-            raise Exception(
-                f"Not all downloads were successfully completed. "
-                f"Re-run to collect missing files. The following failed:\n{failed_res}"
-            )
 
-        files = [res[1] for res in download_res]
+def validate_file_names(paths: list[str], fs_fusion: fsspec.AbstractFileSystem) -> list[bool]:
+    """Validate if the file name format adheres to the standard.
+
+    Args:
+        paths (list): List of file paths.
+        fs_fusion: Fusion filesystem.
+
+    Returns (list): List of booleans.
+
+    """
+    file_names = [i.split("/")[-1].split(".")[0] for i in paths]
+    validation = []
+    all_catalogs = fs_fusion.ls("")
+    all_datasets = {}
+    file_seg_cnt = 3
+    for i, f_n in enumerate(file_names):
+        tmp = f_n.split("__")
+        if len(tmp) == file_seg_cnt:
+            val = tmp[1] in all_catalogs
+            if not val:
+                validation.append(False)
+            else:
+                if tmp[1] not in all_datasets:
+                    all_datasets[tmp[1]] = [i.split("/")[-1] for i in fs_fusion.ls(f"{tmp[1]}/datasets")]
 
-        pd_read_fn_map = {
-            "csv": read_csv,
-            "parquet": read_parquet,
-            "parq": read_parquet,
-            "json": read_json,
-            "raw": read_csv,
-        }
-
-        pd_read_default_kwargs: Dict[str, Dict[str, object]] = {
-            "csv": {"columns": columns, "filters": filters, "fs": self.fs},
-            "parquet": {"columns": columns, "filters": filters, "fs": self.fs},
-            "json": {"columns": columns, "filters": filters, "fs": self.fs},
-            "raw": {"columns": columns, "filters": filters, "fs": self.fs},
-        }
-
-        pd_read_default_kwargs["parq"] = pd_read_default_kwargs["parquet"]
-
-        pd_reader = pd_read_fn_map.get(dataset_format)
-        pd_read_kwargs = pd_read_default_kwargs.get(dataset_format, {})
-        if not pd_reader:
-            raise Exception(
-                f"No pandas function to read file in format {dataset_format}"
+                val = tmp[0] in all_datasets[tmp[1]]
+                validation.append(val)
+        else:
+            validation.append(False)
+        if not validation[-1] and len(tmp) == file_seg_cnt:
+            logger.warning(
+                f"You might not have access to the catalog {tmp[1]} or dataset {tmp[0]}."
+                "Please check you permission on the platform."
+            )
+        if not validation[-1] and len(tmp) != file_seg_cnt:
+            logger.warning(
+                f"The file in {paths[i]} has a non-compliant name and will not be processed. "
+                f"Please rename the file to dataset__catalog__yyyymmdd.format"
             )
 
-        pd_read_kwargs.update(kwargs)
+    return validation
 
-        if len(files) == 0:
-            raise APIResponseError(
-                f"No series members for dataset: {dataset} "
-                f"in date or date range: {dt_str} and format: {dataset_format}"
-            )
-        if dataset_format in ["parquet", "parq"]:
-            df = pd_reader(files, **pd_read_kwargs)  # type: ignore
-        elif dataset_format == "raw":
-            dataframes = (
-                pd.concat(
-                    [pd_reader(ZipFile(f).open(p), **pd_read_kwargs) for p in ZipFile(f).namelist()], ignore_index=True  # type: ignore
-                )  # type: ignore
-                for f in files
-            )  # type: ignore
-            df = pd.concat(dataframes, ignore_index=True)
-        else:
-            dataframes = (pd_reader(f, **pd_read_kwargs) for f in files)  # type: ignore
-            df = pd.concat(dataframes, ignore_index=True)
 
-        return df
+def is_dataset_raw(paths: list[str], fs_fusion: fsspec.AbstractFileSystem) -> list[bool]:
+    """Check if the files correspond to a raw dataset.
 
-    def upload(
-        self,
-        path: str,
-        dataset: str = None,
-        dt_str: str = "latest",
-        catalog: str = None,
-        n_par: int = None,
-        show_progress: bool = True,
-        return_paths: bool = False,
-        multipart=True,
-        chunk_size=5 * 2**20,
-    ):
-        """Uploads the requested files/files to Fusion.
-
-        Args:
-            path (str): path to a file or a folder with files
-            dataset (str, optional): Dataset name to which the file will be uplaoded (for single file only).
-                                    If not provided the dataset will be implied from file's name.
-            dt_str (str, optional): A single date. Defaults to 'latest' which will return the most recent.
-                                    Relevant for a single file upload only. If not provided the dataset will
-                                    be implied from file's name.
-            catalog (str, optional): A catalog identifier. Defaults to 'common'.
-            n_par (int, optional): Specify how many distributions to download in parallel.
-                Defaults to all cpus available.
-            show_progress (bool, optional): Display a progress bar during data download Defaults to True.
-            return_paths (bool, optional): Return paths and success statuses of the downloaded files.
-            multipart (bool): Is multipart upload.
-            chunk_size (int): Maximum chunk size.
-
-        Returns:
-
-
-        """
-        catalog = self.__use_catalog(catalog)
-
-        if not self.fs.exists(path):
-            raise RuntimeError("The provided path does not exist")
-
-        fs_fusion = self.get_fusion_filesystem()
-        if self.fs.info(path)["type"] == "directory":
-            file_path_lst = self.fs.find(path)
-            local_file_validation = validate_file_names(file_path_lst, fs_fusion)
-            file_path_lst = [
-                f for flag, f in zip(local_file_validation, file_path_lst) if flag
-            ]
-            local_url_eqiv = [path_to_url(i) for i in file_path_lst]
-        else:
-            file_path_lst = [path]
-            if not catalog or not dataset:
-                local_file_validation = validate_file_names(file_path_lst, fs_fusion)
-                file_path_lst = [
-                    f for flag, f in zip(local_file_validation, file_path_lst) if flag
-                ]
-                local_url_eqiv = [path_to_url(i) for i in file_path_lst]
-            else:
-                file_format = path.split(".")[-1]
-                dt_str = (
-                    dt_str
-                    if dt_str != "latest"
-                    else pd.Timestamp("today").date().strftime("%Y%m%d")
+    Args:
+        paths (list): List of file paths.
+        fs_fusion: Fusion filesystem.
+
+    Returns (list): List of booleans.
+
+    """
+    file_names = [i.split("/")[-1].split(".")[0] for i in paths]
+    ret = []
+    is_raw = {}
+    for _i, f_n in enumerate(file_names):
+        tmp = f_n.split("__")
+        if tmp[0] not in is_raw:
+            is_raw[tmp[0]] = js.loads(fs_fusion.cat(f"{tmp[1]}/datasets/{tmp[0]}"))["isRawData"]
+        ret.append(is_raw[tmp[0]])
+
+    return ret
+
+
+def path_to_url(x: str, is_raw: bool = False, is_download: bool = False) -> str:
+    """Convert file name to fusion url.
+
+    Args:
+        x (str): File path.
+        is_raw(bool, optional): Is the dataset raw.
+        is_download(bool, optional): Is the url for download.
+
+    Returns (str): Fusion url string.
+
+    """
+    catalog, dataset, date, ext = _filename_to_distribution(x.split("/")[-1])
+    ext = "raw" if is_raw else ext
+    return "/".join(distribution_to_url("", dataset, date, ext, catalog, is_download).split("/")[1:])
+
+
+def upload_files(  # noqa: PLR0913
+    fs_fusion: fsspec.AbstractFileSystem,
+    fs_local: fsspec.AbstractFileSystem,
+    loop: pd.DataFrame,
+    parallel: bool = True,
+    n_par: int = -1,
+    multipart: bool = True,
+    chunk_size: int = 5 * 2**20,
+    show_progress: bool = True,
+    from_date: Optional[str] = None,
+    to_date: Optional[str] = None,
+) -> list[tuple[bool, str, Optional[str]]]:
+    """Upload file into Fusion.
+
+    Args:
+        fs_fusion: Fusion filesystem.
+        fs_local: Local filesystem.
+        loop (pd.DataFrame): DataFrame of files to iterate through.
+        parallel (bool): Is parallel mode enabled.
+        n_par (int): Number of subprocesses.
+        multipart (bool): Is multipart upload.
+        chunk_size (int): Maximum chunk size.
+        show_progress (bool): Show progress bar
+        from_date (str, optional): earliest date of data contained in distribution.
+        to_date (str, optional): latest date of data contained in distribution.
+
+    Returns: List of update statuses.
+
+    """
+
+    def _upload(p_url: str, path: str) -> tuple[bool, str, Optional[str]]:
+        try:
+            mp = multipart and fs_local.size(path) > chunk_size
+
+            if isinstance(fs_local, BytesIO):
+                fs_fusion.put(
+                    fs_local,
+                    p_url,
+                    chunk_size=chunk_size,
+                    method="put",
+                    multipart=mp,
+                    from_date=from_date,
+                    to_date=to_date,
                 )
-                dt_str = pd.Timestamp(dt_str).date().strftime("%Y%m%d")
-                if catalog not in fs_fusion.ls("") or dataset not in [
-                    i.split("/")[-1] for i in fs_fusion.ls(f"{catalog}/datasets")
-                ]:
-                    msg = (
-                        f"File file has not been uploaded, one of the catalog: {catalog} "
-                        f"or dataset: {dataset} does not exit."
+            else:
+                with fs_local.open(path, "rb") as file_local:
+                    fs_fusion.put(
+                        file_local,
+                        p_url,
+                        chunk_size=chunk_size,
+                        method="put",
+                        multipart=mp,
+                        from_date=from_date,
+                        to_date=to_date,
                     )
-                    warnings.warn(msg)
-                    return [(False, path, Exception(msg))]
-                local_url_eqiv = [
-                    path_to_url(f"{dataset}__{catalog}__{dt_str}.{file_format}")
-                ]
-
-        df = pd.DataFrame([file_path_lst, local_url_eqiv]).T
-        df.columns = ["path", "url"]
+            return (True, path, None)
+        except Exception as ex:  # noqa: BLE001
+            logger.log(
+                VERBOSE_LVL,
+                f"Failed to upload {path}.",
+                exc_info=True,
+            )
+            return (False, path, str(ex))
 
+    if parallel:
         if show_progress:
-            loop = tqdm(df.iterrows(), total=len(df))
+            with tqdm_joblib(tqdm(total=len(loop))) as _:
+                res = Parallel(n_jobs=n_par, backend="threading")(
+                    delayed(_upload)(row["url"], row["path"]) for _, row in loop.iterrows()
+                )
         else:
-            loop = df.iterrows()
-
-        n_par = cpu_count(n_par)
-        parallel = True if len(df) > 1 else False
-        res = upload_files(
-            fs_fusion,
-            self.fs,
-            loop,
-            parallel=parallel,
-            n_par=n_par,
-            multipart=multipart,
-            chunk_size=chunk_size,
-        )
-
-        if not all(r[0] for r in res):
-            failed_res = [r for r in res if not r[0]]
-            msg = f"Not all uploads were successfully completed. The following failed:\n{failed_res}"
-            logger.warning(msg)
-            warnings.warn(msg)
+            res = Parallel(n_jobs=n_par, backend="threading")(
+                delayed(_upload)(row["url"], row["path"]) for _, row in loop.iterrows()
+            )
+    else:
+        res = [None] * len(loop)
+        if show_progress:
+            with tqdm(total=len(loop)) as p:
+                for i, row in loop.iterrows():
+                    r = _upload(row["url"], row["path"])
+                    res[i] = r
+                    if r[0] is True:
+                        p.update(1)
+        else:
+            res = [_upload(row["url"], row["path"]) for _, row in loop.iterrows()]
 
-        return res if return_paths else None
+    return res  # type: ignore
```

