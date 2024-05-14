# Comparing `tmp/pandas_stubs-2.2.1.240316.tar.gz` & `tmp/pandas_stubs-2.2.2.240514.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_stubs-2.2.1.240316.tar", max compression
+gzip compressed data, was "pandas_stubs-2.2.2.240514.tar", max compression
```

## Comparing `pandas_stubs-2.2.1.240316.tar` & `pandas_stubs-2.2.2.240514.tar`

### file list

```diff
@@ -1,205 +1,205 @@
--rw-r--r--   0        0        0     1514 2022-08-08 01:00:32.131878 pandas_stubs-2.2.1.240316/LICENSE
--rw-r--r--   0        0        0     3805 2023-05-22 14:12:55.264847 pandas_stubs-2.2.1.240316/pandas-stubs/__init__.pyi
--rw-r--r--   0        0        0      220 2022-08-08 01:00:32.243006 pandas_stubs-2.2.1.240316/pandas-stubs/_config/__init__.pyi
--rw-r--r--   0        0        0     4173 2023-09-23 02:44:57.787235 pandas_stubs-2.2.1.240316/pandas-stubs/_config/config.pyi
--rw-r--r--   0        0        0      285 2023-05-22 14:12:55.265853 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/__init__.pyi
--rw-r--r--   0        0        0      132 2022-08-08 01:00:32.278047 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/indexing.pyi
--rw-r--r--   0        0        0     8429 2023-12-18 16:23:19.658046 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/interval.pyi
--rw-r--r--   0        0        0      130 2022-08-08 01:00:32.293998 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/json.pyi
--rw-r--r--   0        0        0      779 2024-02-14 22:01:29.589865 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/lib.pyi
--rw-r--r--   0        0        0     1893 2023-02-23 17:31:11.761589 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/missing.pyi
--rw-r--r--   0        0        0      126 2022-08-08 01:00:32.310002 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/ops_dispatch.pyi
--rw-r--r--   0        0        0      599 2024-02-14 22:01:29.590444 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/properties.pyi
--rw-r--r--   0        0        0       91 2022-08-08 01:00:32.320997 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/sparse.pyi
--rw-r--r--   0        0        0      666 2023-05-22 14:12:55.265853 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/tslibs/__init__.pyi
--rw-r--r--   0        0        0       65 2022-08-08 01:00:32.332997 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/tslibs/base.pyi
--rw-r--r--   0        0        0      143 2022-08-08 01:00:32.346996 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/tslibs/conversion.pyi
--rw-r--r--   0        0        0     1195 2022-08-10 19:03:04.643581 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/tslibs/dtypes.pyi
--rw-r--r--   0        0        0     3764 2024-02-14 22:01:29.591592 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/tslibs/nattype.pyi
--rw-r--r--   0        0        0       89 2022-12-28 15:28:49.658657 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/tslibs/np_datetime.pyi
--rw-r--r--   0        0        0     8605 2023-09-28 14:06:32.016764 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/tslibs/offsets.pyi
--rw-r--r--   0        0        0      163 2022-08-08 01:00:32.387997 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/tslibs/parsing.pyi
--rw-r--r--   0        0        0     6686 2024-02-14 22:01:29.592119 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/tslibs/period.pyi
--rw-r--r--   0        0        0       72 2022-08-08 01:00:32.405128 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/tslibs/strptime.pyi
--rw-r--r--   0        0        0    14530 2024-02-14 22:01:29.592687 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/tslibs/timedeltas.pyi
--rw-r--r--   0        0        0    11642 2024-02-14 22:01:29.593253 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/tslibs/timestamps.pyi
--rw-r--r--   0        0        0       62 2022-08-08 01:00:32.438009 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/tslibs/tzconversion.pyi
--rw-r--r--   0        0        0      613 2023-02-04 17:09:12.293389 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/tslibs/vectorized.pyi
--rw-r--r--   0        0        0        0 2022-07-03 21:17:38.574585 pandas_stubs-2.2.1.240316/pandas-stubs/_libs/window/__init__.pyi
--rw-r--r--   0        0        0     4100 2023-12-18 16:23:19.658046 pandas_stubs-2.2.1.240316/pandas-stubs/_testing/__init__.pyi
--rw-r--r--   0        0        0    24579 2024-02-14 22:01:29.594308 pandas_stubs-2.2.1.240316/pandas-stubs/_typing.pyi
--rw-r--r--   0        0        0      124 2024-03-16 23:40:52.479745 pandas_stubs-2.2.1.240316/pandas-stubs/_version.pyi
--rw-r--r--   0        0        0      141 2023-06-05 12:34:31.504832 pandas_stubs-2.2.1.240316/pandas-stubs/api/__init__.pyi
--rw-r--r--   0        0        0      603 2023-02-27 22:18:36.851320 pandas_stubs-2.2.1.240316/pandas-stubs/api/extensions/__init__.pyi
--rw-r--r--   0        0        0      241 2022-08-08 01:00:32.486031 pandas_stubs-2.2.1.240316/pandas-stubs/api/indexers/__init__.pyi
--rw-r--r--   0        0        0      164 2022-12-28 15:28:49.664655 pandas_stubs-2.2.1.240316/pandas-stubs/api/interchange/__init__.pyi
--rw-r--r--   0        0        0     1729 2024-02-14 22:01:29.595520 pandas_stubs-2.2.1.240316/pandas-stubs/api/types/__init__.pyi
--rw-r--r--   0        0        0      373 2022-08-08 01:00:32.499997 pandas_stubs-2.2.1.240316/pandas-stubs/arrays/__init__.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.550503 pandas_stubs-2.2.1.240316/pandas-stubs/core/__init__.pyi
--rw-r--r--   0        0        0      437 2023-08-14 14:08:10.526716 pandas_stubs-2.2.1.240316/pandas-stubs/core/accessor.pyi
--rw-r--r--   0        0        0     2345 2023-12-18 16:23:19.665161 pandas_stubs-2.2.1.240316/pandas-stubs/core/algorithms.pyi
--rw-r--r--   0        0        0     2680 2023-04-05 02:20:38.240522 pandas_stubs-2.2.1.240316/pandas-stubs/core/api.pyi
--rw-r--r--   0        0        0     2052 2023-11-03 13:55:15.977230 pandas_stubs-2.2.1.240316/pandas-stubs/core/arraylike.pyi
--rw-r--r--   0        0        0      924 2023-05-22 14:12:55.269816 pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/__init__.pyi
--rw-r--r--   0        0        0      321 2023-02-27 03:32:24.825818 pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/arrow/dtype.pyi
--rw-r--r--   0        0        0     2168 2023-04-01 02:35:39.716027 pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/base.pyi
--rw-r--r--   0        0        0      961 2023-11-03 13:55:15.978208 pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/boolean.pyi
--rw-r--r--   0        0        0     7333 2023-08-14 14:08:10.528724 pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/categorical.pyi
--rw-r--r--   0        0        0     2890 2024-02-14 22:01:29.596147 pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/datetimelike.pyi
--rw-r--r--   0        0        0     2268 2023-11-03 13:55:15.978208 pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/datetimes.pyi
--rw-r--r--   0        0        0      133 2022-12-28 15:28:49.670655 pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/floating.pyi
--rw-r--r--   0        0        0     1060 2023-11-03 13:55:15.979233 pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/integer.pyi
--rw-r--r--   0        0        0     2720 2023-11-03 13:55:15.979233 pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/interval.pyi
--rw-r--r--   0        0        0      824 2023-11-03 13:55:15.980236 pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/masked.pyi
--rw-r--r--   0        0        0       99 2023-02-27 03:32:24.828808 pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/numeric.pyi
--rw-r--r--   0        0        0      513 2023-02-27 03:32:24.828808 pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/numpy_.pyi
--rw-r--r--   0        0        0     1705 2023-11-03 13:55:15.980236 pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/period.pyi
--rw-r--r--   0        0        0      285 2023-05-22 14:12:55.271819 pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/sparse/__init__.pyi
--rw-r--r--   0        0        0      650 2023-04-12 19:14:53.206395 pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/sparse/accessor.pyi
--rw-r--r--   0        0        0     1891 2023-11-03 13:55:15.981208 pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/sparse/array.pyi
--rw-r--r--   0        0        0      448 2023-02-27 03:32:24.829807 pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/sparse/dtype.pyi
--rw-r--r--   0        0        0      715 2023-02-27 03:32:24.830807 pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/string_.pyi
--rw-r--r--   0        0        0     1963 2023-02-04 17:09:12.301416 pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/timedeltas.pyi
--rw-r--r--   0        0        0     2892 2024-02-14 22:01:29.597311 pandas_stubs-2.2.1.240316/pandas-stubs/core/base.pyi
--rw-r--r--   0        0        0      955 2023-02-04 17:09:12.302429 pandas_stubs-2.2.1.240316/pandas-stubs/core/common.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.561504 pandas_stubs-2.2.1.240316/pandas-stubs/core/computation/__init__.pyi
--rw-r--r--   0        0        0       79 2022-08-08 01:00:32.662463 pandas_stubs-2.2.1.240316/pandas-stubs/core/computation/align.pyi
--rw-r--r--   0        0        0       54 2022-08-08 01:00:32.670999 pandas_stubs-2.2.1.240316/pandas-stubs/core/computation/api.pyi
--rw-r--r--   0        0        0       47 2022-08-10 19:03:04.655579 pandas_stubs-2.2.1.240316/pandas-stubs/core/computation/common.pyi
--rw-r--r--   0        0        0      438 2022-12-28 15:28:49.678655 pandas_stubs-2.2.1.240316/pandas-stubs/core/computation/engines.pyi
--rw-r--r--   0        0        0      668 2023-02-04 17:09:12.302429 pandas_stubs-2.2.1.240316/pandas-stubs/core/computation/eval.pyi
--rw-r--r--   0        0        0     2348 2023-08-14 11:37:22.152338 pandas_stubs-2.2.1.240316/pandas-stubs/core/computation/expr.pyi
--rw-r--r--   0        0        0      270 2022-08-08 01:00:32.711086 pandas_stubs-2.2.1.240316/pandas-stubs/core/computation/expressions.pyi
--rw-r--r--   0        0        0     2342 2023-08-14 14:08:10.529736 pandas_stubs-2.2.1.240316/pandas-stubs/core/computation/ops.pyi
--rw-r--r--   0        0        0      487 2023-02-04 17:09:12.303395 pandas_stubs-2.2.1.240316/pandas-stubs/core/computation/parsing.pyi
--rw-r--r--   0        0        0     3066 2023-11-03 13:55:15.981208 pandas_stubs-2.2.1.240316/pandas-stubs/core/computation/pytables.pyi
--rw-r--r--   0        0        0      645 2022-08-08 01:00:32.755711 pandas_stubs-2.2.1.240316/pandas-stubs/core/computation/scope.pyi
--rw-r--r--   0        0        0     1735 2023-09-23 02:44:57.787235 pandas_stubs-2.2.1.240316/pandas-stubs/core/config_init.pyi
--rw-r--r--   0        0        0      926 2023-04-01 02:35:39.718026 pandas_stubs-2.2.1.240316/pandas-stubs/core/construction.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.565503 pandas_stubs-2.2.1.240316/pandas-stubs/core/dtypes/__init__.pyi
--rw-r--r--   0        0        0     1395 2024-02-14 22:01:29.597936 pandas_stubs-2.2.1.240316/pandas-stubs/core/dtypes/api.pyi
--rw-r--r--   0        0        0      834 2023-02-27 22:18:36.858307 pandas_stubs-2.2.1.240316/pandas-stubs/core/dtypes/base.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.681655 pandas_stubs-2.2.1.240316/pandas-stubs/core/dtypes/cast.pyi
--rw-r--r--   0        0        0     2019 2024-02-14 22:01:29.598589 pandas_stubs-2.2.1.240316/pandas-stubs/core/dtypes/common.pyi
--rw-r--r--   0        0        0      308 2023-02-23 17:31:11.771588 pandas_stubs-2.2.1.240316/pandas-stubs/core/dtypes/concat.pyi
--rw-r--r--   0        0        0     1856 2023-09-28 14:06:32.018765 pandas_stubs-2.2.1.240316/pandas-stubs/core/dtypes/dtypes.pyi
--rw-r--r--   0        0        0      207 2022-12-28 15:28:49.683657 pandas_stubs-2.2.1.240316/pandas-stubs/core/dtypes/generic.pyi
--rw-r--r--   0        0        0      579 2024-02-14 22:01:29.599128 pandas_stubs-2.2.1.240316/pandas-stubs/core/dtypes/inference.pyi
--rw-r--r--   0        0        0     1027 2022-12-28 15:28:49.684666 pandas_stubs-2.2.1.240316/pandas-stubs/core/dtypes/missing.pyi
--rw-r--r--   0        0        0    70518 2024-02-26 14:49:23.730970 pandas_stubs-2.2.1.240316/pandas-stubs/core/frame.pyi
--rw-r--r--   0        0        0    15807 2024-02-14 22:01:29.601722 pandas_stubs-2.2.1.240316/pandas-stubs/core/generic.pyi
--rw-r--r--   0        0        0      387 2024-02-14 22:01:29.602317 pandas_stubs-2.2.1.240316/pandas-stubs/core/groupby/__init__.pyi
--rw-r--r--   0        0        0      167 2024-02-14 22:01:29.602849 pandas_stubs-2.2.1.240316/pandas-stubs/core/groupby/base.pyi
--rw-r--r--   0        0        0        0 2024-02-14 22:01:29.603906 pandas_stubs-2.2.1.240316/pandas-stubs/core/groupby/categorical.pyi
--rw-r--r--   0        0        0    11964 2024-02-14 22:01:29.604437 pandas_stubs-2.2.1.240316/pandas-stubs/core/groupby/generic.pyi
--rw-r--r--   0        0        0    12169 2024-02-14 22:01:29.604965 pandas_stubs-2.2.1.240316/pandas-stubs/core/groupby/groupby.pyi
--rw-r--r--   0        0        0     1919 2024-02-14 22:01:29.606027 pandas_stubs-2.2.1.240316/pandas-stubs/core/groupby/grouper.pyi
--rw-r--r--   0        0        0      805 2024-02-14 22:01:29.606556 pandas_stubs-2.2.1.240316/pandas-stubs/core/groupby/indexing.pyi
--rw-r--r--   0        0        0     2777 2024-02-14 22:01:29.607083 pandas_stubs-2.2.1.240316/pandas-stubs/core/groupby/ops.pyi
--rw-r--r--   0        0        0     1689 2023-08-14 11:37:22.156338 pandas_stubs-2.2.1.240316/pandas-stubs/core/indexers.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.575505 pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/__init__.pyi
--rw-r--r--   0        0        0    13258 2024-02-14 22:01:29.607656 pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/accessors.pyi
--rw-r--r--   0        0        0      748 2023-04-05 02:20:38.241521 pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/api.pyi
--rw-r--r--   0        0        0    15414 2024-02-14 22:01:29.608778 pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/base.pyi
--rw-r--r--   0        0        0     1678 2023-11-03 13:55:15.984236 pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/category.pyi
--rw-r--r--   0        0        0     1107 2024-02-14 22:01:29.609309 pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/datetimelike.pyi
--rw-r--r--   0        0        0     4056 2024-02-14 22:01:29.609838 pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/datetimes.pyi
--rw-r--r--   0        0        0      117 2023-08-14 14:08:10.536735 pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/extension.pyi
--rw-r--r--   0        0        0      419 2023-11-03 13:55:15.986234 pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/frozen.pyi
--rw-r--r--   0        0        0    13775 2024-02-14 22:01:29.610367 pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/interval.pyi
--rw-r--r--   0        0        0     5554 2024-03-16 23:39:57.124393 pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/multi.pyi
--rw-r--r--   0        0        0     2861 2024-02-14 22:01:29.611951 pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/period.pyi
--rw-r--r--   0        0        0     2837 2024-02-14 22:01:29.612488 pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/range.pyi
--rw-r--r--   0        0        0     3535 2024-02-14 22:01:29.613112 pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/timedeltas.pyi
--rw-r--r--   0        0        0     1849 2023-02-23 17:31:11.783587 pandas_stubs-2.2.1.240316/pandas-stubs/core/indexing.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.696655 pandas_stubs-2.2.1.240316/pandas-stubs/core/interchange/__init__.pyi
--rw-r--r--   0        0        0     3166 2023-02-04 17:09:12.315386 pandas_stubs-2.2.1.240316/pandas-stubs/core/interchange/dataframe_protocol.pyi
--rw-r--r--   0        0        0       92 2022-12-28 15:28:49.697655 pandas_stubs-2.2.1.240316/pandas-stubs/core/interchange/from_dataframe.pyi
--rw-r--r--   0        0        0      346 2022-12-28 15:28:49.698655 pandas_stubs-2.2.1.240316/pandas-stubs/core/missing.pyi
--rw-r--r--   0        0        0      211 2022-08-10 19:03:04.669578 pandas_stubs-2.2.1.240316/pandas-stubs/core/ops/__init__.pyi
--rw-r--r--   0        0        0      517 2022-08-10 19:03:04.669578 pandas_stubs-2.2.1.240316/pandas-stubs/core/ops/array_ops.pyi
--rw-r--r--   0        0        0       45 2022-08-08 01:00:33.245986 pandas_stubs-2.2.1.240316/pandas-stubs/core/ops/common.pyi
--rw-r--r--   0        0        0      120 2022-12-28 15:28:49.698655 pandas_stubs-2.2.1.240316/pandas-stubs/core/ops/dispatch.pyi
--rw-r--r--   0        0        0       17 2022-08-08 01:00:33.268029 pandas_stubs-2.2.1.240316/pandas-stubs/core/ops/docstrings.pyi
--rw-r--r--   0        0        0       81 2022-08-08 01:00:33.278086 pandas_stubs-2.2.1.240316/pandas-stubs/core/ops/invalid.pyi
--rw-r--r--   0        0        0      606 2022-08-08 01:00:33.289023 pandas_stubs-2.2.1.240316/pandas-stubs/core/ops/mask_ops.pyi
--rw-r--r--   0        0        0     7001 2024-02-14 22:01:29.614161 pandas_stubs-2.2.1.240316/pandas-stubs/core/resample.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.589504 pandas_stubs-2.2.1.240316/pandas-stubs/core/reshape/__init__.pyi
--rw-r--r--   0        0        0      633 2022-12-28 15:28:49.699654 pandas_stubs-2.2.1.240316/pandas-stubs/core/reshape/api.pyi
--rw-r--r--   0        0        0     4969 2024-03-16 23:39:57.125476 pandas_stubs-2.2.1.240316/pandas-stubs/core/reshape/concat.pyi
--rw-r--r--   0        0        0      716 2023-02-04 17:09:12.318387 pandas_stubs-2.2.1.240316/pandas-stubs/core/reshape/encoding.pyi
--rw-r--r--   0        0        0      741 2023-02-04 17:09:12.318387 pandas_stubs-2.2.1.240316/pandas-stubs/core/reshape/melt.pyi
--rw-r--r--   0        0        0     3121 2024-02-14 22:01:29.615233 pandas_stubs-2.2.1.240316/pandas-stubs/core/reshape/merge.pyi
--rw-r--r--   0        0        0     4137 2024-02-14 22:01:29.616332 pandas_stubs-2.2.1.240316/pandas-stubs/core/reshape/pivot.pyi
--rw-r--r--   0        0        0     8001 2024-02-14 22:01:29.617449 pandas_stubs-2.2.1.240316/pandas-stubs/core/reshape/tile.pyi
--rw-r--r--   0        0        0       30 2022-08-08 01:00:33.431568 pandas_stubs-2.2.1.240316/pandas-stubs/core/reshape/util.pyi
--rw-r--r--   0        0        0    70144 2024-02-26 14:49:23.748345 pandas_stubs-2.2.1.240316/pandas-stubs/core/series.pyi
--rw-r--r--   0        0        0        0 2022-07-03 21:17:38.591599 pandas_stubs-2.2.1.240316/pandas-stubs/core/sparse/__init__.pyi
--rw-r--r--   0        0        0     6667 2023-02-04 17:09:12.321425 pandas_stubs-2.2.1.240316/pandas-stubs/core/strings.pyi
--rw-r--r--   0        0        0        0 2022-08-10 19:03:04.672581 pandas_stubs-2.2.1.240316/pandas-stubs/core/tools/__init__.pyi
--rw-r--r--   0        0        0     2781 2024-02-14 22:01:29.619731 pandas_stubs-2.2.1.240316/pandas-stubs/core/tools/datetimes.pyi
--rw-r--r--   0        0        0      942 2024-02-14 22:01:29.620856 pandas_stubs-2.2.1.240316/pandas-stubs/core/tools/numeric.pyi
--rw-r--r--   0        0        0     1088 2024-02-14 22:01:29.621393 pandas_stubs-2.2.1.240316/pandas-stubs/core/tools/timedeltas.pyi
--rw-r--r--   0        0        0        0 2022-07-03 21:17:38.592587 pandas_stubs-2.2.1.240316/pandas-stubs/core/util/__init__.pyi
--rw-r--r--   0        0        0      480 2022-12-28 15:28:49.706655 pandas_stubs-2.2.1.240316/pandas-stubs/core/util/hashing.pyi
--rw-r--r--   0        0        0      420 2024-02-14 22:01:29.621931 pandas_stubs-2.2.1.240316/pandas-stubs/core/window/__init__.pyi
--rw-r--r--   0        0        0     2264 2024-02-14 22:01:29.622995 pandas_stubs-2.2.1.240316/pandas-stubs/core/window/ewm.pyi
--rw-r--r--   0        0        0      278 2024-02-14 22:01:29.623535 pandas_stubs-2.2.1.240316/pandas-stubs/core/window/expanding.pyi
--rw-r--r--   0        0        0     4978 2024-02-14 22:01:29.624073 pandas_stubs-2.2.1.240316/pandas-stubs/core/window/rolling.pyi
--rw-r--r--   0        0        0     1808 2022-12-28 15:28:49.709656 pandas_stubs-2.2.1.240316/pandas-stubs/errors/__init__.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.599505 pandas_stubs-2.2.1.240316/pandas-stubs/io/__init__.pyi
--rw-r--r--   0        0        0     1132 2022-08-08 01:00:33.649500 pandas_stubs-2.2.1.240316/pandas-stubs/io/api.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.710655 pandas_stubs-2.2.1.240316/pandas-stubs/io/clipboard/__init__.pyi
--rw-r--r--   0        0        0     7294 2024-02-14 22:01:29.624605 pandas_stubs-2.2.1.240316/pandas-stubs/io/clipboards.pyi
--rw-r--r--   0        0        0      487 2022-12-28 15:28:49.711655 pandas_stubs-2.2.1.240316/pandas-stubs/io/common.pyi
--rw-r--r--   0        0        0      128 2022-08-08 01:00:33.708448 pandas_stubs-2.2.1.240316/pandas-stubs/io/excel/__init__.pyi
--rw-r--r--   0        0        0    11089 2024-02-14 22:01:29.625692 pandas_stubs-2.2.1.240316/pandas-stubs/io/excel/_base.pyi
--rw-r--r--   0        0        0       73 2022-08-08 01:00:33.734493 pandas_stubs-2.2.1.240316/pandas-stubs/io/excel/_util.pyi
--rw-r--r--   0        0        0      446 2023-04-25 19:40:11.557224 pandas_stubs-2.2.1.240316/pandas-stubs/io/feather_format.pyi
--rw-r--r--   0        0        0        0 2022-07-03 21:17:38.596585 pandas_stubs-2.2.1.240316/pandas-stubs/io/formats/__init__.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.712655 pandas_stubs-2.2.1.240316/pandas-stubs/io/formats/css.pyi
--rw-r--r--   0        0        0      338 2022-12-28 15:28:49.713678 pandas_stubs-2.2.1.240316/pandas-stubs/io/formats/format.pyi
--rw-r--r--   0        0        0    11227 2024-02-14 22:01:29.626236 pandas_stubs-2.2.1.240316/pandas-stubs/io/formats/style.pyi
--rw-r--r--   0        0        0     2343 2023-08-14 11:37:22.162341 pandas_stubs-2.2.1.240316/pandas-stubs/io/formats/style_render.pyi
--rw-r--r--   0        0        0      685 2022-08-20 01:19:02.005181 pandas_stubs-2.2.1.240316/pandas-stubs/io/gbq.pyi
--rw-r--r--   0        0        0     1644 2024-02-14 22:01:29.627315 pandas_stubs-2.2.1.240316/pandas-stubs/io/html.pyi
--rw-r--r--   0        0        0      140 2023-05-22 14:12:55.276816 pandas_stubs-2.2.1.240316/pandas-stubs/io/json/__init__.pyi
--rw-r--r--   0        0        0     4377 2024-02-14 22:01:29.627852 pandas_stubs-2.2.1.240316/pandas-stubs/io/json/_json.pyi
--rw-r--r--   0        0        0      403 2022-08-29 12:14:24.790358 pandas_stubs-2.2.1.240316/pandas-stubs/io/json/_normalize.pyi
--rw-r--r--   0        0        0      285 2022-08-29 12:14:24.790358 pandas_stubs-2.2.1.240316/pandas-stubs/io/json/_table_schema.pyi
--rw-r--r--   0        0        0      393 2023-04-25 19:40:11.558224 pandas_stubs-2.2.1.240316/pandas-stubs/io/orc.pyi
--rw-r--r--   0        0        0      421 2022-08-29 12:14:24.791359 pandas_stubs-2.2.1.240316/pandas-stubs/io/parquet.pyi
--rw-r--r--   0        0        0      168 2022-12-28 15:28:49.716655 pandas_stubs-2.2.1.240316/pandas-stubs/io/parsers/__init__.pyi
--rw-r--r--   0        0        0    16747 2024-02-14 22:01:29.628561 pandas_stubs-2.2.1.240316/pandas-stubs/io/parsers/readers.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.716655 pandas_stubs-2.2.1.240316/pandas-stubs/io/parsers.pyi
--rw-r--r--   0        0        0      558 2022-12-28 15:28:49.717656 pandas_stubs-2.2.1.240316/pandas-stubs/io/pickle.pyi
--rw-r--r--   0        0        0     6712 2024-02-14 22:01:29.629076 pandas_stubs-2.2.1.240316/pandas-stubs/io/pytables.pyi
--rw-r--r--   0        0        0       58 2022-08-29 12:14:24.793360 pandas_stubs-2.2.1.240316/pandas-stubs/io/sas/__init__.pyi
--rw-r--r--   0        0        0      256 2022-12-28 15:28:49.718670 pandas_stubs-2.2.1.240316/pandas-stubs/io/sas/sas7bdat.pyi
--rw-r--r--   0        0        0      250 2022-08-29 12:14:24.794359 pandas_stubs-2.2.1.240316/pandas-stubs/io/sas/sas_xport.pyi
--rw-r--r--   0        0        0     2976 2023-02-23 17:31:11.792588 pandas_stubs-2.2.1.240316/pandas-stubs/io/sas/sasreader.pyi
--rw-r--r--   0        0        0      361 2023-04-25 19:40:11.560224 pandas_stubs-2.2.1.240316/pandas-stubs/io/spss.pyi
--rw-r--r--   0        0        0     5452 2024-02-14 22:01:29.629076 pandas_stubs-2.2.1.240316/pandas-stubs/io/sql.pyi
--rw-r--r--   0        0        0     4334 2023-02-23 17:31:11.795592 pandas_stubs-2.2.1.240316/pandas-stubs/io/stata.pyi
--rw-r--r--   0        0        0     1126 2023-04-25 19:40:11.561224 pandas_stubs-2.2.1.240316/pandas-stubs/io/xml.pyi
--rw-r--r--   0        0        0      587 2022-12-28 15:28:49.720654 pandas_stubs-2.2.1.240316/pandas-stubs/plotting/__init__.pyi
--rw-r--r--   0        0        0    12833 2024-02-14 22:01:29.631088 pandas_stubs-2.2.1.240316/pandas-stubs/plotting/_core.pyi
--rw-r--r--   0        0        0     2360 2023-02-23 17:31:11.797589 pandas_stubs-2.2.1.240316/pandas-stubs/plotting/_misc.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.722656 pandas_stubs-2.2.1.240316/pandas-stubs/py.typed
--rw-r--r--   0        0        0      368 2022-08-08 01:00:34.094401 pandas_stubs-2.2.1.240316/pandas-stubs/testing.pyi
--rw-r--r--   0        0        0       91 2023-05-22 14:12:55.278815 pandas_stubs-2.2.1.240316/pandas-stubs/tseries/__init__.pyi
--rw-r--r--   0        0        0       64 2022-08-08 01:00:34.100409 pandas_stubs-2.2.1.240316/pandas-stubs/tseries/api.pyi
--rw-r--r--   0        0        0      378 2022-12-28 15:28:49.722656 pandas_stubs-2.2.1.240316/pandas-stubs/tseries/frequencies.pyi
--rw-r--r--   0        0        0     4068 2024-02-14 22:01:29.631088 pandas_stubs-2.2.1.240316/pandas-stubs/tseries/holiday.pyi
--rw-r--r--   0        0        0     1312 2022-08-08 01:00:34.111525 pandas_stubs-2.2.1.240316/pandas-stubs/tseries/offsets.pyi
--rw-r--r--   0        0        0      121 2023-05-22 14:12:55.278815 pandas_stubs-2.2.1.240316/pandas-stubs/util/__init__.pyi
--rw-r--r--   0        0        0       70 2024-02-14 22:01:29.631088 pandas_stubs-2.2.1.240316/pandas-stubs/util/_decorators.pyi
--rw-r--r--   0        0        0      279 2022-08-08 01:00:34.130416 pandas_stubs-2.2.1.240316/pandas-stubs/util/_doctools.pyi
--rw-r--r--   0        0        0       57 2022-08-08 01:00:34.135732 pandas_stubs-2.2.1.240316/pandas-stubs/util/_exceptions.pyi
--rw-r--r--   0        0        0       53 2022-12-28 15:28:49.723655 pandas_stubs-2.2.1.240316/pandas-stubs/util/_print_versions.pyi
--rw-r--r--   0        0        0       38 2022-08-08 01:00:34.153394 pandas_stubs-2.2.1.240316/pandas-stubs/util/_tester.pyi
--rw-r--r--   0        0        0      594 2023-02-04 17:09:12.332423 pandas_stubs-2.2.1.240316/pandas-stubs/util/_validators.pyi
--rw-r--r--   0        0        0     1899 2022-12-28 15:28:49.725656 pandas_stubs-2.2.1.240316/pandas-stubs/util/version/__init__.pyi
--rw-r--r--   0        0        0     7237 2024-03-16 23:40:39.007610 pandas_stubs-2.2.1.240316/pyproject.toml
--rw-r--r--   0        0        0     8421 2023-11-03 13:55:15.973232 pandas_stubs-2.2.1.240316/README.md
--rw-r--r--   0        0        0     9500 1970-01-01 00:00:00.000000 pandas_stubs-2.2.1.240316/PKG-INFO
+-rw-r--r--   0        0        0     1514 2022-08-08 01:00:32.131878 pandas_stubs-2.2.2.240514/LICENSE
+-rw-r--r--   0        0        0     3805 2023-05-22 14:12:55.264847 pandas_stubs-2.2.2.240514/pandas-stubs/__init__.pyi
+-rw-r--r--   0        0        0      220 2022-08-08 01:00:32.243006 pandas_stubs-2.2.2.240514/pandas-stubs/_config/__init__.pyi
+-rw-r--r--   0        0        0     4173 2023-09-23 02:44:57.787235 pandas_stubs-2.2.2.240514/pandas-stubs/_config/config.pyi
+-rw-r--r--   0        0        0      285 2023-05-22 14:12:55.265853 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/__init__.pyi
+-rw-r--r--   0        0        0      132 2022-08-08 01:00:32.278047 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/indexing.pyi
+-rw-r--r--   0        0        0     8429 2023-12-18 16:23:19.658046 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/interval.pyi
+-rw-r--r--   0        0        0      130 2022-08-08 01:00:32.293998 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/json.pyi
+-rw-r--r--   0        0        0      779 2024-02-14 22:01:29.589865 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/lib.pyi
+-rw-r--r--   0        0        0     1893 2023-02-23 17:31:11.761589 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/missing.pyi
+-rw-r--r--   0        0        0      126 2022-08-08 01:00:32.310002 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/ops_dispatch.pyi
+-rw-r--r--   0        0        0      599 2024-02-14 22:01:29.590444 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/properties.pyi
+-rw-r--r--   0        0        0       91 2022-08-08 01:00:32.320997 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/sparse.pyi
+-rw-r--r--   0        0        0      666 2023-05-22 14:12:55.265853 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/tslibs/__init__.pyi
+-rw-r--r--   0        0        0       65 2022-08-08 01:00:32.332997 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/tslibs/base.pyi
+-rw-r--r--   0        0        0      143 2022-08-08 01:00:32.346996 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/tslibs/conversion.pyi
+-rw-r--r--   0        0        0     1195 2022-08-10 19:03:04.643581 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/tslibs/dtypes.pyi
+-rw-r--r--   0        0        0     3764 2024-02-14 22:01:29.591592 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/tslibs/nattype.pyi
+-rw-r--r--   0        0        0       89 2022-12-28 15:28:49.658657 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/tslibs/np_datetime.pyi
+-rw-r--r--   0        0        0     8605 2023-09-28 14:06:32.016764 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/tslibs/offsets.pyi
+-rw-r--r--   0        0        0      163 2022-08-08 01:00:32.387997 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/tslibs/parsing.pyi
+-rw-r--r--   0        0        0     6686 2024-02-14 22:01:29.592119 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/tslibs/period.pyi
+-rw-r--r--   0        0        0       72 2022-08-08 01:00:32.405128 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/tslibs/strptime.pyi
+-rw-r--r--   0        0        0    14430 2024-04-26 17:07:19.866092 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/tslibs/timedeltas.pyi
+-rw-r--r--   0        0        0    11589 2024-04-03 13:56:46.108542 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/tslibs/timestamps.pyi
+-rw-r--r--   0        0        0       62 2022-08-08 01:00:32.438009 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/tslibs/tzconversion.pyi
+-rw-r--r--   0        0        0      613 2023-02-04 17:09:12.293389 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/tslibs/vectorized.pyi
+-rw-r--r--   0        0        0        0 2022-07-03 21:17:38.574585 pandas_stubs-2.2.2.240514/pandas-stubs/_libs/window/__init__.pyi
+-rw-r--r--   0        0        0     4100 2023-12-18 16:23:19.658046 pandas_stubs-2.2.2.240514/pandas-stubs/_testing/__init__.pyi
+-rw-r--r--   0        0        0    24743 2024-05-12 17:30:24.439180 pandas_stubs-2.2.2.240514/pandas-stubs/_typing.pyi
+-rw-r--r--   0        0        0      124 2024-05-14 17:41:20.423670 pandas_stubs-2.2.2.240514/pandas-stubs/_version.pyi
+-rw-r--r--   0        0        0      141 2023-06-05 12:34:31.504832 pandas_stubs-2.2.2.240514/pandas-stubs/api/__init__.pyi
+-rw-r--r--   0        0        0      603 2023-02-27 22:18:36.851320 pandas_stubs-2.2.2.240514/pandas-stubs/api/extensions/__init__.pyi
+-rw-r--r--   0        0        0      241 2022-08-08 01:00:32.486031 pandas_stubs-2.2.2.240514/pandas-stubs/api/indexers/__init__.pyi
+-rw-r--r--   0        0        0      164 2024-05-13 18:55:54.245220 pandas_stubs-2.2.2.240514/pandas-stubs/api/interchange/__init__.pyi
+-rw-r--r--   0        0        0     1729 2024-02-14 22:01:29.595520 pandas_stubs-2.2.2.240514/pandas-stubs/api/types/__init__.pyi
+-rw-r--r--   0        0        0      373 2022-08-08 01:00:32.499997 pandas_stubs-2.2.2.240514/pandas-stubs/arrays/__init__.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.550503 pandas_stubs-2.2.2.240514/pandas-stubs/core/__init__.pyi
+-rw-r--r--   0        0        0      437 2023-08-14 14:08:10.526716 pandas_stubs-2.2.2.240514/pandas-stubs/core/accessor.pyi
+-rw-r--r--   0        0        0     2288 2024-04-26 17:07:19.866092 pandas_stubs-2.2.2.240514/pandas-stubs/core/algorithms.pyi
+-rw-r--r--   0        0        0     2680 2023-04-05 02:20:38.240522 pandas_stubs-2.2.2.240514/pandas-stubs/core/api.pyi
+-rw-r--r--   0        0        0     2052 2023-11-03 13:55:15.977230 pandas_stubs-2.2.2.240514/pandas-stubs/core/arraylike.pyi
+-rw-r--r--   0        0        0      924 2023-05-22 14:12:55.269816 pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/__init__.pyi
+-rw-r--r--   0        0        0      321 2023-02-27 03:32:24.825818 pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/arrow/dtype.pyi
+-rw-r--r--   0        0        0     2372 2024-05-14 17:39:47.744399 pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/base.pyi
+-rw-r--r--   0        0        0      961 2023-11-03 13:55:15.978208 pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/boolean.pyi
+-rw-r--r--   0        0        0     7333 2023-08-14 14:08:10.528724 pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/categorical.pyi
+-rw-r--r--   0        0        0     2890 2024-02-14 22:01:29.596147 pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/datetimelike.pyi
+-rw-r--r--   0        0        0     2268 2023-11-03 13:55:15.978208 pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/datetimes.pyi
+-rw-r--r--   0        0        0      133 2022-12-28 15:28:49.670655 pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/floating.pyi
+-rw-r--r--   0        0        0     1060 2023-11-03 13:55:15.979233 pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/integer.pyi
+-rw-r--r--   0        0        0     2720 2023-11-03 13:55:15.979233 pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/interval.pyi
+-rw-r--r--   0        0        0      824 2023-11-03 13:55:15.980236 pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/masked.pyi
+-rw-r--r--   0        0        0       99 2023-02-27 03:32:24.828808 pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/numeric.pyi
+-rw-r--r--   0        0        0      513 2023-02-27 03:32:24.828808 pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/numpy_.pyi
+-rw-r--r--   0        0        0     1705 2023-11-03 13:55:15.980236 pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/period.pyi
+-rw-r--r--   0        0        0      285 2023-05-22 14:12:55.271819 pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/sparse/__init__.pyi
+-rw-r--r--   0        0        0      650 2023-04-12 19:14:53.206395 pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/sparse/accessor.pyi
+-rw-r--r--   0        0        0     1891 2023-11-03 13:55:15.981208 pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/sparse/array.pyi
+-rw-r--r--   0        0        0      448 2023-02-27 03:32:24.829807 pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/sparse/dtype.pyi
+-rw-r--r--   0        0        0      715 2023-02-27 03:32:24.830807 pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/string_.pyi
+-rw-r--r--   0        0        0     1963 2023-02-04 17:09:12.301416 pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/timedeltas.pyi
+-rw-r--r--   0        0        0     2892 2024-02-14 22:01:29.597311 pandas_stubs-2.2.2.240514/pandas-stubs/core/base.pyi
+-rw-r--r--   0        0        0      955 2023-02-04 17:09:12.302429 pandas_stubs-2.2.2.240514/pandas-stubs/core/common.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.561504 pandas_stubs-2.2.2.240514/pandas-stubs/core/computation/__init__.pyi
+-rw-r--r--   0        0        0       79 2022-08-08 01:00:32.662463 pandas_stubs-2.2.2.240514/pandas-stubs/core/computation/align.pyi
+-rw-r--r--   0        0        0       54 2022-08-08 01:00:32.670999 pandas_stubs-2.2.2.240514/pandas-stubs/core/computation/api.pyi
+-rw-r--r--   0        0        0       47 2022-08-10 19:03:04.655579 pandas_stubs-2.2.2.240514/pandas-stubs/core/computation/common.pyi
+-rw-r--r--   0        0        0      438 2022-12-28 15:28:49.678655 pandas_stubs-2.2.2.240514/pandas-stubs/core/computation/engines.pyi
+-rw-r--r--   0        0        0      668 2023-02-04 17:09:12.302429 pandas_stubs-2.2.2.240514/pandas-stubs/core/computation/eval.pyi
+-rw-r--r--   0        0        0     2348 2023-08-14 11:37:22.152338 pandas_stubs-2.2.2.240514/pandas-stubs/core/computation/expr.pyi
+-rw-r--r--   0        0        0      270 2022-08-08 01:00:32.711086 pandas_stubs-2.2.2.240514/pandas-stubs/core/computation/expressions.pyi
+-rw-r--r--   0        0        0     2342 2023-08-14 14:08:10.529736 pandas_stubs-2.2.2.240514/pandas-stubs/core/computation/ops.pyi
+-rw-r--r--   0        0        0      487 2023-02-04 17:09:12.303395 pandas_stubs-2.2.2.240514/pandas-stubs/core/computation/parsing.pyi
+-rw-r--r--   0        0        0     3066 2023-11-03 13:55:15.981208 pandas_stubs-2.2.2.240514/pandas-stubs/core/computation/pytables.pyi
+-rw-r--r--   0        0        0      645 2022-08-08 01:00:32.755711 pandas_stubs-2.2.2.240514/pandas-stubs/core/computation/scope.pyi
+-rw-r--r--   0        0        0     1735 2023-09-23 02:44:57.787235 pandas_stubs-2.2.2.240514/pandas-stubs/core/config_init.pyi
+-rw-r--r--   0        0        0      926 2023-04-01 02:35:39.718026 pandas_stubs-2.2.2.240514/pandas-stubs/core/construction.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.565503 pandas_stubs-2.2.2.240514/pandas-stubs/core/dtypes/__init__.pyi
+-rw-r--r--   0        0        0     1395 2024-02-14 22:01:29.597936 pandas_stubs-2.2.2.240514/pandas-stubs/core/dtypes/api.pyi
+-rw-r--r--   0        0        0      834 2023-02-27 22:18:36.858307 pandas_stubs-2.2.2.240514/pandas-stubs/core/dtypes/base.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.681655 pandas_stubs-2.2.2.240514/pandas-stubs/core/dtypes/cast.pyi
+-rw-r--r--   0        0        0     2019 2024-02-14 22:01:29.598589 pandas_stubs-2.2.2.240514/pandas-stubs/core/dtypes/common.pyi
+-rw-r--r--   0        0        0      308 2023-02-23 17:31:11.771588 pandas_stubs-2.2.2.240514/pandas-stubs/core/dtypes/concat.pyi
+-rw-r--r--   0        0        0     1856 2023-09-28 14:06:32.018765 pandas_stubs-2.2.2.240514/pandas-stubs/core/dtypes/dtypes.pyi
+-rw-r--r--   0        0        0      207 2022-12-28 15:28:49.683657 pandas_stubs-2.2.2.240514/pandas-stubs/core/dtypes/generic.pyi
+-rw-r--r--   0        0        0      579 2024-02-14 22:01:29.599128 pandas_stubs-2.2.2.240514/pandas-stubs/core/dtypes/inference.pyi
+-rw-r--r--   0        0        0     1027 2022-12-28 15:28:49.684666 pandas_stubs-2.2.2.240514/pandas-stubs/core/dtypes/missing.pyi
+-rw-r--r--   0        0        0    72152 2024-05-12 17:30:24.439180 pandas_stubs-2.2.2.240514/pandas-stubs/core/frame.pyi
+-rw-r--r--   0        0        0    15807 2024-02-14 22:01:29.601722 pandas_stubs-2.2.2.240514/pandas-stubs/core/generic.pyi
+-rw-r--r--   0        0        0      387 2024-02-14 22:01:29.602317 pandas_stubs-2.2.2.240514/pandas-stubs/core/groupby/__init__.pyi
+-rw-r--r--   0        0        0      167 2024-02-14 22:01:29.602849 pandas_stubs-2.2.2.240514/pandas-stubs/core/groupby/base.pyi
+-rw-r--r--   0        0        0        0 2024-02-14 22:01:29.603906 pandas_stubs-2.2.2.240514/pandas-stubs/core/groupby/categorical.pyi
+-rw-r--r--   0        0        0    11931 2024-05-12 17:30:24.439180 pandas_stubs-2.2.2.240514/pandas-stubs/core/groupby/generic.pyi
+-rw-r--r--   0        0        0    12169 2024-02-14 22:01:29.604965 pandas_stubs-2.2.2.240514/pandas-stubs/core/groupby/groupby.pyi
+-rw-r--r--   0        0        0     1919 2024-02-14 22:01:29.606027 pandas_stubs-2.2.2.240514/pandas-stubs/core/groupby/grouper.pyi
+-rw-r--r--   0        0        0      805 2024-02-14 22:01:29.606556 pandas_stubs-2.2.2.240514/pandas-stubs/core/groupby/indexing.pyi
+-rw-r--r--   0        0        0     2777 2024-02-14 22:01:29.607083 pandas_stubs-2.2.2.240514/pandas-stubs/core/groupby/ops.pyi
+-rw-r--r--   0        0        0     1689 2023-08-14 11:37:22.156338 pandas_stubs-2.2.2.240514/pandas-stubs/core/indexers.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.575505 pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/__init__.pyi
+-rw-r--r--   0        0        0    13258 2024-02-14 22:01:29.607656 pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/accessors.pyi
+-rw-r--r--   0        0        0      748 2023-04-05 02:20:38.241521 pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/api.pyi
+-rw-r--r--   0        0        0    15414 2024-02-14 22:01:29.608778 pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/base.pyi
+-rw-r--r--   0        0        0     1678 2023-11-03 13:55:15.984236 pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/category.pyi
+-rw-r--r--   0        0        0     1107 2024-02-14 22:01:29.609309 pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/datetimelike.pyi
+-rw-r--r--   0        0        0     4056 2024-02-14 22:01:29.609838 pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/datetimes.pyi
+-rw-r--r--   0        0        0      117 2023-08-14 14:08:10.536735 pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/extension.pyi
+-rw-r--r--   0        0        0      419 2023-11-03 13:55:15.986234 pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/frozen.pyi
+-rw-r--r--   0        0        0    13775 2024-02-14 22:01:29.610367 pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/interval.pyi
+-rw-r--r--   0        0        0     5554 2024-03-16 23:39:57.124393 pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/multi.pyi
+-rw-r--r--   0        0        0     2861 2024-02-14 22:01:29.611951 pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/period.pyi
+-rw-r--r--   0        0        0     2837 2024-02-14 22:01:29.612488 pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/range.pyi
+-rw-r--r--   0        0        0     3467 2024-04-26 17:07:19.871234 pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/timedeltas.pyi
+-rw-r--r--   0        0        0     1849 2023-02-23 17:31:11.783587 pandas_stubs-2.2.2.240514/pandas-stubs/core/indexing.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.696655 pandas_stubs-2.2.2.240514/pandas-stubs/core/interchange/__init__.pyi
+-rw-r--r--   0        0        0     3166 2023-02-04 17:09:12.315386 pandas_stubs-2.2.2.240514/pandas-stubs/core/interchange/dataframe_protocol.pyi
+-rw-r--r--   0        0        0       92 2024-05-13 18:55:44.840816 pandas_stubs-2.2.2.240514/pandas-stubs/core/interchange/from_dataframe.pyi
+-rw-r--r--   0        0        0      346 2022-12-28 15:28:49.698655 pandas_stubs-2.2.2.240514/pandas-stubs/core/missing.pyi
+-rw-r--r--   0        0        0      211 2022-08-10 19:03:04.669578 pandas_stubs-2.2.2.240514/pandas-stubs/core/ops/__init__.pyi
+-rw-r--r--   0        0        0      517 2022-08-10 19:03:04.669578 pandas_stubs-2.2.2.240514/pandas-stubs/core/ops/array_ops.pyi
+-rw-r--r--   0        0        0       45 2022-08-08 01:00:33.245986 pandas_stubs-2.2.2.240514/pandas-stubs/core/ops/common.pyi
+-rw-r--r--   0        0        0      120 2022-12-28 15:28:49.698655 pandas_stubs-2.2.2.240514/pandas-stubs/core/ops/dispatch.pyi
+-rw-r--r--   0        0        0       17 2022-08-08 01:00:33.268029 pandas_stubs-2.2.2.240514/pandas-stubs/core/ops/docstrings.pyi
+-rw-r--r--   0        0        0       81 2022-08-08 01:00:33.278086 pandas_stubs-2.2.2.240514/pandas-stubs/core/ops/invalid.pyi
+-rw-r--r--   0        0        0      606 2022-08-08 01:00:33.289023 pandas_stubs-2.2.2.240514/pandas-stubs/core/ops/mask_ops.pyi
+-rw-r--r--   0        0        0     7001 2024-02-14 22:01:29.614161 pandas_stubs-2.2.2.240514/pandas-stubs/core/resample.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.589504 pandas_stubs-2.2.2.240514/pandas-stubs/core/reshape/__init__.pyi
+-rw-r--r--   0        0        0      633 2022-12-28 15:28:49.699654 pandas_stubs-2.2.2.240514/pandas-stubs/core/reshape/api.pyi
+-rw-r--r--   0        0        0     5018 2024-04-03 13:56:46.112471 pandas_stubs-2.2.2.240514/pandas-stubs/core/reshape/concat.pyi
+-rw-r--r--   0        0        0      716 2023-02-04 17:09:12.318387 pandas_stubs-2.2.2.240514/pandas-stubs/core/reshape/encoding.pyi
+-rw-r--r--   0        0        0      741 2023-02-04 17:09:12.318387 pandas_stubs-2.2.2.240514/pandas-stubs/core/reshape/melt.pyi
+-rw-r--r--   0        0        0     3098 2024-04-26 17:07:19.871234 pandas_stubs-2.2.2.240514/pandas-stubs/core/reshape/merge.pyi
+-rw-r--r--   0        0        0     4137 2024-02-14 22:01:29.616332 pandas_stubs-2.2.2.240514/pandas-stubs/core/reshape/pivot.pyi
+-rw-r--r--   0        0        0     8001 2024-02-14 22:01:29.617449 pandas_stubs-2.2.2.240514/pandas-stubs/core/reshape/tile.pyi
+-rw-r--r--   0        0        0       30 2022-08-08 01:00:33.431568 pandas_stubs-2.2.2.240514/pandas-stubs/core/reshape/util.pyi
+-rw-r--r--   0        0        0    71481 2024-05-12 17:30:24.439180 pandas_stubs-2.2.2.240514/pandas-stubs/core/series.pyi
+-rw-r--r--   0        0        0        0 2022-07-03 21:17:38.591599 pandas_stubs-2.2.2.240514/pandas-stubs/core/sparse/__init__.pyi
+-rw-r--r--   0        0        0     6667 2023-02-04 17:09:12.321425 pandas_stubs-2.2.2.240514/pandas-stubs/core/strings.pyi
+-rw-r--r--   0        0        0        0 2022-08-10 19:03:04.672581 pandas_stubs-2.2.2.240514/pandas-stubs/core/tools/__init__.pyi
+-rw-r--r--   0        0        0     2773 2024-04-03 13:56:46.113574 pandas_stubs-2.2.2.240514/pandas-stubs/core/tools/datetimes.pyi
+-rw-r--r--   0        0        0      942 2024-02-14 22:01:29.620856 pandas_stubs-2.2.2.240514/pandas-stubs/core/tools/numeric.pyi
+-rw-r--r--   0        0        0     1088 2024-02-14 22:01:29.621393 pandas_stubs-2.2.2.240514/pandas-stubs/core/tools/timedeltas.pyi
+-rw-r--r--   0        0        0        0 2022-07-03 21:17:38.592587 pandas_stubs-2.2.2.240514/pandas-stubs/core/util/__init__.pyi
+-rw-r--r--   0        0        0      480 2022-12-28 15:28:49.706655 pandas_stubs-2.2.2.240514/pandas-stubs/core/util/hashing.pyi
+-rw-r--r--   0        0        0      420 2024-02-14 22:01:29.621931 pandas_stubs-2.2.2.240514/pandas-stubs/core/window/__init__.pyi
+-rw-r--r--   0        0        0     2264 2024-02-14 22:01:29.622995 pandas_stubs-2.2.2.240514/pandas-stubs/core/window/ewm.pyi
+-rw-r--r--   0        0        0      278 2024-02-14 22:01:29.623535 pandas_stubs-2.2.2.240514/pandas-stubs/core/window/expanding.pyi
+-rw-r--r--   0        0        0     4978 2024-02-14 22:01:29.624073 pandas_stubs-2.2.2.240514/pandas-stubs/core/window/rolling.pyi
+-rw-r--r--   0        0        0     1808 2022-12-28 15:28:49.709656 pandas_stubs-2.2.2.240514/pandas-stubs/errors/__init__.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.599505 pandas_stubs-2.2.2.240514/pandas-stubs/io/__init__.pyi
+-rw-r--r--   0        0        0     1132 2022-08-08 01:00:33.649500 pandas_stubs-2.2.2.240514/pandas-stubs/io/api.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.710655 pandas_stubs-2.2.2.240514/pandas-stubs/io/clipboard/__init__.pyi
+-rw-r--r--   0        0        0     7294 2024-02-14 22:01:29.624605 pandas_stubs-2.2.2.240514/pandas-stubs/io/clipboards.pyi
+-rw-r--r--   0        0        0      487 2022-12-28 15:28:49.711655 pandas_stubs-2.2.2.240514/pandas-stubs/io/common.pyi
+-rw-r--r--   0        0        0      128 2022-08-08 01:00:33.708448 pandas_stubs-2.2.2.240514/pandas-stubs/io/excel/__init__.pyi
+-rw-r--r--   0        0        0    11004 2024-05-12 17:30:24.439180 pandas_stubs-2.2.2.240514/pandas-stubs/io/excel/_base.pyi
+-rw-r--r--   0        0        0       73 2022-08-08 01:00:33.734493 pandas_stubs-2.2.2.240514/pandas-stubs/io/excel/_util.pyi
+-rw-r--r--   0        0        0      446 2023-04-25 19:40:11.557224 pandas_stubs-2.2.2.240514/pandas-stubs/io/feather_format.pyi
+-rw-r--r--   0        0        0        0 2022-07-03 21:17:38.596585 pandas_stubs-2.2.2.240514/pandas-stubs/io/formats/__init__.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.712655 pandas_stubs-2.2.2.240514/pandas-stubs/io/formats/css.pyi
+-rw-r--r--   0        0        0      338 2022-12-28 15:28:49.713678 pandas_stubs-2.2.2.240514/pandas-stubs/io/formats/format.pyi
+-rw-r--r--   0        0        0    11769 2024-05-13 18:04:22.478468 pandas_stubs-2.2.2.240514/pandas-stubs/io/formats/style.pyi
+-rw-r--r--   0        0        0     2343 2023-08-14 11:37:22.162341 pandas_stubs-2.2.2.240514/pandas-stubs/io/formats/style_render.pyi
+-rw-r--r--   0        0        0      685 2022-08-20 01:19:02.005181 pandas_stubs-2.2.2.240514/pandas-stubs/io/gbq.pyi
+-rw-r--r--   0        0        0     1644 2024-02-14 22:01:29.627315 pandas_stubs-2.2.2.240514/pandas-stubs/io/html.pyi
+-rw-r--r--   0        0        0      140 2023-05-22 14:12:55.276816 pandas_stubs-2.2.2.240514/pandas-stubs/io/json/__init__.pyi
+-rw-r--r--   0        0        0     4377 2024-02-14 22:01:29.627852 pandas_stubs-2.2.2.240514/pandas-stubs/io/json/_json.pyi
+-rw-r--r--   0        0        0      403 2022-08-29 12:14:24.790358 pandas_stubs-2.2.2.240514/pandas-stubs/io/json/_normalize.pyi
+-rw-r--r--   0        0        0      285 2022-08-29 12:14:24.790358 pandas_stubs-2.2.2.240514/pandas-stubs/io/json/_table_schema.pyi
+-rw-r--r--   0        0        0      393 2023-04-25 19:40:11.558224 pandas_stubs-2.2.2.240514/pandas-stubs/io/orc.pyi
+-rw-r--r--   0        0        0      421 2022-08-29 12:14:24.791359 pandas_stubs-2.2.2.240514/pandas-stubs/io/parquet.pyi
+-rw-r--r--   0        0        0      168 2022-12-28 15:28:49.716655 pandas_stubs-2.2.2.240514/pandas-stubs/io/parsers/__init__.pyi
+-rw-r--r--   0        0        0    16747 2024-02-14 22:01:29.628561 pandas_stubs-2.2.2.240514/pandas-stubs/io/parsers/readers.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.716655 pandas_stubs-2.2.2.240514/pandas-stubs/io/parsers.pyi
+-rw-r--r--   0        0        0      558 2022-12-28 15:28:49.717656 pandas_stubs-2.2.2.240514/pandas-stubs/io/pickle.pyi
+-rw-r--r--   0        0        0     6712 2024-02-14 22:01:29.629076 pandas_stubs-2.2.2.240514/pandas-stubs/io/pytables.pyi
+-rw-r--r--   0        0        0       58 2022-08-29 12:14:24.793360 pandas_stubs-2.2.2.240514/pandas-stubs/io/sas/__init__.pyi
+-rw-r--r--   0        0        0      256 2022-12-28 15:28:49.718670 pandas_stubs-2.2.2.240514/pandas-stubs/io/sas/sas7bdat.pyi
+-rw-r--r--   0        0        0      250 2022-08-29 12:14:24.794359 pandas_stubs-2.2.2.240514/pandas-stubs/io/sas/sas_xport.pyi
+-rw-r--r--   0        0        0     2976 2023-02-23 17:31:11.792588 pandas_stubs-2.2.2.240514/pandas-stubs/io/sas/sasreader.pyi
+-rw-r--r--   0        0        0      361 2023-04-25 19:40:11.560224 pandas_stubs-2.2.2.240514/pandas-stubs/io/spss.pyi
+-rw-r--r--   0        0        0     5452 2024-02-14 22:01:29.629076 pandas_stubs-2.2.2.240514/pandas-stubs/io/sql.pyi
+-rw-r--r--   0        0        0     4334 2023-02-23 17:31:11.795592 pandas_stubs-2.2.2.240514/pandas-stubs/io/stata.pyi
+-rw-r--r--   0        0        0     1126 2023-04-25 19:40:11.561224 pandas_stubs-2.2.2.240514/pandas-stubs/io/xml.pyi
+-rw-r--r--   0        0        0      587 2022-12-28 15:28:49.720654 pandas_stubs-2.2.2.240514/pandas-stubs/plotting/__init__.pyi
+-rw-r--r--   0        0        0    12833 2024-02-14 22:01:29.631088 pandas_stubs-2.2.2.240514/pandas-stubs/plotting/_core.pyi
+-rw-r--r--   0        0        0     2360 2023-02-23 17:31:11.797589 pandas_stubs-2.2.2.240514/pandas-stubs/plotting/_misc.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.722656 pandas_stubs-2.2.2.240514/pandas-stubs/py.typed
+-rw-r--r--   0        0        0      368 2022-08-08 01:00:34.094401 pandas_stubs-2.2.2.240514/pandas-stubs/testing.pyi
+-rw-r--r--   0        0        0       91 2023-05-22 14:12:55.278815 pandas_stubs-2.2.2.240514/pandas-stubs/tseries/__init__.pyi
+-rw-r--r--   0        0        0       64 2022-08-08 01:00:34.100409 pandas_stubs-2.2.2.240514/pandas-stubs/tseries/api.pyi
+-rw-r--r--   0        0        0      378 2022-12-28 15:28:49.722656 pandas_stubs-2.2.2.240514/pandas-stubs/tseries/frequencies.pyi
+-rw-r--r--   0        0        0     4068 2024-02-14 22:01:29.631088 pandas_stubs-2.2.2.240514/pandas-stubs/tseries/holiday.pyi
+-rw-r--r--   0        0        0     1312 2022-08-08 01:00:34.111525 pandas_stubs-2.2.2.240514/pandas-stubs/tseries/offsets.pyi
+-rw-r--r--   0        0        0      121 2023-05-22 14:12:55.278815 pandas_stubs-2.2.2.240514/pandas-stubs/util/__init__.pyi
+-rw-r--r--   0        0        0       70 2024-02-14 22:01:29.631088 pandas_stubs-2.2.2.240514/pandas-stubs/util/_decorators.pyi
+-rw-r--r--   0        0        0      279 2022-08-08 01:00:34.130416 pandas_stubs-2.2.2.240514/pandas-stubs/util/_doctools.pyi
+-rw-r--r--   0        0        0       57 2022-08-08 01:00:34.135732 pandas_stubs-2.2.2.240514/pandas-stubs/util/_exceptions.pyi
+-rw-r--r--   0        0        0       53 2022-12-28 15:28:49.723655 pandas_stubs-2.2.2.240514/pandas-stubs/util/_print_versions.pyi
+-rw-r--r--   0        0        0       38 2022-08-08 01:00:34.153394 pandas_stubs-2.2.2.240514/pandas-stubs/util/_tester.pyi
+-rw-r--r--   0        0        0      594 2023-02-04 17:09:12.332423 pandas_stubs-2.2.2.240514/pandas-stubs/util/_validators.pyi
+-rw-r--r--   0        0        0     1899 2022-12-28 15:28:49.725656 pandas_stubs-2.2.2.240514/pandas-stubs/util/version/__init__.pyi
+-rw-r--r--   0        0        0     7265 2024-05-14 17:41:03.978479 pandas_stubs-2.2.2.240514/pyproject.toml
+-rw-r--r--   0        0        0     8994 2024-05-12 17:30:24.439180 pandas_stubs-2.2.2.240514/README.md
+-rw-r--r--   0        0        0    10066 1970-01-01 00:00:00.000000 pandas_stubs-2.2.2.240514/PKG-INFO
```

### Comparing `pandas_stubs-2.2.1.240316/LICENSE` & `pandas_stubs-2.2.2.240514/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/__init__.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/_config/config.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/_config/config.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/_libs/interval.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/_libs/interval.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/_libs/lib.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/_libs/lib.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/_libs/missing.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/_libs/missing.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/_libs/properties.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/_libs/properties.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/_libs/tslibs/__init__.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/_libs/tslibs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/_libs/tslibs/dtypes.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/_libs/tslibs/dtypes.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/_libs/tslibs/nattype.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/_libs/tslibs/nattype.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/_libs/tslibs/offsets.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/_libs/tslibs/offsets.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/_libs/tslibs/period.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/_libs/tslibs/period.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/_libs/tslibs/timedeltas.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/_libs/tslibs/timedeltas.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,58 +44,48 @@
     milliseconds: int
     microseconds: int
     nanoseconds: int
 
 # This should be kept consistent with the keys in the dict timedelta_abbrevs
 # in pandas/_libs/tslibs/timedeltas.pyx
 TimeDeltaUnitChoices: TypeAlias = Literal[
-    "H",
-    "T",
-    "S",
-    "L",
-    "U",
-    "N",
     "W",
     "w",
     "D",
     "d",
     "days",
     "day",
     "hours",
     "hour",
     "hr",
     "h",
     "m",
     "minute",
     "min",
     "minutes",
-    "t",
     "s",
     "seconds",
     "sec",
     "second",
     "ms",
     "milliseconds",
     "millisecond",
     "milli",
     "millis",
-    "l",
     "us",
     "microseconds",
     "microsecond",
     "µs",
     "micro",
     "micros",
-    "u",
     "ns",
     "nanoseconds",
     "nano",
     "nanos",
     "nanosecond",
-    "n",
 ]
 
 UnitChoices: TypeAlias = (
     TimeDeltaUnitChoices
     | Literal[
         "Y",
         "y",
```

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/_libs/tslibs/timestamps.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/_libs/tslibs/timestamps.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,15 @@
     @overload
     def __sub__(self, other: timedelta | np.timedelta64 | Tick) -> Self: ...
     @overload
     def __sub__(self, other: TimedeltaIndex) -> DatetimeIndex: ...
     @overload
     def __sub__(self, other: TimedeltaSeries) -> TimestampSeries: ...
     @overload
-    def __sub__(  # pyright: ignore[reportIncompatibleMethodOverride]
+    def __sub__(
         self, other: npt.NDArray[np.timedelta64]
     ) -> npt.NDArray[np.datetime64]: ...
     @overload
     def __eq__(self, other: Timestamp | datetime | np.datetime64) -> bool: ...  # type: ignore[overload-overlap] # pyright: ignore[reportOverlappingOverload]
     @overload
     def __eq__(self, other: TimestampSeries) -> Series[bool]: ...  # type: ignore[overload-overlap]
     @overload
```

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/_libs/tslibs/vectorized.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/_libs/tslibs/vectorized.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/_testing/__init__.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/_testing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/_typing.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/_typing.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -428,15 +428,15 @@
     def __iter__(self) -> Iterator[AnyStr_cov]: ...
     def fileno(self) -> int: ...
     def readline(self) -> AnyStr_cov: ...
     @property
     def closed(self) -> bool: ...
 
 class WriteExcelBuffer(WriteBuffer[bytes], Protocol):
-    def truncate(self, size: int | None = ...) -> int: ...
+    def truncate(self, size: int | None = ..., /) -> int: ...
 
 FilePath: TypeAlias = str | PathLike[str]
 
 _T_co = TypeVar("_T_co", covariant=True)
 
 class SequenceNotStr(Protocol[_T_co]):
     @overload
@@ -776,8 +776,11 @@
 )
 Frequency: TypeAlias = str | BaseOffset
 TimeUnit: TypeAlias = Literal["s", "ms", "us", "ns"]
 TimeGrouperOrigin: TypeAlias = (
     Timestamp | Literal["epoch", "start", "start_day", "end", "end_day"]
 )
 
+ExcelReadEngine: TypeAlias = Literal["xlrd", "openpyxl", "odf", "pyxlsb", "calamine"]
+ExcelWriteEngine: TypeAlias = Literal["openpyxl", "odf", "xlsxwriter"]
+
 __all__ = ["npt", "type_t"]
```

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/api/extensions/__init__.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/api/extensions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/api/types/__init__.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/api/types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/algorithms.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/algorithms.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from collections.abc import Sequence
 from typing import (
     Literal,
     overload,
 )
 
 import numpy as np
 from pandas import (
@@ -33,20 +32,20 @@
 @overload
 def unique(values: Index) -> np.ndarray: ...
 @overload
 def unique(values: Categorical) -> Categorical: ...
 @overload
 def unique(values: Series) -> np.ndarray | ExtensionArray: ...
 @overload
-def unique(values: np.ndarray | list) -> np.ndarray: ...
+def unique(values: np.ndarray) -> np.ndarray: ...
 @overload
 def unique(values: ExtensionArray) -> ExtensionArray: ...
 @overload
 def factorize(
-    values: Sequence | np.recarray,
+    values: np.ndarray,
     sort: bool = ...,
     use_na_sentinel: bool = ...,
     size_hint: int | None = ...,
 ) -> tuple[np.ndarray, np.ndarray]: ...
 @overload
 def factorize(
     values: Index | Series,
```

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/api.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/api.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/arraylike.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/arraylike.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/__init__.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/base.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/base.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -52,14 +52,18 @@
         allow_fill: bool = ...,
         fill_value=...,
     ) -> Self: ...
     def copy(self) -> Self: ...
     def view(self, dtype=...) -> Self | np.ndarray: ...
     def ravel(self, order=...) -> Self: ...
     def tolist(self) -> list: ...
