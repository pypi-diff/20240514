# Comparing `tmp/pimdb-0.2.3-py3-none-any.whl.zip` & `tmp/pimdb-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 23302 bytes, number of entries: 11
--rw-r--r--  2.0 unx      122 b- defN 20-May-02 16:06 pimdb/__init__.py
--rw-r--r--  2.0 unx     4446 b- defN 20-Apr-26 16:34 pimdb/bulk.py
--rw-r--r--  2.0 unx    11250 b- defN 20-May-02 16:06 pimdb/command.py
--rw-r--r--  2.0 unx    12286 b- defN 20-May-02 16:06 pimdb/common.py
--rw-r--r--  2.0 unx    54339 b- defN 20-May-02 16:06 pimdb/database.py
--rw-r--r--  2.0 unx     1483 b- defN 20-May-02 16:07 pimdb-0.2.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6103 b- defN 20-May-02 16:07 pimdb-0.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 20-May-02 16:07 pimdb-0.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 20-May-02 16:07 pimdb-0.2.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 20-May-02 16:07 pimdb-0.2.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      837 b- defN 20-May-02 16:07 pimdb-0.2.3.dist-info/RECORD
-11 files, 91010 bytes uncompressed, 21906 bytes compressed:  75.9%
+Zip file size: 22893 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      122 b- defN 24-May-14 10:33 pimdb/__init__.py
+-rw-r--r--  2.0 unx     4440 b- defN 24-May-14 10:33 pimdb/bulk.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-May-14 10:33 pimdb/command.py
+-rw-r--r--  2.0 unx    12295 b- defN 24-May-14 10:33 pimdb/common.py
+-rw-r--r--  2.0 unx    52878 b- defN 24-May-14 10:33 pimdb/database.py
+-rw-r--r--  2.0 unx     1483 b- defN 24-May-14 10:34 pimdb-0.3.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6183 b- defN 24-May-14 10:34 pimdb-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 10:34 pimdb-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       45 b- defN 24-May-14 10:34 pimdb-0.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 24-May-14 10:34 pimdb-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      837 b- defN 24-May-14 10:34 pimdb-0.3.0.dist-info/RECORD
+11 files, 89625 bytes uncompressed, 21497 bytes compressed:  76.0%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: pimdb/common.py
 Comment: 
 
 Filename: pimdb/database.py
 Comment: 
 
-Filename: pimdb-0.2.3.dist-info/LICENSE.txt
+Filename: pimdb-0.3.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pimdb-0.2.3.dist-info/METADATA
+Filename: pimdb-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: pimdb-0.2.3.dist-info/WHEEL
+Filename: pimdb-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: pimdb-0.2.3.dist-info/entry_points.txt
+Filename: pimdb-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: pimdb-0.2.3.dist-info/top_level.txt
+Filename: pimdb-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pimdb-0.2.3.dist-info/RECORD
+Filename: pimdb-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pimdb/__init__.py

```diff
@@ -1,3 +1,3 @@
 # Copyright (c) 2020, Thomas Aglassinger.
 # All rights reserved. Distributed under the BSD License.
-__version__ = "0.2.3"
+__version__ = "0.3.0"
```

## pimdb/bulk.py

```diff
@@ -1,11 +1,11 @@
 """Database bulk operations."""
 # Copyright (c) 2020, Thomas Aglassinger.
 # All rights reserved. Distributed under the BSD License.
-from typing import Any, Dict, IO, Optional
+from typing import IO, Any, Optional
 
 from sqlalchemy import Table
 from sqlalchemy.engine import Connection, Engine
 
 from pimdb.common import log
 
 #: Default number of bulk data (for e.g. SQL insert) to be collected in memory before they are sent to the database.
@@ -34,15 +34,15 @@
         assert bulk_size >= 1
         self._connection = connection
         self._table = table
         self._bulk_size = bulk_size
         self._data = []
         self._count = 0
 
-    def add(self, data: Dict[str, Optional[Any]]):
+    def add(self, data: dict[str, Optional[Any]]):
         self._data.append(data)
         self._count += 1
         if len(self._data) >= self._bulk_size:
             self._flush()
 
     def _flush(self):
         data_count = len(self._data)
```

## pimdb/command.py

