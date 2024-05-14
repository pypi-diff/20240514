# Comparing `tmp/sqldatamodel-0.5.2.tar.gz` & `tmp/sqldatamodel-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqldatamodel-0.5.2.tar", last modified: Mon May 13 20:02:20 2024, max compression
+gzip compressed data, was "sqldatamodel-0.6.0.tar", last modified: Tue May 14 19:15:04 2024, max compression
```

## Comparing `sqldatamodel-0.5.2.tar` & `sqldatamodel-0.6.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 20:02:20.331551 sqldatamodel-0.5.2/
--rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 sqldatamodel-0.5.2/LICENSE
--rw-rw-rw-   0        0        0    29574 2024-05-13 20:02:20.320546 sqldatamodel-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0    27682 2024-05-13 19:59:36.000000 sqldatamodel-0.5.2/README.md
--rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 sqldatamodel-0.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 20:02:20.332550 sqldatamodel-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0     2424 2024-05-13 19:59:51.000000 sqldatamodel-0.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 20:02:18.364786 sqldatamodel-0.5.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-13 20:02:19.562318 sqldatamodel-0.5.2/src/SQLDataModel/
--rw-rw-rw-   0        0        0     6644 2024-05-03 15:03:44.000000 sqldatamodel-0.5.2/src/SQLDataModel/ANSIColor.py
--rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 sqldatamodel-0.5.2/src/SQLDataModel/HTMLParser.py
--rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 sqldatamodel-0.5.2/src/SQLDataModel/JSONEncoder.py
--rw-rw-rw-   0        0        0   621050 2024-05-13 20:01:36.000000 sqldatamodel-0.5.2/src/SQLDataModel/SQLDataModel.py
--rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 sqldatamodel-0.5.2/src/SQLDataModel/StandardDeviation.py
--rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 sqldatamodel-0.5.2/src/SQLDataModel/__init__.py
--rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 sqldatamodel-0.5.2/src/SQLDataModel/converters.py
--rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 sqldatamodel-0.5.2/src/SQLDataModel/demo.py
--rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 sqldatamodel-0.5.2/src/SQLDataModel/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-13 20:02:20.222090 sqldatamodel-0.5.2/src/SQLDataModel/extensions/
--rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 sqldatamodel-0.5.2/src/SQLDataModel/extensions/__init__.py
--rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 sqldatamodel-0.5.2/src/SQLDataModel/extensions/str_utils.c
-drwxrwxrwx   0        0        0        0 2024-05-13 20:02:20.313154 sqldatamodel-0.5.2/src/SQLDataModel.egg-info/
--rw-rw-rw-   0        0        0    29574 2024-05-13 20:02:18.000000 sqldatamodel-0.5.2/src/SQLDataModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2024-05-13 20:02:18.000000 sqldatamodel-0.5.2/src/SQLDataModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 20:02:18.000000 sqldatamodel-0.5.2/src/SQLDataModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-13 20:02:18.000000 sqldatamodel-0.5.2/src/SQLDataModel.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 20:02:20.242314 sqldatamodel-0.5.2/tests/
--rw-rw-rw-   0        0        0    66698 2024-05-13 17:45:04.000000 sqldatamodel-0.5.2/tests/test_Future.py
--rw-rw-rw-   0        0        0    66701 2024-05-13 17:46:25.000000 sqldatamodel-0.5.2/tests/test_SQLDataModel.py
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:04.389385 sqldatamodel-0.6.0/
+-rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 sqldatamodel-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0    29574 2024-05-14 19:15:04.379209 sqldatamodel-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0    27682 2024-05-13 19:59:36.000000 sqldatamodel-0.6.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 sqldatamodel-0.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-14 19:15:04.390978 sqldatamodel-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     2424 2024-05-14 19:13:27.000000 sqldatamodel-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:02.932979 sqldatamodel-0.6.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:04.105123 sqldatamodel-0.6.0/src/SQLDataModel/
+-rw-rw-rw-   0        0        0     6644 2024-05-03 15:03:44.000000 sqldatamodel-0.6.0/src/SQLDataModel/ANSIColor.py
+-rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 sqldatamodel-0.6.0/src/SQLDataModel/HTMLParser.py
+-rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 sqldatamodel-0.6.0/src/SQLDataModel/JSONEncoder.py
+-rw-rw-rw-   0        0        0   627438 2024-05-14 19:12:42.000000 sqldatamodel-0.6.0/src/SQLDataModel/SQLDataModel.py
+-rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 sqldatamodel-0.6.0/src/SQLDataModel/StandardDeviation.py
+-rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 sqldatamodel-0.6.0/src/SQLDataModel/__init__.py
+-rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 sqldatamodel-0.6.0/src/SQLDataModel/converters.py
+-rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 sqldatamodel-0.6.0/src/SQLDataModel/demo.py
+-rw-rw-rw-   0        0        0     2820 2024-05-14 15:14:12.000000 sqldatamodel-0.6.0/src/SQLDataModel/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:04.296754 sqldatamodel-0.6.0/src/SQLDataModel/extensions/
+-rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 sqldatamodel-0.6.0/src/SQLDataModel/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 sqldatamodel-0.6.0/src/SQLDataModel/extensions/str_utils.c
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:04.372209 sqldatamodel-0.6.0/src/SQLDataModel.egg-info/
+-rw-rw-rw-   0        0        0    29574 2024-05-14 19:15:02.000000 sqldatamodel-0.6.0/src/SQLDataModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2024-05-14 19:15:02.000000 sqldatamodel-0.6.0/src/SQLDataModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 19:15:02.000000 sqldatamodel-0.6.0/src/SQLDataModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-14 19:15:02.000000 sqldatamodel-0.6.0/src/SQLDataModel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:15:04.313944 sqldatamodel-0.6.0/tests/
+-rw-rw-rw-   0        0        0    69579 2024-05-14 19:12:35.000000 sqldatamodel-0.6.0/tests/test_Future.py
+-rw-rw-rw-   0        0        0    69582 2024-05-14 19:12:37.000000 sqldatamodel-0.6.0/tests/test_SQLDataModel.py
```

### Comparing `sqldatamodel-0.5.2/LICENSE` & `sqldatamodel-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.5.2/PKG-INFO` & `sqldatamodel-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.5.2
+Version: 0.6.0
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal-tables,pretty-print-tables,sql2sql,data-analysis,data-science,datamodel,extract,transform,load,web-scraping-tables,data-mining,html,html-table-parsing,apache-arrow,pyarrow,pyarrow-conversion,pyarrow-to-table,pyarrow-to-sql,pyarrow-to-csv,parquet-file-parsing,csv,csv-parsing,markdown,markdown-table-parsing,latex,latex-table-parsing,delimited,delimited-data-parsing,file-conversion,format-conversion,terminal-styling,table-styling,from-sqlite,to-sqlite,from-postgresql,to-postgresql,sql-to-sql,excel,xlsx-file,excel-to-sql,DataFrames,polars2pandas,pandas2polars
```

### Comparing `sqldatamodel-0.5.2/README.md` & `sqldatamodel-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.5.2/setup.py` & `sqldatamodel-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='SQLDataModel',  
-     version='0.5.2',
+     version='0.6.0',
      scripts=['src/SQLDataModel/SQLDataModel.py'] ,
      author='Ante Tonkovic-Capin',
      author_email='antetc@icloud.com',
      description='SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.',
      keywords=['SQL','ETL','dataframe','terminal-tables','pretty-print-tables','sql2sql','data-analysis','data-science','datamodel','extract','transform','load','web-scraping-tables','data-mining','html','html-table-parsing','apache-arrow','pyarrow','pyarrow-conversion','pyarrow-to-table','pyarrow-to-sql','pyarrow-to-csv','parquet-file-parsing','csv','csv-parsing','markdown','markdown-table-parsing','latex','latex-table-parsing','delimited','delimited-data-parsing','file-conversion','format-conversion','terminal-styling','table-styling','from-sqlite','to-sqlite','from-postgresql','to-postgresql','sql-to-sql','excel','xlsx-file','excel-to-sql','DataFrames','polars2pandas','pandas2polars'],
      license_file='LICENSE',
      long_description=long_description,
