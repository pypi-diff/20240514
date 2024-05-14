# Comparing `tmp/arctix-0.0.4.tar.gz` & `tmp/arctix-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arctix-0.0.4.tar", max compression
+gzip compressed data, was "arctix-0.0.5.tar", max compression
```

## Comparing `arctix-0.0.4.tar` & `arctix-0.0.5.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     1501 2024-05-11 19:35:43.976134 arctix-0.0.4/LICENSE
--rw-r--r--   0        0        0     6556 2024-05-11 19:35:43.976134 arctix-0.0.4/README.md
--rw-r--r--   0        0        0     6664 2024-05-11 19:35:43.980134 arctix-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       21 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/__init__.py
--rw-r--r--   0        0        0       43 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/dataset/__init__.py
--rw-r--r--   0        0        0    22996 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/dataset/breakfast.py
--rw-r--r--   0        0        0    23825 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/dataset/epic_kitchen_100.py
--rw-r--r--   0        0        0    27519 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/dataset/multithumos.py
--rw-r--r--   0        0        0      247 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/testing/__init__.py
--rw-r--r--   0        0        0      538 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/testing/fixtures.py
--rw-r--r--   0        0        0       29 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/__init__.py
--rw-r--r--   0        0        0     3095 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/dataframe/__init__.py
--rw-r--r--   0        0        0     6978 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/dataframe/base.py
--rw-r--r--   0        0        0     6262 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/dataframe/casting.py
--rw-r--r--   0        0        0     2107 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/dataframe/function.py
--rw-r--r--   0        0        0     4084 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/dataframe/json.py
--rw-r--r--   0        0        0     2914 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/dataframe/replace.py
--rw-r--r--   0        0        0     3809 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/dataframe/sequential.py
--rw-r--r--   0        0        0     4352 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/dataframe/sorting.py
--rw-r--r--   0        0        0     3107 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/dataframe/string.py
--rw-r--r--   0        0        0     3200 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/dataframe/time.py
--rw-r--r--   0        0        0     4581 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/transformer/dataframe/vocab.py
--rw-r--r--   0        0        0       34 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/__init__.py
--rw-r--r--   0        0        0      276 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/dataframe/__init__.py
--rw-r--r--   0        0        0     1618 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/dataframe/removing.py
--rw-r--r--   0        0        0     1618 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/dataframe/vocab.py
--rw-r--r--   0        0        0     3196 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/download.py
--rw-r--r--   0        0        0     7145 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/imports.py
--rw-r--r--   0        0        0      190 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/iter/__init__.py
--rw-r--r--   0        0        0     3543 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/iter/path.py
--rw-r--r--   0        0        0     1325 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/mapping.py
--rw-r--r--   0        0        0     3234 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/masking.py
--rw-r--r--   0        0        0      596 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/noop.py
--rw-r--r--   0        0        0    14150 2024-05-11 19:35:43.980134 arctix-0.0.4/src/arctix/utils/vocab.py
--rw-r--r--   0        0        0     7916 1970-01-01 00:00:00.000000 arctix-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1501 2024-05-14 02:18:13.503896 arctix-0.0.5/LICENSE
+-rw-r--r--   0        0        0     6674 2024-05-14 02:18:13.503896 arctix-0.0.5/README.md
+-rw-r--r--   0        0        0     6664 2024-05-14 02:18:13.507896 arctix-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/__init__.py
+-rw-r--r--   0        0        0       43 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/dataset/__init__.py
+-rw-r--r--   0        0        0    29056 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/dataset/breakfast.py
+-rw-r--r--   0        0        0    26642 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/dataset/ego4d.py
+-rw-r--r--   0        0        0    23865 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/dataset/epic_kitchen_100.py
+-rw-r--r--   0        0        0    29698 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/dataset/multithumos.py
+-rw-r--r--   0        0        0      247 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/testing/__init__.py
+-rw-r--r--   0        0        0      538 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/testing/fixtures.py
+-rw-r--r--   0        0        0       29 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/__init__.py
+-rw-r--r--   0        0        0     3095 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/dataframe/__init__.py
+-rw-r--r--   0        0        0     6978 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/dataframe/base.py
+-rw-r--r--   0        0        0     6262 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/dataframe/casting.py
+-rw-r--r--   0        0        0     2107 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/dataframe/function.py
+-rw-r--r--   0        0        0     4084 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/dataframe/json.py
+-rw-r--r--   0        0        0     2914 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/dataframe/replace.py
+-rw-r--r--   0        0        0     3809 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/dataframe/sequential.py
+-rw-r--r--   0        0        0     4352 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/dataframe/sorting.py
+-rw-r--r--   0        0        0     3107 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/dataframe/string.py
+-rw-r--r--   0        0        0     3200 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/dataframe/time.py
+-rw-r--r--   0        0        0     4581 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/dataframe/vocab.py
+-rw-r--r--   0        0        0       34 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/__init__.py
+-rw-r--r--   0        0        0      276 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/dataframe/__init__.py
+-rw-r--r--   0        0        0     1618 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/dataframe/removing.py
+-rw-r--r--   0        0        0     1618 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/dataframe/vocab.py
+-rw-r--r--   0        0        0     3196 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/download.py
+-rw-r--r--   0        0        0     7145 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/imports.py
+-rw-r--r--   0        0        0      190 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/iter/__init__.py
+-rw-r--r--   0        0        0     3543 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/iter/path.py
+-rw-r--r--   0        0        0     1325 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/mapping.py
+-rw-r--r--   0        0        0     3234 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/masking.py
+-rw-r--r--   0        0        0      596 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/noop.py
+-rw-r--r--   0        0        0    14150 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/vocab.py
+-rw-r--r--   0        0        0     8034 1970-01-01 00:00:00.000000 arctix-0.0.5/PKG-INFO
```

### Comparing `arctix-0.0.4/LICENSE` & `arctix-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `arctix-0.0.4/README.md` & `arctix-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,15 @@
 Please check the [get started page](https://durandtibo.github.io/arctix/get_started) to see how to
 install only some specific packages or other alternatives to install the library.
 The following is the corresponding `karbonn` versions and dependencies.
 
 | `batcharray` | `batcharray`   | `coola`      | `iden`           | `numpy`       | `polars`        | `python`      |
 |--------------|----------------|--------------|------------------|---------------|-----------------|---------------|
 | `main`       | `>=0.0.2,<0.1` | `>=0.3,<1.0` | `">=0.0.3,<1.0"` | `>=1.22,<2.0` | `>=0.20.0,<1.0` | `>=3.9,<3.13` |
+| `0.0.5`      | `>=0.0.2,<0.1` | `>=0.3,<1.0` | `">=0.0.3,<1.0"` | `>=1.22,<2.0` | `>=0.20.0,<1.0` | `>=3.9,<3.13` |
 | `0.0.4`      | `>=0.0.2,<0.1` | `>=0.3,<1.0` | `">=0.0.3,<1.0"` | `>=1.22,<2.0` | `>=0.20.0,<1.0` | `>=3.9,<3.13` |
 | `0.0.3`      | `>=0.0.2,<0.1` | `>=0.3,<1.0` | `">=0.0.3,<1.0"` | `>=1.22,<2.0` | `>=0.20.0,<1.0` | `>=3.9,<3.13` |
 
 ## Contributing
 
 Please check the instructions in [CONTRIBUTING.md](.github/CONTRIBUTING.md).
```