```diff
@@ -1,23 +1,23 @@
 # Copyright (c) 2020, Thomas Aglassinger.
 # All rights reserved. Distributed under the BSD License.
 import argparse
 import logging
 import os
 import sys
 from enum import Enum
-from typing import List, Optional
+from typing import Optional
 
 from sqlalchemy import text
 from sqlalchemy.engine import Connection
 
 from pimdb import __version__
-from pimdb.common import download_imdb_dataset, log, ImdbDataset, IMDB_DATASET_NAMES, PimdbError
-from pimdb.database import Database
 from pimdb.bulk import DEFAULT_BULK_SIZE
+from pimdb.common import IMDB_DATASET_NAMES, ImdbDataset, PimdbError, download_imdb_dataset, log
+from pimdb.database import Database
 
 _DEFAULT_DATABASE = "sqlite:///pimdb.db"
 _DEFAULT_LOG_LEVEL = "info"
 _VALID_LOG_LEVELS = ["debug", "info", "sql", "warning"]
 _LOG_LEVEL_MAP = {
     "info": logging.INFO,
 }
@@ -158,15 +158,15 @@
 
     def run(self):
         for dataset_name_to_download in self._imdb_datasets:
             target_path = os.path.join(self._dataset_folder, ImdbDataset(dataset_name_to_download).filename)
             download_imdb_dataset(ImdbDataset(dataset_name_to_download), target_path, self._only_if_newer)
 
 
-def _checked_imdb_dataset_names(parser: argparse.ArgumentParser, args: argparse.Namespace) -> List[str]:
+def _checked_imdb_dataset_names(parser: argparse.ArgumentParser, args: argparse.Namespace) -> list[str]:
     def _check_special_name_is_only_name():
         if len(args.names) >= 2:
             parser.error(f'if NAME "{_ALL_NAME}" is specified, it must be the only NAME')
 
     if _ALL_NAME in args.names:
         _check_special_name_is_only_name()
         result = IMDB_DATASET_NAMES
@@ -244,15 +244,15 @@
     CommandName.BUILD: _BuildCommand,
     CommandName.DOWNLOAD: _DownloadCommand,
     CommandName.QUERY: _QueryCommand,
     CommandName.TRANSFER: _TransferCommand,
 }
 
 
-def exit_code_for(arguments: Optional[List[str]] = None) -> int:
+def exit_code_for(arguments: Optional[list[str]] = None) -> int:
     """
     Exit code for running the command line with the specified ``arguments``,
     or ``sys.argv``if no arguments are specified.
 
     Unlike :py:func:`main`, logging has to be initialized before calling this
     function.
```

## pimdb/common.py

```diff
@@ -2,16 +2,17 @@
 # All rights reserved. Distributed under the BSD License.
 import csv
 import gzip
 import json
 import logging
 import os.path
 import time
+from collections.abc import Generator
 from enum import Enum
-from typing import Optional, Generator, Dict, Callable, Tuple, Set, Any
+from typing import Any, Callable, Optional
 
 import requests
 
 _MEGABYTE = 1048576
 
 #: Logger for all output of the pimdb module.
 log = logging.getLogger("pimdb")
@@ -182,18 +183,18 @@
             log.info('dataset "%s" is up to date, skipping download of "%s"', imdb_dataset.value, source_url)
 
 
 class GzippedTsvReader:
     def __init__(
         self,
         gzipped_tsv_path: str,
-        key_columns: Tuple[str],
+        key_columns: tuple[str],
         indicate_progress: Optional[Callable[[int, int], None]] = None,
         seconds_between_progress_update: float = 3.0,
-        filtered_name_to_values_map: Optional[Dict[str, Set[str]]] = None,
+        filtered_name_to_values_map: Optional[dict[str, set[str]]] = None,
     ):
         self._gzipped_tsv_path = gzipped_tsv_path
         self._row_number = None
         self._key_columns = key_columns
         self._duplicate_count = None
         self._indicate_progress = indicate_progress
         self._seconds_between_progress_update = seconds_between_progress_update
@@ -213,15 +214,15 @@
         row_number_text = f" ({self.row_number})" if self.row_number is not None else ""
         return f"{os.path.basename(self.gzipped_tsv_path)}{row_number_text}"
 
     @property
     def duplicate_count(self) -> int:
         return self._duplicate_count
 
-    def column_names_to_value_maps(self) -> Generator[Dict[str, str], None, None]:
+    def column_names_to_value_maps(self) -> Generator[dict[str, str], None, None]:
         log.info('  reading IMDb dataset file "%s"', self.gzipped_tsv_path)
         with gzip.open(self.gzipped_tsv_path, "rt", encoding="utf-8", newline="") as tsv_file:
             last_progress_time = time.time()
             last_progress_row_number = None
             existing_keys = set()
             self._duplicate_count = 0
             self._row_number = 0
@@ -274,15 +275,15 @@
         self._column_names = None
 
     @property
     def line_number(self) -> int:
         assert self._line_number is not None
         return self._line_number
 
-    def write(self, name_to_value_map: Dict[str, Any]):
+    def write(self, name_to_value_map: dict[str, Any]):
         if self._column_names is None:
             self._column_names = list(name_to_value_map.keys())
             self._line_number = 1
             heading = "\t".join(self._column_names) + "\n"
             self._target_file.write(heading)
         self._line_number += 1
         try:
```

