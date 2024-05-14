# Comparing `tmp/filepattern-2.0.5-cp39-cp39-win_amd64.whl.zip` & `tmp/filepattern-2.0.6-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,20 @@
-Zip file size: 295084 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      307 b- defN 24-Feb-07 15:39 filepattern/__init__.py
--rw-rw-rw-  2.0 fat      518 b- defN 24-Feb-07 15:42 filepattern/_version.py
--rw-rw-rw-  2.0 fat   207872 b- defN 24-Feb-07 15:42 filepattern/backend.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   443392 b- defN 24-Feb-07 15:42 filepattern/filepattern.dll
--rw-rw-rw-  2.0 fat    21050 b- defN 24-Feb-07 15:39 filepattern/filepattern.py
--rw-rw-rw-  2.0 fat     1978 b- defN 24-Feb-07 15:39 filepattern/functions.py
--rw-rw-rw-  2.0 fat      647 b- defN 24-Feb-07 15:39 filepattern/pydantic_filepattern.py
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Feb-07 15:42 filepattern-2.0.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    18538 b- defN 24-Feb-07 15:42 filepattern-2.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Feb-07 15:42 filepattern-2.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       32 b- defN 24-Feb-07 15:42 filepattern-2.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1005 b- defN 24-Feb-07 15:42 filepattern-2.0.5.dist-info/RECORD
-12 files, 696524 bytes uncompressed, 293400 bytes compressed:  57.9%
+Zip file size: 2022996 bytes, number of entries: 18
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 11:34 filepattern.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 11:34 filepattern-2.0.6.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 11:34 filepattern/
+-rwxr-xr-x  2.0 unx  1454465 b- defN 24-May-14 11:34 filepattern.libs/libfilepattern-1ea27f41.so.2.0.5
+-rw-r--r--  2.0 unx     1064 b- defN 24-May-14 11:34 filepattern-2.0.6.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1330 b- defN 24-May-14 11:34 filepattern-2.0.6.dist-info/RECORD
+-rw-r--r--  2.0 unx       32 b- defN 24-May-14 11:34 filepattern-2.0.6.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      148 b- defN 24-May-14 11:34 filepattern-2.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx    18054 b- defN 24-May-14 11:34 filepattern-2.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx      620 b- defN 24-May-14 11:34 filepattern/pydantic_filepattern.py
+-rw-r--r--  2.0 unx    21170 b- defN 24-May-14 11:34 filepattern/filepattern.py
+-rwxr-xr-x  2.0 unx  1364536 b- defN 24-May-14 11:34 filepattern/libfilepattern.so.2.0.5
+-rwxr-xr-x  2.0 unx  1364536 b- defN 24-May-14 11:34 filepattern/libfilepattern.so
+-rw-r--r--  2.0 unx      297 b- defN 24-May-14 11:34 filepattern/__init__.py
+-rwxr-xr-x  2.0 unx  1364536 b- defN 24-May-14 11:34 filepattern/libfilepattern.so.2
+-rw-r--r--  2.0 unx     1930 b- defN 24-May-14 11:34 filepattern/functions.py
+-rw-r--r--  2.0 unx      497 b- defN 24-May-14 11:34 filepattern/_version.py
+-rwxr-xr-x  2.0 unx   246521 b- defN 24-May-14 11:34 filepattern/backend.cpython-39-x86_64-linux-gnu.so
+18 files, 5839736 bytes uncompressed, 2020484 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -1,37 +1,55 @@
-Filename: filepattern/__init__.py
+Filename: filepattern.libs/
 Comment: 
 
-Filename: filepattern/_version.py
+Filename: filepattern-2.0.6.dist-info/
 Comment: 
 
-Filename: filepattern/backend.cp39-win_amd64.pyd
+Filename: filepattern/
 Comment: 
 
-Filename: filepattern/filepattern.dll
+Filename: filepattern.libs/libfilepattern-1ea27f41.so.2.0.5
 Comment: 
 
-Filename: filepattern/filepattern.py
+Filename: filepattern-2.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: filepattern/functions.py
+Filename: filepattern-2.0.6.dist-info/RECORD
+Comment: 
+
+Filename: filepattern-2.0.6.dist-info/top_level.txt
+Comment: 
+
+Filename: filepattern-2.0.6.dist-info/WHEEL
+Comment: 
+
+Filename: filepattern-2.0.6.dist-info/METADATA
 Comment: 
 
 Filename: filepattern/pydantic_filepattern.py
 Comment: 
 
-Filename: filepattern-2.0.5.dist-info/LICENSE
+Filename: filepattern/filepattern.py
+Comment: 
+
+Filename: filepattern/libfilepattern.so.2.0.5
+Comment: 
+
+Filename: filepattern/libfilepattern.so
 Comment: 
 
-Filename: filepattern-2.0.5.dist-info/METADATA
+Filename: filepattern/__init__.py
 Comment: 
 
-Filename: filepattern-2.0.5.dist-info/WHEEL
+Filename: filepattern/libfilepattern.so.2
 Comment: 
 
-Filename: filepattern-2.0.5.dist-info/top_level.txt
+Filename: filepattern/functions.py
+Comment: 
+
+Filename: filepattern/_version.py
 Comment: 
 
-Filename: filepattern-2.0.5.dist-info/RECORD
+Filename: filepattern/backend.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filepattern/__init__.py

 * *Ordering differences only*

```diff
@@ -1,10 +1,10 @@
-# -*- coding: utf-8 -*-
-from __future__ import absolute_import, unicode_literals
-
-from .filepattern import FilePattern
-
-from .functions import infer_pattern, get_regex
-
-__all__ = ["FilePattern", "infer_pattern", "get_regex"]
-from . import _version
-__version__ = _version.get_versions()['version']
+# -*- coding: utf-8 -*-
+from __future__ import absolute_import, unicode_literals
+
+from .filepattern import FilePattern
+
+from .functions import infer_pattern, get_regex
+
+__all__ = ["FilePattern", "infer_pattern", "get_regex"]
+from . import _version
+__version__ = _version.get_versions()['version']
```

## filepattern/_version.py

```diff
@@ -1,21 +1,21 @@
-
-# This file was generated by 'versioneer.py' (0.22) from
-# revision-control system data, or from the parent directory name of an
-# unpacked source archive. Distribution tarballs contain a pre-generated copy
-# of this file.
-
-import json
-
-version_json = '''
-{
- "date": "2024-02-07T10:38:44-0500",
- "dirty": false,
- "error": null,
- "full-revisionid": "84df4392eee0315421ccda6ea4f068bfd6a396ce",
- "version": "2.0.5"
-}
-'''  # END VERSION_JSON
-
-
-def get_versions():
-    return json.loads(version_json)
+
+# This file was generated by 'versioneer.py' (0.22) from
+# revision-control system data, or from the parent directory name of an
+# unpacked source archive. Distribution tarballs contain a pre-generated copy
+# of this file.
+
+import json
+
+version_json = '''
+{
+ "date": "2024-05-08T13:27:44-0400",
+ "dirty": false,
+ "error": null,
+ "full-revisionid": "ccbb583936b00e2222fe3f3d737d08dff8416c24",
+ "version": "2.0.6"
+}
+'''  # END VERSION_JSON
+
+
+def get_versions():
+    return json.loads(version_json)
```

## filepattern/filepattern.py

