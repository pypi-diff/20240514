# Comparing `tmp/fosslight_yocto-3.1.28.tar.gz` & `tmp/fosslight_yocto-3.1.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fosslight_yocto-3.1.28.tar", last modified: Thu Apr 11 00:38:52 2024, max compression
+gzip compressed data, was "fosslight_yocto-3.1.29.tar", last modified: Tue May 14 13:51:02 2024, max compression
```

## Comparing `fosslight_yocto-3.1.28.tar` & `fosslight_yocto-3.1.29.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:38:52.235054 fosslight_yocto-3.1.28/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-11 00:38:52.235054 fosslight_yocto-3.1.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:38:52.235054 fosslight_yocto-3.1.28/files_for_preparation/
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/files_for_preparation/bom.bbclass
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 00:38:52.235054 fosslight_yocto-3.1.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:38:52.231054 fosslight_yocto-3.1.28/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:38:52.235054 fosslight_yocto-3.1.28/src/fosslight_yocto/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/src/fosslight_yocto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/src/fosslight_yocto/_help.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6050 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/src/fosslight_yocto/_overwrite_yaml.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10182 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/src/fosslight_yocto/_package_item.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3947 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/src/fosslight_yocto/_write_result_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/src/fosslight_yocto/_zip_source_works.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    46686 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/src/fosslight_yocto/create_oss_report_for_yocto.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8200 2024-04-11 00:38:38.000000 fosslight_yocto-3.1.28/src/fosslight_yocto/parsing_meta_doubleopen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:38:52.235054 fosslight_yocto-3.1.28/src/fosslight_yocto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-11 00:38:51.000000 fosslight_yocto-3.1.28/src/fosslight_yocto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-11 00:38:52.000000 fosslight_yocto-3.1.28/src/fosslight_yocto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 00:38:51.000000 fosslight_yocto-3.1.28/src/fosslight_yocto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-11 00:38:51.000000 fosslight_yocto-3.1.28/src/fosslight_yocto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-11 00:38:51.000000 fosslight_yocto-3.1.28/src/fosslight_yocto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-11 00:38:51.000000 fosslight_yocto-3.1.28/src/fosslight_yocto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:51:02.398532 fosslight_yocto-3.1.29/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 13:50:47.000000 fosslight_yocto-3.1.29/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-14 13:50:47.000000 fosslight_yocto-3.1.29/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-14 13:51:02.398532 fosslight_yocto-3.1.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-14 13:50:47.000000 fosslight_yocto-3.1.29/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:51:02.398532 fosslight_yocto-3.1.29/files_for_preparation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-14 13:50:47.000000 fosslight_yocto-3.1.29/files_for_preparation/bom.bbclass
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-14 13:50:47.000000 fosslight_yocto-3.1.29/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:51:02.398532 fosslight_yocto-3.1.29/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-14 13:50:47.000000 fosslight_yocto-3.1.29/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:51:02.394532 fosslight_yocto-3.1.29/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:51:02.398532 fosslight_yocto-3.1.29/src/fosslight_yocto/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:50:47.000000 fosslight_yocto-3.1.29/src/fosslight_yocto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-14 13:50:47.000000 fosslight_yocto-3.1.29/src/fosslight_yocto/_help.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6050 2024-05-14 13:50:47.000000 fosslight_yocto-3.1.29/src/fosslight_yocto/_overwrite_yaml.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10182 2024-05-14 13:50:47.000000 fosslight_yocto-3.1.29/src/fosslight_yocto/_package_item.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3947 2024-05-14 13:50:47.000000 fosslight_yocto-3.1.29/src/fosslight_yocto/_write_result_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-05-14 13:50:47.000000 fosslight_yocto-3.1.29/src/fosslight_yocto/_zip_source_works.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46930 2024-05-14 13:50:47.000000 fosslight_yocto-3.1.29/src/fosslight_yocto/create_oss_report_for_yocto.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8200 2024-05-14 13:50:47.000000 fosslight_yocto-3.1.29/src/fosslight_yocto/parsing_meta_doubleopen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:51:02.398532 fosslight_yocto-3.1.29/src/fosslight_yocto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-14 13:51:01.000000 fosslight_yocto-3.1.29/src/fosslight_yocto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-14 13:51:02.000000 fosslight_yocto-3.1.29/src/fosslight_yocto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:51:01.000000 fosslight_yocto-3.1.29/src/fosslight_yocto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-14 13:51:01.000000 fosslight_yocto-3.1.29/src/fosslight_yocto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-14 13:51:01.000000 fosslight_yocto-3.1.29/src/fosslight_yocto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 13:51:01.000000 fosslight_yocto-3.1.29/src/fosslight_yocto.egg-info/top_level.txt
```

### Comparing `fosslight_yocto-3.1.28/LICENSE` & `fosslight_yocto-3.1.29/LICENSE`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.28/PKG-INFO` & `fosslight_yocto-3.1.29/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight_yocto
-Version: 3.1.28
+Version: 3.1.29
 Summary: FOSSLight Yocto
 Home-page: https://github.com/fosslight/fosslight_yocto_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_yocto_scanner
 Description: <!--
         SPDX-FileCopyrightText: Copyright 2023 LG Electronics Inc.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fosslight_yocto Version: 3.1.28 Summary: FOSSLight
+Metadata-Version: 2.1 Name: fosslight_yocto Version: 3.1.29 Summary: FOSSLight
 Yocto Home-page: https://github.com/fosslight/fosslight_yocto_scanner Author:
 LG Electronics License: Apache-2.0 Download-URL: https://github.com/fosslight/
 fosslight_yocto_scanner Description:
                                                                        _[_K_o_r_e_a_n_]
 # FOSSLight Yocto Scanner [FOSSLight Yocto Scanner is released under the
 Apache-2.0 License.][Current python package version.][https://img.shields.io/
 pypi/pyversions/fosslight_yocto][![REUSE status](https://api.reuse.software/
```

