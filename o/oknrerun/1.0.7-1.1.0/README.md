# Comparing `tmp/oknrerun-1.0.7.tar.gz` & `tmp/oknrerun-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oknrerun-1.0.7.tar", last modified: Mon Apr 15 00:54:10 2024, max compression
+gzip compressed data, was "oknrerun-1.1.0.tar", last modified: Tue May 14 08:09:13 2024, max compression
```

## Comparing `oknrerun-1.0.7.tar` & `oknrerun-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 00:54:10.979021 oknrerun-1.0.7/
--rw-rw-rw-   0        0        0    11558 2024-04-14 22:17:50.000000 oknrerun-1.0.7/LICENSE
--rw-rw-rw-   0        0        0       22 2024-04-14 22:17:50.000000 oknrerun-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     4623 2024-04-15 00:54:10.976490 oknrerun-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3823 2024-04-14 22:17:50.000000 oknrerun-1.0.7/README.md
--rw-rw-rw-   0        0        0     1118 2024-04-15 00:50:57.000000 oknrerun-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 00:54:10.979021 oknrerun-1.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-15 00:54:10.926352 oknrerun-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-15 00:54:10.949354 oknrerun-1.0.7/src/oknrerun/
--rw-rw-rw-   0        0        0        0 2024-04-14 22:17:50.000000 oknrerun-1.0.7/src/oknrerun/__init__.py
--rw-rw-rw-   0        0        0     6263 2024-04-14 22:17:50.000000 oknrerun-1.0.7/src/oknrerun/gazefilters.json
--rw-rw-rw-   0        0        0      341 2024-04-14 22:17:50.000000 oknrerun-1.0.7/src/oknrerun/okn_detection_rule.json
--rw-rw-rw-   0        0        0    13419 2024-04-14 22:17:50.000000 oknrerun-1.0.7/src/oknrerun/okndetector.gaze.config
--rw-rw-rw-   0        0        0    44772 2024-04-15 00:49:51.000000 oknrerun-1.0.7/src/oknrerun/oknrerun.py
--rw-rw-rw-   0        0        0     5913 2024-04-14 22:17:50.000000 oknrerun-1.0.7/src/oknrerun/oknserver_graph_plot_config.json
--rw-rw-rw-   0        0        0      260 2024-04-14 22:17:50.000000 oknrerun-1.0.7/src/oknrerun/opm_detector_config.json
--rw-rw-rw-   0        0        0       33 2024-04-14 22:17:50.000000 oknrerun-1.0.7/src/oknrerun/ui.py
-drwxrwxrwx   0        0        0        0 2024-04-15 00:54:10.975493 oknrerun-1.0.7/src/oknrerun.egg-info/
--rw-rw-rw-   0        0        0     4623 2024-04-15 00:54:10.000000 oknrerun-1.0.7/src/oknrerun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      519 2024-04-15 00:54:10.000000 oknrerun-1.0.7/src/oknrerun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 00:54:10.000000 oknrerun-1.0.7/src/oknrerun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-15 00:54:10.000000 oknrerun-1.0.7/src/oknrerun.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      112 2024-04-15 00:54:10.000000 oknrerun-1.0.7/src/oknrerun.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-15 00:54:10.000000 oknrerun-1.0.7/src/oknrerun.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 08:09:13.293929 oknrerun-1.1.0/
+-rw-rw-rw-   0        0        0    11558 2024-04-14 22:17:50.000000 oknrerun-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       22 2024-04-14 22:17:50.000000 oknrerun-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4623 2024-05-14 08:09:13.292931 oknrerun-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3823 2024-04-14 22:17:50.000000 oknrerun-1.1.0/README.md
+-rw-rw-rw-   0        0        0     1118 2024-05-14 07:13:54.000000 oknrerun-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-14 08:09:13.293929 oknrerun-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-14 08:09:13.262010 oknrerun-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 08:09:13.274976 oknrerun-1.1.0/src/oknrerun/
+-rw-rw-rw-   0        0        0        0 2024-04-14 22:17:50.000000 oknrerun-1.1.0/src/oknrerun/__init__.py
+-rw-rw-rw-   0        0        0     6263 2024-04-14 22:17:50.000000 oknrerun-1.1.0/src/oknrerun/gazefilters.json
+-rw-rw-rw-   0        0        0      341 2024-04-14 22:17:50.000000 oknrerun-1.1.0/src/oknrerun/okn_detection_rule.json
+-rw-rw-rw-   0        0        0    13419 2024-04-14 22:17:50.000000 oknrerun-1.1.0/src/oknrerun/okndetector.gaze.config
+-rw-rw-rw-   0        0        0    51287 2024-05-14 08:03:38.000000 oknrerun-1.1.0/src/oknrerun/oknrerun.py
+-rw-rw-rw-   0        0        0     5913 2024-04-14 22:17:50.000000 oknrerun-1.1.0/src/oknrerun/oknserver_graph_plot_config.json
+-rw-rw-rw-   0        0        0      260 2024-04-14 22:17:50.000000 oknrerun-1.1.0/src/oknrerun/opm_detector_config.json
+-rw-rw-rw-   0        0        0       33 2024-04-14 22:17:50.000000 oknrerun-1.1.0/src/oknrerun/ui.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:09:13.291934 oknrerun-1.1.0/src/oknrerun.egg-info/
+-rw-rw-rw-   0        0        0     4623 2024-05-14 08:09:13.000000 oknrerun-1.1.0/src/oknrerun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2024-05-14 08:09:13.000000 oknrerun-1.1.0/src/oknrerun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 08:09:13.000000 oknrerun-1.1.0/src/oknrerun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-14 08:09:13.000000 oknrerun-1.1.0/src/oknrerun.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      112 2024-05-14 08:09:13.000000 oknrerun-1.1.0/src/oknrerun.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-14 08:09:13.000000 oknrerun-1.1.0/src/oknrerun.egg-info/top_level.txt
```

### Comparing `oknrerun-1.0.7/LICENSE` & `oknrerun-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oknrerun-1.0.7/PKG-INFO` & `oknrerun-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oknrerun
-Version: 1.0.7
+Version: 1.1.0
 Summary: Python program to rerun eye health diagnostic group's recording data
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/oknrerun
 Project-URL: Bug Tracker, https://github.com/jtur044/oknrerun/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `oknrerun-1.0.7/README.md` & `oknrerun-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `oknrerun-1.0.7/pyproject.toml` & `oknrerun-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "oknrerun"