```diff
@@ -1,528 +1,546 @@
-# -*- coding: utf-8 -*-
-from . import backend
-from typing import Dict, List, Tuple, Union, Set, Any
-import os
-from .pydantic_filepattern import create_pydantic_fp, get_pydantic_fp
-
-
-class PatternObject:
-
-    def __init__(self, file_pattern, block_size):
-        self._file_pattern = file_pattern
-        self._block_size = block_size
-
-    def get_matching(self, kwargs) -> List[Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]]:
-        """Get all filenames matching specific values
-
-        This method will return a list containing all files where the variable matches the supplied. For example,
-        if the argument `x=1` is passed to get matching, all files where x is 1 will be returned. A list of values
-        can also be passed, such as `x=[1,2,3]`. Furthermore, an arbitrary number of variables and values can be passed,
-        such as `x=1, y=2, z=3` or `x=[1,2,3], y=['a', 'b', 'c'], z=[4, 5, 6]`.
-
-        Args:
-            kwargs: One or more keyword arguments where the key is a variable contained in the filepattern and
-                    the value is a value for the variable
-
-        Returns:
-            List of matching files
-        """
-
-        vars = self.get_variables()
-
-        mapping = []
-        pydantic_output = False
-        for key, value in kwargs.items():
-
-            if (key == 'pydantic_output'):
-                pydantic_output = value
-                continue
-
-            if (key not in vars and key != ""):
-                raise ValueError("Variable \"" + key + "\" is not a valid variable. The variables are: " + str(vars) + ".")
-
-            if (not isinstance(value, list)):
-                value = [value]
-            mapping.append((key, value))
-
-        if self._block_size == "":
-
-            files = self._file_pattern.getMatching(mapping)
-
-            if (pydantic_output):
-
-                if (len(files) > 0):
-
-                    file = files[0]
-
-                    self.FilepatternModel = get_pydantic_fp(file)
-
-                    for i in range(len(files)):
-                        temp = files[i]
-                        file_dict = temp[0]
-                        file_dict['path'] = temp[1]
-                        files[i] = self.FilepatternModel(**file_dict)
-
-            return files
-
-        else:
-            return self._get_matching_out_of_core(mapping, pydantic_output)
-
-    def _get_matching_out_of_core(self, mapping, pydantic_output=False) -> List[Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]]:
-        """get_matching functionality for out of core algorithms
-
-        This method is called by get_mapping and should not be used directly.
-
-        This function will yield blocks of the get_matching functionality for external memory filepattern objects.
-        """
-
-        self._file_pattern.getMatching(mapping)
-
-        while True:
-            matching = self._get_matching_block()
-            if len(matching) == 0:
-                break
-
-            for match in matching:
-
-                if (pydantic_output):
-
-                    if (len(match) > 0):
-
-                        self.FilepatternModel = get_pydantic_fp(match)
-
-                        file_dict = match[0]
-                        file_dict['path'] = match[1]
-                        match = self.FilepatternModel(**file_dict)
-
-                yield match
-
-    def _get_matching_block(self) -> List[Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]]:
-        """
-        Returns block of matching files of size less than or equal to block_size.
-
-        This method should not be called directly. Must be called after making a call to get_matching.
-
-        Returns:
-            List containing a block of matching files.
-        """
-
-        return self._file_pattern.getMatchingBlock()
-
-    def get_occurrences(self, mapping: List[Tuple[str, List[Union[int, float, str]]]]) -> Dict[str, Dict[Union[int, float, str], int]]:
-        """
-        Returns the unique values for each variable along with the number of occurrences for each value.
-
-        Args:
-            **kwargs: Each keyword argument must be a variable. If no arguments are supplied, the occurrences
-            for every variable will be returned.
-
-        Returns:
-            Dictionary of variables mapped to values where each value is mapped to the number of occurrences.
-        """
-
-        return self._file_pattern.getOccurrences(mapping)
-
-    def get_unique_values(self, variables: List[str]) -> Dict[str, Set[Union[int, float, str]]]:
-        """Returns the unique values for each variable.
-
-        This method returns a dictionary of provided variables to a list of all unique occurrences. If no variables are provided,
-        all variables will be returned.
-
-        Args:
-            **args: Variables to get the occurrences of. All variables will be returned if no arguments are provided.
-
-        Returns:
-            Dictionary of variables mapped to values.
-        """
-
-        vars = self.get_variables()
-
-        for var in variables:
-            if (var not in vars and var != ""):
-                raise ValueError("Variable \"" + var + "\" is not a valid variable. The variables are: " + str(vars) + ".")
-
-        return self._file_pattern.getUniqueValues(variables)
-
-    def output_name(self, files: List[Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]] = []) -> str:
-        """Returns a single filename that captures variables from a list of files.
-
-        Given a list of files, this method will return a single filename that captures the variables from each
-        file in the list. If a variable is constant through the list, the variable value will be in the returned
-        name. If a variable is not constant, the minimum and maximum values will appear in the returned name in
-        the form "(min-max)".
-
-        Args:
-            files: List of files to get a single filename of.
-
-        Returns:
-            A string that captures the variable values from each file in files.
-
-        """
-
-        return self._file_pattern.outputName(files)
-
-    def __len__(self) -> int:
-
-        return self._file_pattern.length()
-
-    def get_variables(self) -> List[str]:
-
-        return self._file_pattern.getVariables()
-
-    def __call__(self,
-                 group_by: Union[str, List[str]] = "",
-                 pydantic_output: bool = False) -> Union[List[Tuple[List[Tuple[str, Union[str, int, float]]],
-                                                                    List[Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]]]],
-                                                         Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]]:
-        """Iterate through files parsed using a filepattern
-
-        This method returns an iterable of filenames matched to the filepattern.
-
-        If a group_by variable is provided, lists of files where the variable is held constant are
-        returned on each call.
-
-        Note that the `group_by` argument works in the inverse of the previous version of `filepattern`.
-        The variable passed to `group_by` will be held constant rather than the other variables remaining constant.
-
-        Args:
-            group_by: A string consisting of a single variable or a list of variables to group filenames by.
-            pydantic_output: Get Pydantic models as the output
-        """
-
-        vars = self.get_variables()
-
-        if (isinstance(group_by, str)):
-            if (group_by not in vars and group_by != ""):
-                raise ValueError("Variable \"" + group_by + "\" is not a valid variable. The variables are: " + str(vars) + ".")
-
-        else:
-            for var in group_by:
-                if var not in vars:
-                    raise ValueError("Variable \"" + var + "\" is not a valid variable. The variables are: " + str(vars) + ".")
-
-        self.pydantic_iterator = pydantic_output
-
-        if (self.pydantic_iterator):
-
-            if (self.__len__() > 0):
-                file = self.__getitem__(0)
-
-                self.FilepatternModel = get_pydantic_fp(file)
-
-            else:  # list of files is empty
-
-                # get variables
-                variables = self.get_variables()
-
-                variable_map = {}
-
-                # add paths to map
-                variable_map["path"] = (list, ...)
-
-                for variable in variables:
-                    variable_map[variable] = (Any, ...)
-
-                self.FilepatternModel = create_pydantic_fp(variable_map)
-
-        if (group_by == []):
-            group_by = ['*__all__*']
-
-        if (isinstance(group_by, str)):
-            group_by = [group_by]
-
-        self._file_pattern.setGroup(group_by)
-
-        if self._block_size == "":
-
-            if len(group_by) == 0 or group_by[0] != "":
-                self._file_pattern.groupBy(group_by)
-
-            return self
-
-        if len(group_by) == 0 or (group_by != [""] and len(group_by) != 1):
-            self._file_pattern.setGroup(group_by)
-
-        return self
-
-    def _length(self) -> int:
-        """Get length of current block for out of core algorithms
-        """
-        return self._file_pattern.currentBlockLength()
-
-    def __iter__(self) -> Union[List[Tuple[List[Tuple[str, Union[str, int, float]]], List[Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]]]],
-                                Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]]:
-        """Yields files from files that match the filepattern
-
-        Yields:
-            Union[List[Tuple[List[Tuple[str, Union[str, int, float]]], List[Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]]]],
-                  Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]] : Returns single file when group_by is not used and list of files otherwise
-        """
-
-        if self._block_size == "":
-            for file in self._file_pattern.__iter__():
-                if (self.pydantic_iterator):
-
-                    if (isinstance(file[0], dict)):
-                        map_with_path = file[0]
-                        map_with_path['path'] = file[1]
-
-                        yield self.FilepatternModel(**map_with_path)
-
-                    else:
-                        for i in range(len(file[1])):
-
-                            map_with_path = file[1][i][0]
-                            map_with_path['path'] = file[1][i][1]
-
-                            file[1][i] = self.FilepatternModel(**map_with_path)
-
-                        yield file
-                else:
-                    yield file
-        else:
-            while True:
-                for block in self._file_pattern.__iter__():
-
-                    if self._length() == 0:
-                        break
-
-                    if (self.pydantic_iterator):
-
-                        if (isinstance(block[0], dict)):
-                            map_with_path = block[0]
-                            map_with_path['path'] = block[1]
-
-                            yield self.FilepatternModel(**map_with_path)
-
-                        else:
-                            for i in range(len(block[1])):
-
-                                map_with_path = block[1][i][0]
-                                map_with_path['path'] = block[1][i][1]
-
-                                block[1][i] = self.FilepatternModel(**map_with_path)
-
-                            yield block
-                    else:
-                        yield block
-
-                if self._length() == 0:
-                    break
-
-    def __getitem__(self, key) -> Union[List[Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]],
-                                        Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]]:
-        """Get slices of files that match the filepattern
-
-        Slices of files can be retrieved using [] operator. Files can be accessed using a single index
-        such as fp[1] or slices of files, such as fp[:10], f[1:10], or fp[1:2:10].
-
-        Args:
-            key (int): Index of file
-
-        Returns:
-            Union[List[Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]],
-                Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]]: Returns single file for a single index or a List
-                of files for a slice.
-        """
-
-        if (isinstance(key, int)):
-            return self._file_pattern.getItem(key)
-        if (isinstance(key, list)):
-            return self._file_pattern.getItemList(key)
-
-        slc = [key.start, key.stop, key.step]
-        if (slc[0] is None):
-            slc[0] = 'None'
-        if (slc[1] is None):
-            slc[1] = 'None'
-        if (slc[2] is None):
-            slc[2] = 'None'
-
-        return self._file_pattern.getSlice(slc)
-
-
-class FilePattern(PatternObject):
-    """
-    Class to create a FilePattern object.
-
-    This class take in in 4 arguments: path, pattern, block_size, and recursive. For the path,
-    either a path to a directory, text file, or stitching vector may be provided. ``filepattern`` will
-    then match the filenames in the directory, or each line of the text file, to the provided ``pattern``.
-
-    The ``block_size`` parameter allows for out of core processing, which consume ``block_size`` amount of memory at most.
-
-    The ``recursive`` parameter enables recursive iteration of subdirectories when a directory is passed as ``path``. In
-    this case ``filepattern`` will iterate over the subdirectories, storing filenames with the same basename in the same
-    group.
-
-
-    Args:
-            path: Path to directory or text file
-            pattern: Pattern to compare each filename to
-            block_size: Maximum amount of RAM to consume at once. Defaults to "".
-            recursive: Iterate over subdirectories. Defaults to False.
-    """
-
-    def __init__(
-        self,
-        path: str,
-        pattern: str = "",
-        block_size: str = "",
-        recursive: bool = False,
-        suppress_warnings=False
-    ):
-        """Constructor of the FilePattern class. The path argument can either be a directory, a text file,
-        or a stitching vector. Passing in the optional argument `block_size` will
-        create an ExternalFilePattern object, which will process the directory in blocks which consume less
-        than or equal to `block_size` of memory.
-
-        Just the path may be passed in the pattern is contained within the path. In this case,
-        the names of the subdirectories are captured if they are named is the same manner as the pattern.
-        For example, if just the path 'path/to/files/{channel: c+}/img_r{r:d+}_c{c:d+}.tif' is passed,
-        the names of the channel subdirectories will be captured for each file.
-
-        Args:
-            path: Path to directory or text file
-            pattern: Pattern to compare each filename to
-            block_size: Maximum amount of RAM to consume at once. Defaults to "".
-            recursive: Iterate over subdirectories. Defaults to False.
-            suppress_warnings: True to suppress warning printed to console. Defaults to False.
-        """
-
-        path = str(path)  # change path type to string to support pathlib paths
-
-        self._file_pattern = backend.FilePattern(path, pattern, block_size, recursive, suppress_warnings)
-
-        super().__init__(self._file_pattern, block_size)
-
-    def get_matching(self, **kwargs) -> List[Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]]:
-
-        """Get all filenames matching specific values
-
-        This method will return a list containing all files where the variable matches the supplied. For example,
-        if the argument `x=1` is passed to get matching, all files where x is 1 will be returned. A list of values
-        can also be passed, such as `x=[1,2,3]`. Furthermore, an arbitrary number of variables and values can be passed,
-        such as `x=1, y=2, z=3` or `x=[1,2,3], y=['a', 'b', 'c'], z=[4, 5, 6]`.
-
-        Example:
-
-            For a directory containing the files
-            ```
-                img_r001_c001_DAPI.tif
-                img_r002_c001_DAPI.tif
-                img_r001_c001_TXREAD.tif
-                img_r002_c001_TXREAD.tif
-                img_r001_c001_GFP.tif
-                img_r002_c001_GFP.tif
-            ```
-
-            The `get_matching` method can be used as:
-
-            ```
-                path = /path/to/directory
-
-                pattern = 'img_r{r:ddd}_c{c:ddd}_{channel:c+}.tif'
-
-                files = fp.FilePattern(path, pattern)
-
-                matching = files.get_matching(channel=['TXREAD'])
-            ```
-
-            the `matching` variable will be a list of matching files:
-
-            ```
-                [({'c': 1, 'channel': 'TXREAD', 'r': 1},
-                ['/home/ec2-user/Dev/FilePattern/data/example/img_r001_c001_TXREAD.tif']),
-                ({'c': 1, 'channel': 'TXREAD', 'r': 2},
-                ['/home/ec2-user/Dev/FilePattern/data/example/img_r002_c001_TXREAD.tif'])]
-            ```
-
-        Args:
-            **kwargs: One or more keyword arguments where the key is a variable contained in the filepattern and
-                    the value is a value for the variable. Use pydantic_output=True to get Pydantic models as the output.
-
-        Returns:
-            List of matching files
-        """
-
-        return super().get_matching(kwargs)
-
-    def get_occurrences(self, **kwargs) -> Dict[str, Dict[Union[int, float, str], int]]:
-        """
-        Takes in a variable as the key and a list of values as the value and returns the a dictionary
-        mapping the variable to a dictionary of the values mapped to the number of occurrences of the variable
-        value.
-
-        For example, if the filepattern is `img_r{r:ddd}_c{r:ddd}.tif` and r=1 occurs 20 times in the path,
-        then the passing `r=[1]` will return `{'r': {1: 20}}`.
-
-        Args:
-            **kwargs: Each keyword argument must be a variable. If no arguments are supplied, the occurrences
-            for every variable will be returned.
-
-        Returns:
-            Dictionary of variables mapped to values where each value is mapped to the number of occurrences.
-        """
-
-        vars = self.get_variables()
-
-        mapping = []
-        for key, value in kwargs.items():
-
-            if (key not in vars and key != ""):
-                raise ValueError("Variable \"" + key + "\" is not a valid variable. The variables are: " + str(vars) + ".")
-
-            mapping.append((key, value))
-
-        return super(FilePattern, self).get_occurrences(mapping)
-
-    def get_unique_values(self, *args) -> Dict[str, Set[Union[int, float, str]]]:
-        """Given variable names from the filepattern as arguments, this method returns a dictionary
-        of mapping the variable names to a set of the unique values for each variable. If no variables are
-        provided, all variables will be returned.
-
-        For example if the filepattern is `img_r{r:ddd}_c{r:ddd}.tif` and `r` ranges from 1 to 3 and c ranges from 1 to 2,
-        then fp_object.get_unique_values('r', 'c') will return `{'r': {1,2,3}, 'c': {1,2}}`.
-
-        Args:
-            **args: Variables to get the occurrences of. All variables will be returned if no arguments are provided.
-
-        Returns:
-            Dictionary of variables mapped to values.
-        """
-        vec = []
-        for str in args:
-            vec.append(str)
-
-        return super().get_unique_values(vec)
-
-    def output_name(self, files: list = []) -> str:
-        """Returns a single filename that captures variables from a list of files.
-
-        Given a list of files, this method will return a single filename that captures the variables from each
-        file in the list. If a variable is constant through the list, the variable value will be in the returned
-        name. If a variable is not constant, the minimum and maximum values will appear in the returned name in
-        the form "(min-max)".
-
-        Args:
-            files: List of files to get a single filename of.
-
-        Returns:
-            A string that captures the variable values from each file in files.
-
-        """
-
-        return super().output_name(files)
-
-    def get_variables(self) -> List[str]:
-        """ Returns a list of variables that are contained in the filepattern
-
-        For example, if the filepattern is `img_x{x:d}_y{y:d}_c{c:c+}.tif`, get_variables will return
-        the list `[x, y, c]`.
-
-        Returns:
-            List containing the variables in the filepattern
-
-        """
-
-        return super().get_variables()
+# -*- coding: utf-8 -*-
+from . import backend
+from typing import Dict, List, Tuple, Union, Set, Any
+import os
+from .pydantic_filepattern import create_pydantic_fp, get_pydantic_fp
+
+
+class PatternObject:
+
+    def __init__(self, file_pattern, block_size):
+        self._file_pattern = file_pattern
+        self._block_size = block_size
+        self._pydantic_iterator = False
+
+    def get_matching(self, kwargs) -> List[Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]]:
+        """Get all filenames matching specific values
+
+        This method will return a list containing all files where the variable matches the supplied. For example,
+        if the argument `x=1` is passed to get matching, all files where x is 1 will be returned. A list of values
+        can also be passed, such as `x=[1,2,3]`. Furthermore, an arbitrary number of variables and values can be passed,
+        such as `x=1, y=2, z=3` or `x=[1,2,3], y=['a', 'b', 'c'], z=[4, 5, 6]`.
+
+        Args:
+            kwargs: One or more keyword arguments where the key is a variable contained in the filepattern and
+                    the value is a value for the variable
+
+        Returns:
+            List of matching files
+        """
+
+        vars = self.get_variables()
+
+        mapping = []
+        pydantic_output = False
+        for key, value in kwargs.items():
+
+            if (key == 'pydantic_output'):
+                pydantic_output = value
+                continue
+
+            if (key not in vars and key != ""):
+                raise ValueError("Variable \"" + key + "\" is not a valid variable. The variables are: " + str(vars) + ".")
+
+            if (not isinstance(value, list)):
+                value = [value]
+            mapping.append((key, value))
+
+        if self._block_size == "":
+
+            files = self._file_pattern.getMatching(mapping)
+
+            if (pydantic_output):
+
+                if (len(files) > 0):
+
+                    file = files[0]
+
+                    self.FilepatternModel = get_pydantic_fp(file)
+
+                    for i in range(len(files)):
+                        temp = files[i]
+                        file_dict = temp[0]
+                        file_dict['path'] = temp[1]
+                        files[i] = self.FilepatternModel(**file_dict)
+
+            return files
+
+        else:
+            return self._get_matching_out_of_core(mapping, pydantic_output)
+
+    def _get_matching_out_of_core(self, mapping, pydantic_output=False) -> List[Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]]:
+        """get_matching functionality for out of core algorithms
+
+        This method is called by get_mapping and should not be used directly.
+
+        This function will yield blocks of the get_matching functionality for external memory filepattern objects.
+        """
+
+        self._file_pattern.getMatching(mapping)
+
+        while True:
+            matching = self._get_matching_block()
+            if len(matching) == 0:
+                break
+
+            for match in matching:
+
+                if (pydantic_output):
+
+                    if (len(match) > 0):
+
+                        self.FilepatternModel = get_pydantic_fp(match)
+
+                        file_dict = match[0]
+                        file_dict['path'] = match[1]
+                        match = self.FilepatternModel(**file_dict)
+
+                yield match
+
+    def _get_matching_block(self) -> List[Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]]:
+        """
+        Returns block of matching files of size less than or equal to block_size.
+
+        This method should not be called directly. Must be called after making a call to get_matching.
+
+        Returns:
+            List containing a block of matching files.
+        """
+
+        return self._file_pattern.getMatchingBlock()
+
+    def get_occurrences(self, mapping: List[Tuple[str, List[Union[int, float, str]]]]) -> Dict[str, Dict[Union[int, float, str], int]]:
+        """
+        Returns the unique values for each variable along with the number of occurrences for each value.
+
+        Args:
+            **kwargs: Each keyword argument must be a variable. If no arguments are supplied, the occurrences
+            for every variable will be returned.
+
+        Returns:
+            Dictionary of variables mapped to values where each value is mapped to the number of occurrences.
+        """
+
+        return self._file_pattern.getOccurrences(mapping)
+
+    def get_unique_values(self, variables: List[str]) -> Dict[str, Set[Union[int, float, str]]]:
+        """Returns the unique values for each variable.
+
+        This method returns a dictionary of provided variables to a list of all unique occurrences. If no variables are provided,
+        all variables will be returned.
+
+        Args:
+            **args: Variables to get the occurrences of. All variables will be returned if no arguments are provided.
+
+        Returns:
+            Dictionary of variables mapped to values.
+        """
+
+        vars = self.get_variables()
+
+        for var in variables:
+            if (var not in vars and var != ""):
+                raise ValueError("Variable \"" + var + "\" is not a valid variable. The variables are: " + str(vars) + ".")
+
+        return self._file_pattern.getUniqueValues(variables)
+
+    def output_name(self, files: List[Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]] = []) -> str:
+        """Returns a single filename that captures variables from a list of files.
+
+        Given a list of files, this method will return a single filename that captures the variables from each
+        file in the list. If a variable is constant through the list, the variable value will be in the returned
+        name. If a variable is not constant, the minimum and maximum values will appear in the returned name in
+        the form "(min-max)".
+
+        Args:
+            files: List of files to get a single filename of.
+
+        Returns:
+            A string that captures the variable values from each file in files.
+
+        """
+
+        return self._file_pattern.outputName(files)
+
+    def __len__(self) -> int:
+
+        return self._file_pattern.length()
+
+    def get_variables(self) -> List[str]:
+
+        return self._file_pattern.getVariables()
+
+    def __call__(self,
+                 group_by: Union[str, List[str]] = "",
+                 pydantic_output: bool = False) -> Union[List[Tuple[List[Tuple[str, Union[str, int, float]]],
+                                                                    List[Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]]]],
+                                                         Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]]:
+        """Iterate through files parsed using a filepattern
+
+        This method returns an iterable of filenames matched to the filepattern.
+
+        If a group_by variable is provided, lists of files where the variable is held constant are
+        returned on each call.
+
+        Note that the `group_by` argument works in the inverse of the previous version of `filepattern`.
+        The variable passed to `group_by` will be held constant rather than the other variables remaining constant.
+
+        Args:
+            group_by: A string consisting of a single variable or a list of variables to group filenames by.
+            pydantic_output: Get Pydantic models as the output
+        """
+
+        vars = self.get_variables()
+
+        if (isinstance(group_by, str)):
+            if (group_by not in vars and group_by != ""):
+                raise ValueError("Variable \"" + group_by + "\" is not a valid variable. The variables are: " + str(vars) + ".")
+
+        else:
+            for var in group_by:
+                if var not in vars:
+                    raise ValueError("Variable \"" + var + "\" is not a valid variable. The variables are: " + str(vars) + ".")
+
+        self._pydantic_iterator = pydantic_output
+
+        if (self._pydantic_iterator):
+
+            if (self.__len__() > 0):
+                file = self.__getitem__(0)
+
+                self.FilepatternModel = get_pydantic_fp(file)
+
+            else:  # list of files is empty
+
+                # get variables
+                variables = self.get_variables()
+ 
+                variable_map = {}
+
+                # add paths to map
+                variable_map["path"] = (list, ...)
+
+                for variable in variables:
+                    variable_map[variable] = (Any, ...)
+
+                self.FilepatternModel = create_pydantic_fp(variable_map)
+
+        if (group_by == []):
+            group_by = ['*__all__*']
+
+        if (isinstance(group_by, str)):
+            group_by = [group_by]
+
+        self._file_pattern.setGroup(group_by)
+
+        if self._block_size == "":
+
+            if len(group_by) == 0 or group_by[0] != "":
+                self._file_pattern.groupBy(group_by)
+
+            return self
+
+        if len(group_by) == 0 or (group_by != [""] and len(group_by) != 1):
+            self._file_pattern.setGroup(group_by)
+
+        return self
+
+    def _length(self) -> int:
+        """Get length of current block for out of core algorithms
+        """
+        return self._file_pattern.currentBlockLength()
+
+    def __iter__(self) -> Union[List[Tuple[List[Tuple[str, Union[str, int, float]]], List[Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]]]],
+                                Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]]:
+        """Yields files from files that match the filepattern
+
+        Yields:
+            Union[List[Tuple[List[Tuple[str, Union[str, int, float]]], List[Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]]]],
+                  Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]] : Returns single file when group_by is not used and list of files otherwise
+        """
+
+        # Set pydantic_iterator value if iter is called directly
+        if (self._pydantic_iterator is None):
+            self._pydantic_iterator = False
+
+        if self._block_size == "":
+            
+            if (self._file_pattern.isGrouped()):
+                iterator = self._file_pattern.iteratorGrouped()
+            else:
+                iterator = self._file_pattern.iterator()
+            
+            for file in iterator:
+                if (self._pydantic_iterator):
+
+                    if (isinstance(file[0], dict)):
+                        map_with_path = file[0]
+                        map_with_path['path'] = file[1]
+
+                        yield self.FilepatternModel(**map_with_path)
+
+                    else:
+                        for i in range(len(file[1])):
+
+                            map_with_path = file[1][i][0]
+                            map_with_path['path'] = file[1][i][1]
+
+                            file[1][i] = self.FilepatternModel(**map_with_path)
+
+                        yield file
+                else:
+                    yield file
+        else:
+                
+            while True:
+                
+                if (self._file_pattern.isGrouped()):
+                    iterator = self._file_pattern.iteratorGroupedExternal()
+                else:
+                    iterator = self._file_pattern.iteratorExternal()
+                    
+                for block in iterator:
+
+                    if self._length() == 0:
+                        break
+
+                    if (self._pydantic_iterator):
+
+                        if (isinstance(block[0], dict)):
+                            map_with_path = block[0]
+                            map_with_path['path'] = block[1]
+
+                            yield self.FilepatternModel(**map_with_path)
+
+                        else:
+                            for i in range(len(block[1])):
+
+                                map_with_path = block[1][i][0]
+                                map_with_path['path'] = block[1][i][1]
+
+                                block[1][i] = self.FilepatternModel(**map_with_path)
+
+                            yield block
+                    else:
+                        yield block
+
+                if self._length() == 0:
+                    break
+
+    def __getitem__(self, key) -> Union[List[Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]],
+                                        Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]]:
+        """Get slices of files that match the filepattern
+
+        Slices of files can be retrieved using [] operator. Files can be accessed using a single index
+        such as fp[1] or slices of files, such as fp[:10], f[1:10], or fp[1:2:10].
+
+        Args:
+            key (int): Index of file
+
+        Returns:
+            Union[List[Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]],
+                Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]]: Returns single file for a single index or a List
+                of files for a slice.
+        """
+
+        if (isinstance(key, int)):
+            return self._file_pattern.getItem(key)
+        if (isinstance(key, list)):
+            return self._file_pattern.getItemList(key)
+
+        slc = [key.start, key.stop, key.step]
+        if (slc[0] is None):
+            slc[0] = 'None'
+        if (slc[1] is None):
+            slc[1] = 'None'
+        if (slc[2] is None):
+            slc[2] = 'None'
+
+        return self._file_pattern.getSlice(slc)
+
+
+class FilePattern(PatternObject):
+    """
+    Class to create a FilePattern object.
+
+    This class take in in 4 arguments: path, pattern, block_size, and recursive. For the path,
+    either a path to a directory, text file, or stitching vector may be provided. ``filepattern`` will
+    then match the filenames in the directory, or each line of the text file, to the provided ``pattern``.
+
+    The ``block_size`` parameter allows for out of core processing, which consume ``block_size`` amount of memory at most.
+
+    The ``recursive`` parameter enables recursive iteration of subdirectories when a directory is passed as ``path``. In
+    this case ``filepattern`` will iterate over the subdirectories, storing filenames with the same basename in the same
+    group.
+
+
+    Args:
+            path: Path to directory or text file
+            pattern: Pattern to compare each filename to
+            block_size: Maximum amount of RAM to consume at once. Defaults to "".
+            recursive: Iterate over subdirectories. Defaults to False.
+    """
+
+    def __init__(
+        self,
+        path: str,
+        pattern: str = "",
+        block_size: str = "",
+        recursive: bool = False,
+        suppress_warnings=False
+    ):
+        """Constructor of the FilePattern class. The path argument can either be a directory, a text file,
+        or a stitching vector. Passing in the optional argument `block_size` will
+        create an ExternalFilePattern object, which will process the directory in blocks which consume less
+        than or equal to `block_size` of memory.
+
+        Just the path may be passed in the pattern is contained within the path. In this case,
+        the names of the subdirectories are captured if they are named is the same manner as the pattern.
+        For example, if just the path 'path/to/files/{channel: c+}/img_r{r:d+}_c{c:d+}.tif' is passed,
+        the names of the channel subdirectories will be captured for each file.
+
+        Args:
+            path: Path to directory or text file
+            pattern: Pattern to compare each filename to
+            block_size: Maximum amount of RAM to consume at once. Defaults to "".
+            recursive: Iterate over subdirectories. Defaults to False.
+            suppress_warnings: True to suppress warning printed to console. Defaults to False.
+        """
+
+        path = str(path)  # change path type to string to support pathlib paths
+
+        self._file_pattern = backend.FilePattern(path, pattern, block_size, recursive, suppress_warnings)
+
+        super().__init__(self._file_pattern, block_size)
+
+    def get_matching(self, **kwargs) -> List[Tuple[Dict[str, Union[int, float, str]], List[os.PathLike]]]:
+
+        """Get all filenames matching specific values
+
+        This method will return a list containing all files where the variable matches the supplied. For example,
+        if the argument `x=1` is passed to get matching, all files where x is 1 will be returned. A list of values
+        can also be passed, such as `x=[1,2,3]`. Furthermore, an arbitrary number of variables and values can be passed,
+        such as `x=1, y=2, z=3` or `x=[1,2,3], y=['a', 'b', 'c'], z=[4, 5, 6]`.
+
+        Example:
+
+            For a directory containing the files
+            ```
+                img_r001_c001_DAPI.tif
+                img_r002_c001_DAPI.tif
+                img_r001_c001_TXREAD.tif
+                img_r002_c001_TXREAD.tif
+                img_r001_c001_GFP.tif
+                img_r002_c001_GFP.tif
+            ```
+
+            The `get_matching` method can be used as:
+
+            ```
+                path = /path/to/directory
+
+                pattern = 'img_r{r:ddd}_c{c:ddd}_{channel:c+}.tif'
+
+                files = fp.FilePattern(path, pattern)
+
+                matching = files.get_matching(channel=['TXREAD'])
+            ```
+
+            the `matching` variable will be a list of matching files:
+
+            ```
+                [({'c': 1, 'channel': 'TXREAD', 'r': 1},
+                ['/home/ec2-user/Dev/FilePattern/data/example/img_r001_c001_TXREAD.tif']),
+                ({'c': 1, 'channel': 'TXREAD', 'r': 2},
+                ['/home/ec2-user/Dev/FilePattern/data/example/img_r002_c001_TXREAD.tif'])]
+            ```
+
+        Args:
+            **kwargs: One or more keyword arguments where the key is a variable contained in the filepattern and
+                    the value is a value for the variable. Use pydantic_output=True to get Pydantic models as the output.
+
+        Returns:
+            List of matching files
+        """
+
+        return super().get_matching(kwargs)
+
+    def get_occurrences(self, **kwargs) -> Dict[str, Dict[Union[int, float, str], int]]:
+        """
+        Takes in a variable as the key and a list of values as the value and returns the a dictionary
+        mapping the variable to a dictionary of the values mapped to the number of occurrences of the variable
+        value.
+
+        For example, if the filepattern is `img_r{r:ddd}_c{r:ddd}.tif` and r=1 occurs 20 times in the path,
+        then the passing `r=[1]` will return `{'r': {1: 20}}`.
+
+        Args:
+            **kwargs: Each keyword argument must be a variable. If no arguments are supplied, the occurrences
+            for every variable will be returned.
+
+        Returns:
+            Dictionary of variables mapped to values where each value is mapped to the number of occurrences.
+        """
+
+        vars = self.get_variables()
+
+        mapping = []
+        for key, value in kwargs.items():
+
+            if (key not in vars and key != ""):
+                raise ValueError("Variable \"" + key + "\" is not a valid variable. The variables are: " + str(vars) + ".")
+
+            mapping.append((key, value))
+
+        return super(FilePattern, self).get_occurrences(mapping)
+
+    def get_unique_values(self, *args) -> Dict[str, Set[Union[int, float, str]]]:
+        """Given variable names from the filepattern as arguments, this method returns a dictionary
+        of mapping the variable names to a set of the unique values for each variable. If no variables are
+        provided, all variables will be returned.
+
+        For example if the filepattern is `img_r{r:ddd}_c{r:ddd}.tif` and `r` ranges from 1 to 3 and c ranges from 1 to 2,
+        then fp_object.get_unique_values('r', 'c') will return `{'r': {1,2,3}, 'c': {1,2}}`.
+
+        Args:
+            **args: Variables to get the occurrences of. All variables will be returned if no arguments are provided.
+
+        Returns:
+            Dictionary of variables mapped to values.
+        """
+        vec = []
+        for str in args:
+            vec.append(str)
+
+        return super().get_unique_values(vec)
+
+    def output_name(self, files: list = []) -> str:
+        """Returns a single filename that captures variables from a list of files.
+
+        Given a list of files, this method will return a single filename that captures the variables from each
+        file in the list. If a variable is constant through the list, the variable value will be in the returned
+        name. If a variable is not constant, the minimum and maximum values will appear in the returned name in
+        the form "(min-max)".
+
+        Args:
+            files: List of files to get a single filename of.
+
+        Returns:
+            A string that captures the variable values from each file in files.
+
+        """
+
+        return super().output_name(files)
+
+    def get_variables(self) -> List[str]:
+        """ Returns a list of variables that are contained in the filepattern
+
+        For example, if the filepattern is `img_x{x:d}_y{y:d}_c{c:c+}.tif`, get_variables will return
+        the list `[x, y, c]`.
+
+        Returns:
+            List containing the variables in the filepattern
+
+        """
+
+        return super().get_variables()
```