#### html2text {}

```diff
@@ -37,19 +37,20 @@
 install arctix[all] ``` Please check the [get started page](https://
 durandtibo.github.io/arctix/get_started) to see how to install only some
 specific packages or other alternatives to install the library. The following
 is the corresponding `karbonn` versions and dependencies. | `batcharray` |
 `batcharray` | `coola` | `iden` | `numpy` | `polars` | `python` | |------------
 --|----------------|--------------|------------------|---------------|---------
 --------|---------------| | `main` | `>=0.0.2,<0.1` | `>=0.3,<1.0` |
-`">=0.0.3,<1.0"` | `>=1.22,<2.0` | `>=0.20.0,<1.0` | `>=3.9,<3.13` | | `0.0.4`
+`">=0.0.3,<1.0"` | `>=1.22,<2.0` | `>=0.20.0,<1.0` | `>=3.9,<3.13` | | `0.0.5`
 | `>=0.0.2,<0.1` | `>=0.3,<1.0` | `">=0.0.3,<1.0"` | `>=1.22,<2.0` |
-`>=0.20.0,<1.0` | `>=3.9,<3.13` | | `0.0.3` | `>=0.0.2,<0.1` | `>=0.3,<1.0` |
-`">=0.0.3,<1.0"` | `>=1.22,<2.0` | `>=0.20.0,<1.0` | `>=3.9,<3.13` | ##
-Contributing Please check the instructions in [CONTRIBUTING.md](.github/
-CONTRIBUTING.md). ## API stability :warning: While `arctix` is in development
-stage, no API is guaranteed to be stable from one release to the next. In fact,
-it is very likely that the API will change multiple times before a stable 1.0.0
-release. In practice, this means that upgrading `arctix` to a new version will
-possibly break any code that was using the old version of `arctix`. ## License
-`arctix` is licensed under BSD 3-Clause "New" or "Revised" license available in
-[LICENSE](LICENSE) file.
+`>=0.20.0,<1.0` | `>=3.9,<3.13` | | `0.0.4` | `>=0.0.2,<0.1` | `>=0.3,<1.0` |
+`">=0.0.3,<1.0"` | `>=1.22,<2.0` | `>=0.20.0,<1.0` | `>=3.9,<3.13` | | `0.0.3`
+| `>=0.0.2,<0.1` | `>=0.3,<1.0` | `">=0.0.3,<1.0"` | `>=1.22,<2.0` |
+`>=0.20.0,<1.0` | `>=3.9,<3.13` | ## Contributing Please check the instructions
+in [CONTRIBUTING.md](.github/CONTRIBUTING.md). ## API stability :warning: While
+`arctix` is in development stage, no API is guaranteed to be stable from one
+release to the next. In fact, it is very likely that the API will change
+multiple times before a stable 1.0.0 release. In practice, this means that
+upgrading `arctix` to a new version will possibly break any code that was using
+the old version of `arctix`. ## License `arctix` is licensed under BSD 3-Clause
+"New" or "Revised" license available in [LICENSE](LICENSE) file.
```

### Comparing `arctix-0.0.4/pyproject.toml` & `arctix-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arctix"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/arctix"
 repository = "https://github.com/durandtibo/arctix"
 keywords = ["asynchronous time-series", "dataset", "preprocessing"]
 license = "BSD-3-Clause"