## pimdb/database.py

```diff
@@ -1,69 +1,47 @@
 # Copyright (c) 2020, Thomas Aglassinger.
 # All rights reserved. Distributed under the BSD License.
 import functools
 import gzip
 import json
 import os
 import time
+from collections.abc import Sequence
 from enum import Enum
-from typing import Dict, List, Optional, Sequence, Tuple, Union, Callable
+from typing import Callable, Optional, Union
 
 from sqlalchemy import (
-    Column,
     Boolean,
+    Column,
     Float,
+    ForeignKey,
+    Index,
     Integer,
     MetaData,
     String,
     Table,
+    Text,
+    and_,
     create_engine,
-    ForeignKey,
-    Index,
     text,
-    and_,
 )
-from sqlalchemy.engine import Engine, Connection
+from sqlalchemy.engine import Connection, Engine
 from sqlalchemy.exc import SQLAlchemyError
 from sqlalchemy.sql import select
 from sqlalchemy.sql.functions import coalesce
 from sqlalchemy.sql.selectable import SelectBase
 
 from pimdb.bulk import DEFAULT_BULK_SIZE, BulkInsert, PostgresBulkLoad
-from pimdb.common import log, ImdbDataset, PimdbError, NormalizedTableKey, GzippedTsvReader, IMDB_DATASET_NAMES
-
+from pimdb.common import IMDB_DATASET_NAMES, GzippedTsvReader, ImdbDataset, NormalizedTableKey, PimdbError, log
 
 _TCONST_LENGTH = 12  # current maximum: 10
 _NCONST_LENGTH = 12  # current maximum: 10
-_TITLE_LENGTH = 1024  # current maximum: 831 (in title.akas.title)
-_NAME_LENGTH = 160  # current maximum: 105
-_GENRE_LENGTH = 16
-_GENRE_COUNT = 4
-_REGION_LENGTH = 4
-_LANGUAGE_LENGTH = 4
-_CREW_COUNT = 2048  # current maximum: 1180
-_PROFESSION_LENGTH = 32  # current maximum (from title.principals.category): 19
-_PROFESSION_COUNT = 3
-_JOB_LENGTH = 512  # current maximum: 286
-_CHARACTER_LENGTH = 1024  # current maximum: 459
-_CHARACTERS_LENGTH = 1024  # current maximum: 463
-_KNOWN_FOR_TITLES_LENGTH = (_TCONST_LENGTH + 1) * 20 - 1  # current maximum: 159 resp. 15 titles
-
-#: The "title_akas.attributes" field is a mess.
-_ATTRIBUTES_LENGTH = 128
 
 IMDB_TITLE_ALIAS_TYPES = ["alternative", "dvd", "festival", "tv", "video", "working", "original", "imdbDisplay"]
 
-_ALIAS_TYPE_LENGTH = max(len(item) for item in IMDB_TITLE_ALIAS_TYPES)
-
-#: The "title_akas.types" field is a mess.
-_ALIAS_TYPES_LENGTH = 128
-
-_TITLE_TYPE_LENGTH = 24  # current maximum: 12
-
 
 class NamePool:
     def __init__(self, max_length: int):
         self.max_length = max_length
         self._parts_to_name_map = {}
         self._shortened_count = 0
 
@@ -101,62 +79,62 @@
         return DatabaseSystem.SQLITE
     elif engine_info.startswith("postgresql://") or engine_info.startswith("postgresql+psycopg2://"):
         return DatabaseSystem.POSTGRES
     else:
         return DatabaseSystem.OTHER
 
 
-def imdb_dataset_table_infos() -> List[Tuple[ImdbDataset, List[Column]]]:
+def imdb_dataset_table_infos() -> list[tuple[ImdbDataset, list[Column]]]:
     """SQL tables that represent a direct copy of a TSV file (excluding duplicates)"""
     return [
         (
             ImdbDataset.TITLE_BASICS,
             [
                 Column("tconst", String(_TCONST_LENGTH), nullable=False, primary_key=True),
-                Column("titleType", String(_TITLE_TYPE_LENGTH), nullable=False),
-                Column("primaryTitle", String(_TITLE_LENGTH)),
-                Column("originalTitle", String(_TITLE_LENGTH)),
+                Column("titleType", Text, nullable=False),
+                Column("primaryTitle", Text),
+                Column("originalTitle", Text),
                 Column("isAdult", Boolean, nullable=False),
                 Column("startYear", Integer),
                 Column("endYear", Integer),
                 Column("runtimeMinutes", Integer),
-                Column("genres", String((_GENRE_LENGTH + 1) * _GENRE_COUNT - 1)),
+                Column("genres", Text),
             ],
         ),
         (
             ImdbDataset.NAME_BASICS,
             [
                 Column("nconst", String(_NCONST_LENGTH), nullable=False, primary_key=True),
-                Column("primaryName", String(_NAME_LENGTH), nullable=False),
+                Column("primaryName", Text, nullable=False),
                 Column("birthYear", Integer),
                 Column("deathYear", Integer),
-                Column("primaryProfession", String((_PROFESSION_LENGTH + 1) * _PROFESSION_COUNT - 1)),
-                Column("knownForTitles", String(_KNOWN_FOR_TITLES_LENGTH)),
+                Column("primaryProfession", Text),
+                Column("knownForTitles", Text),
             ],
         ),
         (
             ImdbDataset.TITLE_AKAS,
             [
                 Column("titleId", String(_TCONST_LENGTH), nullable=False, primary_key=True),
                 Column("ordering", Integer, nullable=False, primary_key=True),
-                Column("title", String(_TITLE_LENGTH)),
-                Column("region", String(_REGION_LENGTH)),
-                Column("language", String(_LANGUAGE_LENGTH)),
-                Column("types", String(_ALIAS_TYPES_LENGTH)),
-                Column("attributes", String(_ATTRIBUTES_LENGTH)),
+                Column("title", Text),
+                Column("region", Text),
+                Column("language", Text),
+                Column("types", Text),
+                Column("attributes", Text),
                 # NOTE: isOriginalTitle sometimes actually is null.
                 Column("isOriginalTitle", Boolean),
             ],
         ),
         (
             ImdbDataset.TITLE_CREW,
             [
                 Column("tconst", String(_TCONST_LENGTH), nullable=False, primary_key=True),
-                Column("directors", String((_NCONST_LENGTH + 1) * _CREW_COUNT - 1)),
-                Column("writers", String((_NCONST_LENGTH + 1) * _CREW_COUNT - 1)),
+                Column("directors", Text),
+                Column("writers", Text),
             ],
         ),
         (
             ImdbDataset.TITLE_EPISODE,
             [
                 Column("tconst", String(_TCONST_LENGTH), nullable=False, primary_key=True),
                 Column("parentTconst", String(_TCONST_LENGTH), nullable=False),
@@ -166,49 +144,47 @@
         ),
         (
             ImdbDataset.TITLE_PRINCIPALS,
             [
                 Column("tconst", String(_TCONST_LENGTH), nullable=False, primary_key=True),
                 Column("ordering", Integer, nullable=False, primary_key=True),
                 Column("nconst", String(_NCONST_LENGTH), index=True, nullable=False),
-                Column("category", String(_PROFESSION_LENGTH), nullable=False),
-                Column("job", String(_JOB_LENGTH)),
-                Column("characters", String(_CHARACTERS_LENGTH)),
+                Column("category", Text, nullable=False),
+                Column("job", Text),
+                Column("characters", Text),
             ],
         ),
         (
             ImdbDataset.TITLE_RATINGS,
             [
-                Column("tconst", String, nullable=False, primary_key=True),
+                Column("tconst", String(_TCONST_LENGTH), nullable=False, primary_key=True),
                 Column("averageRating", Float, nullable=False),
                 Column("numVotes", Integer, nullable=False),
             ],
         ),
     ]
 
 
-def _key_table_info(
-    normalized_table_key: NormalizedTableKey, name_length: int
-) -> Tuple[NormalizedTableKey, List[Union[Column, Index]]]:
+def _key_table_info(normalized_table_key: NormalizedTableKey) -> tuple[NormalizedTableKey, list[Union[Column, Index]]]:
     assert isinstance(normalized_table_key, NormalizedTableKey)
     return (
         normalized_table_key,
         [
             Column("id", Integer, nullable=False, primary_key=True),
-            Column("name", String(name_length), index=True, nullable=False, unique=True),
+            Column("name", Text, index=True, nullable=False, unique=True),
         ],
     )
 
 
 def _ordered_relation_table_info(
     index_name_pool: NamePool,
     table_to_create: NormalizedTableKey,
     from_table: NormalizedTableKey,
     to_table: NormalizedTableKey,
-) -> Tuple[NormalizedTableKey, List[Union[Column, Index]]]:
+) -> tuple[NormalizedTableKey, list[Union[Column, Index]]]:
     """
     Information required to create a table representing an ordered relation
     pointing from ``from_table`` to ``to_table``, including the necessary
     indexes and constraints.
     """
     assert isinstance(table_to_create, NormalizedTableKey)
     assert isinstance(from_table, NormalizedTableKey)
@@ -229,38 +205,38 @@
                 unique=True,
             ),
             Index(index_name_pool.name(f"index__{report_table_name}__{to_table_name}_id"), f"{to_table_name}_id"),
         ],
     )
 
 
-def report_table_infos(index_name_pool: NamePool) -> List[Tuple[NormalizedTableKey, List[Union[Column, Index]]]]:
+def report_table_infos(index_name_pool: NamePool) -> list[tuple[NormalizedTableKey, list[Union[Column, Index]]]]:
     return [
-        _key_table_info(NormalizedTableKey.CHARACTER, _CHARACTER_LENGTH),
+        _key_table_info(NormalizedTableKey.CHARACTER),
         (
             NormalizedTableKey.EPISODE,
             [
-                Column("title_id", Integer, ForeignKey(f"title.id"), nullable=False, primary_key=True),
-                Column("parent_title_id", Integer, ForeignKey(f"title.id"), nullable=False),
+                Column("title_id", Integer, ForeignKey("title.id"), nullable=False, primary_key=True),
+                Column("parent_title_id", Integer, ForeignKey("title.id"), nullable=False),
                 Column("season", Integer),
                 Column("episode", Integer),
             ],
         ),
-        _key_table_info(NormalizedTableKey.GENRE, _GENRE_LENGTH),
-        _key_table_info(NormalizedTableKey.PROFESSION, _PROFESSION_LENGTH),
-        _key_table_info(NormalizedTableKey.TITLE_TYPE, _TITLE_TYPE_LENGTH),
+        _key_table_info(NormalizedTableKey.GENRE),
+        _key_table_info(NormalizedTableKey.PROFESSION),
+        _key_table_info(NormalizedTableKey.TITLE_TYPE),
         (
             NormalizedTableKey.NAME,
             [
                 Column("id", Integer, nullable=False, primary_key=True),
                 Column("nconst", String(_NCONST_LENGTH), index=True, nullable=False, unique=True),
-                Column("primary_name", String(_TITLE_LENGTH), nullable=False),
+                Column("primary_name", Text, nullable=False),
                 Column("birth_year", Integer),
                 Column("death_year", Integer),
-                Column("primary_professions", String((_PROFESSION_LENGTH + 1) * _PROFESSION_COUNT - 1)),
+                Column("primary_professions", Text),
             ],
         ),
         _ordered_relation_table_info(
             index_name_pool,
             NormalizedTableKey.NAME_TO_KNOWN_FOR_TITLE,
             NormalizedTableKey.NAME,
             NormalizedTableKey.TITLE,
@@ -269,15 +245,15 @@
             NormalizedTableKey.PARTICIPATION,
             [
                 Column("id", Integer, nullable=False, primary_key=True),
                 Column("title_id", Integer, ForeignKey("title.id"), nullable=False),
                 Column("ordering", Integer, nullable=False),
                 Column("name_id", Integer, ForeignKey("name.id"), index=True, nullable=False),
                 Column("profession_id", Integer, ForeignKey("profession.id")),
-                Column("job", String(_JOB_LENGTH)),
+                Column("job", Text),
                 Index(
                     index_name_pool.name("index__participation__title_id__ordering"),
                     "title_id",
                     "ordering",
                     unique=True,
                 ),
             ],
@@ -287,68 +263,68 @@
             NormalizedTableKey.PARTICIPATION_TO_CHARACTER,
             NormalizedTableKey.PARTICIPATION,
             NormalizedTableKey.CHARACTER,
         ),
         (
             NormalizedTableKey.TEMP_CHARACTERS_TO_CHARACTER,
             [
-                Column(f"characters", String(_CHARACTERS_LENGTH), nullable=False),
+                Column("characters", Text, nullable=False),
                 Column("ordering", Integer, nullable=False),
-                Column(f"character_id", Integer, ForeignKey(f"character.id"), nullable=False),
+                Column("character_id", Integer, ForeignKey("character.id"), nullable=False),
                 Index(index_name_pool.name("index__name__characters__ordering"), "characters", "ordering", unique=True),
             ],
         ),
         (
             NormalizedTableKey.TITLE,
             [
                 Column("id", Integer, nullable=False, primary_key=True),
                 Column("tconst", String(_TCONST_LENGTH), index=True, nullable=False, unique=True),
                 Column("title_type_id", Integer, ForeignKey("title_type.id"), nullable=False),
-                Column("primary_title", String(_TITLE_LENGTH), nullable=False),
-                Column("original_title", String(_TITLE_LENGTH), nullable=False),
+                Column("primary_title", Text, nullable=False),
+                Column("original_title", Text, nullable=False),
                 Column("is_adult", Boolean, nullable=False),
                 Column("start_year", Integer),
                 Column("end_year", Integer),
                 Column("runtime_minutes", Integer),
                 Column("average_rating", Float, default=0.0, nullable=False),
                 Column("rating_count", Integer, default=0, nullable=False),
             ],
         ),
         (
             NormalizedTableKey.TITLE_ALIAS,
             [
                 Column("id", Integer, nullable=False, primary_key=True),
                 Column("title_id", Integer, ForeignKey("title.id"), nullable=False),
                 Column("ordering", Integer, nullable=False),
-                Column("title", String(_TITLE_LENGTH), nullable=False),
-                Column("region_code", String(_REGION_LENGTH)),
-                Column("language_code", String(_LANGUAGE_LENGTH)),
+                Column("title", Text, nullable=False),
+                Column("region_code", Text),
+                Column("language_code", Text),
                 # NOTE: is_original_title sometimes actually is null.
                 Column("is_original_title", Boolean),
                 Index(
                     index_name_pool.name("index__title_alias__title_id__ordering"), "title_id", "ordering", unique=True
                 ),
             ],
         ),
         _ordered_relation_table_info(
             index_name_pool,
             NormalizedTableKey.TITLE_ALIAS_TO_TITLE_ALIAS_TYPE,
             NormalizedTableKey.TITLE_ALIAS,
             NormalizedTableKey.TITLE_ALIAS_TYPE,
         ),
-        _key_table_info(NormalizedTableKey.TITLE_ALIAS_TYPE, _ALIAS_TYPE_LENGTH),
+        _key_table_info(NormalizedTableKey.TITLE_ALIAS_TYPE),
         _ordered_relation_table_info(
             index_name_pool, NormalizedTableKey.TITLE_TO_GENRE, NormalizedTableKey.TITLE, NormalizedTableKey.GENRE
         ),
     ]
 
 
 def typed_column_to_value_map(
-    table: Table, column_name_to_raw_value_map: Dict[str, str]
-) -> Dict[str, Optional[Union[bool, float, int, str]]]:
+    table: Table, column_name_to_raw_value_map: dict[str, str]
+) -> dict[str, Optional[Union[bool, float, int, str]]]:
     result = {}
     for column in table.columns:
         raw_value = column_name_to_raw_value_map[column.name]
         column_python_type = column.type.python_type
         if raw_value == "\\N":
             value = None
             if not column.nullable:
@@ -485,15 +461,15 @@
         return self._engine
 
     @property
     def metadata(self) -> MetaData:
         return self._metadata
 
     @property
-    def imdb_dataset_to_table_map(self) -> Dict[ImdbDataset, Table]:
+    def imdb_dataset_to_table_map(self) -> dict[ImdbDataset, Table]:
         assert self._imdb_dataset_to_table_map is not None, f"call {self.create_imdb_dataset_tables.__name__} first"
         return self._imdb_dataset_to_table_map
 
     def normalized_table_for(self, report_table_key: NormalizedTableKey) -> Table:
         return self._normalized_name_to_table_map[report_table_key]
 
     def _add_report_table(self, table: Table):
@@ -514,15 +490,15 @@
 
     def _natural_key_to_id_map(
         self,
         connection: Connection,
         normalized_table_key: NormalizedTableKey,
         natural_key_column: str = "name",
         id_column: str = "id",
-    ) -> Dict[str, int]:
+    ) -> dict[str, int]:
         table = self.normalized_table_for(normalized_table_key)
         log.info("  building mapping from %s.%s to %s.%s", table.name, natural_key_column, table.name, id_column)
         name_id_select = select([getattr(table.columns, natural_key_column), getattr(table.columns, id_column)])
         result = {name: id_ for name, id_ in connection.execute(name_id_select)}
         log.info("    found %d entries", len(result))
         return result
 
@@ -600,15 +576,15 @@
 
     def _drop_obsolete_normalized_tables(self):
         obsolete_table_names = ["characters_to_character", "title_to_director", "title_to_writer"]
         for obsolete_table_name in obsolete_table_names:
             obsolete_table = Table(obsolete_table_name, self._metadata, Column("_dummy", Integer))
             obsolete_table.drop(self._engine, checkfirst=True)
 
-    def key_columns(self, imdb_dataset: ImdbDataset) -> Tuple:
+    def key_columns(self, imdb_dataset: ImdbDataset) -> tuple:
         return tuple(
             column.name for column in self.imdb_dataset_to_table_map[imdb_dataset].columns if column.primary_key
         )
 
     def build_key_table_from_query(
         self,
         connection: Connection,
@@ -676,15 +652,17 @@
             )
 
     def build_profession_table(self, connection: Connection):
         title_principals_table = self.imdb_dataset_to_table_map[ImdbDataset.TITLE_PRINCIPALS]
         category_column = title_principals_table.c.category
         with connection.begin():
             self.build_key_table_from_query(
-                connection, NormalizedTableKey.PROFESSION, select([category_column]).distinct(),
+                connection,
+                NormalizedTableKey.PROFESSION,
+                select([category_column]).distinct(),
             )
 
     def build_participation_table(self, connection: Connection):
         participation_table = self.normalized_table_for(NormalizedTableKey.PARTICIPATION)
         with TableBuildStatus(connection, participation_table) as table_build_status:
             name_table = self.normalized_table_for(NormalizedTableKey.NAME)
             title_table = self.normalized_table_for(NormalizedTableKey.TITLE)
@@ -946,15 +924,17 @@
                 source_table_count,
                 source_table.name,
             )
 
     def check_table_has_data(self, connection: Connection, target_table: Table):
         target_table_count = table_count(connection, target_table)
         if target_table_count == 0:
-            log.warning('target table "%s" should contain rows but is empty',)
+            log.warning(
+                'target table "%s" should contain rows but is empty',
+            )
 
     def build_episode_table(self, connection: Connection):
         episode_table = self.normalized_table_for(NormalizedTableKey.EPISODE)
         with TableBuildStatus(connection, episode_table) as table_build_status:
             title_for_title_alias = self.normalized_table_for(NormalizedTableKey.TITLE).alias("title_for_title")
             title_for_parent_title_alias = self.normalized_table_for(NormalizedTableKey.TITLE).alias(
                 "title_for_parent_title"
@@ -1008,15 +988,15 @@
                     for title_id, genres in connection.execute(select_genre_data):
                         for ordering, genre in enumerate(genres.split(","), start=1):
                             genre_id = genre_name_to_id_map[genre]
                             bulk_insert.add({"genre_id": genre_id, "ordering": ordering, "title_id": title_id})
                     table_build_status.log_added_rows(bulk_insert.count)
 
     @functools.lru_cache(None)
-    def mappable_title_alias_types(self, raw_title_types: str) -> List[str]:
+    def mappable_title_alias_types(self, raw_title_types: str) -> list[str]:
         # TODO: Make inner function of build_title_alias_to_title_alias_type_table().
         result = []
         if raw_title_types:
             remaining_raw_title_alias_types = raw_title_types
             for title_alias_type_to_check in IMDB_TITLE_ALIAS_TYPES:
                 if title_alias_type_to_check in remaining_raw_title_alias_types:
                     result.append(title_alias_type_to_check)
@@ -1096,17 +1076,19 @@
                     )
                 )
                 .where(title_akas_types_column.isnot(None))
             )
             with connection.begin():
                 table_build_status.clear_table()
                 with BulkInsert(connection, title_alias_to_title_alias_type_table, self._bulk_size) as bulk_insert:
-                    for (title_alias_id, title_alias_ordering, raw_title_alias_types,) in connection.execute(
-                        select_title_akas_data
-                    ):
+                    for (
+                        title_alias_id,
+                        title_alias_ordering,
+                        raw_title_alias_types,
+                    ) in connection.execute(select_title_akas_data):
                         for title_alias_type_ordering, title_alias_type_name in enumerate(
                             self.mappable_title_alias_types(raw_title_alias_types), start=1
                         ):
                             title_alias_type_id = title_alias_type_name_to_id_map[title_alias_type_name]
                             bulk_insert.add(
                                 {
                                     "title_alias_id": title_alias_id,
```