+    def _reduce(
+        self, name: str, *, skipna: bool = ..., keepdims: bool = ..., **kwargs
+    ) -> object: ...
+    def _accumulate(self, name: str, *, skipna: bool = ..., **kwargs) -> Self: ...
 
 class ExtensionOpsMixin:
     @classmethod
     def _add_arithmetic_ops(cls) -> None: ...
     @classmethod
     def _add_comparison_ops(cls) -> None: ...
     @classmethod
```

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/boolean.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/boolean.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/categorical.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/categorical.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/datetimelike.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/datetimelike.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/datetimes.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/datetimes.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/integer.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/integer.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/interval.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/interval.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/masked.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/masked.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/numpy_.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/numpy_.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/period.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/period.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/sparse/accessor.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/sparse/accessor.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/sparse/array.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/sparse/array.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/string_.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/string_.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/arrays/timedeltas.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/arrays/timedeltas.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/base.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/base.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/common.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/common.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/computation/eval.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/computation/eval.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/computation/expr.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/computation/expr.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/computation/ops.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/computation/ops.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/computation/pytables.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/computation/pytables.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/computation/scope.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/computation/scope.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/config_init.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/config_init.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/construction.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/construction.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/dtypes/api.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/dtypes/api.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/dtypes/base.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/dtypes/base.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/dtypes/common.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/dtypes/common.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/dtypes/dtypes.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/dtypes/dtypes.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/dtypes/inference.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/dtypes/inference.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/dtypes/missing.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/dtypes/missing.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/frame.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/frame.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,19 @@
     Expanding,
     ExponentialMovingWindow,
 )
 from pandas.core.window.rolling import (
     Rolling,
     Window,
 )
-from typing_extensions import Self
+from typing_extensions import (
+    Never,
+    Self,
+    TypeAlias,
+)
 import xarray as xr
 
 from pandas._libs.lib import NoDefault
 from pandas._libs.missing import NAType
 from pandas._libs.tslibs import BaseOffset
 from pandas._libs.tslibs.nattype import NaTType
 from pandas._typing import (
@@ -108,14 +112,15 @@
     ReplaceMethod,
     Scalar,
     ScalarT,
     SeriesByT,
     SortKind,
     StataDateFormat,
     StorageOptions,
+    StrDtypeArg,
     StrLike,
     Suffixes,
     T as _T,
     TimestampConvention,
     TimeUnit,
     ValidationOptions,
     WriteBuffer,
@@ -258,31 +263,45 @@
     def axes(self) -> list[Index]: ...
     @property
     def shape(self) -> tuple[int, int]: ...
     @property
     def style(self) -> Styler: ...
     def items(self) -> Iterable[tuple[Hashable, Series]]: ...
     def iterrows(self) -> Iterable[tuple[Hashable, Series]]: ...
+    @overload
     def itertuples(
-        self, index: _bool = ..., name: _str | None = ...
+        self, index: _bool = ..., name: _str = ...
     ) -> Iterable[_PandasNamedTuple]: ...
+    @overload
+    def itertuples(
+        self, index: _bool = ..., name: None = None
+    ) -> Iterable[tuple[Any, ...]]: ...
     def __len__(self) -> int: ...
     @overload
     def dot(self, other: DataFrame | ArrayLike) -> DataFrame: ...
     @overload
     def dot(self, other: Series) -> Series: ...
     def __matmul__(self, other): ...
     def __rmatmul__(self, other): ...
+    @overload
     @classmethod
     def from_dict(
         cls,
         data: dict[Any, Any],
-        orient: Literal["columns", "index", "tight"] = ...,
-        dtype: _str = ...,
-        columns: list[_str] = ...,
+        orient: Literal["index"],
+        dtype: AstypeArg | None = ...,
+        columns: Axes | None = ...,
+    ) -> DataFrame: ...
+    @overload
+    @classmethod
+    def from_dict(
+        cls,
+        data: dict[Any, Any],
+        orient: Literal["columns", "tight"] = ...,
+        dtype: AstypeArg | None = ...,
     ) -> DataFrame: ...
     def to_numpy(
         self,
         dtype: npt.DTypeLike | None = ...,
         copy: bool = ...,
         na_value: Scalar = ...,
     ) -> np.ndarray: ...
@@ -595,18 +614,55 @@
     @overload
     def query(self, expr: _str, *, inplace: Literal[True], **kwargs) -> None: ...
     @overload
     def query(
         self, expr: _str, *, inplace: Literal[False] = ..., **kwargs
     ) -> DataFrame: ...
     def eval(self, expr: _str, *, inplace: _bool = ..., **kwargs): ...
+    AstypeArgExt: TypeAlias = (
+        AstypeArg
+        | Literal[
+            "number",
+            "datetime64",
+            "datetime",
+            "timedelta",
+            "timedelta64",
+            "datetimetz",
+            "datetime64[ns]",
+        ]
+    )
+    AstypeArgExtList: TypeAlias = AstypeArgExt | list[AstypeArgExt]
+    @overload
+    def select_dtypes(
+        self, include: StrDtypeArg, exclude: AstypeArgExtList | None = ...
+    ) -> Never: ...
+    @overload
+    def select_dtypes(
+        self, include: AstypeArgExtList | None, exclude: StrDtypeArg
+    ) -> Never: ...
+    @overload
+    def select_dtypes(self, exclude: StrDtypeArg) -> Never: ...
+    @overload
+    def select_dtypes(self, include: list[Never], exclude: list[Never]) -> Never: ...
+    @overload
+    def select_dtypes(
+        self,
+        include: AstypeArgExtList,
+        exclude: AstypeArgExtList | None = ...,
+    ) -> DataFrame: ...
+    @overload
     def select_dtypes(
         self,
-        include: _str | list[_str] | None = ...,
-        exclude: _str | list[_str] | None = ...,
+        include: AstypeArgExtList | None,
+        exclude: AstypeArgExtList,
+    ) -> DataFrame: ...
+    @overload
+    def select_dtypes(
+        self,
+        exclude: AstypeArgExtList,
     ) -> DataFrame: ...
     def insert(
         self,
         loc: int,
         column,
         value: Scalar | ListLikeU | None,
         allow_duplicates: _bool = ...,
@@ -1121,15 +1177,15 @@
         *,
         index: IndexLabel = ...,
         columns: IndexLabel = ...,
         values: IndexLabel = ...,
     ) -> DataFrame: ...
     def pivot_table(
         self,
-        values: _str | None = ...,
+        values: _str | None | Sequence[_str] = ...,
         index: _str | Grouper | Sequence | None = ...,
         columns: _str | Grouper | Sequence | None = ...,
         aggfunc=...,
         fill_value: Scalar | None = ...,
         margins: _bool = ...,
         dropna: _bool = ...,
         margins_name: _str = ...,
@@ -1773,15 +1829,21 @@
     ) -> Series: ...
     def last(self, offset) -> DataFrame: ...
     def last_valid_index(self) -> Scalar: ...
     def le(self, other, axis: Axis = ..., level: Level | None = ...) -> DataFrame: ...
     def lt(self, other, axis: Axis = ..., level: Level | None = ...) -> DataFrame: ...
     def mask(
         self,
-        cond: Series | DataFrame | np.ndarray,
+        cond: (
+            Series
+            | DataFrame
+            | np.ndarray
+            | Callable[[DataFrame], DataFrame]
+            | Callable[[Any], _bool]
+        ),
         other=...,
         *,
         inplace: _bool = ...,
         axis: Axis | None = ...,
         level: Level | None = ...,
         try_cast: _bool = ...,
     ) -> DataFrame: ...
```

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/generic.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/generic.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/groupby/generic.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/groupby/generic.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
     def apply(
         self,
         func: Callable[[DataFrame], Series | DataFrame],
         *args,
         **kwargs,
     ) -> DataFrame: ...
     @overload
