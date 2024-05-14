# Comparing `tmp/ab_plugin_scenariolink-0.0.6.tar.gz` & `tmp/ab_plugin_scenariolink-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ab_plugin_scenariolink-0.0.6.tar", last modified: Mon Oct 16 08:58:42 2023, max compression
+gzip compressed data, was "ab_plugin_scenariolink-0.0.7.tar", last modified: Tue May 14 15:14:36 2024, max compression
```

## Comparing `ab_plugin_scenariolink-0.0.6.tar` & `ab_plugin_scenariolink-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 08:58:42.480282 ab_plugin_scenariolink-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2023-10-16 08:58:33.000000 ab_plugin_scenariolink-0.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12867 2023-10-16 08:58:42.480282 ab_plugin_scenariolink-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2023-10-16 08:58:33.000000 ab_plugin_scenariolink-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 08:58:42.476282 ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2023-10-16 08:58:33.000000 ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 08:58:42.476282 ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink/layouts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 08:58:42.480282 ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink/layouts/tabs/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-10-16 08:58:33.000000 ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink/layouts/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12698 2023-10-16 08:58:33.000000 ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink/layouts/tabs/right.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2023-10-16 08:58:33.000000 ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 08:58:42.480282 ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink/tables/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-16 08:58:33.000000 ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2023-10-16 08:58:33.000000 ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink/tables/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2023-10-16 08:58:33.000000 ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink/tables/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)    10176 2023-10-16 08:58:33.000000 ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 08:58:42.480282 ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12867 2023-10-16 08:58:42.000000 ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      575 2023-10-16 08:58:42.000000 ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-16 08:58:42.000000 ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-10-16 08:58:42.000000 ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-16 08:58:42.000000 ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-16 08:58:42.480282 ab_plugin_scenariolink-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2023-10-16 08:58:33.000000 ab_plugin_scenariolink-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:36.944443 ab_plugin_scenariolink-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-14 15:14:30.000000 ab_plugin_scenariolink-0.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13007 2024-05-14 15:14:36.944443 ab_plugin_scenariolink-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-14 15:14:30.000000 ab_plugin_scenariolink-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:36.940443 ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-14 15:14:30.000000 ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:36.940443 ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink/layouts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:36.944443 ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink/layouts/tabs/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 15:14:30.000000 ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink/layouts/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13424 2024-05-14 15:14:30.000000 ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink/layouts/tabs/right.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-14 15:14:30.000000 ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:36.944443 ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:14:30.000000 ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-05-14 15:14:30.000000 ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink/tables/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-05-14 15:14:30.000000 ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink/tables/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10767 2024-05-14 15:14:30.000000 ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:36.944443 ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13007 2024-05-14 15:14:36.000000 ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-14 15:14:36.000000 ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:14:36.000000 ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 15:14:36.000000 ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 15:14:36.000000 ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:14:36.944443 ab_plugin_scenariolink-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-14 15:14:30.000000 ab_plugin_scenariolink-0.0.7/setup.py
```

### Comparing `ab_plugin_scenariolink-0.0.6/LICENSE.txt` & `ab_plugin_scenariolink-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ab_plugin_scenariolink-0.0.6/PKG-INFO` & `ab_plugin_scenariolink-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ab_plugin_scenariolink
-Version: 0.0.6
+Version: 0.0.7
 Summary: Activity Browser plugin to download scenario-based LCA databases 
 Home-page: https://github.com/polca/ScenarioLink
 Author: Romain Sacchi, Marc van der Meide
 Author-email: romain.sacchi@psi.ch, m.t.van.der.meide@cml.leidenuniv.nl
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -167,16 +167,16 @@
         
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
 License-File: LICENSE.txt