```

### Comparing `sqldatamodel-0.5.2/src/SQLDataModel/ANSIColor.py` & `sqldatamodel-0.6.0/src/SQLDataModel/ANSIColor.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.5.2/src/SQLDataModel/HTMLParser.py` & `sqldatamodel-0.6.0/src/SQLDataModel/HTMLParser.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.5.2/src/SQLDataModel/JSONEncoder.py` & `sqldatamodel-0.6.0/src/SQLDataModel/JSONEncoder.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.5.2/src/SQLDataModel/SQLDataModel.py` & `sqldatamodel-0.6.0/src/SQLDataModel/SQLDataModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1388,18 +1388,18 @@
             apply_function = lambda x: "_".join(x.strip() for x in re.sub('[^0-9a-z_]+', '', x.lower().replace(" ","_")).split('_') if x !='')
         new_headers = [apply_function(x) for x in self.get_headers()]
         self.set_headers(new_headers)
         return
 
     def get_display_max_rows(self) -> int|None:
         """
-        Retrieves the current value of the ``display_max_rows`` property, which determines the maximum rows displayed for ``SQLDataModel``.
+        Retrieves the current value at :py:attr:`SQLDataModel.display_max_rows`, which determines the maximum rows displayed for the ``SQLDataModel``.
 
         Returns:
-            ``int`` or ``None``: The current value set on :py:attr:`SQLDataModel.display_max_rows`.
+            ``int`` or ``None``: The current value set at :py:attr:`SQLDataModel.display_max_rows`.
 
         Example::
 
             from SQLDataModel import SQLDataModel
 
             # Create model
             sdm = SQLDataModel.from_csv('example.csv', headers=['ID', 'Name', 'Value'])
@@ -1433,18 +1433,18 @@
         Example::
         
             from SQLDataModel import SQLDataModel
 
             # Create model
             sdm = SQLDataModel.from_csv('example.csv', headers=['ID', 'Name', 'Value'])
 
-            # Any call to ``print`` or ``repr`` will be restricted to 500 max rows
+            # Any call to `print` or `repr` will be restricted to 500 max rows
             sdm.set_display_max_rows(500)
 
-            # Alternatively, auto-detect dimensions by setting to ``None``
+            # Alternatively, auto-detect dimensions by setting to `None`
             sdm.set_display_max_rows(None)
         
         Note:
             - Modifying :py:attr:`SQLDataModel.display_max_rows` does not affect the actual number of rows in the model, only the maximum rows **displayed**.
         """
         if not isinstance(rows, (int,type(None))):
             raise TypeError(
@@ -1575,17 +1575,16 @@
 
             # Get the current alignment value
             alignment = sdm.get_column_alignment()
 
             # Outputs 'dynamic'
             print(alignment)
 
-        Related:
-            - See :meth:`SQLDataModel.set_column_alignment` to configure table alignment
-        
+        Note:
+            - Use :meth:`SQLDataModel.set_column_alignment()` to modify column alignment.
         """
         return self.column_alignment
     
     def set_column_alignment(self, alignment:Literal['dynamic', 'left', 'center', 'right']='dynamic') -> None:
         """
         Sets the default alignment behavior for ``SQLDataModel`` when ``repr`` or ``print`` is called, modifies ``column_alignment`` attribute.
         Default behavior set to ``'dynamic'``, which right-aligns numeric data types, left-aligns all other types, with headers matching value alignment.
@@ -1607,77 +1606,76 @@
         Example::
 
             from SQLDataModel import SQLDataModel
 
             # Create the model
             sdm = SQLDataModel.from_csv('example.csv', headers=['ID', 'Name', 'Value'])
 
-            # Set to right-align
+            # Set to right-align columns
             sdm.set_column_alignment('right')
 
             # Output
             print(sdm)
         
-        This will output:
+        This will output the model with values right-aligned:
 
         ```shell
             ┌───┬────────┬─────────┬────────┬─────────┐
             │   │  first │    last │    age │ service │
             ├───┼────────┼─────────┼────────┼─────────┤
             │ 0 │   john │   smith │     27 │    1.22 │
             │ 1 │  sarah │    west │     39 │    0.70 │
             │ 2 │   mike │  harlin │     36 │    3.00 │
             │ 3 │    pat │ douglas │     42 │   11.50 │
             └───┴────────┴─────────┴────────┴─────────┘        
         ```
+
+        Setting columns to be left-aligned:
+
         ```python            
             # Set to left-align
             sdm.set_column_alignment('left')
 
             # Output
             print(sdm)
         ```
 
-        This will output:
+        This will output the model with left-aligned values instead:
 
-        ```shell            
+        ```text            
             ┌───┬────────┬─────────┬────────┬─────────┐
             │   │ first  │ last    │ age    │ service │
             ├───┼────────┼─────────┼────────┼─────────┤
             │ 0 │ john   │ smith   │  27    │  1.22   │
             │ 1 │ sarah  │ west    │  39    │  0.70   │
             │ 2 │ mike   │ harlin  │  36    │  3.00   │
             │ 3 │ pat    │ douglas │  42    │  11.50  │
             └───┴────────┴─────────┴────────┴─────────┘        
         ```
 
         Note:
-            - The options for 'left' and 'right' mirror the '<' and '>' f-string formatters, respectively.
+            - Use :meth:`SQLDataModel.get_column_alignment()` to return the current column alignment setting.
             - When using 'center', if the column contents cannot be perfectly centralized, the left side will be favored.
             - Use 'dynamic' to return to default column alignment, which is right-aligned for numeric types and left-aligned for others.
-
-        Related:
-            - :meth:`SQLDataModel.get_column_alignment` to return the current setting for column alignment.
-
+            - See :meth:`SQLDataModel.set_table_style()` for modifying table format and available styles.
         """
         if not isinstance(alignment, str):
             raise TypeError(
                 SQLDataModel.ErrorFormat(f"TypeError: invalid type '{type(alignment).__name__}', expected type for `alignment` to be type 'str', setting the alignment style to use")
             )
         if alignment not in ('dynamic', 'left', 'center', 'right'):
             raise ValueError(
                 SQLDataModel.ErrorFormat(f"ValueError: invalid value '{alignment}', argument for `alignment` must be one of 'dynamic', 'left', 'center', 'right' representing the column alignment setting, use 'dynamic' for default behaviour")
                 )
         self.column_alignment = alignment
         return
 
     def get_display_index(self) -> bool:
         """
-        Returns the current boolean value for ``is_display_index``, which determines
-        whether or not the ``SQLDataModel`` index will be shown in print or repr calls.
+        Returns the current value set at :py:attr:`SQLDataModel.display_index`, which determines whether or not the index is displayed in the ``SQLDataModel`` representation.
 
         Returns:
             ``bool``: The current value of the ``display_index`` property.
 
         Example::
         
             from SQLDataModel import SQLDataModel
@@ -1687,25 +1685,26 @@
 
             # Get the current value for displaying the index
             display_index = sdm.get_display_index()
 
             # Output: True
             print(display_index)
         
+        Note:
+            - Use :meth:`SQLDataModel.set_display_index()` to modify this property and toggle index display visibility.
         """
         return self.display_index
 
     def set_display_index(self, display_index:bool) -> None:
         """
-        Sets the ``display_index`` property to enable or disable the inclusion of the
-        ``SQLDataModel`` index value in print or repr calls, default set to include.
+        Sets the value for :py:attr:`SQLDataModel.display_index` to enable or disable the inclusion of the
+        ``SQLDataModel`` index value in print or repr calls.
 
         Parameters:
-            ``display_index`` (bool): A boolean value (True | False) to determine whether
-            to include the index in print or repr calls.
+            ``display_index`` (bool): Whether or not to include the index in ``SQLDataModel`` representations.
 
         Raises:
             ``TypeError``: If the provided argument is not a boolean value.
 
         Returns:
             ``None``
 
@@ -1715,18 +1714,20 @@
 
             # Create the model
             sdm = SQLDataModel.from_csv('example.csv', headers=['ID', 'Name', 'Value'])
 
             # Disable displaying index
             sdm.set_display_index(False)
 
+        Note:
+            - Use :meth:`SQLDataModel.set_table_style()` to more broadly modify the appearance and formatting style of ``SQLDataModel`` string representations.
         """
         if not isinstance(display_index, bool):
             raise TypeError(
-                SQLDataModel.ErrorFormat(f'TypeError: invalid argument "{display_index}", please provide a valid boolean (True | False) value to the `display_index` argument...')
+                SQLDataModel.ErrorFormat(f"TypeError: invalid type '{type(display_index).__name__}', argument for `display_index` must be of type 'bool' representating whether or not the index should be displayed")
                 )
         self.display_index = display_index
     
     def get_shape(self) -> tuple[int, int]:
         """
         Returns the current shape of the ``SQLDataModel`` as a tuple of ``(rows x columns)``.
 
@@ -1782,15 +1783,15 @@
 
         Change Log:
             - Version 0.3.6 (2024-04-09):
                 - Returns the new :py:attr:`SQLDataModel.shape` directly, making this method redundant.
 
         Note:
             - If an empty model is initialized, the :py:attr:`SQLDataModel.row_count` will be 0 until the first row is inserted.
-            - Using the :meth:`SQLDataModel.__getitem__` syntax of ``sdm[row, col]`` returns a new model instance with the corresponding shape.
+            - Using the :meth:`SQLDataModel.__getitem__()` syntax of ``sdm[row, col]`` returns a new model instance with the corresponding shape.
         """
         return self.shape
     
     def get_display_float_precision(self) -> int:
         """
         Retrieves the current float display precision used exclusively for representing the values of real numbers
         in the ``repr`` method for the ``SQLDataModel``. Default value is set to 4 decimal places of precision.
@@ -7736,15 +7737,15 @@
         if not isinstance(update_values, (str,int,float,bool,bytes,list,tuple,datetime.date)) and (update_values is not None):
             raise TypeError(
                 SQLDataModel.ErrorFormat(f"TypeError: invalid values type '{type(update_values).__name__}', update values must be compatible with SQL datatypes such as <'str', 'int', 'float', 'datetime', 'bool', 'bytes'>")
             )
         # short circuit remaining operations and proceed to insert row if target_indicies is int and equals current row count
         if isinstance(target_indicies, int) and target_indicies == self.row_count:
             try:
-                self.insert_row(update_values)
+                self.append_row(update_values)
                 return
             except TypeError as e:
                 raise TypeError(
                     SQLDataModel.ErrorFormat(f"{e}")
                 ) from None                
             except DimensionError as e:
                 raise DimensionError(
@@ -8209,20 +8210,98 @@
         # table_low_bar = "".join([low_lh, low_sep.join([low_hbar * header_length_dict[col] for col in display_headers]), low_rh, table_bare_newline])
         table_low_bar = "".join([low_lh, low_sep.join([low_hbar * length for length in col_lengths]), low_rh, table_bare_newline])
         table_low_bar = table_low_bar if len(table_low_bar.strip()) >=1 else """"""
         table_repr = "".join([table_repr, table_low_bar])
         table_caption = f"""[{self.row_count} rows x {self.column_count} columns]"""
         table_repr = "".join([table_repr, table_caption])
         return table_repr if self.display_color is None else self.display_color.wrap(table_repr) 
-        return table_repr if self.display_color is None else self.display_color.wrap(table_repr)
     
 ##################################################################################################################
 ############################################## sqldatamodel methods ##############################################
 ##################################################################################################################
 
+    def append_row(self, values:list|tuple=None) -> None:
+        """
+        Appends ``values`` as a new row in the ``SQLDataModel`` at the next available index based on the current max row index from :py:attr:`SQLDataModel.indicies`. If ``values = None``, an empty row with SQL ``null`` values will be used.
+
+        Parameters:
+            ``values`` (list or tuple, optional): The values to be inserted into the row. If not provided or set to None, an empty row with SQL ``null`` values will be inserted.
+
+        Raises:
+            ``TypeError``: If ``values`` is provided and is not of type list or tuple.
+            ``DimensionError``: If the number of values provided does not match the current column count.
+            ``SQLProgrammingError``: If there is an issue with the SQL execution during the insertion.
+        
+        Returns:
+            ``None``
+
+        Example::
+
+            from SQLDataModel import SQLDataModel
+
+            # Create a rowless model
+            sdm = SQLDataModel(headers=['Name', 'Age'])
+
+            # Append a row with values
+            sdm.append_row(['Alice', 31])
+
+            # Append another row
+            sdm.append_row(['John', 48])
+
+            # View result
+            print(sdm)
+        
+        This will output:
+
+        ```text
+            ┌───┬───────┬──────┐
+            │   │ Name  │ Age  │
+            ├───┼───────┼──────┤
+            │ 0 │ Alice │ 31   │
+            │ 1 │ John  │ 48   │
+            └───┴───────┴──────┘
+            [2 rows x 2 columns]
+        ```
+
+        Change Log:
+            - Version 0.6.0 (2024-05-14):
+                - New method, mirrors previous behavior of :meth:`SQLDataModel.insert_row()` for versions <= 0.5.2.
+
+        Note:
+            - If no values are provided, ``None`` or SQL 'null' will be used for the values.
+            - Rows will be appended to the bottom of the model at one index greater than the current max index.
+        """
+        if values is not None:
+            if not isinstance(values, (list,tuple)):
+                raise TypeError(
+                    SQLDataModel.ErrorFormat(f"TypeError: invalid type '{type(values).__name__}', insert values must be of type 'list' or 'tuple'")
+                    ) from None
+            if isinstance(values,list):
+                values = tuple(values)
+            if (len_val := len(values)) != self.column_count:
+                raise DimensionError(
+                    SQLDataModel.ErrorFormat(f"DimensionError: invalid dimensions '{len_val} != {self.column_count}', the number of values provided: '{len_val}' must match the current column count '{self.column_count}'")
+                    ) from None
+        else:
+            values = tuple([None for _ in range(self.column_count)])
+        insert_cols = ",".join([f'"{col}"' for col in self.headers])
+        insert_vals = ",".join(["?" if not isinstance(val,datetime.date) else "datetime(?)" if isinstance(val, datetime.datetime) else "date(?)" for val in values])
+        insert_stmt = f"""insert into {self.sql_model}({insert_cols}) values ({insert_vals})"""
+        sql_cur = self.sql_db_conn.cursor()
+        try:
+            sql_cur.execute(insert_stmt, values)
+            self.sql_db_conn.commit()
+            self._update_indicies_deterministic(sql_cur.lastrowid)
+        except Exception as e:
+            self.sql_db_conn.rollback()
+            raise SQLProgrammingError(
+                SQLDataModel.ErrorFormat(f'SQLProgrammingError: unable to update values, SQL execution failed with: "{e}"')
+            ) from None
+        self._update_model_metadata(update_row_meta=False)  
+
     def concat(self, other:SQLDataModel|list|tuple, inplace:bool=True) -> None|SQLDataModel:
         """
         Concatenates the provided data to ``SQLDataModel`` along the row axis, returning a new model or modifying the existing instance inplace.
 
         Parameters:
             ``other`` (SQLDataModel | list | tuple): The SQLDataModel, list, or tuple to concatenate or append.
             ``inplace`` (bool, optional): If True (default), performs the concatenation in-place, modifying the current model. If False, returns a new ``SQLDataModel`` instance with the concatenated result.
@@ -8881,14 +8960,108 @@
             self._update_model_metadata()
             return
         else:
             other_data = [(t1 + t2) for t1, t2 in zip(self.data(index=False, include_headers=False, strict_2d=True), other_data)]
             dtype_dict = dict(zip(other_headers, other_dtypes))
             return type(self)(data=other_data, headers=other_headers, dtypes=dtype_dict, **self._get_display_args())
 
+    def insert_row(self, index:int, values:list|tuple, on_conflict:Literal['replace','ignore']='replace') -> None:
+        """
+        Inserts a new row into the ``SQLDataModel`` at the specified ``index`` with the provided ``values``.
+
+        Parameters:
+            ``index`` (int): The position at which to insert the row.
+            ``values`` (list or tuple): The values to be inserted into the row.
+            ``on_conflict`` (Literal['replace', 'ignore'], optional): Specifies the action to take if the index already exists. Default is 'replace'.
+
+        Raises:
+            ``TypeError``: If ``index`` is not an integer or ``values`` is not a list or tuple.
+            ``ValueError``: If ``on_conflict`` is not ``'replace'`` or ``'ignore'``.
+            ``DimensionError``: If the dimensions of the provided ``values`` are incompatible with the current model dimensions.
+            ``SQLProgrammingError``: If there is an issue with the SQL execution during the insertion.
+
+        Returns:
+            ``None``
+
+        Example::
+
+            from SQLDataModel import SQLDataModel
+
+            # Sample data
+            data = [('Alice', 20, 'F'), ('Billy', 25, 'M'), ('Chris', 30, 'M')]
+
+            # Create the model
+            sdm = SQLDataModel(data, headers=['Name','Age','Sex'])    
+
+            # Insert a new row at index 3
+            sdm.insert_row(3, ['David', 35, 'M'])
+
+            # Insert or replace row at index 1
+            sdm.insert_row(1, ['Beth', 27, 'F'], on_conflict='replace')
+            
+            # View result
+            print(sdm)
+
+        This will output the modified model:
+
+        ```text
+            ┌───┬───────┬─────┬─────┐
+            │   │ Name  │ Age │ Sex │
+            ├───┼───────┼─────┼─────┤
+            │ 0 │ Alice │  20 │ F   │
+            │ 1 │ Beth  │  27 │ F   │
+            │ 2 │ Chris │  30 │ M   │
+            │ 3 │ David │  35 │ M   │
+            └───┴───────┴─────┴─────┘
+            [4 rows x 3 columns]
+        ```
+
+        Change Log:
+            - Version 0.6.0 (2024-05-14):
+                - Backward incompatible changes made to arguments and behavior, added ``index`` and ``on_conflict`` parameters for greater specificity and to align with broader conventions surrounding insert methods.
+
+        Note:
+            - Use ``on_conflict = 'ignore'`` to take no action if row already exists, and ``on_conflict = 'replace'`` to replace it.
+            - See :meth:`SQLDataModel.append_row()` for appending rows at the next available index instead of insertion at index.
+        """        
+        if not isinstance(index, int):
+            raise TypeError(
+                SQLDataModel.ErrorFormat(f"TypeError: invalid type '{type(index).__name__}', argument for `index` must be of type 'int' representing the row position to insert into")
+            )
+        if not isinstance(values, (list,tuple)):
+            raise TypeError(
+                SQLDataModel.ErrorFormat(f"TypeError: invalid type '{type(values).__name__}', insert values must be of type 'list' or 'tuple'")
+                )
+        if on_conflict not in ('replace','ignore'):
+            raise ValueError(
+                SQLDataModel.ErrorFormat(f"ValueError: invalid value '{on_conflict}', argument for `on_conflict` must be either 'replace' or 'ignore' representing the action to take if specified index already exists")
+            )
+        if isinstance(values,list):
+            values = tuple(values)
+        if (len_val := len(values)) != self.column_count:
+            raise DimensionError(
+                SQLDataModel.ErrorFormat(f"DimensionError: invalid dimensions '{len_val} != {self.column_count}', the number of values provided: '{len_val}' must match the current column count '{self.column_count}'")
+                )
+        values = (index,*values)
+        insert_cols = self.headers if index is None else [self.sql_idx, *self.headers]
+        insert_cols = ",".join([f'"{col}"' for col in insert_cols])
+        insert_vals = ",".join(["?" if not isinstance(val,datetime.date) else "datetime(?)" if isinstance(val, datetime.datetime) else "date(?)" for val in values])
+        insert_stmt = f"""insert or {on_conflict} into {self.sql_model}({insert_cols}) values ({insert_vals})"""
+        sql_cur = self.sql_db_conn.cursor()
+        try:
+            sql_cur.execute(insert_stmt, values)
+            self.sql_db_conn.commit()
+            self._update_indicies_deterministic(sql_cur.lastrowid)
+        except Exception as e:
+            self.sql_db_conn.rollback()
+            raise SQLProgrammingError(
+                SQLDataModel.ErrorFormat(f'SQLProgrammingError: unable to update values, SQL execution failed with: "{e}"')
+            ) from None
+        self._update_model_metadata(update_row_meta=False)
+
     def iter_rows(self, min_row:int=None, max_row:int=None, index:bool=True, include_headers:bool=False) -> Generator:
         """
         Returns a generator object of the rows in the model from ``min_row`` to `max_row`.
 
         Parameters:
             ``min_row`` (int, optional): The minimum row index to start iterating from (inclusive). Defaults to None.
             ``max_row`` (int, optional): The maximum row index to iterate up to (exclusive). Defaults to None.
@@ -10767,89 +10940,14 @@
         Note:
             - This method is to meant as a general informative tool or for debugging assistance if needed
             - See :meth:`SQLDataModel.apply()` method for usage and implementation of functions in SQLDataModel using ``sqlite3`` 
         """
         func_signature = ", ".join([f"""{k.replace(" ","_")}:{v[1]}""" for k,v in self.header_master.items() if k != self.sql_idx])
         return f"""def func({func_signature}):\n    # apply logic and return value\n    return"""
     
-    def insert_row(self, values:list|tuple=None) -> None:
-        """
-        Inserts a row in the ``SQLDataModel`` at index :py:attr:`self.rowcount + 1 <SQLDataModel.row_count>` with provided ``values``. If ``values=None``, an empty row with SQL ``null`` values will be used.
-
-        Parameters:
-            ``values`` (list or tuple, optional): The values to be inserted into the row. If not provided or set to None, an empty row with SQL ``null`` values will be inserted.
-
-        Raises:
-            ``TypeError``: If ``values`` is provided and is not of type list or tuple.
-            ``DimensionError``: If the number of values provided does not match the current column count.
-            ``SQLProgrammingError``: If there is an issue with the SQL execution during the insertion.
-        
-        Returns:
-            ``None``
-
-        Example::
-
-            from SQLDataModel import SQLDataModel
-
-            # Create a rowless model
-            sdm = SQLDataModel(headers=['Name', 'Age'])
-
-            # Insert row with values
-            sdm.insert_row(['Alice',31])
-
-            # Insert another row
-            sdm.insert_row(['John', 48])
-
-            # View result
-            print(sdm)
-        
-        This will output:
-
-        ```shell
-            ┌───┬───────┬──────┐
-            │   │ Name  │ Age  │
-            ├───┼───────┼──────┤
-            │ 0 │ Alice │ 31   │
-            │ 1 │ John  │ 48   │
-            └───┴───────┴──────┘
-            [2 rows x 2 columns]
-        ```
-
-        Note:
-            - The method handles the insertion of rows into the SQLDataModel, updates metadata, and commits the changes to the database.
-            - If an error occurs during SQL execution, it rolls back the changes and raises a ``SQLProgrammingError`` with an informative message.
-            - Rows are inserted at one index greater than the current max index/row count.
-            - If no insert values are provided, ``None`` or SQL 'null' will be inserted to match the current model dimensions.
-        """
-        if values is not None:
-            if not isinstance(values, (list,tuple)):
-                raise TypeError(
-                    SQLDataModel.ErrorFormat(f"TypeError: invalid type '{type(values).__name__}', insert values must be of type 'list' or 'tuple'")
-                    ) from None
-            if isinstance(values,list):
-                values = tuple(values)
-            if (len_val := len(values)) != self.column_count:
-                raise DimensionError(
-                    SQLDataModel.ErrorFormat(f"DimensionError: invalid dimensions '{len_val} != {self.column_count}', the number of values provided: '{len_val}' must match the current column count '{self.column_count}'")
-                    ) from None
-        else:
-            values = tuple(None for _ in range(self.column_count))
-        insert_cols = ",".join([f'"{col}"' for col in self.headers])
-        insert_vals = ",".join(["?" if not isinstance(val,datetime.date) else "datetime(?)" if isinstance(val, datetime.datetime) else "date(?)" for val in values])
-        insert_stmt = f"""insert into {self.sql_model}({insert_cols}) values ({insert_vals})"""
-        try:
-            self.sql_db_conn.execute(insert_stmt, values)
-            self.sql_db_conn.commit()
-        except Exception as e:
-            self.sql_db_conn.rollback()
-            raise SQLProgrammingError(
-                SQLDataModel.ErrorFormat(f'SQLProgrammingError: unable to update values, SQL execution failed with: "{e}"')
-            ) from None
-        self._update_model_metadata(update_row_meta=True)        
-
     def update_index_at(self, row_index:int, column_index:int|str, value:Any=None) -> None:
         """
         Updates a specific cell in the ``SQLDataModel`` at the given row and column indices with the provided value.
 
         Parameters:
             ``row_index`` (int): The index of the row to be updated.
             ``column_index`` (int or str): The index or name of the column to be updated.
@@ -10990,20 +11088,21 @@
 
             # View header master
             print(sdm.header_master)
 
         This will output:
 
         ```shell
-                {'first': ('TEXT', 'str', True, '<'),
-                 'last': ('TEXT', 'str', True, '<'),
-                 'age': ('INTEGER', 'int', True, '>'),
-                 'service_time': ('REAL', 'float', True, '>'),
-                 'idx': ('INTEGER', 'int', False, '>')}
+            {'first': ('TEXT', 'str', True, '<'),
+             'last': ('TEXT', 'str', True, '<'),
+             'age': ('INTEGER', 'int', True, '>'),
+             'service_time': ('REAL', 'float', True, '>'),
+             'idx': ('INTEGER', 'int', False, '>')}
         ```
+
         Example Attributes Modified:
 
         ```python
             from SQLDataModel import SQLDataModel
 
             headers = ['idx', 'first', 'last', 'age', 'service_time']
             data = [
@@ -11026,15 +11125,18 @@
             sdm._update_model_metadata()
 
             # Get new column count
             num_cols_after = sdm.column_count
 
             # View difference
             print(f"cols before: {num_cols_before}, cols after: {num_cols_after}")
-        ```    
+        ```   
+
+        Note:
+            - This method is called after operations that may modify the current model's structure and require synchronization.
         """        
         fetch_metadata = f"""select "name" as "_ordered_name","type" as "_ordered_type","pk" as "_is_regular_column",case when ("type"='INTEGER' or "type"='REAL') then '>' else '<' end as "_def_alignment" from pragma_table_info('{self.sql_model}') order by {",".join([f'''"_ordered_name"='{col}' desc''' for col in self.headers])}"""
         metadata = self.sql_db_conn.execute(fetch_metadata).fetchall()
         header_master = {m[0]:(m[1], self.static_sql_to_py_map_dict[m[1]],True if m[2] == 0 else False,m[3]) for m in metadata}
         self.headers = list(dict.fromkeys([k for k,v in header_master.items() if v[2]]))
         self.column_count = len(self.headers)
         # format: 'column_name': ('sql_dtype', 'py_dtype', is_regular_column, 'default_alignment')
@@ -11190,14 +11292,30 @@
             - There is no reason to call this method manually unless the model has been changed outside of the standard instance methods.
         """
         fetch_stmt = f"""select "{self.sql_idx}" from "{self.sql_model}" order by "{self.sql_idx}" asc"""
         self.indicies = tuple([x[0] for x in self.sql_db_conn.execute(fetch_stmt).fetchall()])
         self.row_count = len(self.indicies)
         self.shape = (self.row_count,self.shape[1])
     
+    def _update_indicies_deterministic(self, row_index:int) -> None:
+        """
+        Quick implementation to update the :py:attr:`SQLDataModel.indicies` and :py:attr:`SQLDataModel.row_count` properties of the ``SQLDataModel`` instance representing the current valid row indicies and count based on the last inserted rowid.
+
+        Returns:
+            ``None``
+
+        Note:
+            - This method is called internally any time the :py:attr:`SQLDataModel.row_count` property is subject to deterministic change to avoid the more expensive call to :meth:`SQLDataModel._update_indicies()`
+        """
+        if row_index is None:
+            return
+        self.indicies = tuple(sorted(set((*self.indicies,row_index))))
+        self.row_count = len(self.indicies)
+        self.shape = (self.row_count,self.shape[1])    
+
     def get_indicies(self) -> tuple:
         """
         Returns the current valid row indicies for the ``SQLDataModel`` instance.
 
         Returns:
             ``tuple``: A tuple of the current values for :py:attr:`SQLDataModel.sql_idx` in ascending order.
```

### Comparing `sqldatamodel-0.5.2/src/SQLDataModel/StandardDeviation.py` & `sqldatamodel-0.6.0/src/SQLDataModel/StandardDeviation.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.5.2/src/SQLDataModel/converters.py` & `sqldatamodel-0.6.0/src/SQLDataModel/converters.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.5.2/src/SQLDataModel/demo.py` & `sqldatamodel-0.6.0/src/SQLDataModel/demo.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.5.2/src/SQLDataModel/exceptions.py` & `sqldatamodel-0.6.0/src/SQLDataModel/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         # Attempting to assign a row with incompatible shape which also raises `DimensionError` exception:
         try:
             sdm[1] = ['sarah', 'west', 30, 'new york']
         except DimensionError as e:
             print(e)
     
     Note:
-        - An argument could be made for using `ValueError` instead, but there's enough difference to justify a new error.
+        - An argument could be made for using ``ValueError`` instead, but there's enough difference to justify a new error.
     """
 
 class SQLProgrammingError(Exception):
     """
     Raised when invalid or malformed SQL prevents the execution of a method or returns unexpected behavior,
     for example, trying to select a column that does not exist in the current model.
 
@@ -71,10 +71,9 @@
         # Query for non-existing column to raise `SQLProgrammingError` exception:
         try:
             sdm = SQLDataModel.fetch_query("select first, last, date_of_birth from sdm")
         except SQLProgrammingError as e:
             print(e)    
 
     Note:
-        - This exception is used to wrap any ``sqlite3.ProgrammingError`` encountered during SQL related operations.
-        
+        - This exception is used to wrap any ``sqlite3.ProgrammingError`` encountered during SQL related operations.  
     """
```

### Comparing `sqldatamodel-0.5.2/src/SQLDataModel/extensions/str_utils.c` & `sqldatamodel-0.6.0/src/SQLDataModel/extensions/str_utils.c`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.5.2/src/SQLDataModel.egg-info/PKG-INFO` & `sqldatamodel-0.6.0/src/SQLDataModel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.5.2
+Version: 0.6.0
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal-tables,pretty-print-tables,sql2sql,data-analysis,data-science,datamodel,extract,transform,load,web-scraping-tables,data-mining,html,html-table-parsing,apache-arrow,pyarrow,pyarrow-conversion,pyarrow-to-table,pyarrow-to-sql,pyarrow-to-csv,parquet-file-parsing,csv,csv-parsing,markdown,markdown-table-parsing,latex,latex-table-parsing,delimited,delimited-data-parsing,file-conversion,format-conversion,terminal-styling,table-styling,from-sqlite,to-sqlite,from-postgresql,to-postgresql,sql-to-sql,excel,xlsx-file,excel-to-sql,DataFrames,polars2pandas,pandas2polars
```

### Comparing `sqldatamodel-0.5.2/src/SQLDataModel.egg-info/SOURCES.txt` & `sqldatamodel-0.6.0/src/SQLDataModel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.5.2/tests/test_Future.py` & `sqldatamodel-0.6.0/tests/test_Future.py`

 * *Files 2% similar despite different names*

```diff
@@ -651,14 +651,42 @@
     for delimiter in valid_delimiters:
         dsv = sdm.to_csv(delimiter=delimiter)
         sdm = SQLDataModel.from_delimited(dsv)
         output_data = sdm.data(include_headers=True)
         assert input_data == output_data
 
 @pytest.mark.core
+def test_append_row():
+    num_rows = 12
+    data_store = [tuple([f"{i}", i, float(i)]) for i in range(num_rows)] # str, int, float
+    for rid in range(len(data_store)):
+        input_data = data_store[:rid]
+        sdm = SQLDataModel(headers=['A', 'B', 'C'], dtypes={'A':'str','B':'int','C':'float'})
+        for input_row in input_data:
+            sdm.append_row(input_row)
+        output_data = sdm.data(strict_2d=True)
+        assert output_data == input_data
+    # test null append
+    num_null_rows = 4
+    null_row = (None, None, None)
+    sdm = SQLDataModel(data_store, display_float_precision=1)
+    for _ in range(num_null_rows):
+        data_store.append(null_row)
+        sdm.append_row(null_row)
+        output_data = sdm.data(strict_2d=True)
+        assert output_data == data_store 
+    # test model metadata
+    expected_shape = (len(data_store), len(data_store[0]))
+    output_shape = sdm.shape
+    assert output_shape == expected_shape
+    expected_indicies = tuple(range(0,(num_rows+num_null_rows)))
+    output_indicies = sdm.indicies
+    assert output_indicies == expected_indicies
+
+@pytest.mark.core
 def test_concat(sample_data):
     input_data, input_headers = sample_data[1:], sample_data[0]
     mid = len(input_data) // 2
     base_data, other_data = input_data[:mid], input_data[mid:]
     base_sdm = SQLDataModel(base_data, headers=input_headers)    
     other_sdm = SQLDataModel(other_data, headers=input_headers)    
     # Concat other sdm returning new using inplace=False
@@ -704,14 +732,52 @@
     n_value = 24
     input_data, input_headers = sample_data[1:], sample_data[0]
     sdm = SQLDataModel(input_data, headers=input_headers)
     expected_output = input_data[:n_value]
     output_data = sdm.head(n_rows=n_value).data()
     assert output_data == expected_output
 
+@pytest.mark.core    
+def test_insert_row():
+    num_rows = 16
+    data = [[f"{i}", i, float(i)] for i in range(num_rows)] # str, int, float
+    sdm = SQLDataModel(data, display_float_precision=1)
+    # test insert on_conflict = 'replace'
+    rand_row = random.randint(0, (num_rows-2)) # leave room to add +2 to rand_row for ignore test and top and bottom insert new row tests
+    input_data = tuple([f"{10+rand_row}", 10+rand_row, float(10+rand_row)])
+    sdm.insert_row(rand_row, input_data, on_conflict='replace')
+    output_data = sdm[rand_row].data()
+    assert output_data == input_data
+    # test insert on_conflict = 'ignore'
+    rand_row = rand_row + 1
+    input_fail = tuple([None, None, None])
+    sdm.insert_row(rand_row, input_fail, on_conflict='ignore')
+    output_data = sdm[rand_row].data()
+    assert output_data != input_fail
+    # test insert at top of model
+    top_row = -1
+    input_data = tuple([f"{top_row}", top_row, float(top_row)])
+    sdm.insert_row(top_row, input_data, on_conflict='replace')
+    output_data = sdm[0].data()
+    assert output_data == input_data
+    # test insert at bottom of model
+    bottom_row = num_rows
+    input_data = tuple([f"{bottom_row}", bottom_row, float(bottom_row)])
+    sdm.insert_row(bottom_row, input_data, on_conflict='replace')
+    output_data = sdm[-1].data()
+    assert output_data == input_data
+    # test metadata like shape and indicies
+    expected_shape = (num_rows+2, 3)
+    output_shape = sdm.shape
+    print(expected_shape, output_shape)
+    assert output_shape == expected_shape
+    expected_indicies = tuple(range(-1, num_rows+1))
+    output_indicies = sdm.indicies
+    assert output_indicies == expected_indicies
+
 @pytest.mark.core
 def test_tail(sample_data):
     n_value = 24
     input_data, input_headers = sample_data[1:], sample_data[0]
     sdm = SQLDataModel(input_data, headers=input_headers)
     expected_output = input_data[-n_value:]
     output_data = sdm.tail(n_rows=n_value).data()
```

### Comparing `sqldatamodel-0.5.2/tests/test_SQLDataModel.py` & `sqldatamodel-0.6.0/tests/test_SQLDataModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -651,14 +651,42 @@
     for delimiter in valid_delimiters:
         dsv = sdm.to_csv(delimiter=delimiter)
         sdm = SQLDataModel.from_delimited(dsv)
         output_data = sdm.data(include_headers=True)
         assert input_data == output_data
 
 @pytest.mark.core
+def test_append_row():
+    num_rows = 12
+    data_store = [tuple([f"{i}", i, float(i)]) for i in range(num_rows)] # str, int, float
+    for rid in range(len(data_store)):
+        input_data = data_store[:rid]
+        sdm = SQLDataModel(headers=['A', 'B', 'C'], dtypes={'A':'str','B':'int','C':'float'})
+        for input_row in input_data:
+            sdm.append_row(input_row)
+        output_data = sdm.data(strict_2d=True)
+        assert output_data == input_data
+    # test null append
+    num_null_rows = 4
+    null_row = (None, None, None)
+    sdm = SQLDataModel(data_store, display_float_precision=1)
+    for _ in range(num_null_rows):
+        data_store.append(null_row)
+        sdm.append_row(null_row)
+        output_data = sdm.data(strict_2d=True)
+        assert output_data == data_store 
+    # test model metadata
+    expected_shape = (len(data_store), len(data_store[0]))
+    output_shape = sdm.shape
+    assert output_shape == expected_shape
+    expected_indicies = tuple(range(0,(num_rows+num_null_rows)))
+    output_indicies = sdm.indicies
+    assert output_indicies == expected_indicies
+
+@pytest.mark.core
 def test_concat(sample_data):
     input_data, input_headers = sample_data[1:], sample_data[0]
     mid = len(input_data) // 2
     base_data, other_data = input_data[:mid], input_data[mid:]
     base_sdm = SQLDataModel(base_data, headers=input_headers)    
     other_sdm = SQLDataModel(other_data, headers=input_headers)    
     # Concat other sdm returning new using inplace=False
@@ -704,14 +732,52 @@
     n_value = 24
     input_data, input_headers = sample_data[1:], sample_data[0]
     sdm = SQLDataModel(input_data, headers=input_headers)
     expected_output = input_data[:n_value]
     output_data = sdm.head(n_rows=n_value).data()
     assert output_data == expected_output
 
+@pytest.mark.core    
+def test_insert_row():
+    num_rows = 16
+    data = [[f"{i}", i, float(i)] for i in range(num_rows)] # str, int, float
+    sdm = SQLDataModel(data, display_float_precision=1)
+    # test insert on_conflict = 'replace'
+    rand_row = random.randint(0, (num_rows-2)) # leave room to add +2 to rand_row for ignore test and top and bottom insert new row tests
+    input_data = tuple([f"{10+rand_row}", 10+rand_row, float(10+rand_row)])
+    sdm.insert_row(rand_row, input_data, on_conflict='replace')
+    output_data = sdm[rand_row].data()
+    assert output_data == input_data
+    # test insert on_conflict = 'ignore'
+    rand_row = rand_row + 1
+    input_fail = tuple([None, None, None])
+    sdm.insert_row(rand_row, input_fail, on_conflict='ignore')
+    output_data = sdm[rand_row].data()
+    assert output_data != input_fail
+    # test insert at top of model
+    top_row = -1
+    input_data = tuple([f"{top_row}", top_row, float(top_row)])
+    sdm.insert_row(top_row, input_data, on_conflict='replace')
+    output_data = sdm[0].data()
+    assert output_data == input_data
+    # test insert at bottom of model
+    bottom_row = num_rows
+    input_data = tuple([f"{bottom_row}", bottom_row, float(bottom_row)])
+    sdm.insert_row(bottom_row, input_data, on_conflict='replace')
+    output_data = sdm[-1].data()
+    assert output_data == input_data
+    # test metadata like shape and indicies
+    expected_shape = (num_rows+2, 3)
+    output_shape = sdm.shape
+    print(expected_shape, output_shape)
+    assert output_shape == expected_shape
+    expected_indicies = tuple(range(-1, num_rows+1))
+    output_indicies = sdm.indicies
+    assert output_indicies == expected_indicies
+
 @pytest.mark.core
 def test_tail(sample_data):
     n_value = 24
     input_data, input_headers = sample_data[1:], sample_data[0]
     sdm = SQLDataModel(input_data, headers=input_headers)
     expected_output = input_data[-n_value:]
     output_data = sdm.tail(n_rows=n_value).data()
```