-    def apply(  # pyright: ignore[reportOverlappingOverload,reportIncompatibleMethodOverride]
+    def apply(  # pyright: ignore[reportOverlappingOverload]
         self,
         func: Callable[[Iterable], float],
         *args,
         **kwargs,
     ) -> DataFrame: ...
     # error: overload 1 overlaps overload 2 because of different return types
     @overload
```

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/groupby/groupby.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/groupby/groupby.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/groupby/grouper.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/groupby/grouper.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/groupby/indexing.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/groupby/indexing.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/groupby/ops.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/groupby/ops.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/indexers.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/indexers.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/accessors.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/accessors.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/api.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/api.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/base.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/base.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/category.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/category.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/datetimelike.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/datetimelike.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/datetimes.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/datetimes.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/interval.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/interval.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/multi.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/multi.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/period.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/period.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/range.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/range.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/indexes/timedeltas.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/indexes/timedeltas.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     def __new__(
         cls,
         data: (
             AnyArrayLike
             | list[str]
             | Sequence[dt.timedelta | Timedelta | np.timedelta64 | float]
         ) = ...,
-        unit: Literal["D", "h", "m", "s", "ms", "us", "ns"] = ...,
         freq: str | BaseOffset = ...,
         closed: object = ...,
         dtype: Literal["<m8[ns]"] = ...,
         copy: bool = ...,
         name: str = ...,
     ) -> Self: ...
     # various ignores needed for mypy, as we do want to restrict what can be used in
```

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/indexing.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/indexing.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/interchange/dataframe_protocol.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/interchange/dataframe_protocol.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/ops/array_ops.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/ops/array_ops.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/ops/mask_ops.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/ops/mask_ops.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/resample.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/resample.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/reshape/api.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/reshape/api.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/reshape/concat.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/reshape/concat.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -28,85 +28,85 @@
     objs: Iterable[DataFrame] | Mapping[HashableT1, DataFrame],
     *,
     axis: Axis = ...,
     join: Literal["inner", "outer"] = ...,
     ignore_index: bool = ...,
     keys: Iterable[HashableT2] = ...,
     levels: Sequence[list[HashableT3] | tuple[HashableT3, ...]] = ...,
-    names: list[HashableT4] = ...,
+    names: list[HashableT4] | None = ...,
     verify_integrity: bool = ...,
     sort: bool = ...,
     copy: bool = ...,
 ) -> DataFrame: ...
 @overload
 def concat(  # type: ignore[overload-overlap] # pyright: ignore[reportOverlappingOverload]
     objs: Iterable[Series] | Mapping[HashableT1, Series],
     *,
     axis: AxisIndex = ...,
     join: Literal["inner", "outer"] = ...,
     ignore_index: bool = ...,
     keys: Iterable[HashableT2] = ...,
     levels: Sequence[list[HashableT3] | tuple[HashableT3, ...]] = ...,
-    names: list[HashableT4] = ...,
+    names: list[HashableT4] | None = ...,
     verify_integrity: bool = ...,
     sort: bool = ...,
     copy: bool = ...,
 ) -> Series: ...
 @overload
 def concat(  # type: ignore[overload-overlap] # pyright: ignore[reportOverlappingOverload]
     objs: Iterable[Series | DataFrame] | Mapping[HashableT1, Series | DataFrame],
     *,
     axis: Axis = ...,
     join: Literal["inner", "outer"] = ...,
     ignore_index: bool = ...,
     keys: Iterable[HashableT2] = ...,
     levels: Sequence[list[HashableT3] | tuple[HashableT3, ...]] = ...,
-    names: list[HashableT4] = ...,
+    names: list[HashableT4] | None = ...,
     verify_integrity: bool = ...,
     sort: bool = ...,
     copy: bool = ...,
 ) -> DataFrame: ...
 @overload
 def concat(
     objs: Iterable[None] | Mapping[HashableT1, None],
     *,
     axis: Axis = ...,
     join: Literal["inner", "outer"] = ...,
     ignore_index: bool = ...,
     keys: Iterable[HashableT2] = ...,
     levels: Sequence[list[HashableT3] | tuple[HashableT3, ...]] = ...,
-    names: list[HashableT4] = ...,
+    names: list[HashableT4] | None = ...,
     verify_integrity: bool = ...,
     sort: bool = ...,
     copy: bool = ...,
 ) -> Never: ...
 @overload
 def concat(  # type: ignore[overload-overlap]
     objs: Iterable[DataFrame | None] | Mapping[HashableT1, DataFrame | None],
     *,
     axis: Axis = ...,
     join: Literal["inner", "outer"] = ...,
     ignore_index: bool = ...,
     keys: Iterable[HashableT2] = ...,
     levels: Sequence[list[HashableT3] | tuple[HashableT3, ...]] = ...,
-    names: list[HashableT4] = ...,
+    names: list[HashableT4] | None = ...,
     verify_integrity: bool = ...,
     sort: bool = ...,
     copy: bool = ...,
 ) -> DataFrame: ...
 @overload
 def concat(  # type: ignore[overload-overlap]
     objs: Iterable[Series | None] | Mapping[HashableT1, Series | None],
     *,
     axis: AxisIndex = ...,
     join: Literal["inner", "outer"] = ...,
     ignore_index: bool = ...,
     keys: Iterable[HashableT2] = ...,
     levels: Sequence[list[HashableT3] | tuple[HashableT3, ...]] = ...,
-    names: list[HashableT4] = ...,
+    names: list[HashableT4] | None = ...,
     verify_integrity: bool = ...,
     sort: bool = ...,
     copy: bool = ...,
 ) -> Series: ...
 @overload
 def concat(
     objs: (
@@ -115,15 +115,15 @@
     ),
     *,
     axis: Axis = ...,
     join: Literal["inner", "outer"] = ...,
     ignore_index: bool = ...,
     keys: Iterable[HashableT2] = ...,
     levels: Sequence[list[HashableT3] | tuple[HashableT3, ...]] = ...,
-    names: list[HashableT4] = ...,
+    names: list[HashableT4] | None = ...,
     verify_integrity: bool = ...,
     sort: bool = ...,
     copy: bool = ...,
 ) -> DataFrame: ...
 
 # Including either of the next 2 overloads causes mypy to complain about
 # test_pandas.py:test_types_concat() in assert_type(pd.concat([s, s2]), "pd.Series")