```

### Comparing `arctix-0.0.4/src/arctix/dataset/breakfast.py` & `arctix-0.0.5/src/arctix/dataset/breakfast.py`

 * *Files 18% similar despite different names*

```diff
@@ -201,14 +201,24 @@
 
     Args:
         path: The directory where the dataset annotations are stored.
         remove_duplicate: If ``True``, the duplicate rows are removed.
 
     Returns:
         The annotations in a DataFrame.
+
+    Example usage:
+
+    ```pycon
+
+    >>> from pathlib import Path
+    >>> from arctix.dataset.breakfast import load_data
+    >>> data = load_data(Path("/path/to/data/breakfast/"))  # doctest: +SKIP
+
+    ```
     """
     paths = FileFilter(PathLister([sanitize_path(path)], pattern="**/*.txt"))
     annotations = list(map(load_annotation_file, paths))
     data = convert_to_dict_of_flat_lists(annotations)
     data = pl.DataFrame(data)
     if remove_duplicate:
         data = drop_duplicates(data)
@@ -226,14 +236,24 @@
 
     Args:
         path: The file path to the annotation data.
 
     Returns:
         A dictionary with the action, the start time, and end time
             of each action.
+
+    Example usage:
+
+    ```pycon
+
+    >>> from pathlib import Path
+    >>> from arctix.dataset.breakfast import load_annotation_file
+    >>> data = load_annotation_file(Path("/path/to/data/breakfast/segmentation_coarse/cereals/P03_cam01_P03_cereals.txt"))  # doctest: +SKIP
+
+    ```
     """
     path = sanitize_path(path)
     if path.suffix != ".txt":
         msg = (
             "Incorrect file extension. This function can only parse `.txt` files "
             f"but received {path.suffix}"
         )
@@ -295,14 +315,114 @@
     Args:
         frame: The raw DataFrame.
         split: The dataset split. By default, the union of all the
             dataset splits is used.
 
     Returns:
         A tuple containing the prepared data and the metadata.