## Comparing `pimdb-0.2.3.dist-info/LICENSE.txt` & `pimdb-0.3.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pimdb-0.2.3.dist-info/METADATA` & `pimdb-0.3.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: pimdb
-Version: 0.2.3
+Version: 0.3.0
 Summary: build a database from IMDb datasets
 Home-page: https://github.com/roskakori/pimdb
 Author: Thomas Aglassinger
 Author-email: roskakori@users.sourceforge.net
 License: BSD
 Project-URL: Documentation, https://pimdb.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/roskakori/pimdb/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 Requires-Dist: requests
-Requires-Dist: sqlalchemy (>=1.3)
+Requires-Dist: sqlalchemy <2,>=1.4
 Provides-Extra: postgres
-Requires-Dist: psycopg2-binary (>=2.5) ; extra == 'postgres'
+Requires-Dist: psycopg2-binary >=2.5 ; extra == 'postgres'
 
 # pimdb
 
 Pimdb is a python package and command line utility to maintain a local copy of
 the essential parts of the
 [Internet Movie Database](https://imdb.com) (IMDb) based in the TSV files
 available from [IMDb datasets](https://www.imdb.com/interfaces/).
@@ -58,15 +59,15 @@
 
 
 ## Quick start
 
 
 ### Downloading datasets
 
-To download the current IMDb datsets to the current folder, run:
+To download the current IMDb datasets to the current folder, run:
 
 ```bash
 pimdb download all
 ```
 
 (This downloads about 1 GB of data and might take a couple of minutes).
 
@@ -76,18 +77,17 @@
 To import them in a local SQLite database `pimdb.db` located in the current
 folder, run:
 
 ```bash
 pimdb transfer all
 ```
 
-(This will take a while. On a reasonably modern laptop with a local database
-you can expect about 2 hours).
+This will take several hours, on a MacBook Pro M1 about 11 hours.
 
-The resulting database contains one tables for each dataset. The table names
+The resulting database contains one table for each dataset. The table names
 are PascalCase variants of the dataset name. For example, the date from the
 dataset `title.basics` are stored in the table `TitleBasics`. The column names
 in the table match the names from the datasets, for example
 `TitleBasics.primaryTitle`. A short description of all the datasets and
 columns can be found at the download page for the
 [IMDb datasets](https://www.imdb.com/interfaces/).
 
@@ -136,14 +136,15 @@
 pimdb build
 ```
 If you did specify a `--database` for the `transfer` command before, you have to
 specify the same value for `build` in order to find the source data. These tables
 generally use snake_case names for both tables and columns, for example
 `title_allias.is_original`.
 
+This will take some time, on a MacBook Pro M1 about 30 minutes.
 
 ## Querying normalized tables
 
 N:M relations are stored in tables using the naming template `some_to_other`,
 for example `name_to_known_for_title`. These relation tables contain only the
 numeric ID's to the respective actual data and a numeric column `ordering` to
 remember the sort order of the comma separated list in the IMDb dataset column.
@@ -178,9 +179,7 @@
 
 * [Usage](https://pimdb.readthedocs.io/en/latest/usage.html): all command line
   options explained
 * [Data model](https://pimdb.readthedocs.io/en/latest/datamodel.html):
   available tables and example SQL queries
 * [Contributing](https://pimdb.readthedocs.io/en/latest/contributing.html):
   obtaining the source code and building the project locally
-
-
```