```

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/reshape/encoding.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/reshape/encoding.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/reshape/melt.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/reshape/melt.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/reshape/merge.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/reshape/merge.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     right_on: Label | list[HashableT] | AnyArrayLike | None = ...,
     left_index: bool = ...,
     right_index: bool = ...,
     sort: bool = ...,
     suffixes: (
         list[str | None] | tuple[str, str] | tuple[None, str] | tuple[str, None]
     ) = ...,
-    copy: bool = ...,
     indicator: bool | str = ...,
     validate: ValidationOptions = ...,
 ) -> DataFrame: ...
 @overload
 def merge_ordered(
     left: DataFrame,
     right: DataFrame,
```

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/reshape/pivot.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/reshape/pivot.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/reshape/tile.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/reshape/tile.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/series.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/series.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,15 @@
         idx: (
             MaskType
             | Index
             | Sequence[float]
             | list[str]
             | slice
             | _IndexSliceTuple
+            | Sequence[_IndexSliceTuple]
             | Callable
         ),
         # _IndexSliceTuple is when having a tuple that includes a slice.  Could just
         # be s.loc[1, :], or s.loc[pd.IndexSlice[1, :]]
     ) -> Series[S1]: ...
     @overload
     def __setitem__(
@@ -230,18 +231,19 @@
     __hash__: ClassVar[None]
 
     @overload
     def __new__(  # type: ignore[overload-overlap]
         cls,
         data: (
             DatetimeIndex
-            | Sequence[np.datetime64 | datetime]
-            | dict[HashableT1, np.datetime64 | datetime]
+            | Sequence[np.datetime64 | datetime | date]
+            | dict[HashableT1, np.datetime64 | datetime | date]
             | np.datetime64
             | datetime
+            | date
         ),
         index: Axes | None = ...,
         *,
         dtype: TimestampDtypeArg = ...,
         name: Hashable = ...,
         copy: bool = ...,
     ) -> TimestampSeries: ...
@@ -254,15 +256,15 @@
         dtype: TimestampDtypeArg,
         name: Hashable = ...,
         copy: bool = ...,
     ) -> TimestampSeries: ...
     @overload
     def __new__(  # type: ignore[overload-overlap]
         cls,
-        data: PeriodIndex,
+        data: PeriodIndex | Sequence[Period],
         index: Axes | None = ...,
         *,
         dtype: PeriodDtype = ...,
         name: Hashable = ...,
         copy: bool = ...,
     ) -> PeriodSeries: ...
     @overload