+
+    Example usage:
+
+    ```pycon
+
+    >>> import polars as pl
+    >>> from arctix.dataset.breakfast import Column, group_by_sequence
+    >>> frame = pl.DataFrame(
+    ...     {
+    ...         Column.ACTION: [
+    ...             "SIL",
+    ...             "take_bowl",
+    ...             "pour_cereals",
+    ...             "pour_milk",
+    ...             "stir_cereals",
+    ...             "SIL",
+    ...             "SIL",
+    ...             "pour_milk",
+    ...             "spoon_powder",
+    ...             "SIL",
+    ...         ],
+    ...         Column.COOKING_ACTIVITY: [
+    ...             "cereals",
+    ...             "cereals",
+    ...             "cereals",
+    ...             "cereals",
+    ...             "cereals",
+    ...             "cereals",
+    ...             "milk",
+    ...             "milk",
+    ...             "milk",
+    ...             "milk",
+    ...         ],
+    ...         Column.END_TIME: [
+    ...             30.0,
+    ...             150.0,
+    ...             428.0,
+    ...             575.0,
+    ...             705.0,
+    ...             836.0,
+    ...             47.0,
+    ...             215.0,
+    ...             565.0,
+    ...             747.0,
+    ...         ],
+    ...         Column.PERSON: [
+    ...             "P03",
+    ...             "P03",
+    ...             "P03",
+    ...             "P03",
+    ...             "P03",
+    ...             "P03",
+    ...             "P54",
+    ...             "P54",
+    ...             "P54",
+    ...             "P54",
+    ...         ],
+    ...         Column.START_TIME: [1.0, 31.0, 151.0, 429.0, 576.0, 706.0, 1.0, 48.0, 216.0, 566.0],
+    ...     },
+    ... )
+    >>> data, metadata = prepare_data(frame)
+    >>> with pl.Config(tbl_cols=-1):
+    ...     data
+    shape: (10, 8)
+    ┌─────────────┬───────────┬─────────────┬─────────────┬──────────┬────────┬───────────┬────────────┐
+    │ action      ┆ action_id ┆ cooking_act ┆ cooking_act ┆ end_time ┆ person ┆ person_id ┆ start_time │
+    │ ---         ┆ ---       ┆ ivity       ┆ ivity_id    ┆ ---      ┆ ---    ┆ ---       ┆ ---        │
+    │ str         ┆ i64       ┆ ---         ┆ ---         ┆ f64      ┆ str    ┆ i64       ┆ f64        │
+    │             ┆           ┆ str         ┆ i64         ┆          ┆        ┆           ┆            │
+    ╞═════════════╪═══════════╪═════════════╪═════════════╪══════════╪════════╪═══════════╪════════════╡
+    │ SIL         ┆ 0         ┆ cereals     ┆ 0           ┆ 30.0     ┆ P03    ┆ 0         ┆ 1.0        │
+    │ take_bowl   ┆ 2         ┆ cereals     ┆ 0           ┆ 150.0    ┆ P03    ┆ 0         ┆ 31.0       │
+    │ pour_cereal ┆ 5         ┆ cereals     ┆ 0           ┆ 428.0    ┆ P03    ┆ 0         ┆ 151.0      │
+    │ s           ┆           ┆             ┆             ┆          ┆        ┆           ┆            │
+    │ pour_milk   ┆ 1         ┆ cereals     ┆ 0           ┆ 575.0    ┆ P03    ┆ 0         ┆ 429.0      │
+    │ stir_cereal ┆ 3         ┆ cereals     ┆ 0           ┆ 705.0    ┆ P03    ┆ 0         ┆ 576.0      │
+    │ s           ┆           ┆             ┆             ┆          ┆        ┆           ┆            │
+    │ SIL         ┆ 0         ┆ cereals     ┆ 0           ┆ 836.0    ┆ P03    ┆ 0         ┆ 706.0      │
+    │ SIL         ┆ 0         ┆ milk        ┆ 1           ┆ 47.0     ┆ P54    ┆ 1         ┆ 1.0        │
+    │ pour_milk   ┆ 1         ┆ milk        ┆ 1           ┆ 215.0    ┆ P54    ┆ 1         ┆ 48.0       │
+    │ spoon_powde ┆ 4         ┆ milk        ┆ 1           ┆ 565.0    ┆ P54    ┆ 1         ┆ 216.0      │
+    │ r           ┆           ┆             ┆             ┆          ┆        ┆           ┆            │
+    │ SIL         ┆ 0         ┆ milk        ┆ 1           ┆ 747.0    ┆ P54    ┆ 1         ┆ 566.0      │
+    └─────────────┴───────────┴─────────────┴─────────────┴──────────┴────────┴───────────┴────────────┘
+    >>> metadata
+    {'vocab_action': Vocabulary(
+      counter=Counter({'SIL': 4, 'pour_milk': 2, 'take_bowl': 1, 'stir_cereals': 1, 'spoon_powder': 1, 'pour_cereals': 1}),
+      index_to_token=('SIL', 'pour_milk', 'take_bowl', 'stir_cereals', 'spoon_powder', 'pour_cereals'),
+      token_to_index={'SIL': 0, 'pour_milk': 1, 'take_bowl': 2, 'stir_cereals': 3, 'spoon_powder': 4, 'pour_cereals': 5},
+    ), 'vocab_activity': Vocabulary(
+      counter=Counter({'cereals': 6, 'milk': 4}),
+      index_to_token=('cereals', 'milk'),
+      token_to_index={'cereals': 0, 'milk': 1},
+    ), 'vocab_person': Vocabulary(
+      counter=Counter({'P03': 6, 'P54': 4}),
+      index_to_token=('P03', 'P54'),
+      token_to_index={'P03': 0, 'P54': 1},
+    )}
+
+    ```
     """
     vocab_action = generate_vocabulary(frame, col=Column.ACTION).sort_by_count()
     vocab_person = generate_vocabulary(frame, col=Column.PERSON).sort_by_count()
     vocab_activity = (
         generate_vocabulary(frame, col=Column.COOKING_ACTIVITY).sort_by_token().sort_by_count()
     )
     transformer = td.Sequential(
@@ -386,15 +506,15 @@
     >>> with pl.Config(tbl_cols=-1):
     ...     groups
     shape: (2, 9)
     ┌───────────┬───────────┬──────────┬──────────┬──────────┬────────┬──────────┬──────────┬──────────┐
     │ action    ┆ action_id ┆ cooking_ ┆ cooking_ ┆ end_time ┆ person ┆ person_i ┆ sequence ┆ start_ti │
     │ ---       ┆ ---       ┆ activity ┆ activity ┆ ---      ┆ ---    ┆ d        ┆ _length  ┆ me       │
     │ list[str] ┆ list[i64] ┆ ---      ┆ _id      ┆ list[f64 ┆ str    ┆ ---      ┆ ---      ┆ ---      │
-    │           ┆           ┆ str      ┆ ---      ┆ ]        ┆        ┆ i64      ┆ u32      ┆ list[f64 │
+    │           ┆           ┆ str      ┆ ---      ┆ ]        ┆        ┆ i64      ┆ i64      ┆ list[f64 │
     │           ┆           ┆          ┆ i64      ┆          ┆        ┆          ┆          ┆ ]        │
     ╞═══════════╪═══════════╪══════════╪══════════╪══════════╪════════╪══════════╪══════════╪══════════╡
     │ ["SIL",   ┆ [0, 2, …  ┆ cereals  ┆ 0        ┆ [30.0,   ┆ P03    ┆ 0        ┆ 6        ┆ [1.0,    │
     │ "take_bow ┆ 0]        ┆          ┆          ┆ 150.0, … ┆        ┆          ┆          ┆ 31.0, …  │
     │ l", …     ┆           ┆          ┆          ┆ 836.0]   ┆        ┆          ┆          ┆ 706.0]   │
     │ "SIL"]    ┆           ┆          ┆          ┆          ┆        ┆          ┆          ┆          │
     │ ["SIL",   ┆ [0, 1, …  ┆ milk     ┆ 1        ┆ [47.0,   ┆ P54    ┆ 1        ┆ 4        ┆ [1.0,    │
@@ -408,15 +528,15 @@
     data = frame.group_by([Column.PERSON_ID, Column.COOKING_ACTIVITY_ID]).agg(
         pl.first(Column.COOKING_ACTIVITY),
         pl.first(Column.PERSON),
         pl.col(Column.ACTION),
         pl.col(Column.ACTION_ID),
         pl.col(Column.START_TIME),
         pl.col(Column.END_TIME),
-        pl.len().alias(Column.SEQUENCE_LENGTH),
+        pl.len().cast(pl.Int64).alias(Column.SEQUENCE_LENGTH),
     )
     transformer = td.Sequential(
         [
             td.Sort(columns=[Column.PERSON_ID, Column.COOKING_ACTIVITY_ID]),
             td.SortColumns(),
         ]
     )
```

### Comparing `arctix-0.0.4/src/arctix/dataset/epic_kitchen_100.py` & `arctix-0.0.5/src/arctix/dataset/epic_kitchen_100.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     r"""Indicate the metadata keys."""
 
     VOCAB_NOUN: str = "vocab_noun"
     VOCAB_VERB: str = "vocab_verb"
 
 
 def fetch_data(path: Path, split: str, force_download: bool = False) -> tuple[pl.DataFrame, dict]:
-    r"""Download and load the data for Breakfast dataset.
+    r"""Download and load the data for EPIC-KITCHENS-100 dataset.
 
     Args:
         path: The path where to store the downloaded data.
         split: The dataset split.
         force_download: If ``True``, the annotations are downloaded
             everytime this function is called. If ``False``,
             the annotations are downloaded only if the
@@ -187,15 +187,15 @@
     ```
     """
     path = sanitize_path(path)
     return all(path.joinpath(filename).is_file() for filename in ANNOTATION_FILENAMES)
 
 
 def load_data(path: Path, split: str) -> tuple[pl.DataFrame, dict]:
-    r"""Load all the annotations in a DataFrame.
+    r"""Load all the annotations in a DataFrame and the metadata.
 
     Args:
         path: The directory where the dataset annotations are stored.
         split: The dataset split.
 
     Returns:
         The annotations in a DataFrame and the metadata.
@@ -479,15 +479,15 @@
             pl.col(Column.START_TIMESTAMP),
             pl.col(Column.START_TIME_SECOND),
             pl.col(Column.STOP_FRAME),
             pl.col(Column.STOP_TIMESTAMP),
             pl.col(Column.STOP_TIME_SECOND),
             pl.col(Column.VERB),
             pl.col(Column.VERB_ID),
-            pl.len().alias(Column.SEQUENCE_LENGTH),
+            pl.len().cast(pl.Int64).alias(Column.SEQUENCE_LENGTH),
         )
     )
     transformer = td.Sequential(
         [
             td.Sort(columns=[Column.VIDEO_ID]),
             td.SortColumns(),
         ]
```

### Comparing `arctix-0.0.4/src/arctix/dataset/multithumos.py` & `arctix-0.0.5/src/arctix/dataset/multithumos.py`

 * *Files 4% similar despite different names*

```diff
@@ -247,14 +247,24 @@
 
     Args:
         path: The directory where the dataset annotations are stored.
         remove_duplicate: If ``True``, the duplicate rows are removed.
 
     Returns:
         The annotations in a DataFrame.
+
+    Example usage:
+
+    ```pycon
+
+    >>> from pathlib import Path
+    >>> from arctix.dataset.multithumos import load_data
+    >>> data = load_data(Path("/path/to/data/multithumos/"))  # doctest: +SKIP
+
+    ```
     """
     paths = FileFilter(PathLister([sanitize_path(path)], pattern="annotations/*.txt"))
     annotations = list(map(load_annotation_file, paths))
     data = convert_to_dict_of_flat_lists(annotations)
     data = pl.DataFrame(data)
     transformer = td.Sequential(
         [
@@ -270,14 +280,26 @@
 
     Args:
         path: The file path to the annotation data.
 
     Returns:
         A dictionary with the action, the start time, and end time
             of each action.
+
+    Example usage:
+
+    ```pycon
+
+    >>> from pathlib import Path
+    >>> from arctix.dataset.multithumos import load_annotation_file
+    >>> data = load_annotation_file(
+    ...     Path("/path/to/data/multithumos/annotations/BasketballBlock.txt")
+    ... )  # doctest: +SKIP
+
+    ```
     """
     path = sanitize_path(path)
     if path.suffix != ".txt":
         msg = (
             "Incorrect file extension. This function can only parse `.txt` files "
             f"but received {path.suffix}"
         )
@@ -449,14 +471,69 @@
     Args:
         frame: The DataFrame to filter.
         split: The dataset split. By default, the union of all the
             dataset splits is used.
 
     Returns:
         The filtered DataFrame.
+
+    Example usage:
+
+    ```pycon
+
+    >>> import polars as pl
+    >>> from arctix.dataset.multithumos import Column, filter_by_split
+    >>> frame = pl.DataFrame(
+    ...     {
+    ...         Column.VIDEO: [
+    ...             "video_test_1",
+    ...             "video_test_1",
+    ...             "video_test_1",
+    ...             "video_validation_2",
+    ...             "video_validation_2",
+    ...             "video_validation_2",
+    ...             "video_validation_2",
+    ...         ],
+    ...         Column.START_TIME: [1.50, 17.57, 79.30, 2.97, 4.54, 20.22, 27.42],
+    ...         Column.END_TIME: [5.40, 18.33, 83.90, 3.60, 5.07, 20.49, 30.23],
+    ...         Column.ACTION: [
+    ...             "dribble",
+    ...             "guard",
+    ...             "dribble",
+    ...             "guard",
+    ...             "guard",
+    ...             "guard",
+    ...             "shoot",
+    ...         ],
+    ...         Column.ACTION_ID: [1, 0, 1, 0, 0, 0, 2],
+    ...         Column.SPLIT: [
+    ...             "test",
+    ...             "test",
+    ...             "test",
+    ...             "validation",
+    ...             "validation",
+    ...             "validation",
+    ...             "validation",
+    ...         ],
+    ...     },
+    ... )
+    >>> data = filter_by_split(frame, split='test')
+    >>> data
+    shape: (3, 6)
+    ┌──────────────┬────────────┬──────────┬─────────┬───────────┬───────┐
+    │ video        ┆ start_time ┆ end_time ┆ action  ┆ action_id ┆ split │
+    │ ---          ┆ ---        ┆ ---      ┆ ---     ┆ ---       ┆ ---   │
+    │ str          ┆ f64        ┆ f64      ┆ str     ┆ i64       ┆ str   │
+    ╞══════════════╪════════════╪══════════╪═════════╪═══════════╪═══════╡
+    │ video_test_1 ┆ 1.5        ┆ 5.4      ┆ dribble ┆ 1         ┆ test  │
+    │ video_test_1 ┆ 17.57      ┆ 18.33    ┆ guard   ┆ 0         ┆ test  │
+    │ video_test_1 ┆ 79.3       ┆ 83.9     ┆ dribble ┆ 1         ┆ test  │
+    └──────────────┴────────────┴──────────┴─────────┴───────────┴───────┘
+
+    ```
     """
     splits = {split}
     if split == "all":
         splits = {"validation", "test"}
     return frame.filter(pl.col(Column.SPLIT).is_in(splits))
 
 
@@ -504,50 +581,41 @@
     ...             "validation",
     ...             "validation",
     ...             "validation",
     ...             "validation",
     ...             "validation",
     ...         ],
     ...     },
-    ...     schema={
-    ...         Column.VIDEO: pl.String,
-    ...         Column.START_TIME: pl.Float64,
-    ...         Column.END_TIME: pl.Float64,
-    ...         Column.ACTION: pl.String,
-    ...         Column.ACTION_ID: pl.Int64,
-    ...         Column.SPLIT: pl.String,
-    ...     },
     ... )
     >>> groups = group_by_sequence(frame)
     >>> groups
     shape: (2, 7)
     ┌──────────────┬─────────────┬──────────────┬─────────────┬────────────┬─────────────┬─────────────┐
     │ action       ┆ action_id   ┆ end_time     ┆ sequence_le ┆ split      ┆ start_time  ┆ video       │
     │ ---          ┆ ---         ┆ ---          ┆ ngth        ┆ ---        ┆ ---         ┆ ---         │
     │ list[str]    ┆ list[i64]   ┆ list[f64]    ┆ ---         ┆ str        ┆ list[f64]   ┆ str         │
-    │              ┆             ┆              ┆ u32         ┆            ┆             ┆             │
+    │              ┆             ┆              ┆ i64         ┆            ┆             ┆             │
     ╞══════════════╪═════════════╪══════════════╪═════════════╪════════════╪═════════════╪═════════════╡
     │ ["dribble",  ┆ [1, 0, 1]   ┆ [5.4, 18.33, ┆ 3           ┆ validation ┆ [1.5,       ┆ video_valid │
     │ "guard",     ┆             ┆ 83.9]        ┆             ┆            ┆ 17.57,      ┆ ation_1     │
     │ "dribble"…   ┆             ┆              ┆             ┆            ┆ 79.3]       ┆             │
     │ ["guard",    ┆ [0, 0, … 2] ┆ [3.6, 5.07,  ┆ 4           ┆ validation ┆ [2.97,      ┆ video_valid │
     │ "guard", …   ┆             ┆ … 30.23]     ┆             ┆            ┆ 4.54, …     ┆ ation_2     │
     │ "shoot"]     ┆             ┆              ┆             ┆            ┆ 27.42]      ┆             │
     └──────────────┴─────────────┴──────────────┴─────────────┴────────────┴─────────────┴─────────────┘
 
-
     ```
     """
     data = frame.group_by([Column.VIDEO]).agg(
         pl.first(Column.SPLIT),
         pl.col(Column.ACTION),
         pl.col(Column.ACTION_ID),
         pl.col(Column.START_TIME),
         pl.col(Column.END_TIME),
-        pl.len().alias(Column.SEQUENCE_LENGTH),
+        pl.len().cast(pl.Int64).alias(Column.SEQUENCE_LENGTH),
     )
     transformer = td.Sequential(
         [
             td.Sort(columns=[Column.VIDEO]),
             td.SortColumns(),
         ]
     )
@@ -598,22 +666,14 @@
     ...             "validation",
     ...             "validation",
     ...             "validation",
     ...             "validation",
     ...             "validation",
     ...         ],
     ...     },