### Comparing `fosslight_yocto-3.1.28/README.md` & `fosslight_yocto-3.1.29/README.md`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.28/files_for_preparation/bom.bbclass` & `fosslight_yocto-3.1.29/files_for_preparation/bom.bbclass`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.28/setup.py` & `fosslight_yocto-3.1.29/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 if __name__ == "__main__":
     setup(
         name='fosslight_yocto',
-        version='3.1.28',
+        version='3.1.29',
         package_dir={"": "src"},
         packages=find_packages(where='src'),
         description='FOSSLight Yocto',
         long_description=readme,
         long_description_content_type='text/markdown',
         license='Apache-2.0',
         author='LG Electronics',
```

### Comparing `fosslight_yocto-3.1.28/src/fosslight_yocto/_help.py` & `fosslight_yocto-3.1.29/src/fosslight_yocto/_help.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,23 +10,22 @@
     FOSSLight Yocto for parsing BOM.json
 
     Options:
         Mandatory
             -p <path>\t\t   Path of buildhistory/package
             -b <file_with_path>\t\t   bom.json
             -i <file_with_path>\t\t   installed-package-names.txt
-            -ip <file_with_path>\t\t   installed-packages.txt
+            -ip <file_with_path>\t   installed-packages.txt
 
         Optional
             -h\t\t\t\t   Print help message
             -v\t\t\t\t   Print FOSSLight yocto version
             -y <file_with_path>\t\t   oss-pkg-info.yaml
             -a <path>\t\t\t   Path to analyze the binaries
             -n\t\t\t\t   Print result in BIN(Android) format
-            -d\t\t\t\t   Change license to declared license
             -s\t\t\t\t   Analyze source code for unconfirmed Open Source
             -c\t\t\t\t   Analyze all the source code
             -e\t\t\t\t   Compress all the source code
             -o <path>\t\t\t   Output Path
             -f <format>\t\t\t   Output file format (excel, csv, opossum)
             -pr\t\t\t\t   Print all data of bom.json"""
```

### Comparing `fosslight_yocto-3.1.28/src/fosslight_yocto/_overwrite_yaml.py` & `fosslight_yocto-3.1.29/src/fosslight_yocto/_overwrite_yaml.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.28/src/fosslight_yocto/_package_item.py` & `fosslight_yocto-3.1.29/src/fosslight_yocto/_package_item.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.28/src/fosslight_yocto/_write_result_file.py` & `fosslight_yocto-3.1.29/src/fosslight_yocto/_write_result_file.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.28/src/fosslight_yocto/_zip_source_works.py` & `fosslight_yocto-3.1.29/src/fosslight_yocto/_zip_source_works.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.28/src/fosslight_yocto/create_oss_report_for_yocto.py` & `fosslight_yocto-3.1.29/src/fosslight_yocto/create_oss_report_for_yocto.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,29 +72,40 @@
 OSC_DB_USER = 'user_oss_license'
 OSC_DB_PASSWORD = 'oss_lic123'
 
 
 def read_installed_pkg_file(installed_pkg_names_file):
     global installed_packages_src
     installed_packages_src = []
-
+    success = True
     try:
         success, lines = read_file(installed_pkg_names_file)
         for line in lines:
             if line != "":
                 pkg_name = line.strip()
                 pkg_item = PackageItem()
-                if pkg_name != "":
+                if pkg_name:
                     pkg_item = update_package_name(pkg_item, pkg_name, nested_pkg_name)
                     if pkg_name in bom_pkg_data:
                         for key, value in bom_pkg_data[pkg_name].items():
                             set_value_switch(pkg_item, key, value, nested_pkg_name)
                     installed_packages_src.append(pkg_item)
+                    if not pkg_item.oss_name:
+                        logger.error(f"Can't find recipe for {pkg_name}")
+                        logger.error("Check whether you entered installed-package-names.txt with -i.")
+                        logger.info(f"---- Value entered with -i:{installed_pkg_names_file}")
+                        success = False
+                        break
     except Exception as ex:
         logger.error(f"Read {installed_pkg_names_file}: {ex}")
+        success = False
+    if not installed_packages_src:
+        logger.error(f"Empty File : {installed_pkg_names_file}")
+        success = False
+    return success
 
 
 def get_json_object(str_data):
     json_object = ""
     try:
         json_object = json.loads(str_data)
     except ValueError:
@@ -209,14 +220,17 @@
     global nested_pkg_name
     buildhistory_latest_pkg = {}  # Key :Recipe, Value: Recipe -- Parsed from buildhistory
     tmp_package_per_recipe_info = {}
     nested_pkg_name = {}
     not_installed_pkg = {}
 
     success, installed_pkg_version_lines = read_file(installed_pkg_version)
+    if not installed_pkg_version_lines:
+        logger.error(f"Empty File:{installed_pkg_version}")
+        return buildhistory_latest_pkg
 
     for root, dirs, files in os.walk(path_buildhistory):
         for file in files:
             if file == "latest":
                 dir_name, recipe_name = os.path.split(root)
                 read_sucess, lines = read_file(os.path.join(root, file))
                 file_contents = '\n'.join(lines)
@@ -337,16 +351,16 @@
     except Exception as error:
         logger.debug(f"get_checksum_and_tlsh: {error}")
     return checksum_value, tlsh_value
 
 
 def get_binary_list(buildhistory_package_files, path_to_find, output_txt):
     global installed_packages_bin, binary_list
-    _EXCLUDE_FILE_EXTENSION = ['png', 'gif', 'jpg', 'bmp', 'jpeg', 'qm']
-    _EXCLUDE_FILE_COMMAND_RESULT = ['data', 'timezone data']
+    EXCLUDE_FILE_EXTENSION = ['qm', 'pyc']
+    EXCLUDE_FILE_COMMAND_RESULT = ['data', 'timezone data']
     str_files = []  # string to print binary.txt
     file_list = []
     success = False
     PREFIX_BIN_FAILED = "[Binary Analysis Error] "
 
     if not os.path.isdir(path_to_find):
         logger.error(f"{PREFIX_BIN_FAILED}Directory not found: {path_to_find}\nPlease check the Path again.")
@@ -362,24 +376,24 @@
         return success
 
     for file_abs_path in tqdm(file_list):
         try:
             file = os.path.basename(file_abs_path)
             extension = os.path.splitext(file)[1][1:]
 
-            if not os.path.islink(file_abs_path) and extension not in _EXCLUDE_FILE_EXTENSION:
+            if not os.path.islink(file_abs_path) and extension not in EXCLUDE_FILE_EXTENSION:
                 file_abs_path = os.path.realpath(file_abs_path)
                 file_rel_path = "./" + os.path.relpath(file_abs_path, path_to_find)
 
                 if stat.S_ISFIFO(os.stat(file_abs_path).st_mode):
                     continue
                 if is_binary(file_abs_path):
                     file_command_result = magic.from_file(file_abs_path)
                     if file_command_result != "":
-                        excluded_keyword = [x for x in _EXCLUDE_FILE_COMMAND_RESULT if
+                        excluded_keyword = [x for x in EXCLUDE_FILE_COMMAND_RESULT if
                                             file_command_result.startswith(x)]
                         if len(excluded_keyword) > 0:
                             continue
                     file_to_find = ' '.join(
                         file_rel_path.split())  # If there are two or more spaces, it is changed to one space.
                     if file_to_find in buildhistory_package_files:
                         pkg_names = buildhistory_package_files[file_to_find]
@@ -401,25 +415,21 @@
                     if pkg_items is not None and len(pkg_items) > 0:
                         # Package already inserted. Just add file to it.
                         pkg_items[0].source_name_or_path = file_rel_path
                     else:  # New Package
                         pkg_item = PackageItem()
                         pkg_item = update_package_name(pkg_item, pkg_name, nested_pkg_name)
                         pkg_item.source_name_or_path = file_rel_path
-                        if pkg_name != "" and pkg_name in bom_pkg_data:
-                            for key, value in bom_pkg_data[pkg_name].items():
-                                set_value_switch(pkg_item, key, value, nested_pkg_name)
-                        else:
-                            if pkg_name != "":
+                        if pkg_name:
+                            if pkg_name in bom_pkg_data:
+                                for key, value in bom_pkg_data[pkg_name].items():
+                                    set_value_switch(pkg_item, key, value, nested_pkg_name)
+                            else:
                                 pkg_item.oss_name = pkg_name
                                 pkg_item.comment = "Can't find package info from bom."
-                            else:
-                                pkg_item.exclude = True
-                                pkg_item.comment = "Can't find package info from bom & buildhistory."
-
                         installed_packages_bin.append(pkg_item)
         except Exception as ex:
             logger.error(f"Get_binary_list: {ex}")
     if installed_packages_bin:
         success = True
     else:
         logger.error(f"{PREFIX_BIN_FAILED}Binary cannot be found (File Count: {len(file_list)}): {path_to_find}\nPlease check the Path again.")
@@ -966,15 +976,14 @@
     bom_file = "bom.json"
     installed_pkgs = "installed-package-names.txt"
     installed_pkgs_with_version = "installed-packages.txt"
     oss_pkg_yaml_file = ""
     buildhistory_path = ""
     bin_analysis_path = ""
     _print_bin_android = False
-    _change_license_to_declared_license = False
     _analyze_source = False
     _analyze_source_all = False
     _compress_source_all = False
     output_path = os.getcwd()
     output_src_analysis_file = "source_analysis_report"
     file_format = ""
 
@@ -986,15 +995,14 @@
     parser.add_argument('-y', '--yaml', type=str, required=False)
     parser.add_argument('-b', '--bom', type=str, required=False)
     parser.add_argument('-p', '--buildhistory', type=str, required=False)
     parser.add_argument('-a', '--analysis', type=str, required=False)
     parser.add_argument('-o', '--output', type=str, required=False)
     parser.add_argument('-f', '--format', type=str, required=False)
     parser.add_argument('-n', '--another', action='store_true', required=False)
-    parser.add_argument('-d', '--declared', action='store_true', required=False)
     parser.add_argument('-s', '--source', action='store_true', required=False)
     parser.add_argument('-c', '--complete', action='store_true', required=False)
     parser.add_argument('-e', '--compress', action='store_true', required=False)
     parser.add_argument('-pr', '--printall', action='store_true', required=False)
 
     args = parser.parse_args()
     if args.help:
@@ -1016,16 +1024,14 @@
     if args.format:
         file_format = args.format
     if args.output:
         output_path = args.output
     if args.another:
         # Print SRC result on BIN(Android) Sheet
         _print_bin_android = True
-    if args.declared:
-        _change_license_to_declared_license = True
     if args.source:
         _analyze_source = True
     if args.complete:
         _analyze_source = True
         _analyze_source_all = True
     if args.compress:
         _compress_source_all = True
@@ -1050,32 +1056,33 @@
     if not success:
         logger.error(f"Format error. {msg}")
         sys.exit(1)
 
     check_required_files(bom_file, installed_pkgs, buildhistory_path, installed_pkgs_with_version)
 
     # Parsing bom file for packages' data
-    read_bom_file(bom_file, find_latest_pkg_from_buildhistory(buildhistory_path, installed_pkgs_with_version))
+    pkg_from_buildhistory = find_latest_pkg_from_buildhistory(buildhistory_path, installed_pkgs_with_version)
+    if not pkg_from_buildhistory:
+        sys.exit(1)
+    read_bom_file(bom_file, pkg_from_buildhistory)
 
     # Dependency Analysis - SRC Sheet or BIN(Android) Sheet
-    read_installed_pkg_file(installed_pkgs)
+    success = read_installed_pkg_file(installed_pkgs)
+    if not success:
+        sys.exit(1)
 
     # Binary Analysis - BIN Sheet
-    if bin_analysis_path != "":
+    if bin_analysis_path:
         get_binary_list(find_package_files(buildhistory_path), bin_analysis_path, out_bin_txt)
 
     # Load oss-pkg-info.yaml
-    if oss_pkg_yaml_file != "":
+    if oss_pkg_yaml_file:
         installed_packages_src, installed_packages_bin = load_oss_pkg_info_yaml(oss_pkg_yaml_file, _print_bin_android,
                                                                                 installed_packages_src, installed_packages_bin, nested_pkg_name)
 
-    # Declare License by OSC System's OSS DB only in case multi or dual licenses
-    if _change_license_to_declared_license:
-        declare_license_by_osc_db()
-
     # Source Code Analysis
     if _analyze_source:
         run_source_code_analysis_multiprocessing(_analyze_source_all, output_path, os.path.join(output_path, output_src_analysis_file))
 
     # Write the result to excel file
     write_result_from_bom(output_file, installed_packages_src, installed_packages_bin,
                           _print_bin_android, output_extension,
```

### Comparing `fosslight_yocto-3.1.28/src/fosslight_yocto/parsing_meta_doubleopen.py` & `fosslight_yocto-3.1.29/src/fosslight_yocto/parsing_meta_doubleopen.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.28/src/fosslight_yocto.egg-info/PKG-INFO` & `fosslight_yocto-3.1.29/src/fosslight_yocto.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight-yocto
-Version: 3.1.28
+Version: 3.1.29
 Summary: FOSSLight Yocto
 Home-page: https://github.com/fosslight/fosslight_yocto_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_yocto_scanner
 Description: <!--
         SPDX-FileCopyrightText: Copyright 2023 LG Electronics Inc.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fosslight-yocto Version: 3.1.28 Summary: FOSSLight
+Metadata-Version: 2.1 Name: fosslight-yocto Version: 3.1.29 Summary: FOSSLight
 Yocto Home-page: https://github.com/fosslight/fosslight_yocto_scanner Author:
 LG Electronics License: Apache-2.0 Download-URL: https://github.com/fosslight/
 fosslight_yocto_scanner Description:
                                                                        _[_K_o_r_e_a_n_]
 # FOSSLight Yocto Scanner [FOSSLight Yocto Scanner is released under the
 Apache-2.0 License.][Current python package version.][https://img.shields.io/
 pypi/pyversions/fosslight_yocto][![REUSE status](https://api.reuse.software/
```

### Comparing `fosslight_yocto-3.1.28/src/fosslight_yocto.egg-info/SOURCES.txt` & `fosslight_yocto-3.1.29/src/fosslight_yocto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