@@ -743,15 +745,26 @@
         other: Series[S1],
         method: Literal["pearson", "kendall", "spearman"] = ...,
         min_periods: int = ...,
     ) -> float: ...
     def cov(
         self, other: Series[S1], min_periods: int | None = ..., ddof: int = ...
     ) -> float: ...
-    def diff(self, periods: int = ...) -> Series[S1]: ...
+    @overload
+    def diff(self: Series[_bool], periods: int = ...) -> Series[type[object]]: ...  # type: ignore[overload-overlap]
+    @overload
+    def diff(self: Series[complex], periods: int = ...) -> Series[complex]: ...  # type: ignore[overload-overlap]
+    @overload
+    def diff(self: Series[bytes], periods: int = ...) -> Never: ...
+    @overload
+    def diff(self: Series[type], periods: int = ...) -> Never: ...
+    @overload
+    def diff(self: Series[str], periods: int = ...) -> Never: ...
+    @overload
+    def diff(self, periods: int = ...) -> Series[float]: ...
     def autocorr(self, lag: int = ...) -> float: ...
     @overload
     def dot(self, other: Series[S1]) -> Scalar: ...
     @overload
     def dot(self, other: DataFrame) -> Series[S1]: ...
     @overload
     def dot(
@@ -935,15 +948,17 @@
         axis: AxisIndex = ...,
         *args,
         **kwargs,
     ) -> DataFrame: ...
     @overload
     def apply(
         self,
-        func: Callable[..., Scalar | Sequence | set | Mapping | NAType | None],
+        func: Callable[
+            ..., Scalar | Sequence | set | Mapping | NAType | frozenset | None
+        ],
         convertDType: _bool = ...,
         args: tuple = ...,
         **kwds,
     ) -> Series: ...
     @overload
     def apply(
         self,
@@ -1414,15 +1429,21 @@
         inplace: _bool = ...,
         axis: AxisIndex | None = ...,
         level: Level | None = ...,
         try_cast: _bool = ...,
     ) -> Series[S1]: ...
     def mask(
         self,
-        cond: MaskType,
+        cond: (
+            Series[S1]
+            | Series[_bool]
+            | np.ndarray
+            | Callable[[Series[S1]], Series[bool]]
+            | Callable[[S1], bool]
+        ),
         other: Scalar | Series[S1] | DataFrame | Callable | NAType | None = ...,
         *,
         inplace: _bool = ...,
         axis: AxisIndex | None = ...,
         level: Level | None = ...,
         try_cast: _bool = ...,
     ) -> Series[S1]: ...