-    ...     schema={
-    ...         Column.VIDEO: pl.String,
-    ...         Column.START_TIME: pl.Float64,
-    ...         Column.END_TIME: pl.Float64,
-    ...         Column.ACTION: pl.String,
-    ...         Column.ACTION_ID: pl.Int64,
-    ...         Column.SPLIT: pl.String,
-    ...     },
     ... )
     >>> arrays = to_array(frame)
     >>> arrays
     {'action': masked_array(
       data=[['dribble', 'guard', 'dribble', --],
             ['guard', 'guard', 'guard', 'shoot']],
       mask=[[False, False, False,  True],
@@ -732,22 +792,14 @@
     ...             "validation",
     ...             "validation",
     ...             "validation",
     ...             "validation",
     ...             "validation",
     ...         ],
     ...     },
-    ...     schema={
-    ...         Column.VIDEO: pl.String,
-    ...         Column.START_TIME: pl.Float64,
-    ...         Column.END_TIME: pl.Float64,
-    ...         Column.ACTION: pl.String,
-    ...         Column.ACTION_ID: pl.Int64,
-    ...         Column.SPLIT: pl.String,
-    ...     },
     ... )
     >>> data_list = to_list(frame)
     >>> data_list
     {'action': [['dribble', 'guard', 'dribble'], ['guard', 'guard', 'guard', 'shoot']],
      'action_id': [[1, 0, 1], [0, 0, 0, 2]],
      'end_time': [[5.0, 18.0, 83.0], [3.0, 5.0, 20.0, 30.0]],
      'sequence_length': [3, 4], 'split': ['validation', 'validation'],
```

### Comparing `arctix-0.0.4/src/arctix/testing/fixtures.py` & `arctix-0.0.5/src/arctix/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.4/src/arctix/transformer/dataframe/__init__.py` & `arctix-0.0.5/src/arctix/transformer/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.4/src/arctix/transformer/dataframe/base.py` & `arctix-0.0.5/src/arctix/transformer/dataframe/base.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.4/src/arctix/transformer/dataframe/casting.py` & `arctix-0.0.5/src/arctix/transformer/dataframe/casting.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.4/src/arctix/transformer/dataframe/function.py` & `arctix-0.0.5/src/arctix/transformer/dataframe/function.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.4/src/arctix/transformer/dataframe/json.py` & `arctix-0.0.5/src/arctix/transformer/dataframe/json.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.4/src/arctix/transformer/dataframe/replace.py` & `arctix-0.0.5/src/arctix/transformer/dataframe/replace.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.4/src/arctix/transformer/dataframe/sequential.py` & `arctix-0.0.5/src/arctix/transformer/dataframe/sequential.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.4/src/arctix/transformer/dataframe/sorting.py` & `arctix-0.0.5/src/arctix/transformer/dataframe/sorting.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.4/src/arctix/transformer/dataframe/string.py` & `arctix-0.0.5/src/arctix/transformer/dataframe/string.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.4/src/arctix/transformer/dataframe/time.py` & `arctix-0.0.5/src/arctix/transformer/dataframe/time.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.4/src/arctix/transformer/dataframe/vocab.py` & `arctix-0.0.5/src/arctix/transformer/dataframe/vocab.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.4/src/arctix/utils/dataframe/removing.py` & `arctix-0.0.5/src/arctix/utils/dataframe/removing.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.4/src/arctix/utils/dataframe/vocab.py` & `arctix-0.0.5/src/arctix/utils/dataframe/vocab.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.4/src/arctix/utils/download.py` & `arctix-0.0.5/src/arctix/utils/download.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.4/src/arctix/utils/imports.py` & `arctix-0.0.5/src/arctix/utils/imports.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.4/src/arctix/utils/iter/path.py` & `arctix-0.0.5/src/arctix/utils/iter/path.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.4/src/arctix/utils/mapping.py` & `arctix-0.0.5/src/arctix/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.4/src/arctix/utils/masking.py` & `arctix-0.0.5/src/arctix/utils/masking.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.4/src/arctix/utils/noop.py` & `arctix-0.0.5/src/arctix/utils/noop.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.4/src/arctix/utils/vocab.py` & `arctix-0.0.5/src/arctix/utils/vocab.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.4/PKG-INFO` & `arctix-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arctix
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Home-page: https://github.com/durandtibo/arctix
 License: BSD-3-Clause
 Keywords: asynchronous time-series,dataset,preprocessing
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<3.13
@@ -156,14 +156,15 @@
 Please check the [get started page](https://durandtibo.github.io/arctix/get_started) to see how to
 install only some specific packages or other alternatives to install the library.
 The following is the corresponding `karbonn` versions and dependencies.
 
 | `batcharray` | `batcharray`   | `coola`      | `iden`           | `numpy`       | `polars`        | `python`      |
 |--------------|----------------|--------------|------------------|---------------|-----------------|---------------|
 | `main`       | `>=0.0.2,<0.1` | `>=0.3,<1.0` | `">=0.0.3,<1.0"` | `>=1.22,<2.0` | `>=0.20.0,<1.0` | `>=3.9,<3.13` |
+| `0.0.5`      | `>=0.0.2,<0.1` | `>=0.3,<1.0` | `">=0.0.3,<1.0"` | `>=1.22,<2.0` | `>=0.20.0,<1.0` | `>=3.9,<3.13` |
 | `0.0.4`      | `>=0.0.2,<0.1` | `>=0.3,<1.0` | `">=0.0.3,<1.0"` | `>=1.22,<2.0` | `>=0.20.0,<1.0` | `>=3.9,<3.13` |
 | `0.0.3`      | `>=0.0.2,<0.1` | `>=0.3,<1.0` | `">=0.0.3,<1.0"` | `>=1.22,<2.0` | `>=0.20.0,<1.0` | `>=3.9,<3.13` |
 
 ## Contributing
 
 Please check the instructions in [CONTRIBUTING.md](.github/CONTRIBUTING.md).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: arctix Version: 0.0.4 Summary: Home-page: https://
+Metadata-Version: 2.1 Name: arctix Version: 0.0.5 Summary: Home-page: https://
 github.com/durandtibo/arctix License: BSD-3-Clause Keywords: asynchronous time-
 series,dataset,preprocessing Author: Thibaut Durand Author-email:
 durand.tibo+gh@gmail.com Requires-Python: >=3.9,<3.13 Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Operating System :: POSIX :: Linux Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
@@ -55,19 +55,20 @@
 install arctix[all] ``` Please check the [get started page](https://
 durandtibo.github.io/arctix/get_started) to see how to install only some
 specific packages or other alternatives to install the library. The following
 is the corresponding `karbonn` versions and dependencies. | `batcharray` |
 `batcharray` | `coola` | `iden` | `numpy` | `polars` | `python` | |------------
 --|----------------|--------------|------------------|---------------|---------
 --------|---------------| | `main` | `>=0.0.2,<0.1` | `>=0.3,<1.0` |
-`">=0.0.3,<1.0"` | `>=1.22,<2.0` | `>=0.20.0,<1.0` | `>=3.9,<3.13` | | `0.0.4`
+`">=0.0.3,<1.0"` | `>=1.22,<2.0` | `>=0.20.0,<1.0` | `>=3.9,<3.13` | | `0.0.5`
 | `>=0.0.2,<0.1` | `>=0.3,<1.0` | `">=0.0.3,<1.0"` | `>=1.22,<2.0` |
-`>=0.20.0,<1.0` | `>=3.9,<3.13` | | `0.0.3` | `>=0.0.2,<0.1` | `>=0.3,<1.0` |
-`">=0.0.3,<1.0"` | `>=1.22,<2.0` | `>=0.20.0,<1.0` | `>=3.9,<3.13` | ##
-Contributing Please check the instructions in [CONTRIBUTING.md](.github/
-CONTRIBUTING.md). ## API stability :warning: While `arctix` is in development
-stage, no API is guaranteed to be stable from one release to the next. In fact,
-it is very likely that the API will change multiple times before a stable 1.0.0
-release. In practice, this means that upgrading `arctix` to a new version will
-possibly break any code that was using the old version of `arctix`. ## License
-`arctix` is licensed under BSD 3-Clause "New" or "Revised" license available in
-[LICENSE](LICENSE) file.
+`>=0.20.0,<1.0` | `>=3.9,<3.13` | | `0.0.4` | `>=0.0.2,<0.1` | `>=0.3,<1.0` |
+`">=0.0.3,<1.0"` | `>=1.22,<2.0` | `>=0.20.0,<1.0` | `>=3.9,<3.13` | | `0.0.3`
+| `>=0.0.2,<0.1` | `>=0.3,<1.0` | `">=0.0.3,<1.0"` | `>=1.22,<2.0` |
+`>=0.20.0,<1.0` | `>=3.9,<3.13` | ## Contributing Please check the instructions
+in [CONTRIBUTING.md](.github/CONTRIBUTING.md). ## API stability :warning: While
+`arctix` is in development stage, no API is guaranteed to be stable from one
+release to the next. In fact, it is very likely that the API will change
+multiple times before a stable 1.0.0 release. In practice, this means that
+upgrading `arctix` to a new version will possibly break any code that was using
+the old version of `arctix`. ## License `arctix` is licensed under BSD 3-Clause
+"New" or "Revised" license available in [LICENSE](LICENSE) file.
```