-version = "1.0.7"
+version = "1.1.0"
 authors = [
   { name="Zaw Lin Tun", email="zawlintun1511@gmail.com" },
 ]
 description = "Python program to rerun eye health diagnostic group's recording data"
 readme = "README.md"
 dependencies = ["setuptools>=61.0", "numpy", "commentjson", "scipy", "matplotlib", "ehdg_tools>=4.0.8", "ehdg_pupil_detector", "okntool", "opencv-python"]
 classifiers = [
```

### Comparing `oknrerun-1.0.7/src/oknrerun/gazefilters.json` & `oknrerun-1.1.0/src/oknrerun/gazefilters.json`

 * *Files identical despite different names*

### Comparing `oknrerun-1.0.7/src/oknrerun/okndetector.gaze.config` & `oknrerun-1.1.0/src/oknrerun/okndetector.gaze.config`

 * *Files identical despite different names*

### Comparing `oknrerun-1.0.7/src/oknrerun/oknrerun.py` & `oknrerun-1.1.0/src/oknrerun/oknrerun.py`

 * *Files 9% similar despite different names*

```diff
@@ -211,15 +211,14 @@
                 trial_plot_info = plot_info["trial_plot"]
                 print(trial_plot_info)
 
                 # Retrieve summary plot info from config
                 summary_plot_info = plot_info["summary_plot"]
                 print(summary_plot_info)
 
-                signal_csv_folder_name = trial_plot_info["signal_csv_folder_name"]
                 signal_csv_name = trial_plot_info["signal_csv_name"]
             except KeyError:
                 print(f"Error in retrieving plot info from config file:{pil}!")
                 return False, str(KeyError)
     except Exception as error:
         print(f"Error in retrieving plot info from config file:{pil}!")
         return False, error
@@ -510,23 +509,26 @@
                         metavar="extra string to be used to named update csv")
     parser.add_argument("-di", dest="direction_input", required=False, default=None,
                         metavar="direction input to rerun")
     parser.add_argument("-ri", dest="rule_info", required=False, default=None,
                         metavar="rule info")
     parser.add_argument("-pi", dest="plot_info", required=False, default=None,
                         metavar="plot info")