@@ -1504,24 +1525,24 @@
         self, other: int | np_ndarray_anyint | Series[int]
     ) -> Series[int]: ...
     # def __array__(self, dtype: Optional[_bool] = ...) -> _np_ndarray
     def __div__(self, other: num | _ListLike | Series[S1]) -> Series[S1]: ...
     def __eq__(self, other: object) -> Series[_bool]: ...  # type: ignore[override] # pyright: ignore[reportIncompatibleMethodOverride]
     def __floordiv__(self, other: num | _ListLike | Series[S1]) -> Series[int]: ...
     def __ge__(  # type: ignore[override] # pyright: ignore[reportIncompatibleMethodOverride]
-        self, other: S1 | _ListLike | Series[S1] | datetime | timedelta
+        self, other: S1 | _ListLike | Series[S1] | datetime | timedelta | date
     ) -> Series[_bool]: ...
     def __gt__(  # type: ignore[override] # pyright: ignore[reportIncompatibleMethodOverride]
-        self, other: S1 | _ListLike | Series[S1] | datetime | timedelta
+        self, other: S1 | _ListLike | Series[S1] | datetime | timedelta | date
     ) -> Series[_bool]: ...
     def __le__(  # type: ignore[override] # pyright: ignore[reportIncompatibleMethodOverride]
-        self, other: S1 | _ListLike | Series[S1] | datetime | timedelta
+        self, other: S1 | _ListLike | Series[S1] | datetime | timedelta | date
     ) -> Series[_bool]: ...
     def __lt__(  # type: ignore[override] # pyright: ignore[reportIncompatibleMethodOverride]
-        self, other: S1 | _ListLike | Series[S1] | datetime | timedelta
+        self, other: S1 | _ListLike | Series[S1] | datetime | timedelta | date
     ) -> Series[_bool]: ...
     @overload
     def __mul__(
         self, other: timedelta | Timedelta | TimedeltaSeries | np.timedelta64
     ) -> TimedeltaSeries: ...
     @overload
     def __mul__(self, other: num | _ListLike | Series) -> Series: ...