## filepattern/functions.py

 * *Ordering differences only*

```diff
@@ -1,48 +1,48 @@
-# -*- coding: utf-8 -*-
-from . import backend
-# Reference/Functions
-
-
-def get_regex(filepattern: str, suppress_warnings=False) -> str:
-    """Returns the regex equivalent of the filepattern.
-
-    Args:
-        filepattern: A filepattern to get the regex equivalent of.
-        suppress_warnings: True to suppress warnings (Defaults False)
-
-    Returns:
-        String containing the regex equivalent of the filepattern
-
-    """
-    return backend.FilePattern.getRegex(filepattern, suppress_warnings)
-    
-
-
-def infer_pattern(
-    path: str = "", files: list = [], variables: str = "", block_size: str = ""
-):
-    """Returns a guess of a pattern given path to a directory of files or a list of files.
-
-    This function takes in either a path to a directory or a list of filenames  to provide a guess
-    of the filepattern. The optional argument `variables` will provide names for the variables.
-    If variable names are not given, default variable names will be used. If a `block_size` is
-    specified, this method will only used the specified amount of RAM.
-
-    Args:
-        path: The path to a directory of files. Defaults to "".
-        files: A list of files. Defaults to [].
-        variables: A string of variables. If an empty string, variable names will be provided. Defaults to "".
-        block_size: An string that specifies a maximum amount of RAM to consume. If "", no limit will be imposed. Defaults to "".
-
-    Returns:
-        A string that is a guess of the pattern for the supplied filenames.
-    """
-    if path == "" and files == []:
-        raise ValueError("A path or list of files must be provided")
-    elif path != "" and files != []:
-        raise ValueError("Pass in only a path or list of files, not both.")
-
-    if files == []:
-        return backend.FilePattern.inferPattern(str(path), str(variables), str(block_size))
-    else:
-        return backend.FilePattern.inferPattern(files, variables)
+# -*- coding: utf-8 -*-
+from . import backend
+# Reference/Functions
+
+
+def get_regex(filepattern: str, suppress_warnings=False) -> str:
+    """Returns the regex equivalent of the filepattern.
+
+    Args:
+        filepattern: A filepattern to get the regex equivalent of.
+        suppress_warnings: True to suppress warnings (Defaults False)
+
+    Returns:
+        String containing the regex equivalent of the filepattern
+
+    """
+    return backend.FilePattern.getRegex(filepattern, suppress_warnings)
+    
+
+
+def infer_pattern(
+    path: str = "", files: list = [], variables: str = "", block_size: str = ""
+):
+    """Returns a guess of a pattern given path to a directory of files or a list of files.
+
+    This function takes in either a path to a directory or a list of filenames  to provide a guess
+    of the filepattern. The optional argument `variables` will provide names for the variables.
+    If variable names are not given, default variable names will be used. If a `block_size` is
+    specified, this method will only used the specified amount of RAM.
+
+    Args:
+        path: The path to a directory of files. Defaults to "".
+        files: A list of files. Defaults to [].
+        variables: A string of variables. If an empty string, variable names will be provided. Defaults to "".
+        block_size: An string that specifies a maximum amount of RAM to consume. If "", no limit will be imposed. Defaults to "".
+
+    Returns:
+        A string that is a guess of the pattern for the supplied filenames.
+    """
+    if path == "" and files == []:
+        raise ValueError("A path or list of files must be provided")
+    elif path != "" and files != []:
+        raise ValueError("Pass in only a path or list of files, not both.")
+
+    if files == []:
+        return backend.FilePattern.inferPattern(str(path), str(variables), str(block_size))
+    else:
+        return backend.FilePattern.inferPattern(files, variables)
```