+    parser.add_argument("--overwrite", dest="force_overwrite", required=False,
+                        help="force overwrite", action="store_true")
 
     args = parser.parse_args()
     # checking whether just display config or rerun
     display = args.display
     default_extra_string = "updated_"
     default_buffer_length = 7
     default_pupil_detector_type = "opm"
     if display is None:
         directory_input = args.directory_input
+        force_overwrite = args.force_overwrite
         if directory_input is None:
             print("There is no directory input.")
             print("Please use flag -d to input recording folder directory.")
             return
         else:
             if not os.path.isdir(str(directory_input)):
                 print(f"Invalid directory input: {str(directory_input)}")
@@ -536,23 +538,14 @@
                 config_folder_dir = os.path.join(directory_input, "config")
                 if os.path.isdir(config_folder_dir):
                     print("Config folder is found.")
                 else:
                     print("Config folder could not be found.")
                     return
 
-                    # Get new folder name which will not overwrite existing folders
-        rerun_folder_dir = get_rerun_folder_dir(str(directory_input))
-
-        # Ignore folders so that it will not copy unnecessary files
-        ignore_folder_array = ["config", "trials"]
-
-        # Copy all files but ignore config and trials folders
-        rerun_folder_dir = copy_folder_with_ignore_folder(str(directory_input), rerun_folder_dir, ignore_folder_array)
-
         # Check whether summary csv is there or not.
         # If not, ask user to give the file link and continue.
         # If user gives invalid link, then stop the process.
         summary_csv_dir = os.path.join(str(directory_input), "trials", "okn_detector_summary.csv")
         if not os.path.isfile(summary_csv_dir):
             print(f"Expected summary csv: {summary_csv_dir} could not be found.")
             new_summary_csv_dir = input("Please link for summary csv here: ")
@@ -601,14 +594,15 @@
                 else:
                     print(f"Stopping the process.")
                     return
         else:
             pupil_detector = False
             print(f"Rerunning without pupil detector.")
             print("Add -pd flag in the command line to use pupil detector.")
+
         buffer_length = args.buffer_length
         if buffer_length is not None:
             try:
                 buffer_length = int(buffer_length)
                 if pupil_detector:
                     print("There is buffer length input.")
                     print(f"Pupil detector will be using Tiny Fill Buffer with length:{buffer_length}.")
@@ -619,16 +613,14 @@
                     print(f"Pupil detector will be using Tiny Fill Buffer with default length:{buffer_length}.")
         else:
             buffer_length = default_buffer_length
             if pupil_detector:
                 print("There is no buffer length input.")
                 print(f"Pupil detector will be using Tiny Fill Buffer with default length:{buffer_length}.")
 
-        extra_string = args.extra_string
-        updater_config = args.updater_config
         direction_input = args.direction_input
         if direction_input:
             try:
                 direction_input = int(direction_input)
                 if direction_input == -1 or direction_input == 1:
                     direction_input = None
             except ValueError:
@@ -645,22 +637,22 @@
                 print("")
         else:
             print("")
             print("There is no direction input.")
             print("Therefore, direction will be set according to the summary csv.")
             print("")
 
-        okn_detector_config = args.okn_detector_config
-        opm_detector_config = args.opm_detector_config
-
+        extra_string = args.extra_string
         if extra_string:
             extra_string = str(extra_string)
         else:
             extra_string = default_extra_string
 
+        updater_config = args.updater_config
+        updater_config_exist = False
         if updater_config:
             valid_file_name = valid_config_name(str(updater_config))
             if valid_file_name:
                 config_dir_exist = os.path.isfile(updater_config)
                 if config_dir_exist:
                     print("Input updater config config location is found.")
                     updater_config_location = updater_config