-Requires-Dist: activity-browser
-Requires-Dist: unfold>=1.1.5
+Requires-Dist: activity-browser>=2.9.7
+Requires-Dist: unfold>=1.2.0
 Requires-Dist: datapackage
 Requires-Dist: pandas
 Requires-Dist: tqdm
 
 # ScenarioLink: An Activity Browser Plugin for Scenario-Based LCA Databases
 
 ScenarioLink is a specialized plugin for the [Activity Browser](https://github.com/LCA-ActivityBrowser/activity-browser), an open-source software for Life Cycle Assessment (LCA). This plugin enables you to seamlessly fetch and reproduce scenario-based LCA databases, such as those generated by [premise](https://github.com/polca/premise), using [unfold](https://github.com/polca/unfold) datapackages.
@@ -192,27 +192,34 @@
 The Activity Browser builds upon the [Brightway2](https://brightway.dev) LCA framework. ScenarioLink aims to simplify the use of scenario-based LCA databases within the Activity Browser by:
 
 - Eliminating the need for separate tools required to generate these databases (e.g., premise).
 - Utilizing `unfold` datapackages that contain scaling factors essential for reproducing scenario-based LCA databases, assuming a consistent source database (e.g., ecoinvent 3.7.1).
 
 ![Flow Diagram](assets/flow_diagram.png)
 
+## Requirements
+
+- ``activty-browser >= 2.9.7``
+
 ## Installation
 
 1. Activate your existing Activity Browser conda environment.
-2. Install the ScenarioLink plugin using Pypi or conda:
+2. Install the ScenarioLink plugin using conda (preferred) or Pypi (may create conflicts with `activity-browser` dependencies):
 
     ```bash
-    pip install ab-plugin-scenariolink
+    conda install -c romainsacchi ab-plugin-scenariolink
     ```
+   
+    or
 
     ```bash
-    conda install -c romainsacchi ab-plugin-scenariolink
+    pip install ab-plugin-scenariolink
     ```
 
+
 4. Launch the Activity Browser.
 5. Navigate to `Tools > Plugins` and select ScenarioLink from the plugin list.
 
 ## Usage
 
 ### Reproduce a scenario-based database
```

### Comparing `ab_plugin_scenariolink-0.0.6/README.md` & `ab_plugin_scenariolink-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,27 +13,34 @@
 The Activity Browser builds upon the [Brightway2](https://brightway.dev) LCA framework. ScenarioLink aims to simplify the use of scenario-based LCA databases within the Activity Browser by:
 
 - Eliminating the need for separate tools required to generate these databases (e.g., premise).
 - Utilizing `unfold` datapackages that contain scaling factors essential for reproducing scenario-based LCA databases, assuming a consistent source database (e.g., ecoinvent 3.7.1).
 
 ![Flow Diagram](assets/flow_diagram.png)
 
+## Requirements
+
+- ``activty-browser >= 2.9.7``
+
 ## Installation
 
 1. Activate your existing Activity Browser conda environment.
-2. Install the ScenarioLink plugin using Pypi or conda:
+2. Install the ScenarioLink plugin using conda (preferred) or Pypi (may create conflicts with `activity-browser` dependencies):
 
     ```bash
-    pip install ab-plugin-scenariolink
+    conda install -c romainsacchi ab-plugin-scenariolink
     ```
+   
+    or
 
     ```bash
-    conda install -c romainsacchi ab-plugin-scenariolink
+    pip install ab-plugin-scenariolink
     ```
 
+
 4. Launch the Activity Browser.
 5. Navigate to `Tools > Plugins` and select ScenarioLink from the plugin list.
 
 ## Usage
 
 ### Reproduce a scenario-based database
```

### Comparing `ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink/layouts/tabs/right.py` & `ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink/layouts/tabs/right.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from activity_browser.layouts.tabs import PluginTab
 from activity_browser.ui.style import horizontal_line, header
 from activity_browser.ui.widgets.dialog import DatabaseLinkingDialog
 from activity_browser.signals import signals as ab_signals
 
 from ...tables.tables import FoldsTable, DataPackageTable
 from ...signals import signals
-from ...utils import unfold_databases, UpdateManager
+from ...utils import unfold_databases, clear_sl_datapackage_cache, UpdateManager
 
 class RightTab(PluginTab):
     def __init__(self, plugin, parent=None):
         super(RightTab, self).__init__(plugin=plugin, panel="right", parent=parent)
 
         self.layout = QtWidgets.QVBoxLayout()
 
@@ -92,18 +92,24 @@
         self.label = QtWidgets.QLabel('Select the datapackage you want to use')
         self.layout.addWidget(self.label)
 
         # Radio buttons to choose where to get Fold from
         self.radio_default = QtWidgets.QRadioButton('Online datapackages')
         self.radio_default.setChecked(True)
         self.radio_custom = QtWidgets.QRadioButton('Local datapackages')
+        self.clear_datapackage_cache = QtWidgets.QPushButton('Clear datapackage cache')
+        self.clear_datapackage_cache.setToolTip(
+            'ScenarioLink caches the downloaded datapackages, though sometimes\n'
+            'these may be updated and you need to clear the cache.'
+        )
         self.radio_layout = QtWidgets.QHBoxLayout()
         self.radio_layout.addWidget(self.radio_default)
         self.radio_layout.addWidget(self.radio_custom)
         self.radio_layout.addStretch()
+        self.radio_layout.addWidget(self.clear_datapackage_cache)
         self.radio_widget = QtWidgets.QWidget()
         self.radio_widget.setLayout(self.radio_layout)
         self.layout.addWidget(self.radio_widget)
 
         # Folds table
         self.table_label = QtWidgets.QLabel('Doubleclick to open a datapackage (if not present locally, it will be downloaded - this may take a while).')
         self.layout.addWidget(self.table_label)
@@ -126,20 +132,23 @@
         self.custom_widg = QtWidgets.QWidget()
         self.custom_widg.setLayout(self.custom_layout)
         self.layout.addWidget(self.custom_widg)
 
         self.layout.addWidget(horizontal_line())
         self.setLayout(self.layout)
 
+        # signals
         self.radio_custom.toggled.connect(self.radio_toggled)
         self.custom.clicked.connect(self.get_datapackage_custom_path)
+        self.clear_datapackage_cache.clicked.connect(self.do_clear_cache)
 
     def radio_toggled(self, toggled: bool) -> None:
         self.use_table = not toggled
         self.folds_table.setVisible(not toggled)
+        self.clear_datapackage_cache.setVisible(not toggled)
         self.table_label.setVisible(not toggled)
 
         self.custom.setVisible(toggled)
         signals.record_ready.emit(False)
 
     def get_datapackage_custom_path(self) -> None:
         """"Start a dialog to retrieve a datapackage from disk."""
@@ -147,14 +156,19 @@
             caption="Select datapackage zip file",
             filter='*.zip'
         )
         print('file selected from path:', path)
         self.custom_package_path = path
         signals.get_datapackage_from_disk.emit(path)
 
+    def do_clear_cache(self) -> None:
+        print('Clearing the datapackage cache')
+        clear_sl_datapackage_cache()
+        self.folds_table.model.sync()
+
 
 class ScenarioChooserWidget(QtWidgets.QWidget):
     def __init__(self):
         super(ScenarioChooserWidget, self).__init__()
 
         self.layout = QtWidgets.QVBoxLayout()
         self.sdf_path = None
@@ -191,33 +205,33 @@
 
         # Import button
         self.import_b = QtWidgets.QPushButton('Import')
         self.import_b.setEnabled(False)
         self.import_layout = QtWidgets.QHBoxLayout()
         self.import_layout.addWidget(self.import_b)
         self.import_layout.addStretch()
-        self.clear_cache = QtWidgets.QPushButton('Clear unfold cache')
-        self.clear_cache.setToolTip('Unfold caches some data to work faster, though sometimes this can store old data\n'
+        self.clear_unfold_cache = QtWidgets.QPushButton('Clear unfold cache')
+        self.clear_unfold_cache.setToolTip('Unfold caches some data to work faster, though sometimes this can store old data\n'
                                     'that should be renewed, clearing the cache allows new data to be cached.')
-        self.import_layout.addWidget(self.clear_cache)
+        self.import_layout.addWidget(self.clear_unfold_cache)
         self.import_b_widg = QtWidgets.QWidget()
         self.import_b_widg.setLayout(self.import_layout)
         self.layout.addWidget(self.import_b_widg)
         self.import_b.clicked.connect(self.import_state)
-        self.clear_cache.clicked.connect(self.clear_unfold_cache)
+        self.clear_unfold_cache.clicked.connect(self.do_clear_cache)
 
         self.layout.addWidget(horizontal_line())
         self.setLayout(self.layout)
 
         # signals
         signals.no_or_1_scenario_selected.connect(self.manage_sdf_state)
         signals.no_scenario_selected.connect(self.manage_import_button_state)
         self.sdf_file_loc.clicked.connect(self.choose_sdf_location)
 
-    def clear_unfold_cache(self):
+    def do_clear_cache(self):
         print('Clearing the unfold cache')
         clear_cache()
 
     def import_state(self):
 
         # convert the binary list to a list of indices that were selected
         include_scenarios = [i for i, state in enumerate(self.data_package_table.model.include) if state]
```

### Comparing `ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink/signals.py` & `ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink/signals.py`

 * *Files identical despite different names*

### Comparing `ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink/tables/models.py` & `ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink/tables/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 This module contains the models for the tables used in the ScenarioLink plugin.
 """
-from PySide2 import QtWidgets
 
 from urllib.error import HTTPError, URLError
 import pandas as pd
 
 from activity_browser.ui.tables.models import PandasModel
 from ..utils import download_files_from_zenodo, package_from_path, record_cached
 from ..signals import signals
@@ -21,14 +20,17 @@
 
     def __init__(self, parent=None):
         """Initialize the FoldsModel."""
         super().__init__(parent=parent)
         self.selected_record = None
         self.df_columns = {}  # a dict with all column names as keys and indices as values
 
+        # once a datapackage is extracted, update this table too so the 'cached' column is updated if needed
+        signals.record_ready.connect(self.record_ready)
+
     def sync(self):
         """
         Fetch and synchronize the scenarios list from a remote URL.
 
         The scenarios list is fetched from a CSV file hosted online.
         The fetched data is then stored in a Pandas DataFrame.
         """
@@ -59,14 +61,17 @@
         record = self._dataframe.iat[idx.row(), self.df_columns['Zenodo record ID']]
         self.selected_record = record
         return record
 
     def get_link(self, row: int) -> str:
         return self._dataframe.iloc[row, self.df_columns['link']]
 
+    def record_ready(self, ready: bool) -> None:
+        if ready:
+            self.sync()
 
 
 class DataPackageModel(PandasModel):
     """
     A model for the DataPackage table that inherits from PandasModel.
 
     This model manages the data related to the datapackages containing
```

### Comparing `ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink/tables/tables.py` & `ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink/tables/tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     @Slot(QtCore.QModelIndex, name="row_selected")
     def row_selected(self, index) -> None:
         """Handle row selection and emit a signal with the selected record."""
         record = self.model.get_record(index)
         signals.get_datapackage_from_record.emit(record)
 
     def open_link(self):
+        """Open the link in the selected row of the table."""
         index = self.selectedIndexes()[0]
         webbrowser.open(self.model.get_link(index.row()))
 
 
 class DataPackageTable(ABDataFrameView):
     """
     A table view class for displaying the DataPackage model data.
```

### Comparing `ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink/utils.py` & `ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -223,14 +223,29 @@
     folder_name = appdirs.user_cache_dir('ActivityBrowser', 'ActivityBrowser')
     if not os.path.exists(folder_name):
         os.makedirs(folder_name)
 
     zip_filename = record + '.zip'
     return os.path.exists(os.path.join(folder_name, zip_filename))
 
+def clear_sl_datapackage_cache() -> None:
+    """Clear all datapackages from the ScenarioLink cache"""
+    folder_name = appdirs.user_cache_dir('ActivityBrowser', 'ActivityBrowser')
+    if not os.path.exists(folder_name):
+        # the cache folder does not exist, so nothing to clear
+        return
+
+    # Get a list of all the files in the folder
+    for filename in os.listdir(folder_name):
+        file_path = os.path.join(folder_name, filename)
+
+        # Remove each file in the list
+        if os.path.isfile(file_path) or os.path.islink(file_path):
+            os.unlink(file_path)
+
 class UpdateManager():
 
     @classmethod
     def get_versions(cls) -> Tuple[str, str, bool]:
         """Get the version of this plugin and the most recent version.
 
         Return (current, latest, newer)
```

### Comparing `ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink.egg-info/PKG-INFO` & `ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ab-plugin-scenariolink
-Version: 0.0.6
+Name: ab_plugin_scenariolink
+Version: 0.0.7
 Summary: Activity Browser plugin to download scenario-based LCA databases 
 Home-page: https://github.com/polca/ScenarioLink
 Author: Romain Sacchi, Marc van der Meide
 Author-email: romain.sacchi@psi.ch, m.t.van.der.meide@cml.leidenuniv.nl
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -167,16 +167,16 @@
         
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
 License-File: LICENSE.txt
-Requires-Dist: activity-browser
-Requires-Dist: unfold>=1.1.5
+Requires-Dist: activity-browser>=2.9.7
+Requires-Dist: unfold>=1.2.0
 Requires-Dist: datapackage
 Requires-Dist: pandas
 Requires-Dist: tqdm
 
 # ScenarioLink: An Activity Browser Plugin for Scenario-Based LCA Databases
 
 ScenarioLink is a specialized plugin for the [Activity Browser](https://github.com/LCA-ActivityBrowser/activity-browser), an open-source software for Life Cycle Assessment (LCA). This plugin enables you to seamlessly fetch and reproduce scenario-based LCA databases, such as those generated by [premise](https://github.com/polca/premise), using [unfold](https://github.com/polca/unfold) datapackages.
@@ -192,27 +192,34 @@
 The Activity Browser builds upon the [Brightway2](https://brightway.dev) LCA framework. ScenarioLink aims to simplify the use of scenario-based LCA databases within the Activity Browser by:
 
 - Eliminating the need for separate tools required to generate these databases (e.g., premise).
 - Utilizing `unfold` datapackages that contain scaling factors essential for reproducing scenario-based LCA databases, assuming a consistent source database (e.g., ecoinvent 3.7.1).
 
 ![Flow Diagram](assets/flow_diagram.png)
 
+## Requirements
+
+- ``activty-browser >= 2.9.7``
+
 ## Installation
 
 1. Activate your existing Activity Browser conda environment.
-2. Install the ScenarioLink plugin using Pypi or conda:
+2. Install the ScenarioLink plugin using conda (preferred) or Pypi (may create conflicts with `activity-browser` dependencies):
 
     ```bash
-    pip install ab-plugin-scenariolink
+    conda install -c romainsacchi ab-plugin-scenariolink
     ```
+   
+    or
 
     ```bash
-    conda install -c romainsacchi ab-plugin-scenariolink
+    pip install ab-plugin-scenariolink
     ```
 
+
 4. Launch the Activity Browser.
 5. Navigate to `Tools > Plugins` and select ScenarioLink from the plugin list.
 
 ## Usage
 
 ### Reproduce a scenario-based database
```

### Comparing `ab_plugin_scenariolink-0.0.6/ab_plugin_scenariolink.egg-info/SOURCES.txt` & `ab_plugin_scenariolink-0.0.7/ab_plugin_scenariolink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ab_plugin_scenariolink-0.0.6/setup.py` & `ab_plugin_scenariolink-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,23 @@
         pkg = dirpath.replace(os.path.sep, '.')
         if os.path.altsep:
             pkg = pkg.replace(os.path.altsep, '.')
         packages.append(pkg)
 
 setup(
     name="ab_plugin_scenariolink",
-    version="0.0.6",
+    version="0.0.7",
     packages=packages,
     include_package_data=True,
     author="Romain Sacchi, Marc van der Meide",
     author_email="romain.sacchi@psi.ch, m.t.van.der.meide@cml.leidenuniv.nl",
     license=open('LICENSE.txt').read(),
     install_requires=[
-        "activity-browser",
-        "unfold >=1.1.5",
+        "activity-browser >=2.9.7",
+        "unfold >=1.2.0",
         "datapackage",
         "pandas",
         "tqdm"
     ],
     url="https://github.com/polca/ScenarioLink",
     long_description=open('README.md').read(),
     description="Activity Browser plugin to download scenario-based LCA databases ",
```