@@ -2068,14 +2089,15 @@
         axis: AxisIndex | None = ...,
         skipna: _bool | None = ...,
         level: None = ...,
         ddof: int = ...,
         numeric_only: _bool = ...,
         **kwargs,
     ) -> Timedelta: ...
+    def diff(self, periods: int = ...) -> TimedeltaSeries: ...  # type: ignore[override] # pyright: ignore[reportIncompatibleMethodOverride]
 
 class TimedeltaSeries(Series[Timedelta]):
     # ignores needed because of mypy
     @overload  # type: ignore[override]
     def __add__(self, other: Period) -> PeriodSeries: ...
     @overload
     def __add__(
@@ -2164,24 +2186,27 @@
         axis: AxisIndex | None = ...,
         skipna: _bool | None = ...,
         level: None = ...,
         ddof: int = ...,
         numeric_only: _bool = ...,
         **kwargs,
     ) -> Timedelta: ...
+    def diff(self, periods: int = ...) -> TimedeltaSeries: ...  # type: ignore[override] # pyright: ignore[reportIncompatibleMethodOverride]
 
 class PeriodSeries(Series[Period]):
     @property
     def dt(self) -> PeriodProperties: ...  # type: ignore[override] # pyright: ignore[reportIncompatibleMethodOverride]
     def __sub__(self, other: PeriodSeries) -> OffsetSeries: ...  # type: ignore[override] # pyright: ignore[reportIncompatibleMethodOverride]
+    def diff(self, periods: int = ...) -> OffsetSeries: ...  # type: ignore[override] # pyright: ignore[reportIncompatibleMethodOverride]
 
 class OffsetSeries(Series[BaseOffset]):
     @overload  # type: ignore[override]
     def __radd__(self, other: Period) -> PeriodSeries: ...
     @overload
     def __radd__(  # pyright: ignore[reportIncompatibleMethodOverride]
         self, other: BaseOffset
     ) -> OffsetSeries: ...
 
 class IntervalSeries(Series[Interval[_OrderableT]], Generic[_OrderableT]):
     @property
     def array(self) -> IntervalArray: ...
+    def diff(self, periods: int = ...) -> Never: ...
```

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/strings.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/strings.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/tools/datetimes.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/tools/datetimes.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -78,17 +78,17 @@
     infer_datetime_format: bool = ...,
     origin: Literal["julian", "unix"] | TimestampConvertibleTypes = ...,
     cache: bool = ...,
 ) -> TimestampSeries: ...
 @overload
 def to_datetime(
     arg: (
-        Sequence[float | datetime]
+        Sequence[float | date]
         | list[str]
-        | tuple[float | str | datetime, ...]
+        | tuple[float | str | date, ...]
         | npt.NDArray[np.datetime64]
         | npt.NDArray[np.str_]
         | npt.NDArray[np.int_]
         | Index
         | ExtensionArray
     ),
     errors: RaiseCoerce = ...,
```

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/tools/numeric.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/tools/numeric.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/tools/timedeltas.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/tools/timedeltas.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/window/ewm.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/window/ewm.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/core/window/rolling.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/core/window/rolling.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/errors/__init__.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/errors/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/io/api.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/io/api.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/io/clipboards.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/io/clipboards.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/io/excel/_base.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/io/excel/_base.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from typing_extensions import Self
 from xlrd.book import Book
 
 from pandas._libs.lib import NoDefault
 from pandas._typing import (
     Dtype,
     DtypeBackend,
+    ExcelReadEngine,
+    ExcelWriteEngine,
     FilePath,
     IntStrT,
     ListLikeHashable,
     ReadBuffer,
     StorageOptions,
     UsecolsArgType,
     WriteExcelBuffer,
@@ -43,18 +45,18 @@
         | OpenDocument
         | pyxlsb.workbook.Workbook
     ),
     sheet_name: list[IntStrT],
     *,
     header: int | Sequence[int] | None = ...,
     names: ListLikeHashable | None = ...,
-    index_col: int | Sequence[int] | None = ...,
+    index_col: int | Sequence[int] | str | None = ...,
     usecols: str | UsecolsArgType = ...,
     dtype: str | Dtype | Mapping[str, str | Dtype] | None = ...,
-    engine: Literal["xlrd", "openpyxl", "odf", "pyxlsb"] | None = ...,
+    engine: ExcelReadEngine | None = ...,
     converters: Mapping[int | str, Callable[[object], object]] | None = ...,
     true_values: Iterable[Hashable] | None = ...,
     false_values: Iterable[Hashable] | None = ...,
     skiprows: int | Sequence[int] | Callable[[object], bool] | None = ...,
     nrows: int | None = ...,
     na_values: Sequence[str] | dict[str | int, Sequence[str]] = ...,
     keep_default_na: bool = ...,
@@ -85,18 +87,18 @@
         | OpenDocument
         | pyxlsb.workbook.Workbook
     ),
     sheet_name: None,
     *,
     header: int | Sequence[int] | None = ...,
     names: ListLikeHashable | None = ...,