@@ -673,19 +665,22 @@
                 print("It must be .json file or .config file.")
                 return
         else:
             updater_config_name = get_config_name(config_folder_dir, "gazefilter")
             updater_config_location = os.path.join(config_folder_dir, updater_config_name)
             if os.path.isfile(updater_config_location):
                 print(f"Using updater config from {updater_config_location}.")
+                updater_config_exist = True
             else:
                 print("There is no updater config input and cannot be found in config folder.")
                 updater_config_location = get_config_location("oknrerun", "gazefilters.json")
                 print(f"Therefore using built-in updater config from package.")
 
+        okn_detector_config = args.okn_detector_config
+        okn_detector_config_exist = False
         if okn_detector_config:
             valid_file_name = valid_config_name(str(okn_detector_config))
             if valid_file_name:
                 okn_detector_config_dir_exist = os.path.isfile(okn_detector_config)
                 if okn_detector_config_dir_exist:
                     print("Input okn detector config location is found.")
                     okn_detector_config_location = okn_detector_config
@@ -698,41 +693,68 @@
                 print("It must be .json file or .config file.")
                 return
         else:
             detector_config_name = get_config_name(config_folder_dir, "okndetector")
             okn_detector_config_location = os.path.join(config_folder_dir, detector_config_name)
             if os.path.isfile(okn_detector_config_location):
                 print(f"Using detector config from {okn_detector_config_location}.")
+                okn_detector_config_exist = True
             else:
                 print("There is no detector config input and cannot be found in config folder.")
                 okn_detector_config_location = get_config_location("oknrerun", "okndetector.gaze.config")
                 print(f"Therefore using built-in okn detector config from package.")
 
-        if opm_detector_config:
-            valid_file_name = valid_config_name(str(opm_detector_config))
-            if valid_file_name:
-                okn_detector_config_dir_exist = os.path.isfile(opm_detector_config)
-                if okn_detector_config_dir_exist:
-                    print("Input opm detector config location is found.")
-                    opm_detector_config_location = opm_detector_config
+        if pupil_detector and pupil_detector_type == "opm":
+            opm_detector_config = args.opm_detector_config
+            if opm_detector_config:
+                valid_file_name = valid_config_name(str(opm_detector_config))
+                if valid_file_name:
+                    opm_detector_config_dir_exist = os.path.isfile(opm_detector_config)
+                    if opm_detector_config_dir_exist:
+                        print("Input opm detector config location is found.")
+                        opm_detector_config_location = opm_detector_config
+                        need_to_copy_opm_config = True
+                    else:
+                        print("Input opm detector config does not exist.")
+                        opm_detector_config_location = get_config_location("oknrerun", "opm_detector_config.json")
+                        print(f"Therefore using default opm detector config from package.")
+                        need_to_copy_opm_config = True
+                else:
+                    print(f"Input opm detector config:{opm_detector_config} is not a config file.")
+                    print("It must be .json file or .config file.")
+                    return
+            else:
+                opm_detector_config_name = get_config_name(config_folder_dir, "opm_detector")
+                opm_detector_config_location = os.path.join(config_folder_dir, opm_detector_config_name)
+                if os.path.isfile(opm_detector_config_location):
+                    print(f"Using opm detector config from {okn_detector_config_location}.")
+                    if force_overwrite:
+                        need_to_copy_opm_config = False
+                    else:
+                        need_to_copy_opm_config = True
                 else:
-                    print("Input opm detector config does not exist.")
                     opm_detector_config_location = get_config_location("oknrerun", "opm_detector_config.json")
+                    need_to_copy_opm_config = True
+                    print("There is no opm detector config location input.")
                     print(f"Therefore using default opm detector config from package.")
-            else:
-                print(f"Input opm detector config:{opm_detector_config} is not a config file.")
-                print("It must be .json file or .config file.")
-                return
         else:
-            opm_detector_config_location = get_config_location("oknrerun", "opm_detector_config.json")
-            if pupil_detector:
-                print("There is no opm detector config location input.")
-                print(f"Therefore using default opm detector config from package.")
+            opm_detector_config_name = get_config_name(config_folder_dir, "opm_detector")
+            opm_detector_config_location = os.path.join(config_folder_dir, opm_detector_config_name)
+            if os.path.isfile(opm_detector_config_location):
+                print(f"Using opm detector config from {okn_detector_config_location}.")
+                if force_overwrite:
+                    need_to_copy_opm_config = False
+                else:
+                    need_to_copy_opm_config = True
+            else:
+                need_to_copy_opm_config = False
+                opm_detector_config_location = None
 
         plot_info = args.plot_info
+        plot_info_exist = False
         if plot_info:
             valid_file_name = valid_config_name(str(plot_info))
             if valid_file_name:
                 plot_info_exist = os.path.isfile(plot_info)
                 if plot_info_exist:
                     print("Input plot info location is found.")
                     plot_info_location = plot_info
@@ -745,20 +767,22 @@
                 print("It must be .json file or .config file.")
                 return
         else:
             plot_config_name = get_config_name(config_folder_dir, "plot")
             plot_info_location = os.path.join(config_folder_dir, plot_config_name)
             if os.path.isfile(plot_info_location):
                 print(f"Using plot config from {plot_info_location}.")
+                plot_info_exist = True
             else:
                 print("There is no plot config input and cannot be found in config folder.")
                 plot_info_location = get_config_location("oknrerun", "oknserver_graph_plot_config.json")
                 print(f"Therefore using default plot info from package.")
 
         rule_info = args.rule_info
+        rule_info_exist = False
         if rule_info:
             valid_file_name = valid_config_name(str(rule_info))
             if valid_file_name:
                 rule_info_exist = os.path.isfile(rule_info)
                 if rule_info_exist:
                     print("Input rule info location is found.")
                     rule_info_location = rule_info
@@ -771,114 +795,192 @@
                 print("It must be .json file or .config file.")
                 return
         else:
             rule_info_name = get_config_name(config_folder_dir, "oknserver_config", "rule")
             rule_info_location = os.path.join(config_folder_dir, rule_info_name)
             if os.path.isfile(rule_info_location):
                 print(f"Using rule info from {rule_info_location}.")
+                rule_info_exist = True
             else:
                 print("There is no rule info input and cannot be found in config folder.")
                 rule_info_location = get_config_location("oknrerun", "okn_detection_rule.json")
                 print(f"Therefore using default rule info from package.")
 
-        # copy config files which will be used in the process into config folder
-        config_folder_dir = os.path.join(rerun_folder_dir, "config")
-        shutil.copy(updater_config_location, os.path.join(config_folder_dir,
-                                                          os.path.basename(updater_config_location)))
-        shutil.copy(okn_detector_config_location, os.path.join(config_folder_dir,
-                                                               os.path.basename(okn_detector_config_location)))
-        shutil.copy(plot_info_location, os.path.join(config_folder_dir, os.path.basename(plot_info_location)))
-        shutil.copy(rule_info_location, os.path.join(config_folder_dir, os.path.basename(rule_info_location)))
-        if pupil_detector:
-            shutil.copy(opm_detector_config_location, os.path.join(config_folder_dir,
-                                                                   os.path.basename(opm_detector_config_location)))
-
-        # copy file from directory input
-        copy_trials_dir = os.path.join(str(directory_input), "trials")
-        paste_trials_dir = os.path.join(rerun_folder_dir, "trials")
-        for data_info in data_info_array:
-            trial_id = data_info["trial_id"]
-            disk_condition = data_info["disk_condition"]
-            trial_name = f"{trial_id}_{disk_condition}"
-            paste_trial_folder_dir = os.path.join(paste_trials_dir, trial_name)
-            if not os.path.isdir(paste_trial_folder_dir):
-                os.mkdir(paste_trial_folder_dir)
-
-        if pupil_detector:
-            # If using pupil detector, check whether there is trial video or not
-            # If not, create trial videos in rerun trials folder
-            # If yes, just copy videos into rerun trials folder
+        if force_overwrite:
+            # Get new folder name which will not overwrite existing folders
+            rerun_folder_dir = str(directory_input)
+
+            # copy config files which will be used in the process into config folder
+            config_folder_dir = os.path.join(rerun_folder_dir, "config")
+            if not updater_config_exist:
+                shutil.copy(updater_config_location, os.path.join(config_folder_dir,
+                                                                  os.path.basename(updater_config_location)))
+            if not okn_detector_config_exist:
+                shutil.copy(okn_detector_config_location, os.path.join(config_folder_dir,
+                                                                       os.path.basename(okn_detector_config_location)))
+            if not plot_info_exist:
+                shutil.copy(plot_info_location, os.path.join(config_folder_dir, os.path.basename(plot_info_location)))
+            if not rule_info_exist:
+                shutil.copy(rule_info_location, os.path.join(config_folder_dir, os.path.basename(rule_info_location)))
+
+            if need_to_copy_opm_config:
+                shutil.copy(opm_detector_config_location, os.path.join(config_folder_dir,
+                                                                       os.path.basename(opm_detector_config_location)))
 
