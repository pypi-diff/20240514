# Comparing `tmp/atap_corpus_loader-1.4.0.tar.gz` & `tmp/atap_corpus_loader-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atap_corpus_loader-1.4.0.tar", max compression
+gzip compressed data, was "atap_corpus_loader-1.5.0.tar", max compression
```

## Comparing `atap_corpus_loader-1.4.0.tar` & `atap_corpus_loader-1.5.0.tar`

### file list

```diff
@@ -1,51 +1,55 @@
--rw-r--r--   0        0        0     1091 2023-12-21 02:04:16.054274 atap_corpus_loader-1.4.0/LICENSE
--rw-r--r--   0        0        0     1121 2024-03-26 05:34:13.109832 atap_corpus_loader-1.4.0/README.md
--rw-r--r--   0        0        0     2893 2024-04-10 05:12:13.211543 atap_corpus_loader-1.4.0/atap_corpus_loader/CorpusLoader.py
--rw-r--r--   0        0        0       56 2024-04-10 05:17:32.850808 atap_corpus_loader-1.4.0/atap_corpus_loader/__init__.py
--rw-r--r--   0        0        0    15161 2024-04-10 05:06:31.912428 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/Controller.py
--rw-r--r--   0        0        0     3726 2024-04-04 00:22:30.044441 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/CorpusExportService.py
--rw-r--r--   0        0        0    10879 2024-04-03 02:16:08.621920 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/FileLoaderService.py
--rw-r--r--   0        0        0      120 2024-04-10 03:12:40.044309 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/OniAPIService.py
--rw-r--r--   0        0        0       35 2024-01-31 04:39:45.157711 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/__init__.py
--rw-r--r--   0        0        0      869 2024-03-26 23:51:50.596436 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/data_objects/CorpusHeader.py
--rw-r--r--   0        0        0      269 2024-02-07 03:45:55.625849 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/data_objects/DataType.py
--rw-r--r--   0        0        0    10450 2024-04-03 04:03:28.002110 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/data_objects/FileReference.py
--rw-r--r--   0        0        0     4113 2024-04-01 23:58:39.235829 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/data_objects/UniqueNameCorpora.py
--rw-r--r--   0        0        0      556 2024-04-02 01:55:47.521647 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/data_objects/ViewCorpusInfo.py
--rw-r--r--   0        0        0      243 2024-03-26 05:34:13.113505 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/data_objects/__init__.py
--rw-r--r--   0        0        0       42 2024-01-31 04:39:45.159548 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/FileLoadError.py
--rw-r--r--   0        0        0     2854 2024-04-03 01:49:20.162871 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/FileLoaderFactory.py
--rw-r--r--   0        0        0     2333 2024-02-01 00:33:21.789787 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/FileLoaderStrategy.py
--rw-r--r--   0        0        0      141 2024-01-31 04:39:45.160266 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/__init__.py
--rw-r--r--   0        0        0     1258 2024-04-03 00:34:17.993483 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/CSVLoaderStrategy.py
--rw-r--r--   0        0        0     1388 2024-04-03 01:49:20.163247 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/DOCXLoaderStrategy.py
--rw-r--r--   0        0        0     1295 2024-03-26 23:51:50.585036 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/ODSLoaderStrategy.py
--rw-r--r--   0        0        0     1546 2024-04-04 00:22:30.045254 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/ODTLoaderStrategy.py
--rw-r--r--   0        0        0     2120 2024-03-26 23:51:50.591361 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/RLoaderStrategy.py
--rw-r--r--   0        0        0     1278 2024-04-03 00:15:00.851696 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/TSVLoaderStrategy.py
--rw-r--r--   0        0        0     1271 2024-04-03 01:49:20.163973 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/TXTLoaderStrategy.py
--rw-r--r--   0        0        0     1253 2024-04-03 00:15:00.852579 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/XLSXLoaderStrategy.py
--rw-r--r--   0        0        0     1644 2024-04-03 01:49:20.164171 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/XMLLoaderStrategy.py
--rw-r--r--   0        0        0      441 2024-04-03 01:49:20.164466 atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/__init__.py
--rw-r--r--   0        0        0     2394 2024-04-10 03:12:40.044796 atap_corpus_loader-1.4.0/atap_corpus_loader/view/ViewWrapperWidget.py
--rw-r--r--   0        0        0      108 2024-01-31 04:39:45.163251 atap_corpus_loader-1.4.0/atap_corpus_loader/view/__init__.py
--rw-r--r--   0        0        0      908 2024-03-26 05:34:13.115036 atap_corpus_loader-1.4.0/atap_corpus_loader/view/gui/AbstractWidget.py
--rw-r--r--   0        0        0     5745 2024-04-10 05:00:40.159485 atap_corpus_loader-1.4.0/atap_corpus_loader/view/gui/CorpusInfoWidget.py
--rw-r--r--   0        0        0     6626 2024-04-04 03:08:33.397254 atap_corpus_loader-1.4.0/atap_corpus_loader/view/gui/FileLoaderWidget.py
--rw-r--r--   0        0        0     5339 2024-03-28 00:37:16.585867 atap_corpus_loader-1.4.0/atap_corpus_loader/view/gui/FileSelectorWidget.py
--rw-r--r--   0        0        0     8527 2024-03-28 03:29:31.348900 atap_corpus_loader-1.4.0/atap_corpus_loader/view/gui/MetaEditorWidget.py
--rw-r--r--   0        0        0      368 2024-04-10 03:12:40.045249 atap_corpus_loader-1.4.0/atap_corpus_loader/view/gui/OniLoaderWidget.py
--rw-r--r--   0        0        0      182 2024-01-31 04:39:45.165382 atap_corpus_loader-1.4.0/atap_corpus_loader/view/gui/__init__.py
--rw-r--r--   0        0        0      884 2024-03-28 04:28:43.163463 atap_corpus_loader-1.4.0/atap_corpus_loader/view/notifications/NotifierService.py
--rw-r--r--   0        0        0       45 2024-01-31 04:39:45.165968 atap_corpus_loader-1.4.0/atap_corpus_loader/view/notifications/__init__.py
--rw-r--r--   0        0        0     1620 2024-04-03 01:49:20.165187 atap_corpus_loader-1.4.0/atap_corpus_loader/view/tooltips/TooltipManager.py
--rw-r--r--   0        0        0       43 2024-03-27 23:21:38.983306 atap_corpus_loader-1.4.0/atap_corpus_loader/view/tooltips/__init__.py
--rw-r--r--   0        0        0      156 2024-03-27 23:35:47.897183 atap_corpus_loader-1.4.0/atap_corpus_loader/view/tooltips/markdown/build_button.md
--rw-r--r--   0        0        0      972 2024-03-28 02:04:53.521402 atap_corpus_loader-1.4.0/atap_corpus_loader/view/tooltips/markdown/corpus_editor.md
--rw-r--r--   0        0        0      271 2024-03-28 01:27:53.108446 atap_corpus_loader-1.4.0/atap_corpus_loader/view/tooltips/markdown/file_filter_input.md
--rw-r--r--   0        0        0      425 2024-03-28 03:09:31.422589 atap_corpus_loader-1.4.0/atap_corpus_loader/view/tooltips/markdown/linking_selectors.md
--rw-r--r--   0        0        0      889 2024-03-28 01:52:42.823366 atap_corpus_loader-1.4.0/atap_corpus_loader/view/tooltips/markdown/load_buttons.md
--rw-r--r--   0        0        0      234 2024-03-28 01:08:20.066821 atap_corpus_loader-1.4.0/atap_corpus_loader/view/tooltips/markdown/load_corpus_button.md
--rw-r--r--   0        0        0     1182 2024-03-28 03:09:31.426273 atap_corpus_loader-1.4.0/atap_corpus_loader/view/tooltips/markdown/meta_editor.md
--rw-r--r--   0        0        0      637 2024-04-10 05:25:30.592478 atap_corpus_loader-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     1845 1970-01-01 00:00:00.000000 atap_corpus_loader-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-12-21 02:04:16.054274 atap_corpus_loader-1.5.0/LICENSE
+-rw-r--r--   0        0        0     1177 2024-05-06 06:47:40.545891 atap_corpus_loader-1.5.0/README.md
+-rw-r--r--   0        0        0     2893 2024-04-24 06:52:07.725642 atap_corpus_loader-1.5.0/atap_corpus_loader/CorpusLoader.py
+-rw-r--r--   0        0        0       56 2024-04-10 06:28:42.036892 atap_corpus_loader-1.5.0/atap_corpus_loader/__init__.py
+-rw-r--r--   0        0        0    17303 2024-05-08 06:53:19.775018 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/Controller.py
+-rw-r--r--   0        0        0     3726 2024-04-04 00:22:30.044441 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/CorpusExportService.py
+-rw-r--r--   0        0        0       35 2024-01-31 04:39:45.157711 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/__init__.py
+-rw-r--r--   0        0        0      869 2024-03-26 23:51:50.596436 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/data_objects/CorpusHeader.py
+-rw-r--r--   0        0        0      269 2024-02-07 03:45:55.625849 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/data_objects/DataType.py
+-rw-r--r--   0        0        0     9018 2024-04-19 06:10:10.225435 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/data_objects/FileReference.py
+-rw-r--r--   0        0        0     4113 2024-04-01 23:58:39.235829 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/data_objects/UniqueNameCorpora.py
+-rw-r--r--   0        0        0      556 2024-04-02 01:55:47.521647 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/data_objects/ViewCorpusInfo.py
+-rw-r--r--   0        0        0      243 2024-03-26 05:34:13.113505 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/data_objects/__init__.py
+-rw-r--r--   0        0        0       41 2024-04-18 23:16:51.051195 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/FileLoadError.py
+-rw-r--r--   0        0        0     4349 2024-04-18 23:16:51.051415 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/FileLoaderService.py
+-rw-r--r--   0        0        0     7116 2024-04-18 23:16:51.051630 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/LoaderService.py
+-rw-r--r--   0        0        0     6493 2024-05-07 05:49:25.219705 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/OniLoaderService.py
+-rw-r--r--   0        0        0       41 2024-04-18 23:16:51.052018 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/__init__.py
+-rw-r--r--   0        0        0     2878 2024-04-18 23:16:51.052238 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/file_loader_strategy/FileLoaderFactory.py
+-rw-r--r--   0        0        0     2333 2024-04-18 23:16:51.052499 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/file_loader_strategy/FileLoaderStrategy.py
+-rw-r--r--   0        0        0      100 2024-04-18 23:16:51.052698 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/file_loader_strategy/__init__.py
+-rw-r--r--   0        0        0     1273 2024-04-18 23:16:51.052990 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/CSVLoaderStrategy.py
+-rw-r--r--   0        0        0     1388 2024-04-18 23:16:51.053223 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/DOCXLoaderStrategy.py
+-rw-r--r--   0        0        0     1295 2024-04-18 23:16:51.053432 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/ODSLoaderStrategy.py
+-rw-r--r--   0        0        0     1561 2024-04-18 23:16:51.053669 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/ODTLoaderStrategy.py
+-rw-r--r--   0        0        0     1293 2024-04-18 23:16:51.053908 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/TSVLoaderStrategy.py
+-rw-r--r--   0        0        0     1286 2024-04-18 23:16:51.054122 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/TXTLoaderStrategy.py
+-rw-r--r--   0        0        0     1268 2024-04-18 23:16:51.054322 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/XLSXLoaderStrategy.py
+-rw-r--r--   0        0        0     1659 2024-04-18 23:16:51.054502 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/XMLLoaderStrategy.py
+-rw-r--r--   0        0        0      396 2024-04-18 23:16:51.054681 atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/__init__.py
+-rw-r--r--   0        0        0     3032 2024-05-07 03:59:14.809614 atap_corpus_loader-1.5.0/atap_corpus_loader/view/ViewWrapperWidget.py
+-rw-r--r--   0        0        0      108 2024-01-31 04:39:45.163251 atap_corpus_loader-1.5.0/atap_corpus_loader/view/__init__.py
+-rw-r--r--   0        0        0      908 2024-03-26 05:34:13.115036 atap_corpus_loader-1.5.0/atap_corpus_loader/view/gui/AbstractWidget.py
+-rw-r--r--   0        0        0     5745 2024-04-10 06:28:42.037873 atap_corpus_loader-1.5.0/atap_corpus_loader/view/gui/CorpusInfoWidget.py
+-rw-r--r--   0        0        0     6626 2024-04-18 05:38:14.976878 atap_corpus_loader-1.5.0/atap_corpus_loader/view/gui/FileLoaderWidget.py
+-rw-r--r--   0        0        0     5339 2024-04-24 06:52:07.727106 atap_corpus_loader-1.5.0/atap_corpus_loader/view/gui/FileSelectorWidget.py
+-rw-r--r--   0        0        0     8527 2024-05-02 01:59:44.016873 atap_corpus_loader-1.5.0/atap_corpus_loader/view/gui/MetaEditorWidget.py
+-rw-r--r--   0        0        0     5651 2024-05-08 06:53:19.780245 atap_corpus_loader-1.5.0/atap_corpus_loader/view/gui/OniLoaderWidget.py
+-rw-r--r--   0        0        0      182 2024-01-31 04:39:45.165382 atap_corpus_loader-1.5.0/atap_corpus_loader/view/gui/__init__.py
+-rw-r--r--   0        0        0      884 2024-03-28 04:28:43.163463 atap_corpus_loader-1.5.0/atap_corpus_loader/view/notifications/NotifierService.py
+-rw-r--r--   0        0        0       45 2024-01-31 04:39:45.165968 atap_corpus_loader-1.5.0/atap_corpus_loader/view/notifications/__init__.py
+-rw-r--r--   0        0        0     2182 2024-05-07 03:36:07.954193 atap_corpus_loader-1.5.0/atap_corpus_loader/view/tooltips/TooltipManager.py
+-rw-r--r--   0        0        0       43 2024-03-27 23:21:38.983306 atap_corpus_loader-1.5.0/atap_corpus_loader/view/tooltips/__init__.py
+-rw-r--r--   0        0        0      156 2024-03-27 23:35:47.897183 atap_corpus_loader-1.5.0/atap_corpus_loader/view/tooltips/markdown/build_button.md
+-rw-r--r--   0        0        0      972 2024-04-24 06:52:07.728330 atap_corpus_loader-1.5.0/atap_corpus_loader/view/tooltips/markdown/corpus_editor.md
+-rw-r--r--   0        0        0      271 2024-03-28 01:27:53.108446 atap_corpus_loader-1.5.0/atap_corpus_loader/view/tooltips/markdown/file_filter_input.md
+-rw-r--r--   0        0        0      425 2024-03-28 03:09:31.422589 atap_corpus_loader-1.5.0/atap_corpus_loader/view/tooltips/markdown/linking_selectors.md
+-rw-r--r--   0        0        0      889 2024-03-28 01:52:42.823366 atap_corpus_loader-1.5.0/atap_corpus_loader/view/tooltips/markdown/load_buttons.md
+-rw-r--r--   0        0        0      234 2024-03-28 01:08:20.066821 atap_corpus_loader-1.5.0/atap_corpus_loader/view/tooltips/markdown/load_corpus_button.md
+-rw-r--r--   0        0        0     1182 2024-03-28 03:09:31.426273 atap_corpus_loader-1.5.0/atap_corpus_loader/view/tooltips/markdown/meta_editor.md
+-rw-r--r--   0        0        0      431 2024-05-07 04:05:07.032191 atap_corpus_loader-1.5.0/atap_corpus_loader/view/tooltips/markdown/oni_api_key.md
+-rw-r--r--   0        0        0      545 2024-05-08 00:59:11.772629 atap_corpus_loader-1.5.0/atap_corpus_loader/view/tooltips/markdown/oni_provider.md
+-rw-r--r--   0        0        0      372 2024-05-07 05:49:25.223351 atap_corpus_loader-1.5.0/atap_corpus_loader/view/tooltips/markdown/oni_retrieve_collection.md
+-rw-r--r--   0        0        0      825 2024-05-14 01:47:25.748701 atap_corpus_loader-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2193 1970-01-01 00:00:00.000000 atap_corpus_loader-1.5.0/PKG-INFO
```

### Comparing `atap_corpus_loader-1.4.0/LICENSE` & `atap_corpus_loader-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.4.0/README.md` & `atap_corpus_loader-1.5.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -8,30 +8,29 @@
 - txt
 - odt
 - docx
 - csv
 - tsv
 - xlsx
 - ods