-    index_col: int | Sequence[int] | None = ...,
+    index_col: int | Sequence[int] | str | None = ...,
     usecols: str | UsecolsArgType = ...,
     dtype: str | Dtype | Mapping[str, str | Dtype] | None = ...,
-    engine: Literal["xlrd", "openpyxl", "odf", "pyxlsb"] | None = ...,
+    engine: ExcelReadEngine | None = ...,
     converters: Mapping[int | str, Callable[[object], object]] | None = ...,
     true_values: Iterable[Hashable] | None = ...,
     false_values: Iterable[Hashable] | None = ...,
     skiprows: int | Sequence[int] | Callable[[object], bool] | None = ...,
     nrows: int | None = ...,
     na_values: Sequence[str] | dict[str | int, Sequence[str]] = ...,
     keep_default_na: bool = ...,
@@ -128,18 +130,18 @@
         | OpenDocument
         | pyxlsb.workbook.Workbook
     ),
     sheet_name: list[int | str],
     *,
     header: int | Sequence[int] | None = ...,
     names: ListLikeHashable | None = ...,
-    index_col: int | Sequence[int] | None = ...,
+    index_col: int | Sequence[int] | str | None = ...,
     usecols: str | UsecolsArgType = ...,
     dtype: str | Dtype | Mapping[str, str | Dtype] | None = ...,
-    engine: Literal["xlrd", "openpyxl", "odf", "pyxlsb"] | None = ...,
+    engine: ExcelReadEngine | None = ...,
     converters: Mapping[int | str, Callable[[object], object]] | None = ...,
     true_values: Iterable[Hashable] | None = ...,
     false_values: Iterable[Hashable] | None = ...,
     skiprows: int | Sequence[int] | Callable[[object], bool] | None = ...,
     nrows: int | None = ...,
     na_values: Sequence[str] | dict[str | int, Sequence[str]] = ...,
     keep_default_na: bool = ...,
@@ -170,18 +172,18 @@
         | OpenDocument
         | pyxlsb.workbook.Workbook
     ),
     sheet_name: int | str = ...,
     *,
     header: int | Sequence[int] | None = ...,
     names: ListLikeHashable | None = ...,
-    index_col: int | Sequence[int] | None = ...,
+    index_col: int | Sequence[int] | str | None = ...,
     usecols: str | UsecolsArgType = ...,
     dtype: str | Dtype | Mapping[str, str | Dtype] | None = ...,
-    engine: Literal["xlrd", "openpyxl", "odf", "pyxlsb"] | None = ...,
+    engine: ExcelReadEngine | None = ...,
     converters: Mapping[int | str, Callable[[object], object]] | None = ...,
     true_values: Iterable[Hashable] | None = ...,
     false_values: Iterable[Hashable] | None = ...,
     skiprows: int | Sequence[int] | Callable[[object], bool] | None = ...,
     nrows: int | None = ...,
     na_values: Sequence[str] | dict[str | int, Sequence[str]] = ...,
     keep_default_na: bool = ...,
@@ -202,26 +204,26 @@
     dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> DataFrame: ...
 
 class ExcelWriter:
     def __init__(
         self,
         path: FilePath | WriteExcelBuffer | ExcelWriter,
-        engine: Literal["auto", "openpyxl", "odf", "xlsxwriter"] | None = ...,
+        engine: ExcelWriteEngine | Literal["auto"] | None = ...,
         date_format: str | None = ...,
         datetime_format: str | None = ...,
         mode: Literal["w", "a"] = ...,
         storage_options: StorageOptions = ...,
         if_sheet_exists: Literal["error", "new", "replace", "overlay"] | None = ...,
         engine_kwargs: dict[str, Any] | None = ...,
     ) -> None: ...
     @property
     def supported_extensions(self) -> tuple[str, ...]: ...
     @property
-    def engine(self) -> Literal["openpyxl", "odf", "xlsxwriter"]: ...
+    def engine(self) -> ExcelWriteEngine: ...
     @property
     def sheets(self) -> dict[str, Any]: ...
     @property
     def book(self) -> Workbook | OpenDocument: ...
     @property
     def date_format(self) -> str: ...
     @property
```

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/io/formats/style.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/io/formats/style.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from collections.abc import (
     Callable,
     Sequence,
 )
 from typing import (
     Any,
     Literal,
+    Protocol,
     overload,
 )
 
 from matplotlib.colors import Colormap
 import numpy as np
 from pandas.core.frame import DataFrame
 from pandas.core.series import Series
@@ -36,14 +37,24 @@
     CSSStyles,
     ExtFormatter,
     StyleExportDict,
     StylerRenderer,
     Subset,
 )
 
+class _SeriesFunc(Protocol):
+    def __call__(
+        self, series: Series, /, *args: Any, **kwargs: Any
+    ) -> list | Series: ...
+
+class _DataFrameFunc(Protocol):
+    def __call__(
+        self, series: DataFrame, /, *args: Any, **kwargs: Any
+    ) -> npt.NDArray | DataFrame: ...
+
 class Styler(StylerRenderer):
     def __init__(
         self,
         data: DataFrame | Series,
         precision: int | None = ...,
         table_styles: CSSStyles | None = ...,
         uuid: str | None = ...,
@@ -194,34 +205,41 @@
     def set_td_classes(self, classes: DataFrame) -> Styler: ...
     def __copy__(self) -> Styler: ...
     def __deepcopy__(self, memo) -> Styler: ...
     def clear(self) -> None: ...
     @overload
     def apply(
         self,
-        func: Callable[[Series], list | Series],
+        func: _SeriesFunc | Callable[[Series], list | Series],
         axis: Axis = ...,
         subset: Subset | None = ...,
         **kwargs: Any,
     ) -> Styler: ...
     @overload
     def apply(
         self,
-        func: Callable[[DataFrame], npt.NDArray | DataFrame],
+        func: _DataFrameFunc | Callable[[DataFrame], npt.NDArray | DataFrame],
         axis: None,
         subset: Subset | None = ...,
         **kwargs: Any,
     ) -> Styler: ...
     def apply_index(
         self,
         func: Callable[[Series], npt.NDArray[np.str_] | list[str] | Series[str]],
         axis: Axis = ...,
         level: Level | list[Level] | None = ...,
         **kwargs: Any,
     ) -> Styler: ...
+    def map_index(
+        self,
+        func: Callable[[Scalar], str | None],
+        axis: Axis = ...,
+        level: Level | list[Level] | None = ...,
+        **kwargs,
+    ) -> Styler: ...
     def set_table_attributes(self, attributes: str) -> Styler: ...
     def export(self) -> StyleExportDict: ...
     def use(self, styles: StyleExportDict) -> Styler: ...
     def set_uuid(self, uuid: str) -> Styler: ...
     def set_caption(self, caption: str | tuple[str, str]) -> Styler: ...
     def set_sticky(
         self,
```

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/io/formats/style_render.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/io/formats/style_render.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/io/gbq.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/io/gbq.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/io/html.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/io/html.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/io/json/_json.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/io/json/_json.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/io/parsers/readers.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/io/parsers/readers.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/io/pickle.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/io/pickle.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/io/pytables.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/io/pytables.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/io/sas/sasreader.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/io/sas/sasreader.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/io/sql.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/io/sql.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/io/stata.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/io/stata.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/io/xml.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/io/xml.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/plotting/__init__.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/plotting/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/plotting/_core.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/plotting/_core.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/plotting/_misc.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/plotting/_misc.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/tseries/holiday.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/tseries/holiday.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/tseries/offsets.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/tseries/offsets.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/util/_validators.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/util/_validators.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pandas-stubs/util/version/__init__.pyi` & `pandas_stubs-2.2.2.240514/pandas-stubs/util/version/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.2.1.240316/pyproject.toml` & `pandas_stubs-2.2.2.240514/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandas-stubs"
-version = "2.2.1.240316"
+version = "2.2.2.240514"
 description = "Type annotations for pandas"
 authors = ["The Pandas Development Team <pandas-dev@python.org>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://pandas.pydata.org"
 repository = "https://github.com/pandas-dev/pandas-stubs"
 classifiers = [
@@ -31,43 +31,44 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 types-pytz = ">= 2022.1.1"
 numpy = { version = ">=1.26.0", python = "<3.13" }
 
 [tool.poetry.group.dev.dependencies]
-mypy = "1.9.0"
-pandas = "2.2.1"
+mypy = "1.10.0"
+pandas = "2.2.2"
 pyarrow = ">=10.0.1"
 pytest = ">=7.1.2"
-pyright = ">=1.1.354"
+pyright = ">=1.1.362"
 poethepoet = ">=0.16.5"
 loguru = ">=0.6.0"
 typing-extensions = ">=4.4.0"
 matplotlib = ">=3.5.1"
 pre-commit = ">=2.19.0"
 black = ">=23.3.0"
 isort = ">=5.12.0"
 openpyxl = ">=3.0.10"
 # for tables, MacOS gives random CI failures on 3.9.2
-tables = { version = "==3.9.1",  python = "<4"}  # 3.8.0 depends on blosc2 which caps python to <4
+tables = { version = "==3.9.2",  python = "<4"}  # 3.8.0 depends on blosc2 which caps python to <4
 lxml = ">=4.9.1"
 pyreadstat = ">=1.2.0"
 xlrd = ">=2.0.1"
 xlsxwriter = ">=3.0.3"
 pyxlsb = ">=1.0.10"
 odfpy = ">=1.4.1"
 xarray = ">=22.6.0"
 tabulate = ">=0.8.10"
 jinja2 = ">=3.1"
 scipy = { version = ">=1.9.1", python = "<3.13" }
 SQLAlchemy = ">=2.0.12"
 types-python-dateutil = ">=2.8.19"
 beautifulsoup4 = ">=4.12.2"
 html5lib = ">=1.1"
+python-calamine = "0.2.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poe.tasks.test_all]
 help = "Run all tests"
```

### Comparing `pandas_stubs-2.2.1.240316/README.md` & `pandas_stubs-2.2.2.240514/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -153,12 +153,19 @@
 
 ## Getting help
 
 Ask questions and report issues on the [pandas-stubs repository](https://github.com/pandas-dev/pandas-stubs/issues).  
 
 ## Discussion and Development
 
-Most development discussions take place on GitHub in the [pandas-stubs repository](https://github.com/pandas-dev/pandas-stubs/). Further, the [pandas-dev mailing list](https://mail.python.org/mailman/listinfo/pandas-dev) can also be used for specialized discussions or design issues, and a [Gitter channel](https://gitter.im/pydata/pandas) is available for quick development related questions.
+Most development discussions take place on GitHub in the [pandas-stubs repository](https://github.com/pandas-dev/pandas-stubs/).
+
+Further, the [pandas-dev mailing list](https://mail.python.org/mailman/listinfo/pandas-dev) can also be used for specialized discussions or design issues, and a [Slack channel](https://pandas.pydata.org/docs/dev/development/community.html?highlight=slack#community-slack) is available for quick development related questions.
+
+There are also frequent [community meetings](https://pandas.pydata.org/docs/dev/development/community.html#community-meeting) for project maintainers open to the community as well as monthly [new contributor meetings](https://pandas.pydata.org/docs/dev/development/community.html#new-contributor-meeting) to help support new contributors.
+
+Additional information on the communication channels can be found on the [contributor community](https://pandas.pydata.org/docs/development/community.html) page.
+
 
 ## Contributing to pandas-stubs
 
 All contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome.  See <https://github.com/pandas-dev/pandas-stubs/tree/main/docs/> for instructions.
```

### Comparing `pandas_stubs-2.2.1.240316/PKG-INFO` & `pandas_stubs-2.2.2.240514/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-stubs
-Version: 2.2.1.240316
+Version: 2.2.2.240514
 Summary: Type annotations for pandas
 Home-page: https://pandas.pydata.org
 License: BSD-3-Clause
 Author: The Pandas Development Team
 Author-email: pandas-dev@python.org
 Requires-Python: >=3.9
 Classifier: Development Status :: 5 - Production/Stable
@@ -182,13 +182,20 @@
 
 ## Getting help
 
 Ask questions and report issues on the [pandas-stubs repository](https://github.com/pandas-dev/pandas-stubs/issues).  
 
 ## Discussion and Development
 
-Most development discussions take place on GitHub in the [pandas-stubs repository](https://github.com/pandas-dev/pandas-stubs/). Further, the [pandas-dev mailing list](https://mail.python.org/mailman/listinfo/pandas-dev) can also be used for specialized discussions or design issues, and a [Gitter channel](https://gitter.im/pydata/pandas) is available for quick development related questions.
+Most development discussions take place on GitHub in the [pandas-stubs repository](https://github.com/pandas-dev/pandas-stubs/).
+
+Further, the [pandas-dev mailing list](https://mail.python.org/mailman/listinfo/pandas-dev) can also be used for specialized discussions or design issues, and a [Slack channel](https://pandas.pydata.org/docs/dev/development/community.html?highlight=slack#community-slack) is available for quick development related questions.
+
+There are also frequent [community meetings](https://pandas.pydata.org/docs/dev/development/community.html#community-meeting) for project maintainers open to the community as well as monthly [new contributor meetings](https://pandas.pydata.org/docs/dev/development/community.html#new-contributor-meeting) to help support new contributors.
+
+Additional information on the communication channels can be found on the [contributor community](https://pandas.pydata.org/docs/development/community.html) page.
+
 
 ## Contributing to pandas-stubs
 
 All contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome.  See <https://github.com/pandas-dev/pandas-stubs/tree/main/docs/> for instructions.
```