-            all_videos_found = True
-            for data_info in data_info_array:
-                trial_id = data_info["trial_id"]
-                disk_condition = data_info["disk_condition"]
-                trial_name = f"{trial_id}_{disk_condition}"
-                trial_video_name = f"{trial_name}_cropped.mp4"
-                trial_video_dir = os.path.join(copy_trials_dir, trial_name, trial_video_name)
-                if not os.path.isfile(trial_video_dir):
-                    all_videos_found = False
-                    break
-
-            if all_videos_found:
-                print("Split videos are found in input trial folders")
-                print("Therefore, copying those videos into rerun trials folder")
+            trials_dir = os.path.join(str(directory_input), "trials")
+            if pupil_detector:
+                # If using pupil detector, check whether there is trial video or not
+                # If not, create trial videos in rerun trials folder
+                # If yes, just copy videos into rerun trials folder
+
+                all_videos_found = True
                 for data_info in data_info_array:
                     trial_id = data_info["trial_id"]
                     disk_condition = data_info["disk_condition"]
                     trial_name = f"{trial_id}_{disk_condition}"
                     trial_video_name = f"{trial_name}_cropped.mp4"
-                    trial_video_dir = os.path.join(copy_trials_dir, trial_name, trial_video_name)
-                    paste_trial_folder_dir = os.path.join(paste_trials_dir, trial_name)
-                    if not os.path.isdir(paste_trial_folder_dir):
-                        os.mkdir(paste_trial_folder_dir)
-                    paste_video_dir = os.path.join(paste_trial_folder_dir, trial_video_name)
-                    shutil.copy(trial_video_dir, paste_video_dir)
-            else:
-                print("Split videos are not found in input trial folders")
-                print("Starting splitting the video.")
-                print("Checking whether there is okntool in this computer or not.")
-                is_there_okntool = check_commandline_program("okntool")
-                if is_there_okntool:
-                    split_video_cmd = f"okntool -t sv -d {str(rerun_folder_dir)}"
-                    os.system(split_video_cmd)
+                    trial_video_dir = os.path.join(trials_dir, trial_name, trial_video_name)
+                    if not os.path.isfile(trial_video_dir):
+                        all_videos_found = False
+                        break
+
+                if all_videos_found:
+                    print("All split videos are found in input trial folders")
                 else:
-                    print("Please install or upgrade okntool first then rerun this process.")
-                    print("pip install okntool -U")
-                    return
-        else:
-            # If running without pupil detector then copy individual trial csv to rerun trial folders
+                    print("Split videos are not found in input trial folders")
+                    print("Starting splitting the video.")
+                    print("Checking whether there is okntool in this computer or not.")
+                    is_there_okntool = check_commandline_program("okntool")
+                    if is_there_okntool:
+                        split_video_cmd = f"okntool -t sv -d {str(rerun_folder_dir)}"
+                        os.system(split_video_cmd)
+                    else:
+                        print("Please install or upgrade okntool first then rerun this process.")
+                        print("pip install okntool -U")
+                        return
+
+            success, error, rerun_folder_dir = rerun_recording(rerun_folder_dir, data_info_array,
+                                                               opm_detector_config_location,
+                                                               extra_string, updater_config_location,
+                                                               direction_input, okn_detector_config_location,
+                                                               plot_info_location, rule_info_location,
+                                                               summary_csv_dir, pupil_detector,
+                                                               pupil_detector_type, buffer_length)
+            if success:
+                print(f"Rerun recording is successful and all the rerun data will be in {rerun_folder_dir}.")
+            else:
+                print(f"Rerun recording is unsuccessful.")
+                if error:
+                    print(error)
+        else:
+            # Get new folder name which will not overwrite existing folders
+            rerun_folder_dir = get_rerun_folder_dir(str(directory_input))
+
+            # Ignore folders so that it will not copy unnecessary files
+            ignore_folder_array = ["config", "trials"]
+
+            # Copy all files but ignore config and trials folders
+            rerun_folder_dir = copy_folder_with_ignore_folder(str(directory_input), rerun_folder_dir,
+                                                              ignore_folder_array)
+
+            # copy config files which will be used in the process into config folder
+            config_folder_dir = os.path.join(rerun_folder_dir, "config")
+            shutil.copy(updater_config_location, os.path.join(config_folder_dir,
+                                                              os.path.basename(updater_config_location)))
+            shutil.copy(okn_detector_config_location, os.path.join(config_folder_dir,
+                                                                   os.path.basename(okn_detector_config_location)))
+            shutil.copy(plot_info_location, os.path.join(config_folder_dir, os.path.basename(plot_info_location)))
+            shutil.copy(rule_info_location, os.path.join(config_folder_dir, os.path.basename(rule_info_location)))
+            if need_to_copy_opm_config:
+                shutil.copy(opm_detector_config_location, os.path.join(config_folder_dir,
+                                                                       os.path.basename(opm_detector_config_location)))
+
+            # copy file from directory input
+            copy_trials_dir = os.path.join(str(directory_input), "trials")
+            paste_trials_dir = os.path.join(rerun_folder_dir, "trials")
             for data_info in data_info_array:
                 trial_id = data_info["trial_id"]
                 disk_condition = data_info["disk_condition"]
                 trial_name = f"{trial_id}_{disk_condition}"
-                trial_csv_name = f"{trial_name}.csv"
-                trial_csv_dir = os.path.join(copy_trials_dir, trial_name, trial_csv_name)
-                if not os.path.isfile(trial_csv_dir):
-                    print(f"{trial_csv_dir} could not be found.")
-                    return
                 paste_trial_folder_dir = os.path.join(paste_trials_dir, trial_name)
                 if not os.path.isdir(paste_trial_folder_dir):
                     os.mkdir(paste_trial_folder_dir)
-                paste_csv_dir = os.path.join(paste_trial_folder_dir, trial_csv_name)
-                shutil.copy(trial_csv_dir, paste_csv_dir)
 