## filepattern/pydantic_filepattern.py

 * *Ordering differences only*

```diff
@@ -1,27 +1,27 @@
-# -*- coding: utf-8 -*-
-from pydantic import create_model
-
-
-def get_pydantic_fp(file: tuple):
-    # get variable names and types for pydantic class
-    variable_type_map = {}
-
-    # add paths to map
-    variable_type_map["path"] = (list, ...)
-
-    # get variables mapped to values
-    variables = file[0]
-
-    # loop over variables and get type
-    for variable in variables:
-        variable_type_map[variable] = (type(variables[variable]), ...)
-
-    return create_pydantic_fp(variable_type_map)
-
-
-def create_pydantic_fp(file_dict: dict):
-
-    return create_model(
-        'FilepatternModel',
-        **file_dict
-    )
+# -*- coding: utf-8 -*-
+from pydantic import create_model
+
+
+def get_pydantic_fp(file: tuple):
+    # get variable names and types for pydantic class
+    variable_type_map = {}
+
+    # add paths to map
+    variable_type_map["path"] = (list, ...)
+
+    # get variables mapped to values
+    variables = file[0]
+
+    # loop over variables and get type
+    for variable in variables:
+        variable_type_map[variable] = (type(variables[variable]), ...)
+
+    return create_pydantic_fp(variable_type_map)
+
+
+def create_pydantic_fp(file_dict: dict):
+
+    return create_model(
+        'FilepatternModel',
+        **file_dict
+    )
```