-- rds
-- RData/RDa
+- xml
 
 ## Installation
 
 ```shell
 python3 -m pip install atap-corpus-loader
 ```
 
 ### Prerequisites
 
 - [Python 3.10](https://www.python.org/)
 
 ## Documentation
 
-Documentation can be found in [DOCS.md](DOCS.md)
+Documentation can be found [here](https://australian-text-analytics-platform.github.io/atap-corpus-loader/DOCS.html)
 
 ## Tests
 
 ```shell
 python3 tests/tests.py
 ```
```

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/CorpusLoader.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/CorpusLoader.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/controller/Controller.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/controller/Controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 import logging
-from datetime import datetime
 from logging.handlers import RotatingFileHandler
 from io import BytesIO
 from os.path import abspath, join, dirname
-from typing import Optional, Callable
+from typing import Optional, Callable, Literal
 
 from atap_corpus.corpus.corpus import DataFrameCorpus
 from pandas import DataFrame
 from panel.widgets import Tqdm
 
 from atap_corpus_loader.controller.CorpusExportService import CorpusExportService
-from atap_corpus_loader.controller.FileLoaderService import FileLoaderService, FileLoadError
-from atap_corpus_loader.controller.OniAPIService import OniAPIService
+from atap_corpus_loader.controller.loader_service import LoaderService
+from atap_corpus_loader.controller.loader_service.FileLoadError import FileLoadError
+from atap_corpus_loader.controller.loader_service.FileLoaderService import FileLoaderService
 from atap_corpus_loader.controller.data_objects import (FileReference, ViewCorpusInfo, CorpusHeader, DataType,
                                                         UniqueNameCorpora)
-from atap_corpus_loader.controller.file_loader_strategy.FileLoaderFactory import ValidFileType
+from atap_corpus_loader.controller.loader_service.OniLoaderService import OniLoaderService
+from atap_corpus_loader.controller.loader_service.file_loader_strategy.FileLoaderFactory import ValidFileType
 from atap_corpus_loader.view.notifications import NotifierService
 
 
 class Controller:
     LOGGER: logging.Logger = None
     """
     Provides methods for indirection between the corpus loading logic and the user interface
     Holds a reference to the latest corpus built.
     The build_callback_fn will be called when a corpus is built (can be set using set_build_callback()).
     """
+
     def __init__(self, root_directory: str):
         Controller.setup_logger()
 
         self.file_loader_service: FileLoaderService = FileLoaderService(root_directory)
-        self.oni_api_service: OniAPIService = OniAPIService()
+        self.oni_loader_service: OniLoaderService = OniLoaderService()
+        self.loader_service: LoaderService = self.file_loader_service
         self.corpus_export_service: CorpusExportService = CorpusExportService()
         self.notifier_service: NotifierService = NotifierService()
 
         self.text_header: Optional[CorpusHeader] = None
         self.corpus_link_header: Optional[CorpusHeader] = None
         self.meta_link_header: Optional[CorpusHeader] = None
 
@@ -96,55 +99,65 @@
         corpora_list: list = self.corpora.items()
         corpora_dict: dict[str, DataFrameCorpus] = {}
         for corpus in corpora_list:
             corpora_dict[corpus.name] = corpus
 
         return corpora_dict
 
+    def set_loader_service_type(self, loader_type: Literal['file', 'oni']):
+        if loader_type == 'file':
+            self.loader_service = self.file_loader_service
+        elif loader_type == 'oni':
+            self.loader_service = self.oni_loader_service
+        else:
+            raise ValueError("loader_type specified must be either 'file' or 'oni'")
+
     def load_corpus_from_filepaths(self, filepath_ls: list[str], include_hidden: bool) -> bool:
         Controller.LOGGER.debug(f"Files loaded as corpus: {filepath_ls}")
+        self.build_tqdm.visible = True
         try:
-            self.file_loader_service.add_corpus_files(filepath_ls, include_hidden, self.build_tqdm)
-            self.corpus_headers = self.file_loader_service.get_inferred_corpus_headers()
+            self.loader_service.add_corpus_files(filepath_ls, include_hidden, self.build_tqdm)
+            self.corpus_headers = self.loader_service.get_inferred_corpus_headers()
         except FileLoadError as e:
             self.display_error(str(e))
             self.unload_all()
+            self.build_tqdm.visible = False
             return False
 
+        self.build_tqdm.visible = False
         return True
 
     def load_meta_from_filepaths(self, filepath_ls: list[str], include_hidden: bool) -> bool:
         Controller.LOGGER.debug(f"Files loaded as meta: {filepath_ls}")
+        self.build_tqdm.visible = True
         try:
-            self.file_loader_service.add_meta_files(filepath_ls, include_hidden, self.build_tqdm)
-            self.meta_headers = self.file_loader_service.get_inferred_meta_headers()
+            self.loader_service.add_meta_files(filepath_ls, include_hidden, self.build_tqdm)
+            self.meta_headers = self.loader_service.get_inferred_meta_headers()
         except FileLoadError as e:
             self.display_error(str(e))
             self.unload_all()
+            self.build_tqdm.visible = False
             return False
 
+        self.build_tqdm.visible = False
         return True
 
-    def build_corpus(self, corpus_name: str) -> bool:
-        Controller.LOGGER.debug(f"build_corpus method: Building corpus with name {corpus_name}")
+    def build_corpus(self, corpus_id: str) -> bool:
+        Controller.LOGGER.debug(f"build_corpus method: Building corpus with name: {corpus_id}")
         if self.is_meta_added():
             if (self.corpus_link_header is None) or (self.meta_link_header is None):
                 self.display_error("Cannot build without link headers set. Select a corpus header and a meta header as linking headers in the dropdowns")
                 return False
 
-        if (corpus_name == '') or (corpus_name is None):
-            corpus_name = f"Corpus-{datetime.now()}"
-            Controller.LOGGER.debug(f"build_corpus method: No name provided, so corpus name generated: {corpus_name}")
-
         self.build_tqdm.visible = True
         try:
-            corpus = self.file_loader_service.build_corpus(corpus_name, self.corpus_headers,
-                                                           self.meta_headers, self.text_header,
-                                                           self.corpus_link_header, self.meta_link_header,
-                                                           self.build_tqdm)
+            corpus = self.loader_service.build_corpus(corpus_id, self.corpus_headers,
+                                                      self.meta_headers, self.text_header,
+                                                      self.corpus_link_header, self.meta_link_header,
+                                                      self.build_tqdm)
             Controller.LOGGER.debug(f"build_corpus method: corpus built")
         except FileLoadError as e:
             Controller.LOGGER.exception("Exception while building corpus: ")
             self.display_error(str(e))
             self.build_tqdm.visible = False
             return False
         except Exception as e:
@@ -217,56 +230,56 @@
             corpus.rename(new_name)
         except ValueError as e:
             self.display_error(str(e))
         except Exception as e:
             self.display_error(f"Unexpected error while renaming: {e}")
 
     def get_loaded_file_counts(self) -> dict[str, int]:
-        corpus_file_set = set(self.file_loader_service.get_loaded_corpus_files())
-        meta_file_set = set(self.file_loader_service.get_loaded_meta_files())
+        corpus_file_set = self.loader_service.get_loaded_corpus_files()
+        meta_file_set = self.loader_service.get_loaded_meta_files()
         file_set = corpus_file_set | meta_file_set
 
         file_counts: dict[str, int] = {"Total files": len(file_set)}
         for file_ref in file_set:
             extension = file_ref.get_extension().upper()
             if file_counts.get(extension) is None:
                 file_counts[extension] = 1
             else:
                 file_counts[extension] += 1
 
         return file_counts
 
     def unload_filepaths(self, filepath_ls: list[str]):
         for filepath in filepath_ls:
-            self.file_loader_service.remove_meta_filepath(filepath)
-            self.file_loader_service.remove_corpus_filepath(filepath)
+            self.loader_service.remove_meta_filepath(filepath)
+            self.loader_service.remove_corpus_filepath(filepath)
 
-        if len(self.file_loader_service.get_loaded_corpus_files()) == 0:
+        if not self.is_corpus_added():
             self.text_header = None
             self.corpus_headers = []
             self.corpus_link_header = None
-        if len(self.file_loader_service.get_loaded_meta_files()) == 0:
+        if not self.is_meta_added():
             self.meta_headers = []
             self.meta_link_header = None
 
     def unload_all(self):
         Controller.LOGGER.debug("All files unloaded")
-        self.file_loader_service.remove_all_files()
+        self.loader_service.remove_all_files()
 
         self.text_header = None
         self.corpus_headers = []
         self.meta_headers = []
         self.corpus_link_header = None
         self.meta_link_header = None
 
     def get_loaded_corpus_files(self) -> set[FileReference]:
-        return self.file_loader_service.get_loaded_corpus_files_set()
+        return self.loader_service.get_loaded_corpus_files()
 
     def get_loaded_meta_files(self) -> set[FileReference]:
-        return self.file_loader_service.get_loaded_meta_files_set()
+        return self.loader_service.get_loaded_meta_files()
 
     def get_corpus_headers(self) -> list[CorpusHeader]:
         return self.corpus_headers
 
     def get_meta_headers(self) -> list[CorpusHeader]:
         return self.meta_headers
 
@@ -285,18 +298,18 @@
     def get_valid_filetypes(self) -> list[str]:
         return [ft.name for ft in ValidFileType]
 
     def get_build_progress_bar(self) -> Tqdm:
         return self.build_tqdm
 
     def is_corpus_added(self) -> bool:
-        return len(self.file_loader_service.get_loaded_corpus_files()) > 0
+        return self.loader_service.is_corpus_loaded()
 
     def is_meta_added(self) -> bool:
-        return len(self.file_loader_service.get_loaded_meta_files()) > 0
+        return self.loader_service.is_meta_loaded()
 
     def update_corpus_header(self, header: CorpusHeader, include: Optional[bool], datatype_name: Optional[str]):
         if include is not None:
             header.include = include
         if datatype_name is not None:
             header.datatype = DataType[datatype_name]
 
@@ -339,15 +352,15 @@
             if header.name == link_header_name:
                 self.meta_link_header = header
                 header.include = True
                 return
         self.meta_link_header = None
 
     def retrieve_all_files(self, expand_archived: bool) -> list[FileReference]:
-        return self.file_loader_service.get_all_files(expand_archived)
+        return self.loader_service.get_all_files(expand_archived)
 
     def get_export_types(self) -> list[str]:
         return self.corpus_export_service.get_filetypes()
 
     def export_corpus(self, corpus_name: str, filetype: str) -> Optional[BytesIO]:
         corpus: Optional[DataFrameCorpus] = self.corpora.get(corpus_name)
         if corpus is None:
@@ -363,7 +376,53 @@
             self.display_error(str(e))
         except Exception as e:
             self.display_error(f"Unexpected error while exporting: {e}")
         self.export_tqdm.visible = False
 
     def get_export_progress_bar(self) -> Tqdm:
         return self.export_tqdm
+
+    # Oni Loader methods
+
+    def set_provider(self, name: str, address: str) -> bool:
+        try:
+            self.oni_loader_service.set_provider(name, address)
+        except FileLoadError as e:
+            self.display_error(str(e))
+            return False
+        except Exception as e:
+            self.display_error(f"Unexpected error while adding provider: {e}")
+        return True
+
+    def get_providers(self) -> list[str]:
+        return self.oni_loader_service.get_providers()
+
+    def set_curr_provider(self, name: str):
+        try:
+            self.oni_loader_service.set_curr_provider(name)
+        except ValueError as e:
+            self.display_error(str(e))
+        except Exception as e:
+            self.display_error(f"Unexpected error while setting provider: {e}")
+
+    def get_curr_provider(self) -> str:
+        return self.oni_loader_service.get_curr_provider()
+
+    def get_curr_provider_address(self) -> str:
+        return self.oni_loader_service.get_curr_provider_address()
+
+    def set_api_key(self, api_key: str):
+        success: bool = self.oni_loader_service.set_api_key(api_key)
+        if success:
+            self.display_success("API key set")
+        else:
+            self.display_error("API key not valid. Please try again")
+
+    def set_collection_id(self, collection_id: str):
+        try:
+            self.oni_loader_service.set_collection_id(collection_id)
+            self.unload_all()
+            self.display_success(f"Collection files retrieved successfully for '{collection_id}'")
+        except FileLoadError as e:
+            self.display_error(str(e))
+        except Exception as e:
+            self.display_error(f"Unexpected error while setting collection ID: {e}")
```

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/controller/CorpusExportService.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/controller/CorpusExportService.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/controller/FileLoaderService.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/LoaderService.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,106 +1,56 @@
-from glob import iglob
-from os import R_OK, access
-from os.path import normpath, sep, isdir, exists
-from typing import Optional, Iterator
-from zipfile import BadZipFile
+from abc import abstractmethod, ABC
+from datetime import datetime
+from typing import Optional
 
+from atap_corpus.corpus.corpus import DataFrameCorpus
 from pandas import DataFrame, merge, concat
 from panel.widgets import Tqdm
-from atap_corpus.corpus.corpus import DataFrameCorpus
 
 from atap_corpus_loader.controller.data_objects import FileReference, CorpusHeader, FileReferenceFactory
-from atap_corpus_loader.controller.file_loader_strategy import FileLoaderStrategy, FileLoaderFactory, FileLoadError
+from atap_corpus_loader.controller.loader_service.FileLoadError import FileLoadError
+from atap_corpus_loader.controller.loader_service.file_loader_strategy import FileLoaderStrategy, FileLoaderFactory
 
 """
 Some methods in this module utilise Tqdm from the panel library, which breaks the Model-View separation.
 This has been done out of necessity for a progress bar for particular operations.
 The panel Tqdm is a wrapper for the standard tqdm module and can be replaced if needed.
 """
 
 
-class FileLoaderService:
-    """
-    Provides methods that handle the logic of loading files and building the DataFrameCorpus object from the loaded
-    files.
-    Maintains a reference to files loaded as corpus files and files loaded as metadata files.
-    """
-    def __init__(self, root_directory: str):
-        self.root_directory: str = self._sanitise_root_dir(root_directory)
+class LoaderService(ABC):
+    def __init__(self):
         self.loaded_corpus_files: set[FileReference] = set()
         self.loaded_meta_files: set[FileReference] = set()
         # Utilise FileReferenceFactory.clear_cache() if memory overhead is raised as an issue.
         self.file_ref_factory: FileReferenceFactory = FileReferenceFactory()
 
-        self.all_files_cache: list[FileReference] = []
-        self.all_files_count: int = 0
-
+    @abstractmethod
     def get_all_files(self, expand_archived: bool) -> list[FileReference]:
-        path_iter: Iterator = iglob(f"{self.root_directory}**", recursive=True)
-        all_file_refs: list[FileReference] = []
-        for path in path_iter:
-            if isdir(path):
-                continue
-
-            file_refs: list[FileReference] = self.file_ref_factory.get_file_refs_from_path(path, expand_archived)
-            all_file_refs.extend(file_refs)
-
-        all_file_refs.sort(key=lambda ref: ref.get_path())
+        raise NotImplementedError()
 
-        return all_file_refs
-
-    def get_loaded_corpus_files(self) -> list[FileReference]:
-        return [f for f in self.loaded_corpus_files if not f.is_archive()]
+    @abstractmethod
+    def add_corpus_files(self, corpus_filepaths: list[str], include_hidden: bool, tqdm_obj: Tqdm):
+        raise NotImplementedError()
 
-    def get_loaded_meta_files(self) -> list[FileReference]:
-        return [f for f in self.loaded_meta_files if not f.is_archive()]
+    @abstractmethod
+    def add_meta_files(self, meta_filepaths: list[str], include_hidden: bool, tqdm_obj: Tqdm):
+        raise NotImplementedError()
 
-    def get_loaded_corpus_files_set(self) -> set[FileReference]:
-        return set(self.get_loaded_corpus_files())
+    def is_corpus_loaded(self) -> bool:
+        return len(self.loaded_corpus_files) > 0
 
-    def get_loaded_meta_files_set(self) -> set[FileReference]:
-        return set(self.get_loaded_meta_files())
+    def is_meta_loaded(self) -> bool:
+        return len(self.loaded_meta_files) > 0
 
-    def add_corpus_files(self, corpus_filepaths: list[str], include_hidden: bool, tqdm_obj: Tqdm):
-        for filepath in tqdm_obj(corpus_filepaths, desc="Loading corpus files", unit="files", leave=False):
-            file_ref: FileReference = self.file_ref_factory.get_file_ref(filepath)
-            if file_ref in self.loaded_corpus_files:
-                continue
-            if not include_hidden and file_ref.is_hidden():
-                continue
-            FileLoaderService._check_filepath_permissions(file_ref)
-
-            self.loaded_corpus_files.add(file_ref)
-            if file_ref.is_archive():
-                try:
-                    zip_refs: list[FileReference] = self.file_ref_factory.get_zip_file_refs(filepath)
-                except BadZipFile:
-                    raise FileLoadError(f"Can't read Zip file as it is malformed: {file_ref.get_filename()}")
-                for zip_ref in zip_refs:
-                    if not zip_ref.is_hidden() or include_hidden:
-                        self.loaded_corpus_files.add(zip_ref)
+    def get_loaded_corpus_files(self) -> set[FileReference]:
+        return set([f for f in self.loaded_corpus_files if not f.is_archive()])
 
-    def add_meta_files(self, meta_filepaths: list[str], include_hidden: bool, tqdm_obj: Tqdm):
-        for filepath in tqdm_obj(meta_filepaths, desc="Loading metadata files", unit="files", leave=False):
-            file_ref: FileReference = self.file_ref_factory.get_file_ref(filepath)
-            if file_ref in self.loaded_meta_files:
-                continue
-            if not include_hidden and file_ref.is_hidden():
-                continue
-            FileLoaderService._check_filepath_permissions(file_ref)
-
-            self.loaded_meta_files.add(file_ref)
-            if file_ref.is_archive():
-                try:
-                    zip_refs: list[FileReference] = self.file_ref_factory.get_zip_file_refs(filepath)
-                except BadZipFile:
-                    raise FileLoadError(f"Can't read Zip file as it is malformed: {file_ref.get_filename()}")
-                for zip_ref in zip_refs:
-                    if not zip_ref.is_hidden() or include_hidden:
-                        self.loaded_meta_files.add(zip_ref)
+    def get_loaded_meta_files(self) -> set[FileReference]:
+        return set(f for f in self.loaded_meta_files if not f.is_archive())
 
     def remove_corpus_filepath(self, corpus_filepath: str):
         file_ref: FileReference = self.file_ref_factory.get_file_ref(corpus_filepath)
         if file_ref in self.loaded_corpus_files:
             self.loaded_corpus_files.remove(file_ref)
 
     def remove_meta_filepath(self, meta_filepath: str):
@@ -120,15 +70,15 @@
 
     def get_inferred_corpus_headers(self) -> list[CorpusHeader]:
         return self._get_file_headers(self.get_loaded_corpus_files())
 
     def get_inferred_meta_headers(self) -> list[CorpusHeader]:
         return self._get_file_headers(self.get_loaded_meta_files())
 
-    def _get_file_headers(self, file_refs: list[FileReference]) -> list[CorpusHeader]:
+    def _get_file_headers(self, file_refs: set[FileReference]) -> list[CorpusHeader]:
         headers: Optional[list[CorpusHeader]] = None
         for ref in file_refs:
             file_loader: FileLoaderStrategy = FileLoaderFactory.get_file_loader(ref)
             try:
                 path_headers: list[CorpusHeader] = file_loader.get_inferred_headers()
             except UnicodeDecodeError:
                 self.remove_corpus_filepath(ref.get_path())
@@ -157,22 +107,18 @@
                      text_header: CorpusHeader,
                      corpus_link_header: Optional[CorpusHeader],
                      meta_link_header: Optional[CorpusHeader],
                      tqdm_obj: Tqdm) -> DataFrameCorpus:
         corpus_files: list[FileReference] = sorted(self.get_loaded_corpus_files(), key=lambda f: f.get_path())
         meta_files: list[FileReference] = sorted(self.get_loaded_meta_files(), key=lambda f: f.get_path())
 
-        corpus_df: DataFrame = FileLoaderService._get_concatenated_dataframe(corpus_files,
-                                                                             corpus_headers,
-                                                                             tqdm_obj,
-                                                                             "Building corpus")
-        meta_df: DataFrame = FileLoaderService._get_concatenated_dataframe(meta_files,
-                                                                           meta_headers,
-                                                                           tqdm_obj,
-                                                                           "Building metadata")
+        corpus_df: DataFrame = self._get_concatenated_dataframe(corpus_files, corpus_headers,
+                                                                tqdm_obj, "Building corpus")
+        meta_df: DataFrame = self._get_concatenated_dataframe(meta_files, meta_headers,
+                                                              tqdm_obj, "Building metadata")
 
         load_corpus: bool = len(corpus_headers) > 0
         load_meta: bool = len(meta_headers) > 0
 
         final_df: DataFrame
         if load_corpus and load_meta:
             final_df = merge(left=corpus_df, right=meta_df,
@@ -181,38 +127,18 @@
         elif load_corpus:
             final_df = corpus_df
         elif load_meta:
             final_df = meta_df
         else:
             raise ValueError("No corpus headers or metadata headers provided")
 
-        return DataFrameCorpus.from_dataframe(final_df, text_header.name, corpus_name)
-
-    @staticmethod
-    def _sanitise_root_dir(root_directory: str) -> str:
-        if type(root_directory) is not str:
-            raise TypeError(f"root_directory argument: expected string, got {type(root_directory)}")
-        sanitised_directory = normpath(root_directory)
-
-        if not sanitised_directory.endswith(sep):
-            sanitised_directory += sep
+        if (corpus_name == '') or (corpus_name is None):
+            corpus_name = f"Corpus-{datetime.now()}"
 
-        return sanitised_directory
-
-    @staticmethod
-    def _check_filepath_permissions(file_ref: FileReference):
-        filepath: str
-        if file_ref.is_zipped():
-            filepath = file_ref.get_directory_path()
-        else:
-            filepath = file_ref.get_path()
-        if not exists(filepath):
-            raise FileLoadError(f"No file found at: {filepath}")
-        if not access(filepath, R_OK):
-            raise FileLoadError(f"No permissions to read the file at: {filepath}")
+        return DataFrameCorpus.from_dataframe(final_df, text_header.name, corpus_name)
 
     @staticmethod
     def _get_concatenated_dataframe(file_refs: list[FileReference],
                                     headers: list[CorpusHeader],
                                     tqdm_obj: Tqdm,
                                     loading_msg: str) -> DataFrame:
         if len(file_refs) == 0:
@@ -225,8 +151,8 @@
             except UnicodeDecodeError:
                 raise FileLoadError(f"Error loading file at {ref.get_path()}: file is not UTF-8 encoded")
             except Exception as e:
                 raise FileLoadError(f"Error loading file at {ref.get_path()}: {e}")
 
             df_list.append(path_df)
 
-        return concat(df_list, ignore_index=True)
+        return concat(df_list, ignore_index=True)
```

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/controller/data_objects/CorpusHeader.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/controller/data_objects/CorpusHeader.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/controller/data_objects/FileReference.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/controller/data_objects/FileReference.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,16 @@
+from abc import ABC, abstractmethod
 from io import BytesIO
 from os.path import join, dirname, basename
-from tempfile import NamedTemporaryFile
 from typing import Optional
 from zipfile import ZipFile, BadZipFile
 
 
-class FileReference:
-    """
-    A general purpose object to hold information regarding a specific file in the file system.
-    Folder structure is preserved as a path-like string
-    """
+class FileReference(ABC):
     def __init__(self, path: str):
-        """
-        :param path: the path to the file. This can be absolute or relative to the root_directory specified in CorpusLoader
-        """
         self.path: str = path
         self.path_hash: int = hash(self.path)
         self.directory_path: str = dirname(path)
         self.filename: str = basename(path)
 
         self.filename_no_ext: str
         self.extension: str
@@ -27,49 +20,37 @@
         else:
             filename_dot_split = self.filename.split('.')
             self.extension = filename_dot_split[-1]
             self.filename_no_ext = '.'.join(filename_dot_split[:-1])
 
         self.is_ref_archive = self.extension.lower() == 'zip'
 
+    @abstractmethod
+    def get_content_buffer(self) -> BytesIO:
+        """
+        Provides a BytesIO object which contains the contents of the file.
+        :return: The BytesIO object containing the file contents
+        :rtype: BytesIO
+        """
+        raise NotImplementedError()
+
     def __eq__(self, other):
         if not isinstance(other, FileReference):
             return False
         return self.path_hash == other.path_hash
 
     def __hash__(self):
         return self.path_hash
 
     def __str__(self):
         return self.get_path()
 
     def __repr__(self):
         return self.get_path()
 
-    def get_content_buffer(self) -> BytesIO:
-        """
-        Provides a BytesIO object which contains the contents of the file. This is used to avoid writing to a
-        temporary file if the FileReference object is an instance of ZipFileReference,
-        as is done in resolve_real_file_path()
-        :return: The BytesIO object containing the file contents
-        :rtype: BytesIO
-        """
-        with open(self.get_path(), 'rb') as bytes_f:
-            buf = BytesIO(bytes_f.read())
-        return buf
-
-    def resolve_real_file_path(self) -> str:
-        """
-        Provides a real addressable path to the file contents. If the FileReference object is an instance of
-        ZipFileReference, the file is extracted, placed in a temporary file, and the temporary file path will be provided
-        :return: the full addressable path of the file
-        :rtype: str
-        """
-        return self.get_path()
-
     def get_path(self) -> str:
         """
         :return: the path to the file
         :rtype: str
         """
         return self.path
 
@@ -105,107 +86,98 @@
         """
         :return: the filetype extension of the file (case-sensitive), excluding the '.'.
         If the filename is 'example.txt', this method will return 'txt'.
         :rtype: str
         """
         return self.extension
 
-    def is_zipped(self) -> bool:
-        """
-        If True, the file is contained within a zip archive. In this case, the path returned by get_full_path()
-        is not a real addressable path, just a string representation of where the file is located. A real addressable
-        path can be obtained from resolve_real_file_path()
-        :return: True if FileReference object is an instance of ZipFileReference, False otherwise
-        :rtype: bool
-        """
-        return False
-
     def is_archive(self) -> bool:
         """
         Returns True if the file is an archive file (e.g. example.zip), False otherwise.
         Returns False for files within an archive (e.g. example.zip/text.txt)
         :return: True if the file is an archive file (e.g. example.zip), False otherwise.
         :rtype: bool
         """
         return self.is_ref_archive
 
+    @staticmethod
+    def is_zipped() -> bool:
+        """
+        Returns True if the file is within an archive (e.g. example.zip/text.txt), False otherwise.
+        Returns False if file is an archive (e.g. example.zip)
+        :return: True if the file is within an archive (e.g. example.zip/text.txt), False otherwise.
+        :rtype: bool
+        """
+        return False
+
+
+class DiskFileReference(FileReference):
+    """
+    A general purpose object to hold information regarding a specific file in the file system.
+    Folder structure is preserved as a path-like string
+    """
+    def get_content_buffer(self) -> BytesIO:
+        """
+        Provides a BytesIO object which contains the contents of the file.
+        :return: The BytesIO object containing the file contents
+        :rtype: BytesIO
+        """
+        with open(self.get_path(), 'rb') as bytes_f:
+            buf = BytesIO(bytes_f.read())
+        return buf
+
 
 class ZipFileReference(FileReference):
     def __init__(self, zip_file: ZipFile, zip_file_path: str, internal_path: str):
         """
         :param zip_file: the ZipFile object corresponding to the zip file that holds this zipped file. This allows multiple zipped files to share the same ZipFile object
         :param zip_file_path: the path to the zip file that holds this zipped file. This can be absolute or relative to the root_directory specified in CorpusLoader
         :param internal_path: the path within the zip file to this zipped file
         """
+        super().__init__(join(zip_file_path, internal_path))
         self.zip_file = zip_file
-        self.path: str = join(zip_file_path, internal_path)
-        self.path_hash: int = hash(self.path)
         self.directory_path: str = zip_file_path
         self.internal_directory: str = dirname(internal_path)
-        self.filename: str = basename(internal_path)
-
-        self.filename_no_ext: str
-        self.extension: str
-        if '.' not in self.filename:
-            self.extension = ''
-            self.filename_no_ext = self.filename
-        else:
-            filename_dot_split = self.filename.split('.')
-            self.extension = filename_dot_split[-1]
-            self.filename_no_ext = '.'.join(filename_dot_split[:-1])
-
-        self.is_ref_archive = self.extension.lower() == 'zip'
-
-    def get_path(self) -> str:
-        """
-        :return: the joined zip_file_path and internal_path to form the full path of the file
-        :rtype: str
-        """
-        return self.path
-
-    def is_zipped(self) -> bool:
-        """
-        If True, the file is contained within a zip archive. In this case, the path returned by get_full_path()
-        is not a real addressable path, just a string representation of where the file is located. A real addressable
-        path can be obtained from resolve_real_file_path()
-        :return: True as FileReference object is an instance of ZipFileReference
-        :rtype: bool
-        """
-        return True
 
     def get_content_buffer(self) -> BytesIO:
         """
-        Provides a BytesIO object which contains the contents of the file. This is used to avoid writing to a
-        temporary file if the FileReference object is an instance of ZipFileReference,
-        as is done in resolve_real_file_path()
+        Provides a BytesIO object which contains the contents of the file.
         :return: The BytesIO object containing the file contents
         :rtype: BytesIO
         """
         internal_path = join(self.internal_directory, self.filename)
         with self.zip_file.open(internal_path, force_zip64=True) as zip_f:
             buf = BytesIO(zip_f.read())
 
         return buf
 
-    def resolve_real_file_path(self) -> str:
-        """
-        Provides a real addressable path to the file contents. If the FileReference object is an instance of
-        ZipFileReference, the file is extracted, placed in a temporary file, and the temporary file path will be provided
-        :return: the full addressable path of the file
-        :rtype: str
-        """
-        internal_path = join(self.internal_directory, self.filename)
-        with self.zip_file.open(internal_path, force_zip64=True) as zip_f:
-            file_content = zip_f.read()
+    @staticmethod
+    def is_zipped() -> bool:
+        return True
 
-        with NamedTemporaryFile(delete=False) as temp_f:
-            temp_f.write(file_content)
-            real_path = temp_f.name
 
-        return real_path
+class RemoteFileReference(FileReference):
+    def __init__(self, path: str):
+        super().__init__(path)
+        self.content_buffer: Optional[BytesIO] = None
+
+    def set_content_buffer(self, content_buffer: BytesIO):
+        content_buffer.seek(0)
+        self.content_buffer = content_buffer
+
+    def get_content_buffer(self) -> BytesIO:
+        """
+        Provides a BytesIO object which contains the contents of the file.
+        :return: The BytesIO object containing the file contents
+        :rtype: BytesIO
+        """
+        if self.content_buffer is None:
+            return BytesIO()
+        self.content_buffer.seek(0)
+        return BytesIO(self.content_buffer.read())
 
 
 class FileReferenceFactory:
     """
     Implements the Flyweight pattern to mitigate the overhead of re-creating FileReference objects, as the files within
     the file system are expected to change far less frequently than FileReference objects are referred to.
     An add-only cache for FileReference objects is maintained in the form of a dictionary which maps full_path strings
@@ -234,15 +206,15 @@
             file_refs = curr_file_ref
 
         return file_refs
 
     def get_file_ref(self, path: str) -> FileReference:
         cached_ref: Optional[FileReference] = self.file_ref_cache.get(path)
         if cached_ref is None:
-            cached_ref = FileReference(path)
+            cached_ref = DiskFileReference(path)
             self.file_ref_cache[path] = cached_ref
 
         return cached_ref
 
     def get_zip_file_refs(self, zip_file_path: str) -> list[FileReference]:
         """
         Accepts a zip file and provides a list of FileReference
@@ -266,7 +238,16 @@
         full_path: str = join(zip_file_path, internal_path)
         cached_ref: Optional[ZipFileReference] = self.file_ref_cache.get(full_path)
         if cached_ref is None:
             cached_ref = ZipFileReference(zip_file, zip_file_path, internal_path)
             self.file_ref_cache[full_path] = cached_ref
 
         return cached_ref
+
+    def get_oni_file_ref(self, path: str) -> RemoteFileReference:
+        cached_ref: Optional[FileReference] = self.file_ref_cache.get(path)
+        if (cached_ref is None) or (type(cached_ref) is not RemoteFileReference):
+            cached_ref = RemoteFileReference(path)
+            self.file_ref_cache[path] = cached_ref
+        cached_ref: RemoteFileReference
+
+        return cached_ref
```

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/controller/data_objects/UniqueNameCorpora.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/controller/data_objects/UniqueNameCorpora.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/controller/data_objects/ViewCorpusInfo.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/controller/data_objects/ViewCorpusInfo.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/FileLoaderFactory.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/file_loader_strategy/FileLoaderFactory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from enum import Enum, auto
 
 from atap_corpus_loader.controller.data_objects import FileReference
-from atap_corpus_loader.controller.file_loader_strategy.FileLoadError import FileLoadError
-from atap_corpus_loader.controller.file_loader_strategy.concrete_strategies import *
-from atap_corpus_loader.controller.file_loader_strategy.FileLoaderStrategy import FileLoaderStrategy
+from atap_corpus_loader.controller.loader_service.FileLoadError import FileLoadError
+from atap_corpus_loader.controller.loader_service.file_loader_strategy.concrete_strategies import *
+from atap_corpus_loader.controller.loader_service.file_loader_strategy.FileLoaderStrategy import FileLoaderStrategy
 
 
 class ValidFileType(Enum):
     """
     An enum of valid file extensions that are supported with a loader
     """
     TXT = auto()
```

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/FileLoaderStrategy.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/file_loader_strategy/FileLoaderStrategy.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/CSVLoaderStrategy.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/XLSXLoaderStrategy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from io import BytesIO
 
-from pandas import DataFrame, read_csv
+from pandas import DataFrame, read_excel
 
 from atap_corpus_loader.controller.data_objects import CorpusHeader, DataType
-from atap_corpus_loader.controller.file_loader_strategy.FileLoaderStrategy import FileLoaderStrategy
+from atap_corpus_loader.controller.loader_service.file_loader_strategy.FileLoaderStrategy import FileLoaderStrategy
 
 
-class CSVLoaderStrategy(FileLoaderStrategy):
+class XLSXLoaderStrategy(FileLoaderStrategy):
     def get_inferred_headers(self) -> list[CorpusHeader]:
         file_buf: BytesIO = self.file_ref.get_content_buffer()
-        df: DataFrame = read_csv(file_buf, header=0, nrows=2)
+        df: DataFrame = read_excel(file_buf, nrows=2)
         headers: list[CorpusHeader] = []
         for header_name, dtype_obj in df.dtypes.items():
             dtype: DataType
             try:
                 dtype = DataType(str(dtype_obj))
             except ValueError:
                 dtype = DataType.TEXT
             headers.append(CorpusHeader(str(header_name), dtype))
 
         return headers
 
     def get_dataframe(self, headers: list[CorpusHeader]) -> DataFrame:
         included_headers: list[str] = [header.name for header in headers if header.include]
         file_buf: BytesIO = self.file_ref.get_content_buffer()
-        df: DataFrame = read_csv(file_buf, header=0, usecols=included_headers)
+        df: DataFrame = read_excel(file_buf, header=0, names=included_headers)
         dtypes_applied_df: DataFrame = FileLoaderStrategy._apply_selected_dtypes(df, headers)
 
         return dtypes_applied_df
```

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/DOCXLoaderStrategy.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/DOCXLoaderStrategy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from io import BytesIO
 
 from docx import Document
 from pandas import DataFrame
 
-from atap_corpus_loader.controller.data_objects import CorpusHeader, DataType, FileReference
-from atap_corpus_loader.controller.file_loader_strategy.FileLoaderStrategy import FileLoaderStrategy
+from atap_corpus_loader.controller.data_objects import CorpusHeader, DataType
+from atap_corpus_loader.controller.loader_service.file_loader_strategy.FileLoaderStrategy import FileLoaderStrategy
 
 
 class DOCXLoaderStrategy(FileLoaderStrategy):
     def get_inferred_headers(self) -> list[CorpusHeader]:
         headers: list[CorpusHeader] = [
             CorpusHeader('document', DataType.TEXT, include=True),
             CorpusHeader('filename', DataType.TEXT),
```

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/ODSLoaderStrategy.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/CSVLoaderStrategy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from io import BytesIO
 
-from pandas import DataFrame, read_excel
+from pandas import DataFrame, read_csv
 
-from atap_corpus_loader.controller.data_objects import CorpusHeader, DataType, FileReference
-from atap_corpus_loader.controller.file_loader_strategy.FileLoaderStrategy import FileLoaderStrategy
+from atap_corpus_loader.controller.data_objects import CorpusHeader, DataType
+from atap_corpus_loader.controller.loader_service.file_loader_strategy.FileLoaderStrategy import FileLoaderStrategy
 
 
-class ODSLoaderStrategy(FileLoaderStrategy):
+class CSVLoaderStrategy(FileLoaderStrategy):
     def get_inferred_headers(self) -> list[CorpusHeader]:
         file_buf: BytesIO = self.file_ref.get_content_buffer()
-        df: DataFrame = read_excel(file_buf, engine='odf', nrows=2)
+        df: DataFrame = read_csv(file_buf, header=0, nrows=2)
         headers: list[CorpusHeader] = []
         for header_name, dtype_obj in df.dtypes.items():
             dtype: DataType
             try:
                 dtype = DataType(str(dtype_obj))
             except ValueError:
                 dtype = DataType.TEXT
             headers.append(CorpusHeader(str(header_name), dtype))
 
         return headers
 
     def get_dataframe(self, headers: list[CorpusHeader]) -> DataFrame:
         included_headers: list[str] = [header.name for header in headers if header.include]
         file_buf: BytesIO = self.file_ref.get_content_buffer()
-        df: DataFrame = read_excel(file_buf, engine='odf', header=0, names=included_headers)
+        df: DataFrame = read_csv(file_buf, header=0, usecols=included_headers)
         dtypes_applied_df: DataFrame = FileLoaderStrategy._apply_selected_dtypes(df, headers)
 
         return dtypes_applied_df
```

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/ODTLoaderStrategy.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/ODTLoaderStrategy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from io import BytesIO
 
 from odf import text, teletype
 from odf.opendocument import load
 from pandas import DataFrame
 
 from atap_corpus_loader.controller.data_objects import CorpusHeader, DataType
-from atap_corpus_loader.controller.file_loader_strategy.FileLoaderStrategy import FileLoaderStrategy
+from atap_corpus_loader.controller.loader_service.file_loader_strategy.FileLoaderStrategy import FileLoaderStrategy
 
 
 class ODTLoaderStrategy(FileLoaderStrategy):
     def get_inferred_headers(self) -> list[CorpusHeader]:
         headers: list[CorpusHeader] = [
             CorpusHeader('document', DataType.TEXT, include=True),
             CorpusHeader('filename', DataType.TEXT),
```

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/TSVLoaderStrategy.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/TSVLoaderStrategy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from io import BytesIO
 
 from pandas import DataFrame, read_csv
 
 from atap_corpus_loader.controller.data_objects import CorpusHeader, DataType
-from atap_corpus_loader.controller.file_loader_strategy.FileLoaderStrategy import FileLoaderStrategy
+from atap_corpus_loader.controller.loader_service.file_loader_strategy.FileLoaderStrategy import FileLoaderStrategy
 
 
 class TSVLoaderStrategy(FileLoaderStrategy):
     def get_inferred_headers(self) -> list[CorpusHeader]:
         file_buf: BytesIO = self.file_ref.get_content_buffer()
         df: DataFrame = read_csv(file_buf, sep='\t', header=0, nrows=2)
         headers: list[CorpusHeader] = []
```

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/TXTLoaderStrategy.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/TXTLoaderStrategy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from io import BytesIO
 
 from pandas import DataFrame
 
 from atap_corpus_loader.controller.data_objects import CorpusHeader, DataType
-from atap_corpus_loader.controller.file_loader_strategy.FileLoaderStrategy import FileLoaderStrategy
+from atap_corpus_loader.controller.loader_service.file_loader_strategy.FileLoaderStrategy import FileLoaderStrategy
 
 
 class TXTLoaderStrategy(FileLoaderStrategy):
     def get_inferred_headers(self) -> list[CorpusHeader]:
         headers: list[CorpusHeader] = [
             CorpusHeader('document', DataType.TEXT, include=True),
             CorpusHeader('filename', DataType.TEXT),
```

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/XLSXLoaderStrategy.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/ODSLoaderStrategy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from io import BytesIO
 
 from pandas import DataFrame, read_excel
 
 from atap_corpus_loader.controller.data_objects import CorpusHeader, DataType
-from atap_corpus_loader.controller.file_loader_strategy.FileLoaderStrategy import FileLoaderStrategy
+from atap_corpus_loader.controller.loader_service.file_loader_strategy.FileLoaderStrategy import FileLoaderStrategy
 
 
-class XLSXLoaderStrategy(FileLoaderStrategy):
+class ODSLoaderStrategy(FileLoaderStrategy):
     def get_inferred_headers(self) -> list[CorpusHeader]:
         file_buf: BytesIO = self.file_ref.get_content_buffer()
-        df: DataFrame = read_excel(file_buf, nrows=2)
+        df: DataFrame = read_excel(file_buf, engine='odf', nrows=2)
         headers: list[CorpusHeader] = []
         for header_name, dtype_obj in df.dtypes.items():
             dtype: DataType
             try:
                 dtype = DataType(str(dtype_obj))
             except ValueError:
                 dtype = DataType.TEXT
             headers.append(CorpusHeader(str(header_name), dtype))
 
         return headers
 
     def get_dataframe(self, headers: list[CorpusHeader]) -> DataFrame:
         included_headers: list[str] = [header.name for header in headers if header.include]
         file_buf: BytesIO = self.file_ref.get_content_buffer()
-        df: DataFrame = read_excel(file_buf, header=0, names=included_headers)
+        df: DataFrame = read_excel(file_buf, engine='odf', header=0, names=included_headers)
         dtypes_applied_df: DataFrame = FileLoaderStrategy._apply_selected_dtypes(df, headers)
 
         return dtypes_applied_df
```

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/XMLLoaderStrategy.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/XMLLoaderStrategy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from io import BytesIO
 from xml.etree.ElementTree import parse, Element
 
 from pandas import DataFrame
 
 from atap_corpus_loader.controller.data_objects import CorpusHeader, DataType
-from atap_corpus_loader.controller.file_loader_strategy import FileLoaderStrategy
+from atap_corpus_loader.controller.loader_service.file_loader_strategy import FileLoaderStrategy
 
 
 class XMLLoaderStrategy(FileLoaderStrategy):
     def _extract_text(self, element: Element) -> str:
         text = element.text or ''
         for child in element:
             text += self._extract_text(child)
```

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/view/ViewWrapperWidget.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/view/ViewWrapperWidget.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 from typing import Optional
 
 from panel import Tabs
 from panel.widgets import TooltipIcon
 
 from atap_corpus_loader.controller import Controller
-from atap_corpus_loader.view.gui import AbstractWidget, FileLoaderWidget, CorpusInfoWidget
+from atap_corpus_loader.view.gui import AbstractWidget, FileLoaderWidget, CorpusInfoWidget, OniLoaderWidget
 from atap_corpus_loader.view.tooltips import TooltipManager
 
 
 class ViewWrapperWidget(AbstractWidget):
     """
     A wrapper class that holds different loading method interfaces within a Tab
     """
     def __init__(self, controller: Controller, include_meta_loader: bool):
         super().__init__()
         self.controller: Controller = controller
         self.tooltip_manager: TooltipManager = TooltipManager()
 
         self.file_loader: FileLoaderWidget = FileLoaderWidget(self, controller, include_meta_loader)
+        self.oni_loader: OniLoaderWidget = OniLoaderWidget(self, controller, include_meta_loader)
         self.corpus_display: CorpusInfoWidget = CorpusInfoWidget(controller)
 
+        # set_load_service_type depends on the order of these tabs
         self.panel = Tabs(("File Loader", self.file_loader),
+                          ("Oni Loader", self.oni_loader),
                           ("Corpus Overview", self.corpus_display))
+        self.panel.param.watch(self.set_load_service_type, parameter_names=['active'])
         self.corpus_info_idx: int = len(self.panel) - 1
-        self.children = [self.file_loader, self.corpus_display]
+        self.children = [self.file_loader, self.oni_loader, self.corpus_display]
 
     def update_display(self):
         pass
 
     def load_corpus_from_filepaths(self, filepath_ls: list[str], include_hidden: bool):
         if len(filepath_ls) == 0:
             return
@@ -40,20 +44,28 @@
         if len(filepath_ls) == 0:
             return
         success = self.controller.load_meta_from_filepaths(filepath_ls, include_hidden)
         self.update_displays()
         if success:
             self.controller.display_success("Metadata files loaded successfully")
 
-    def build_corpus(self, corpus_name: str) -> bool:
-        success: bool = self.controller.build_corpus(corpus_name)
+    def build_corpus(self, corpus_id: str) -> bool:
+        success: bool = self.controller.build_corpus(corpus_id)
         if success:
             self.update_displays()
 
             self.panel.active = self.corpus_info_idx
-            corpus_name: str = self.controller.get_latest_corpus().name
-            self.controller.display_success(f"Corpus {corpus_name} built successfully")
+            corpus_id: str = self.controller.get_latest_corpus().name
+            self.controller.display_success(f"Corpus {corpus_id} built successfully")
 
         return success
 
+    def set_load_service_type(self, *_):
+        active_tab: int = self.panel.active
+        if active_tab == 0:
+            self.controller.set_loader_service_type('file')
+        elif active_tab == 1:
+            self.controller.set_loader_service_type('oni')
+        self.file_loader.unload_all()
+
     def get_tooltip(self, tooltip_name: str) -> Optional[TooltipIcon]:
         return self.tooltip_manager.get_tooltip(tooltip_name)
```

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/view/gui/AbstractWidget.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/view/gui/AbstractWidget.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/view/gui/CorpusInfoWidget.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/view/gui/CorpusInfoWidget.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/view/gui/FileLoaderWidget.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/view/gui/FileLoaderWidget.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/view/gui/FileSelectorWidget.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/view/gui/FileSelectorWidget.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/view/gui/MetaEditorWidget.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/view/gui/MetaEditorWidget.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,19 +21,19 @@
         self.controller: Controller = controller
 
         self.corpus_table_container = GridBox(styles=MetaEditorWidget.TABLE_BORDER_STYLE)
         self.meta_table_container = GridBox(styles=MetaEditorWidget.TABLE_BORDER_STYLE)
 
         corpus_table_title = Markdown("## Corpus editor")
         corpus_table_tooltip = self.view_handler.get_tooltip('corpus_editor')
-        self.corpus_table_row: Row = Row(corpus_table_title, corpus_table_tooltip)
+        self.corpus_table_row: Row = Row(corpus_table_tooltip, corpus_table_title)
 
         meta_table_title = Markdown("## Metadata editor")
         meta_table_tooltip = self.view_handler.get_tooltip('meta_editor')
-        self.meta_table_row: Row = Row(meta_table_title, meta_table_tooltip)
+        self.meta_table_row: Row = Row(meta_table_tooltip, meta_table_title)
 
         self.text_header_dropdown = Select(name='Select document label', width=200)
         text_header_fn = bind(self._set_text_header, self.text_header_dropdown)
 
         self.link_row = Row(visible=False, styles=MetaEditorWidget.ERROR_BORDER_STYLE)
         link_row_tooltip = self.view_handler.get_tooltip('linking_selectors')
         self.corpus_link_dropdown = Select(name='Select corpus linking label', width=180)
```

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/view/notifications/NotifierService.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/view/notifications/NotifierService.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/view/tooltips/TooltipManager.py` & `atap_corpus_loader-1.5.0/atap_corpus_loader/view/tooltips/TooltipManager.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,27 +3,32 @@
 from os.path import sep, isdir, basename, join
 from typing import Optional
 
 from panel.widgets import TooltipIcon
 
 
 class TooltipManager:
+    """
+    The TooltipManager class is a retrieval interface for TooltipIcon objects.
+    The only public method is get_tooltip(), which provides a TooltipIcon object corresponding to the given tooltip_name
+    """
+
     @staticmethod
     def _resolve_dir(dir_path: str) -> str:
         if type(dir_path) is not str:
             raise TypeError(f"expected string argument, got {type(dir_path)}")
         file_parent = pathlib.Path(__file__).parent.resolve()
         sanitised_directory = join(file_parent, dir_path)
         if not sanitised_directory.endswith(sep):
             sanitised_directory += sep
 
         return sanitised_directory
 
     @staticmethod
-    def read_markdown_contents() -> dict[str, str]:
+    def _read_markdown_contents() -> dict[str, str]:
         path_pattern: str = f"{TooltipManager.MARKDOWN_DIR}**"
         tooltip_map: dict[str, str] = {}
         for path in iglob(path_pattern, recursive=True):
             if isdir(path):
                 continue
             filename_split = basename(path).split('.')
             if len(filename_split) == 1:
@@ -36,14 +41,20 @@
             tooltip_map[filename] = contents
 
         return tooltip_map
 
     MARKDOWN_DIR: str = _resolve_dir("./markdown")
 
     def __init__(self):
-        self.tooltip_map: dict[str, str] = self.read_markdown_contents()
+        self.tooltip_map: dict[str, str] = self._read_markdown_contents()
 
     def get_tooltip(self, tooltip_name: str) -> Optional[TooltipIcon]:
+        """
+        Returns a TooltipIcon object whose text value is the markdown found in the file at MARKDOWN_DIR / tooltip_name + '.md'
+        :param tooltip_name: The name of the file in the MARKDOWN_DIR that contains the tooltip markdown (without the '.md' suffix)
+        :type tooltip_name: str
+        :rtype: TooltipIcon
+        """
         text = self.tooltip_map.get(tooltip_name)
         if text is None:
             return None
         return TooltipIcon(value=text, margin=(0, 0))
```

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/view/tooltips/markdown/corpus_editor.md` & `atap_corpus_loader-1.5.0/atap_corpus_loader/view/tooltips/markdown/corpus_editor.md`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/view/tooltips/markdown/load_buttons.md` & `atap_corpus_loader-1.5.0/atap_corpus_loader/view/tooltips/markdown/load_buttons.md`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.4.0/atap_corpus_loader/view/tooltips/markdown/meta_editor.md` & `atap_corpus_loader-1.5.0/atap_corpus_loader/view/tooltips/markdown/meta_editor.md`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.4.0/PKG-INFO` & `atap_corpus_loader-1.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: atap-corpus-loader
-Version: 1.4.0
+Version: 1.5.0
 Summary:  A GUI loader for atap_corpus using the Panel library.
+Home-page: https://github.com/Australian-Text-Analytics-Platform/atap-corpus-loader
 License: MIT
 Author: Hamish Croser
 Author-email: hamish.croser@sydney.edu.au
 Requires-Python: >=3.10.0,<3.12.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: atap_corpus (>=0.1.13,<0.2.0)
 Requires-Dist: odfpy (>=1.4.0,<1.5.0)
 Requires-Dist: pandas (>=2.1.0,<2.2.0)
 Requires-Dist: panel (>=1.4.0,<1.5.0)
 Requires-Dist: pyreadr (>=0.5.0,<0.6.0)
 Requires-Dist: python-docx (>=1.1.0,<1.2.0)
+Project-URL: Documentation, https://australian-text-analytics-platform.github.io/atap-corpus-loader/DOCS.html
+Project-URL: Repository, https://github.com/Australian-Text-Analytics-Platform/atap-corpus-loader
 Description-Content-Type: text/markdown
 
 # Corpus Loader
 
 A GUI loader for atap_corpus using the Panel library. Provides a single Panel-compatible widget in which a user can construct a corpus object for use by the client code.
 
 ### File Type support
@@ -28,30 +31,29 @@
 - txt
 - odt
 - docx
 - csv
 - tsv
 - xlsx
 - ods
-- rds
-- RData/RDa
+- xml
 
 ## Installation
 
 ```shell
 python3 -m pip install atap-corpus-loader
 ```
 
 ### Prerequisites
 
 - [Python 3.10](https://www.python.org/)
 
 ## Documentation
 
-Documentation can be found in [DOCS.md](DOCS.md)
+Documentation can be found [here](https://australian-text-analytics-platform.github.io/atap-corpus-loader/DOCS.html)
 
 ## Tests
 
 ```shell
 python3 tests/tests.py
 ```
```