-        success, error, rerun_folder_dir = rerun_recording(rerun_folder_dir, data_info_array,
-                                                           opm_detector_config_location,
-                                                           extra_string, updater_config_location,
-                                                           direction_input, okn_detector_config_location,
-                                                           plot_info_location, rule_info_location,
-                                                           summary_csv_dir, pupil_detector,
-                                                           pupil_detector_type, buffer_length)
-        if success:
-            print(f"Rerun recording is successful and all the rerun data will be in {rerun_folder_dir}.")
-        else:
-            print(f"Rerun recording is unsuccessful.")
-            if error:
-                print(error)
+            if pupil_detector:
+                # If using pupil detector, check whether there is trial video or not
+                # If not, create trial videos in rerun trials folder
+                # If yes, just copy videos into rerun trials folder
+
+                all_videos_found = True
+                for data_info in data_info_array:
+                    trial_id = data_info["trial_id"]
+                    disk_condition = data_info["disk_condition"]
+                    trial_name = f"{trial_id}_{disk_condition}"
+                    trial_video_name = f"{trial_name}_cropped.mp4"
+                    trial_video_dir = os.path.join(copy_trials_dir, trial_name, trial_video_name)
+                    if not os.path.isfile(trial_video_dir):
+                        all_videos_found = False
+                        break
+
+                if all_videos_found:
+                    print("Split videos are found in input trial folders")
+                    print("Therefore, copying those videos into rerun trials folder")
+                    for data_info in data_info_array:
+                        trial_id = data_info["trial_id"]
+                        disk_condition = data_info["disk_condition"]
+                        trial_name = f"{trial_id}_{disk_condition}"
+                        trial_video_name = f"{trial_name}_cropped.mp4"
+                        trial_video_dir = os.path.join(copy_trials_dir, trial_name, trial_video_name)
+                        paste_trial_folder_dir = os.path.join(paste_trials_dir, trial_name)
+                        if not os.path.isdir(paste_trial_folder_dir):
+                            os.mkdir(paste_trial_folder_dir)
+                        paste_video_dir = os.path.join(paste_trial_folder_dir, trial_video_name)
+                        shutil.copy(trial_video_dir, paste_video_dir)
+                else:
+                    print("Split videos are not found in input trial folders")
+                    print("Starting splitting the video.")
+                    print("Checking whether there is okntool in this computer or not.")
+                    is_there_okntool = check_commandline_program("okntool")
+                    if is_there_okntool:
+                        split_video_cmd = f"okntool -t sv -d {str(rerun_folder_dir)}"
+                        os.system(split_video_cmd)
+                    else:
+                        print("Please install or upgrade okntool first then rerun this process.")
+                        print("pip install okntool -U")
+                        return
+            else:
+                # If running without pupil detector then copy individual trial csv to rerun trial folders
+                for data_info in data_info_array:
+                    trial_id = data_info["trial_id"]
+                    disk_condition = data_info["disk_condition"]
+                    trial_name = f"{trial_id}_{disk_condition}"
+                    trial_csv_name = f"{trial_name}.csv"
+                    trial_csv_dir = os.path.join(copy_trials_dir, trial_name, trial_csv_name)
+                    if not os.path.isfile(trial_csv_dir):
+                        print(f"{trial_csv_dir} could not be found.")
+                        return
+                    paste_trial_folder_dir = os.path.join(paste_trials_dir, trial_name)
+                    if not os.path.isdir(paste_trial_folder_dir):
+                        os.mkdir(paste_trial_folder_dir)
+                    paste_csv_dir = os.path.join(paste_trial_folder_dir, trial_csv_name)
+                    shutil.copy(trial_csv_dir, paste_csv_dir)
+
+            success, error, rerun_folder_dir = rerun_recording(rerun_folder_dir, data_info_array,
+                                                               opm_detector_config_location,
+                                                               extra_string, updater_config_location,
+                                                               direction_input, okn_detector_config_location,
+                                                               plot_info_location, rule_info_location,
+                                                               summary_csv_dir, pupil_detector,
+                                                               pupil_detector_type, buffer_length)
+            if success:
+                print(f"Rerun recording is successful and all the rerun data will be in {rerun_folder_dir}.")
+            else:
+                print(f"Rerun recording is unsuccessful.")
+                if error:
+                    print(error)
     else:
         display_flag = str(display)
         if display_flag == "uc":
             print("Default Updater Config Info")
             updater_config_location = get_config_location("oknrerun", "gazefilters.json")
             show_uc(updater_config_location)
         elif display_flag == "okndc":
```

### Comparing `oknrerun-1.0.7/src/oknrerun/oknserver_graph_plot_config.json` & `oknrerun-1.1.0/src/oknrerun/oknserver_graph_plot_config.json`

 * *Files identical despite different names*

### Comparing `oknrerun-1.0.7/src/oknrerun.egg-info/PKG-INFO` & `oknrerun-1.1.0/src/oknrerun.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oknrerun
-Version: 1.0.7
+Version: 1.1.0
 Summary: Python program to rerun eye health diagnostic group's recording data
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/oknrerun
 Project-URL: Bug Tracker, https://github.com/jtur044/oknrerun/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `oknrerun-1.0.7/src/oknrerun.egg-info/SOURCES.txt` & `oknrerun-1.1.0/src/oknrerun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