## Comparing `filepattern-2.0.5.dist-info/METADATA` & `filepattern-2.0.6.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,484 +1,484 @@
-Metadata-Version: 2.1
-Name: filepattern
-Version: 2.0.5
-Summary: Utilities for parsing files in a directory based on a file name pattern.
-Home-page: https://github.com/PolusAI/filepattern
-Author: Jesse McKinzie, Nick Schaub
-Author-email: Jesse.McKinzie@axleinfo.com, nick.schaub@nih.gov
-Project-URL: Documentation, https://filepattern.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/PolusAI/filepattern
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pydantic
-
-# Filepattern
-
-[![Documentation Status](https://readthedocs.org/projects/filepattern/badge/?version=latest)](https://filepattern.readthedocs.io/en/latest/?badge=latest)
-[![PyPI](https://img.shields.io/pypi/v/filepattern)](https://pypi.org/project/filepattern/)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/filepattern)
-![Bower](https://img.shields.io/bower/l/MI)
-
-The ``filepattern`` utility is used to store files that follow a pattern, where the pattern is analogous to a simplified regular expression. The need for
-``filepattern`` arises in situations where large amounts of data with a systematic naming convention needs to be filtered by patterns in the naming. For example, one may have
-a directory containing segmented images where the name contains information such as the channel, the column value, and the row value. ``filepattern`` provides the ability to
-extract all images containing such a naming pattern, filter by the row or column value, or group files by one or more of the aforementioned variables.
-
-## Summary
-- [Read the Docs](https://filepattern2.readthedocs.io/en/latest/Home.html)
-- [Install](#install)
-- [Authors](#authors)
-- [License](#license)
-- [Acknowledgments](#acknowledgments)
-
-## Install
-
-`filepattern` is pip installable from https://pypi.org/project/filepattern/.
-
-or by running
-
-pip install -i https://pypi.org/simple/ filepattern
-
-
-## Build and Install
-Alternatively, ``filepattern`` can either be build inside a `conda` environment or independently outside of it directly from the source.
-
-### __Inside Conda__
-``filepattern`` uses a CMake build system.
-Below is an example of how to build ``filepattern`` Python package inside a `conda` environment on Linux.
-
-```bash
-git clone https://github.com/PolusAI/filepattern.git
-cd filepattern
-conda install -y -c conda-forge compilers --file ci-utils/envs/conda_cpp.txt --file ci-utils/envs/conda_py.txt
-CMAKE_ARGS="-DCMAKE_PREFIX_PATH=$CONDA_PREFIX -DCMAKE_INSTALL_PREFIX=$CONDA_PREFIX " python -m pip install . -vv
-```
-
-### __Without Using Conda__
-To build ``filepattern`` outside of a `conda` environment, use the following example.
-```bash
-git clone https://github.com/PolusAI/filepattern.git
-cd filepattern
-mkdir build_dep
-cd build_dep
-bash ../ci-utils/install_prereq_linux.sh
-cd ..
-export FILEPATTERN_DEP_DIR=./build_dep/local_install
-python -m pip install . -vv
-```
-
-### __C++ Library__
-``filepattern`` also comes with a C++ API. To build and install ``filepattern`` as a C++ library, following the steps below.
-```bash
-git clone https://github.com/PolusAI/filepattern.git
-cd filepattern
-mkdir build
-cd build
-bash ../ci-utils/install_prereq_linux.sh
-cmake -Dfilepattern_SHARED_LIB=ON -DCMAKE_PREFIX_PATH=./local_install -DCMAKE_INSTALL_PREFIX=./local_install ../src/filepattern/cpp/
-make -j4
-make install
-```
-To link ``filepattern`` with the client code, use the following CMake statements.
-```
-find_package(filepattern REQUIRED)
-target_link_libraries(client_executable PRIVATE filepattern::filepattern)
-```
-
-<h2 id="filepattern-section"> Filepattern </h2>
-
-When only a path to a directory and a pattern are supplied to the constructor of ``filepattern``, ``filepattern`` will iterate over the directory, matching the filenames in the directory to the ``filepattern``. The  ``filepattern`` can either be supplied by  the user or can be found using the ``infer_pattern`` method of ``filepattern``. For example, consider a directory containing the following files,
-
-```
-img_r001_c001_DAPI.tif
-img_r001_c001_TXREAD.tif
-img_r001_c001_GFP.tif
-```
-
-In each of these filenames, there are three descriptors of the image: the row, the column, and the channel. To match these files, the pattern ``img_r{r:ddd}_c{c:ddd}_{channel:c+}`` can be used. In this pattern, the named groups are contained within the curly brackets, where the variable name is before the colon and the value is after the colon. For the value, the descriptors ``d`` and ``c`` are used, which represent a digit and a character, respectively. In the example pattern, three `d`'s are used to capture three digits. The ``+`` after ``c`` denotes that one or more characters will be captured, which is equivalent to ``[a-zA-z]+`` in a regular expression. The ``+`` symbol may be used after either ``d`` or ``c``.
-
-To have ``filepattern`` guess what the pattern is for a directory, the static method ``infer_pattern`` can be used:
-
-```python
-import filepattern as fp
-
-path = 'path/to/directory'
-
-pattern = fp.infer_pattern(path)
-
-print(pattern)
-
-```
-The result is:
-
-```
-img_r001_c001_{r:c+}.tif
-```
-
-Note that the ``infer_pattern`` can also guess the patterns from stitching vectors and text files when a path to a text file is passed, rather than a path to a directory.
-
-To retrieve files from a directory that match the ``filepattern``, an iterator is called on the `FilePattern` object, as shown below. A user specified custom pattern, such as the one below, or the guessed pattern can be passed to the constructor.
-
-```python
-import filepattern as fp
-import pprint
-
-filepath = "path/to/directory"
-
-pattern = "img_r{r:ddd}_c{c:ddd}_{channel:c+}.tif"
-
-files = fp.FilePattern(filepath, pattern)
-
-for file in files():
-    pprint.pprint(file)
-```
-The output is:
-```
-({'c': 1, 'channel': 'DAPI', 'r': 1},
- ['path/to/directory/img_r001_c001_DAPI.tif'])
-({'c': 1, 'channel': 'TXREAD', 'r': 1},
- ['path/to/directory/img_r001_c001_TXREAD.tif'])
-({'c': 1, 'channel': 'GFP', 'r': 1},
- ['path/to/directory/img_r001_c001_GFP.tif'])
-```
-
-As shown in this example, the output is a tuple where the first member is a map between the group name supplied in the pattern and the value of the group for each file name. The second member of the tuple is a vector containing the path to the matched file. The second member is stored in a vector for the case where a directory is supplied with multiple subdirectories. In this case, a third optional parameter can be passed to the constructor. If the parameter ``recursive`` is set to `True`, a recursive directory iterator will be used, which iterates over all subdirectories. If the basename of two files from two different subdirectories match, ``filepattern`` will add the path of the file to the vector in the existing tuple rather than creating a new tuple.
-
- For example, consider the directory with the structure
-
-```
-/root_directory
-    /DAPI
-        img_r001_c001.tif
-    /GFP
-        img_r001_c001.tif
-    /TXREAD
-        img_r001_c001.tif
-```
-
-In this case, the subdirectories are split by the channel. Recursive matching can be used as shown below.
-
-```python
-import filepattern as fp
-import pprint
-
-filepath = "path/to/root/directory"
-
-pattern = "img_r{r:ddd}_c{c:ddd}.tif"
-
-files = fp.FilePattern(filepath, pattern, recursive=True)
-
-for file in files():
-    pprint.pprint(file)
-```
-
-The output of this case is:
-```
-({'c': 1, 'r': 1},
- ['path/to/root/directory/DAPI/img_r001_c001.tif',
-  'path/to/root/directory/GFP/img_r001_c001.tif',
-  'path/to/root/directory/TXREAD/img_r001_c001.tif'])
-```
-
-<h3 id="floating-point"> Floating Point Support </h3>
-`filepattern` has the ability to capture floating point values in file patterns. For example, if we have a set of files
-
-```
-img_r0.05_c1.15.tif
-img_r1.05_c2.25.tif
-img_r2.05_c3.35.tif
-```
-
-We can capture the values in a couple of different ways. Similar to capturing digits, the character `f` can be used to capture an element of a floating point number.
-Note that with this method, the decimal point in the number must be captured by an `f`. For example, in the file `img_r0.05_c1.15.tif`, the floating point numbers would be capture with `ffff`.
-The code to utilize this method is
-
-```python
-filepath = "path/to/directory"
-
-pattern = "img_r{r:ffff}_c{c:ffff}.tif"
-
-files = fp.FilePattern(filepath, pattern)
-
-for file in files():
-    pprint.pprint(file)
-```
-
-The result is:
-```
-({'c': 1.15, 'r': 0.05},
- ['path/to/directory/img_r0.05_c1.15.tif'])
-({'c': 2.25, 'r': 1.05},
- ['path/to/directory/img_r1.05_c2.25.tif'])
-({'c': 3.35, 'r': 2.05},
- ['path/to/directory/img_r2.05_c3.35.tif'])
-```
-
-To capture floating point numbers with an arbitrary number of digits, we can use `f+`. This method operates in the same way as using `d+` or `c+`, where all digits (and the decimal point) will be
-captured for a floating point of any length. The code for this method is
-
-```python
-filepath = "path/to/directory"
-
-pattern = "img_r{r:f+}_c{c:f+}.tif"
-
-files = fp.FilePattern(filepath, pattern)
-
-for file in files():
-    pprint.pprint(file)
-```
-
-The result of this code is the same as the previous example.
-
-The final method for capturing floating points is to use `d` to capture the digits and to add the decimal point where needed. For example, in the file `img_r0.05_c1.15.tif`, the floating point numbers could be captured using `d.dd`. The code for this method is:
-
-```python
-filepath = "path/to/directory"
-
-pattern = "img_r{r:d.dd}_c{c:d.dd}.tif"
-
-files = fp.FilePattern(filepath, pattern)
-
-for file in files():
-    pprint.pprint(file)
-```
-
-Once again, the results are the same as the first example.
-
-Note that `d` can be used to specify even more specific floating points. For example, if we want to capturing all floating points with one digit in the whole part and an arbitrary number of digits in the decimal, we can add `d.d+` for the pattern. Similarly, this could be used in a reverse manner to capture an arbitrary number of digits in the whole part using `d+.ddd`.
-
-<h3 id="group-by"> Group By </h3>
-
-If images need to be processed in a specific order, for example by the row number, the ``group_by`` function is used. With the directory
-
-```
-img_r001_c001_DAPI.tif
-img_r002_c001_DAPI.tif
-img_r001_c001_TXREAD.tif
-img_r002_c001_TXREAD.tif
-img_r001_c001_GFP.tif
-img_r002_c001_GFP.tif
-```
-
-the images can be returned in groups where ``r`` is held constant by passing the parameter ``group_by='r'`` to the object iterator.
-
-```python
-import filepattern as fp
-import pprint
-
-filepath = "path/to/directory"
-
-pattern = "img_r{r:ddd}_c{c:ddd}_{channel:c+}.tif"
-
-files = fp.FilePattern(filepath, pattern)
-
-for file in files(group_by='r'):
-    pprint.pprint(file)
-```
-
-The output is:
-```
-('r': 1, [({'c': 1, 'channel': 'DAPI', 'file': 0, 'r': 1},
-  ['/home/ec2-user/Dev/FilePattern/data/example/img_r001_c001_DAPI.tif']),
- ({'c': 1, 'channel': 'TXREAD', 'file': 0, 'r': 1},
-  ['/home/ec2-user/Dev/FilePattern/data/example/img_r001_c001_TXREAD.tif']),
- ({'c': 1, 'channel': 'GFP', 'file': 0, 'r': 1},
-  ['/home/ec2-user/Dev/FilePattern/data/example/img_r001_c001_GFP.tif'])])
-('r': 2, [({'c': 1, 'channel': 'DAPI', 'file': 0, 'r': 2},
-  ['/home/ec2-user/Dev/FilePattern/data/example/img_r002_c001_DAPI.tif']),
- ({'c': 1, 'channel': 'GFP', 'file': 0, 'r': 2},
-  ['/home/ec2-user/Dev/FilePattern/data/example/img_r002_c001_GFP.tif']),
- ({'c': 1, 'channel': 'TXREAD', 'file': 0, 'r': 2},
-  ['/home/ec2-user/Dev/FilePattern/data/example/img_r002_c001_TXREAD.tif'])])
-```
-Note that the return of each call is a tuple where the first member is the ``group_by`` variable mapped to the current value and the second member is a list of files where the ``group_by`` variable matches the current value.
-
-<h3 id="get-matching"> Get Matching </h3>
-
-To get files where the variable matches a value, the ``get_matching`` method is used. For example, if only files from the TXREAD channel are needed, ``get_matching(channel=['TXREAD']`` is called.
-
-```python
-filepath = "/home/ec2-user/Dev/FilePattern/data/example"
-
-pattern = "img_r{r:ddd}_c{c:ddd}_{channel:c+}.tif"
-
-files = fp.FilePattern(filepath, pattern)
-
-matching = files.get_matching(channel=['TXREAD'])
-
-pprint.pprint(matching)
-```
-
-The output is:
-```
-[({'c': 1, 'channel': 'TXREAD', 'r': 1},
-  ['/home/ec2-user/Dev/FilePattern/data/example/img_r001_c001_TXREAD.tif']),
- ({'c': 1, 'channel': 'TXREAD', 'r': 2},
-  ['/home/ec2-user/Dev/FilePattern/data/example/img_r002_c001_TXREAD.tif'])]
-```
-
-## Text files
-``filepattern`` can also take in a text file as an input rather than a directory. To use this functionality, a path to a text file is supplied to the ``path`` variable rather than a directory. When a text file is passed as input, each line of the text file will be matched to the pattern. For example, a text file containing containing the strings
-```
-img_r001_c001_DAPI.tif
-img_r001_c001_TXREAD.tif
-img_r001_c001_GFP.tif
-```
-
-can be matched to the pattern ```img_r{r:ddd}_c{c:ddd}_{channel:c+}.tif``` with:
-
-```python
-import filepattern as fp
-import pprint
-
-filepath = "path/to/file.txt"
-
-pattern = "img_r{r:ddd}_c{c:ddd}_{channel:c+}.tif"
-
-files = fp.FilePattern(filepath, pattern)
-
-for file in files():
-    pprint.pprint(file)
-
-```
-
-The output is:
-
-```
-({'c': 1, 'channel': 'DAPI', 'r': 1},
- ['img_r001_c001_DAPI.tif'])
-({'c': 1, 'channel': 'TXREAD', 'r': 1},
- ['img_r001_c001_TXREAD.tif'])
-({'c': 1, 'channel': 'GFP', 'r': 1},
- ['img_r001_c001_GFP.tif'])
-```
-
- After calling ``filepattern`` on a text file,  the [group_by](#group-by) and [get_matching](#get-matching) functionality can be used the same as outlined in the [FilePattern](#filepattern-section) section.
-
-## Stitching vectors
-
-``filepattern`` can also take in stitching vectors as input. In this case, a path to a text file containing a stitching vector is passed to the ``path`` variable. A stitching vector has the following form,
-
-```
-file: x01_y01_wx0_wy0_c1.ome.tif; corr: 0; position: (0, 0); grid: (0, 0);
-file: x02_y01_wx0_wy0_c1.ome.tif; corr: 0; position: (3496, 0); grid: (3, 0);
-file: x03_y01_wx0_wy0_c1.ome.tif; corr: 0; position: (6992, 0); grid: (6, 0);
-file: x04_y01_wx0_wy0_c1.ome.tif; corr: 0; position: (10488, 0); grid: (9, 0);
-```
-
-This stitching vector can be processed using
-
-```python
-import filepattern as fp
-
-filepath = 'path/to/stitching/vector.txt'
-
-pattern = 'x0{x:d}_y01_wx0_wy0_c1.ome.tif'
-
-files = fp.FilePattern(filepath, pattern)
-
-for file in files():
-    pprint.pprint(files)
-```
-
-The output is:
-```
-({'correlation': 0, 'gridX': 0, 'gridY': 0, 'posX': 0, 'posY': 0, 'x': 1},
- ['x01_y01_wx0_wy0_c1.ome.tif'])
-({'correlation': 0, 'gridX': 3, 'gridY': 0, 'posX': 3496, 'posY': 0, 'x': 2},
- ['x02_y01_wx0_wy0_c1.ome.tif'])
-({'correlation': 0, 'gridX': 6, 'gridY': 0, 'posX': 6992, 'posY': 0, 'x': 3},
- ['x03_y01_wx0_wy0_c1.ome.tif'])
-({'correlation': 0, 'gridX': 9, 'gridY': 0, 'posX': 10488, 'posY': 0, 'x': 4},
- ['x04_y01_wx0_wy0_c1.ome.tif'])
-```
-As shown in the output, ``filepattern`` not only captures the specified variables from the pattern, but also captures the variables supplied in the stitching vector.
-
-## Out of core
-
-``filepattern`` has the ability to use external memory when the dataset is too large to fit in main memory, i.e. it utilizes disk memory along with RAM. It has the same functionality as ``filepattern``, however it takes in an addition parameter called `block_size`, which limits the amount of main memory used by ``filepattern``. Consider a directory containing the files:
-
-```
-img_r001_c001_DAPI.tif
-img_r001_c001_TXREAD.tif
-img_r001_c001_GFP.tif
-```
-
-This directory can be processed with only one file in memory as:
-
-```python
-import filepattern as fp
-import pprint
-
-filepath = "path/to/directory"
-
-pattern = "img_r{r:ddd}_c{c:ddd}_{channel:c+}.tif"
-
-files = fp.FilePattern(filepath, pattern, block_size="125 B")
-
-
-for file in files():
-    pprint.pprint(file)
-
-
-```
-The output from this example is:
-
-```
-({'c': 1, 'channel': 'DAPI', 'r': 1},
- ['/home/ec2-user/Dev/FilePattern/data/example/img_r001_c001_DAPI.tif'])
-({'c': 1, 'channel': 'TXREAD', 'r': 1},
- ['/home/ec2-user/Dev/FilePattern/data/example/img_r001_c001_TXREAD.tif'])
-({'c': 1, 'channel': 'GFP', 'r': 1},
- ['/home/ec2-user/Dev/FilePattern/data/example/img_r001_c001_GFP.tif'])
-```
-Note that the ``block_size`` argument is provided in bytes (B) in this example, but also has the options for kilobytes (KB), megabytes (MB), and gigabytes (GB). The ``block_size`` must be under 1000 GB.
-
-<h3 id="group-by-external"> Group by and get matching</h3>
-
-The out of core version of ``filepattern`` contains the same functionalities as the in memory version. ``group_by`` is called the same way, i.e.,
-
-```python
-for file in files(group_by="r"):
-    pprint.pprint(file)
-```
-
-The output remains identical to the in memory version.
-
-The ``get_matching`` functionality remains the same, however the API is slightly different. In this case, ``get_matching`` is called as
-
-```python
-
-for matching in files.get_matching(channel=['TXREAD'])
-    pprint.pprint(matching)
-```
-where the output is returned in blocks of `block_size`. The output is:
-
-```
-({'c': 1, 'channel': 'TXREAD', 'r': 1},
- ['/home/ec2-user/Dev/FilePattern/data/example/img_r001_c001_TXREAD.tif'])
-```
-
-## Out of Core: text files and stitching vectors
-
-Out of core processing can also be used for stitching vectors and text files. To utilize this functionality, call ``filepattern`` the same way as described previously, but add in the ``block_size`` parameter, as described in the (Out of Core)[#out-of-core] section.
-
-## Authors
-
-Jesse McKinzie(Jesse.McKinzie@axleinfo.com, jesse.mckinzie@nih.gov)
-Nick Schaub (nick.schaub@nih.gov, nick.schaub@labshare.org)
-
-## License
-
-This project is licensed under the [MIT License](LICENSE)
-Creative Commons License - see the [LICENSE](LICENSE) file for
-details
-
-## Acknowledgments
-
-- This utility was inspired by the notation found in the
-[MIST](https://github.com/usnistgov/MIST)
-algorithm developed at NIST.
+Metadata-Version: 2.1
+Name: filepattern
+Version: 2.0.6
+Summary: Utilities for parsing files in a directory based on a file name pattern.
+Home-page: https://github.com/PolusAI/filepattern
+Author: Jesse McKinzie, Nick Schaub
+Author-email: Jesse.McKinzie@axleinfo.com, nick.schaub@nih.gov
+Project-URL: Documentation, https://filepattern.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/PolusAI/filepattern
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pydantic
+
+# Filepattern
+
+[![Documentation Status](https://readthedocs.org/projects/filepattern/badge/?version=latest)](https://filepattern.readthedocs.io/en/latest/?badge=latest)
+[![PyPI](https://img.shields.io/pypi/v/filepattern)](https://pypi.org/project/filepattern/)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/filepattern)
+![Bower](https://img.shields.io/bower/l/MI)
+
+The ``filepattern`` utility is used to store files that follow a pattern, where the pattern is analogous to a simplified regular expression. The need for
+``filepattern`` arises in situations where large amounts of data with a systematic naming convention needs to be filtered by patterns in the naming. For example, one may have
+a directory containing segmented images where the name contains information such as the channel, the column value, and the row value. ``filepattern`` provides the ability to
+extract all images containing such a naming pattern, filter by the row or column value, or group files by one or more of the aforementioned variables.
+
+## Summary
+- [Read the Docs](https://filepattern2.readthedocs.io/en/latest/Home.html)
+- [Install](#install)
+- [Authors](#authors)
+- [License](#license)
+- [Acknowledgments](#acknowledgments)
+
+## Install
+
+`filepattern` is pip installable from https://pypi.org/project/filepattern/.
+
+or by running
+
+pip install -i https://pypi.org/simple/ filepattern
+
+
+## Build and Install
+Alternatively, ``filepattern`` can either be build inside a `conda` environment or independently outside of it directly from the source.
+
+### __Inside Conda__
+``filepattern`` uses a CMake build system.
+Below is an example of how to build ``filepattern`` Python package inside a `conda` environment on Linux.
+
+```bash
+git clone https://github.com/PolusAI/filepattern.git
+cd filepattern
+conda install -y -c conda-forge compilers --file ci-utils/envs/conda_cpp.txt --file ci-utils/envs/conda_py.txt
+CMAKE_ARGS="-DCMAKE_PREFIX_PATH=$CONDA_PREFIX -DCMAKE_INSTALL_PREFIX=$CONDA_PREFIX " python -m pip install . -vv
+```
+
+### __Without Using Conda__
+To build ``filepattern`` outside of a `conda` environment, use the following example.
+```bash
+git clone https://github.com/PolusAI/filepattern.git
+cd filepattern
+mkdir build_dep
+cd build_dep
+bash ../ci-utils/install_prereq_linux.sh
+cd ..
+export FILEPATTERN_DEP_DIR=./build_dep/local_install
+python -m pip install . -vv
+```
+
+### __C++ Library__
+``filepattern`` also comes with a C++ API. To build and install ``filepattern`` as a C++ library, following the steps below.
+```bash
+git clone https://github.com/PolusAI/filepattern.git
+cd filepattern
+mkdir build
+cd build
+bash ../ci-utils/install_prereq_linux.sh
+cmake -Dfilepattern_SHARED_LIB=ON -DCMAKE_PREFIX_PATH=./local_install -DCMAKE_INSTALL_PREFIX=./local_install ../src/filepattern/cpp/
+make -j4
+make install
+```
+To link ``filepattern`` with the client code, use the following CMake statements.
+```
+find_package(filepattern REQUIRED)
+target_link_libraries(client_executable PRIVATE filepattern::filepattern)
+```
+
+<h2 id="filepattern-section"> Filepattern </h2>
+
+When only a path to a directory and a pattern are supplied to the constructor of ``filepattern``, ``filepattern`` will iterate over the directory, matching the filenames in the directory to the ``filepattern``. The  ``filepattern`` can either be supplied by  the user or can be found using the ``infer_pattern`` method of ``filepattern``. For example, consider a directory containing the following files,
+
+```
+img_r001_c001_DAPI.tif
+img_r001_c001_TXREAD.tif
+img_r001_c001_GFP.tif
+```
+
+In each of these filenames, there are three descriptors of the image: the row, the column, and the channel. To match these files, the pattern ``img_r{r:ddd}_c{c:ddd}_{channel:c+}`` can be used. In this pattern, the named groups are contained within the curly brackets, where the variable name is before the colon and the value is after the colon. For the value, the descriptors ``d`` and ``c`` are used, which represent a digit and a character, respectively. In the example pattern, three `d`'s are used to capture three digits. The ``+`` after ``c`` denotes that one or more characters will be captured, which is equivalent to ``[a-zA-z]+`` in a regular expression. The ``+`` symbol may be used after either ``d`` or ``c``.
+
+To have ``filepattern`` guess what the pattern is for a directory, the static method ``infer_pattern`` can be used:
+
+```python
+import filepattern as fp
+
+path = 'path/to/directory'
+
+pattern = fp.infer_pattern(path)
+
+print(pattern)
+
+```
+The result is:
+
+```
+img_r001_c001_{r:c+}.tif
+```
+
+Note that the ``infer_pattern`` can also guess the patterns from stitching vectors and text files when a path to a text file is passed, rather than a path to a directory.
+
+To retrieve files from a directory that match the ``filepattern``, an iterator is called on the `FilePattern` object, as shown below. A user specified custom pattern, such as the one below, or the guessed pattern can be passed to the constructor.
+
+```python
+import filepattern as fp
+import pprint
+
+filepath = "path/to/directory"
+
+pattern = "img_r{r:ddd}_c{c:ddd}_{channel:c+}.tif"
+
+files = fp.FilePattern(filepath, pattern)
+
+for file in files():
+    pprint.pprint(file)
+```
+The output is:
+```
+({'c': 1, 'channel': 'DAPI', 'r': 1},
+ ['path/to/directory/img_r001_c001_DAPI.tif'])
+({'c': 1, 'channel': 'TXREAD', 'r': 1},
+ ['path/to/directory/img_r001_c001_TXREAD.tif'])
+({'c': 1, 'channel': 'GFP', 'r': 1},
+ ['path/to/directory/img_r001_c001_GFP.tif'])
+```
+
+As shown in this example, the output is a tuple where the first member is a map between the group name supplied in the pattern and the value of the group for each file name. The second member of the tuple is a vector containing the path to the matched file. The second member is stored in a vector for the case where a directory is supplied with multiple subdirectories. In this case, a third optional parameter can be passed to the constructor. If the parameter ``recursive`` is set to `True`, a recursive directory iterator will be used, which iterates over all subdirectories. If the basename of two files from two different subdirectories match, ``filepattern`` will add the path of the file to the vector in the existing tuple rather than creating a new tuple.
+
+ For example, consider the directory with the structure
+
+```
+/root_directory
+    /DAPI
+        img_r001_c001.tif
+    /GFP
+        img_r001_c001.tif
+    /TXREAD
+        img_r001_c001.tif
+```
+
+In this case, the subdirectories are split by the channel. Recursive matching can be used as shown below.
+
+```python
+import filepattern as fp
+import pprint
+
+filepath = "path/to/root/directory"
+
+pattern = "img_r{r:ddd}_c{c:ddd}.tif"
+
+files = fp.FilePattern(filepath, pattern, recursive=True)
+
+for file in files():
+    pprint.pprint(file)
+```
+
+The output of this case is:
+```
+({'c': 1, 'r': 1},
+ ['path/to/root/directory/DAPI/img_r001_c001.tif',
+  'path/to/root/directory/GFP/img_r001_c001.tif',
+  'path/to/root/directory/TXREAD/img_r001_c001.tif'])
+```
+
+<h3 id="floating-point"> Floating Point Support </h3>
+`filepattern` has the ability to capture floating point values in file patterns. For example, if we have a set of files
+
+```
+img_r0.05_c1.15.tif
+img_r1.05_c2.25.tif
+img_r2.05_c3.35.tif
+```
+
+We can capture the values in a couple of different ways. Similar to capturing digits, the character `f` can be used to capture an element of a floating point number.
+Note that with this method, the decimal point in the number must be captured by an `f`. For example, in the file `img_r0.05_c1.15.tif`, the floating point numbers would be capture with `ffff`.
+The code to utilize this method is
+
+```python
+filepath = "path/to/directory"
+
+pattern = "img_r{r:ffff}_c{c:ffff}.tif"
+
+files = fp.FilePattern(filepath, pattern)
+
+for file in files():
+    pprint.pprint(file)
+```
+
+The result is:
+```
+({'c': 1.15, 'r': 0.05},
+ ['path/to/directory/img_r0.05_c1.15.tif'])
+({'c': 2.25, 'r': 1.05},
+ ['path/to/directory/img_r1.05_c2.25.tif'])
+({'c': 3.35, 'r': 2.05},
+ ['path/to/directory/img_r2.05_c3.35.tif'])
+```
+
+To capture floating point numbers with an arbitrary number of digits, we can use `f+`. This method operates in the same way as using `d+` or `c+`, where all digits (and the decimal point) will be
+captured for a floating point of any length. The code for this method is
+
+```python
+filepath = "path/to/directory"
+
+pattern = "img_r{r:f+}_c{c:f+}.tif"
+
+files = fp.FilePattern(filepath, pattern)
+
+for file in files():
+    pprint.pprint(file)
+```
+
+The result of this code is the same as the previous example.
+
+The final method for capturing floating points is to use `d` to capture the digits and to add the decimal point where needed. For example, in the file `img_r0.05_c1.15.tif`, the floating point numbers could be captured using `d.dd`. The code for this method is:
+
+```python
+filepath = "path/to/directory"
+
+pattern = "img_r{r:d.dd}_c{c:d.dd}.tif"
+
+files = fp.FilePattern(filepath, pattern)
+
+for file in files():
+    pprint.pprint(file)
+```
+
+Once again, the results are the same as the first example.
+
+Note that `d` can be used to specify even more specific floating points. For example, if we want to capturing all floating points with one digit in the whole part and an arbitrary number of digits in the decimal, we can add `d.d+` for the pattern. Similarly, this could be used in a reverse manner to capture an arbitrary number of digits in the whole part using `d+.ddd`.
+
+<h3 id="group-by"> Group By </h3>
+
+If images need to be processed in a specific order, for example by the row number, the ``group_by`` function is used. With the directory
+
+```
+img_r001_c001_DAPI.tif
+img_r002_c001_DAPI.tif
+img_r001_c001_TXREAD.tif
+img_r002_c001_TXREAD.tif
+img_r001_c001_GFP.tif
+img_r002_c001_GFP.tif
+```
+
+the images can be returned in groups where ``r`` is held constant by passing the parameter ``group_by='r'`` to the object iterator.
+
+```python
+import filepattern as fp
+import pprint
+
+filepath = "path/to/directory"
+
+pattern = "img_r{r:ddd}_c{c:ddd}_{channel:c+}.tif"
+
+files = fp.FilePattern(filepath, pattern)
+
+for file in files(group_by='r'):
+    pprint.pprint(file)
+```
+
+The output is:
+```
+('r': 1, [({'c': 1, 'channel': 'DAPI', 'file': 0, 'r': 1},
+  ['/home/ec2-user/Dev/FilePattern/data/example/img_r001_c001_DAPI.tif']),
+ ({'c': 1, 'channel': 'TXREAD', 'file': 0, 'r': 1},
+  ['/home/ec2-user/Dev/FilePattern/data/example/img_r001_c001_TXREAD.tif']),
+ ({'c': 1, 'channel': 'GFP', 'file': 0, 'r': 1},
+  ['/home/ec2-user/Dev/FilePattern/data/example/img_r001_c001_GFP.tif'])])
+('r': 2, [({'c': 1, 'channel': 'DAPI', 'file': 0, 'r': 2},
+  ['/home/ec2-user/Dev/FilePattern/data/example/img_r002_c001_DAPI.tif']),
+ ({'c': 1, 'channel': 'GFP', 'file': 0, 'r': 2},
+  ['/home/ec2-user/Dev/FilePattern/data/example/img_r002_c001_GFP.tif']),
+ ({'c': 1, 'channel': 'TXREAD', 'file': 0, 'r': 2},
+  ['/home/ec2-user/Dev/FilePattern/data/example/img_r002_c001_TXREAD.tif'])])
+```
+Note that the return of each call is a tuple where the first member is the ``group_by`` variable mapped to the current value and the second member is a list of files where the ``group_by`` variable matches the current value.
+
+<h3 id="get-matching"> Get Matching </h3>
+
+To get files where the variable matches a value, the ``get_matching`` method is used. For example, if only files from the TXREAD channel are needed, ``get_matching(channel=['TXREAD']`` is called.
+
+```python
+filepath = "/home/ec2-user/Dev/FilePattern/data/example"
+
+pattern = "img_r{r:ddd}_c{c:ddd}_{channel:c+}.tif"
+
+files = fp.FilePattern(filepath, pattern)
+
+matching = files.get_matching(channel=['TXREAD'])
+
+pprint.pprint(matching)
+```
+
+The output is:
+```
+[({'c': 1, 'channel': 'TXREAD', 'r': 1},
+  ['/home/ec2-user/Dev/FilePattern/data/example/img_r001_c001_TXREAD.tif']),
+ ({'c': 1, 'channel': 'TXREAD', 'r': 2},
+  ['/home/ec2-user/Dev/FilePattern/data/example/img_r002_c001_TXREAD.tif'])]
+```
+
+## Text files
+``filepattern`` can also take in a text file as an input rather than a directory. To use this functionality, a path to a text file is supplied to the ``path`` variable rather than a directory. When a text file is passed as input, each line of the text file will be matched to the pattern. For example, a text file containing containing the strings
+```
+img_r001_c001_DAPI.tif
+img_r001_c001_TXREAD.tif
+img_r001_c001_GFP.tif
+```
+
+can be matched to the pattern ```img_r{r:ddd}_c{c:ddd}_{channel:c+}.tif``` with:
+
+```python
+import filepattern as fp
+import pprint
+
+filepath = "path/to/file.txt"
+
+pattern = "img_r{r:ddd}_c{c:ddd}_{channel:c+}.tif"
+
+files = fp.FilePattern(filepath, pattern)
+
+for file in files():
+    pprint.pprint(file)
+
+```
+
+The output is:
+
+```
+({'c': 1, 'channel': 'DAPI', 'r': 1},
+ ['img_r001_c001_DAPI.tif'])
+({'c': 1, 'channel': 'TXREAD', 'r': 1},
+ ['img_r001_c001_TXREAD.tif'])
+({'c': 1, 'channel': 'GFP', 'r': 1},
+ ['img_r001_c001_GFP.tif'])
+```
+
+ After calling ``filepattern`` on a text file,  the [group_by](#group-by) and [get_matching](#get-matching) functionality can be used the same as outlined in the [FilePattern](#filepattern-section) section.
+
+## Stitching vectors
+
+``filepattern`` can also take in stitching vectors as input. In this case, a path to a text file containing a stitching vector is passed to the ``path`` variable. A stitching vector has the following form,
+
+```
+file: x01_y01_wx0_wy0_c1.ome.tif; corr: 0; position: (0, 0); grid: (0, 0);
+file: x02_y01_wx0_wy0_c1.ome.tif; corr: 0; position: (3496, 0); grid: (3, 0);
+file: x03_y01_wx0_wy0_c1.ome.tif; corr: 0; position: (6992, 0); grid: (6, 0);
+file: x04_y01_wx0_wy0_c1.ome.tif; corr: 0; position: (10488, 0); grid: (9, 0);
+```
+
+This stitching vector can be processed using
+
+```python
+import filepattern as fp
+
+filepath = 'path/to/stitching/vector.txt'
+
+pattern = 'x0{x:d}_y01_wx0_wy0_c1.ome.tif'
+
+files = fp.FilePattern(filepath, pattern)
+
+for file in files():
+    pprint.pprint(files)
+```
+
+The output is:
+```
+({'correlation': 0, 'gridX': 0, 'gridY': 0, 'posX': 0, 'posY': 0, 'x': 1},
+ ['x01_y01_wx0_wy0_c1.ome.tif'])
+({'correlation': 0, 'gridX': 3, 'gridY': 0, 'posX': 3496, 'posY': 0, 'x': 2},
+ ['x02_y01_wx0_wy0_c1.ome.tif'])
+({'correlation': 0, 'gridX': 6, 'gridY': 0, 'posX': 6992, 'posY': 0, 'x': 3},
+ ['x03_y01_wx0_wy0_c1.ome.tif'])
+({'correlation': 0, 'gridX': 9, 'gridY': 0, 'posX': 10488, 'posY': 0, 'x': 4},
+ ['x04_y01_wx0_wy0_c1.ome.tif'])
+```
+As shown in the output, ``filepattern`` not only captures the specified variables from the pattern, but also captures the variables supplied in the stitching vector.
+
+## Out of core
+
+``filepattern`` has the ability to use external memory when the dataset is too large to fit in main memory, i.e. it utilizes disk memory along with RAM. It has the same functionality as ``filepattern``, however it takes in an addition parameter called `block_size`, which limits the amount of main memory used by ``filepattern``. Consider a directory containing the files:
+
+```
+img_r001_c001_DAPI.tif
+img_r001_c001_TXREAD.tif
+img_r001_c001_GFP.tif
+```
+
+This directory can be processed with only one file in memory as:
+
+```python
+import filepattern as fp
+import pprint
+
+filepath = "path/to/directory"
+
+pattern = "img_r{r:ddd}_c{c:ddd}_{channel:c+}.tif"
+
+files = fp.FilePattern(filepath, pattern, block_size="125 B")
+
+
+for file in files():
+    pprint.pprint(file)
+
+
+```
+The output from this example is:
+
+```
+({'c': 1, 'channel': 'DAPI', 'r': 1},
+ ['/home/ec2-user/Dev/FilePattern/data/example/img_r001_c001_DAPI.tif'])
+({'c': 1, 'channel': 'TXREAD', 'r': 1},
+ ['/home/ec2-user/Dev/FilePattern/data/example/img_r001_c001_TXREAD.tif'])
+({'c': 1, 'channel': 'GFP', 'r': 1},
+ ['/home/ec2-user/Dev/FilePattern/data/example/img_r001_c001_GFP.tif'])
+```
+Note that the ``block_size`` argument is provided in bytes (B) in this example, but also has the options for kilobytes (KB), megabytes (MB), and gigabytes (GB). The ``block_size`` must be under 1000 GB.
+
+<h3 id="group-by-external"> Group by and get matching</h3>
+
+The out of core version of ``filepattern`` contains the same functionalities as the in memory version. ``group_by`` is called the same way, i.e.,
+
+```python
+for file in files(group_by="r"):
+    pprint.pprint(file)
+```
+
+The output remains identical to the in memory version.
+
+The ``get_matching`` functionality remains the same, however the API is slightly different. In this case, ``get_matching`` is called as
+
+```python
+
+for matching in files.get_matching(channel=['TXREAD'])
+    pprint.pprint(matching)
+```
+where the output is returned in blocks of `block_size`. The output is:
+
+```
+({'c': 1, 'channel': 'TXREAD', 'r': 1},
+ ['/home/ec2-user/Dev/FilePattern/data/example/img_r001_c001_TXREAD.tif'])
+```
+
+## Out of Core: text files and stitching vectors
+
+Out of core processing can also be used for stitching vectors and text files. To utilize this functionality, call ``filepattern`` the same way as described previously, but add in the ``block_size`` parameter, as described in the (Out of Core)[#out-of-core] section.
+
+## Authors
+
+Jesse McKinzie(Jesse.McKinzie@axleinfo.com, jesse.mckinzie@nih.gov)
+Nick Schaub (nick.schaub@nih.gov, nick.schaub@labshare.org)
+
+## License
+
+This project is licensed under the [MIT License](LICENSE)
+Creative Commons License - see the [LICENSE](LICENSE) file for
+details
+
+## Acknowledgments
+
+- This utility was inspired by the notation found in the
+[MIST](https://github.com/usnistgov/MIST)
+algorithm developed at NIST.
```

