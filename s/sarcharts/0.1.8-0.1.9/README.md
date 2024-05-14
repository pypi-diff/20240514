# Comparing `tmp/sarcharts-0.1.8.tar.gz` & `tmp/sarcharts-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarcharts-0.1.8.tar", last modified: Sat May 11 15:51:06 2024, max compression
+gzip compressed data, was "sarcharts-0.1.9.tar", last modified: Tue May 14 15:42:44 2024, max compression
```

## Comparing `sarcharts-0.1.8.tar` & `sarcharts-0.1.9.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.257505 sarcharts-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.249505 sarcharts-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.253505 sarcharts-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-11 15:51:00.000000 sarcharts-0.1.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-11 15:51:00.000000 sarcharts-0.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-11 15:51:06.000000 sarcharts-0.1.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-11 15:51:06.000000 sarcharts-0.1.8/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-11 15:51:00.000000 sarcharts-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-11 15:51:06.257505 sarcharts-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-11 15:51:00.000000 sarcharts-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.253505 sarcharts-0.1.8/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-11 15:51:00.000000 sarcharts-0.1.8/doc/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   137178 2024-05-11 15:51:00.000000 sarcharts-0.1.8/doc/sarcharts.png
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-11 15:51:00.000000 sarcharts-0.1.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.253505 sarcharts-0.1.8/sarcharts/
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.257505 sarcharts-0.1.8/sarcharts/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/bin/sarcharts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.249505 sarcharts-0.1.8/sarcharts/html/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.257505 sarcharts-0.1.8/sarcharts/html/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/html/css/sarcharts.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.257505 sarcharts-0.1.8/sarcharts/html/js/
--rw-r--r--   0 runner    (1001) docker     (127)   205214 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/html/js/chart.umd.js
--rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/html/js/chartjs-plugin-zoom.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/html/js/hammer.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   271751 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/html/js/jquery.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.257505 sarcharts-0.1.8/sarcharts/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/lib/chartjs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/lib/chartsconf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/lib/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/lib/sadf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/lib/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.257505 sarcharts-0.1.8/sarcharts/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/templates/chart.html
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/templates/header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.257505 sarcharts-0.1.8/sarcharts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-11 15:51:06.000000 sarcharts-0.1.8/sarcharts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-11 15:51:06.000000 sarcharts-0.1.8/sarcharts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 15:51:06.000000 sarcharts-0.1.8/sarcharts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-11 15:51:06.000000 sarcharts-0.1.8/sarcharts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 15:51:06.000000 sarcharts-0.1.8/sarcharts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-11 15:51:06.000000 sarcharts-0.1.8/sarcharts.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-11 15:51:06.000000 sarcharts-0.1.8/sarcharts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-11 15:51:06.000000 sarcharts-0.1.8/sarcharts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-11 15:51:06.261505 sarcharts-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-11 15:51:00.000000 sarcharts-0.1.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-11 15:51:00.000000 sarcharts-0.1.8/test-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-11 15:51:00.000000 sarcharts-0.1.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.468326 sarcharts-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.460326 sarcharts-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.464326 sarcharts-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-14 15:42:39.000000 sarcharts-0.1.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-14 15:42:39.000000 sarcharts-0.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 15:42:44.000000 sarcharts-0.1.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 15:42:44.000000 sarcharts-0.1.9/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-14 15:42:39.000000 sarcharts-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-14 15:42:44.468326 sarcharts-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-14 15:42:39.000000 sarcharts-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.464326 sarcharts-0.1.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-14 15:42:39.000000 sarcharts-0.1.9/doc/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   137178 2024-05-14 15:42:39.000000 sarcharts-0.1.9/doc/sarcharts.png
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-14 15:42:39.000000 sarcharts-0.1.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.464326 sarcharts-0.1.9/sarcharts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.468326 sarcharts-0.1.9/sarcharts/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/bin/sarcharts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.464326 sarcharts-0.1.9/sarcharts/html/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.468326 sarcharts-0.1.9/sarcharts/html/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/html/css/sarcharts.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/html/css/ul-select.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.468326 sarcharts-0.1.9/sarcharts/html/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/html/img/chevron.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.468326 sarcharts-0.1.9/sarcharts/html/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   205214 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/html/js/chart.umd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/html/js/chartjs-plugin-zoom.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/html/js/hammer.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   271751 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/html/js/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/html/js/ul-select.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.468326 sarcharts-0.1.9/sarcharts/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/lib/chartjs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/lib/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/lib/sadf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/lib/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.468326 sarcharts-0.1.9/sarcharts/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/templates/chart.html
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-14 15:42:39.000000 sarcharts-0.1.9/sarcharts/templates/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:42:44.468326 sarcharts-0.1.9/sarcharts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-14 15:42:44.000000 sarcharts-0.1.9/sarcharts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-14 15:42:44.000000 sarcharts-0.1.9/sarcharts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:42:44.000000 sarcharts-0.1.9/sarcharts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 15:42:44.000000 sarcharts-0.1.9/sarcharts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:42:44.000000 sarcharts-0.1.9/sarcharts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 15:42:44.000000 sarcharts-0.1.9/sarcharts.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 15:42:44.000000 sarcharts-0.1.9/sarcharts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 15:42:44.000000 sarcharts-0.1.9/sarcharts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-14 15:42:44.472326 sarcharts-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-14 15:42:39.000000 sarcharts-0.1.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-14 15:42:39.000000 sarcharts-0.1.9/test-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-14 15:42:39.000000 sarcharts-0.1.9/tox.ini
```

### Comparing `sarcharts-0.1.8/.github/workflows/python-publish.yml` & `sarcharts-0.1.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.8/.pylintrc` & `sarcharts-0.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.8/LICENSE` & `sarcharts-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.8/PKG-INFO` & `sarcharts-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarcharts
-Version: 0.1.8
+Version: 0.1.9
 Summary: SarCharts gets sysstat files from provided sarfilespaths and generates dynamic HTML Charts
 Home-page: https://github.com/pafernanr/sarcharts
 Author: Pablo Fernández Rodríguez
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `sarcharts-0.1.8/README.md` & `sarcharts-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.8/doc/README.md` & `sarcharts-0.1.9/doc/README.md`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.8/doc/sarcharts.png` & `sarcharts-0.1.9/doc/sarcharts.png`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.8/sarcharts/__init__.py` & `sarcharts-0.1.9/sarcharts/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,21 @@
 
 import argparse
 import fnmatch
 import shutil
 import webbrowser
 
 from sarcharts.lib.chartjs import ChartJS
-from sarcharts.lib.chartsconf import ChartsConf
 from sarcharts.lib.sadf import Sadf
 from sarcharts.lib import util
 
 
 class SarCharts:
     args = ()
     cwd = os.getcwd()
-    C = ChartsConf()
 
     def valid_date(self, d):
         valid = ["%Y-%m-%d %H:%M:%S",
                  "%Y-%m-%d %H",
                  "%Y-%m-%d %H:%M",
                  "%Y-%m-%d"
                  ]
@@ -57,63 +55,63 @@
             help='Set debug level. Default `W`.',
             default='W',
             choices=['D', 'I', 'W', 'E']
             )
         self.parser.add_argument(
             '-f',
             '--fromdate',
-            help='Read metric starting on this date.',
-            default='1970-01-01 00:00:00',
+            help='Include metrics from this date.',
+            default=datetime.datetime.strptime('1970-01-01', '%Y-%m-%d'),
             type=self.valid_date
             )
         self.parser.add_argument(
             '-o',
             '--outputpath',
             help='Path to put output files. Default `./sarcharts`.',
             default='.'
             )
         self.parser.add_argument(
             '-t',
             '--todate',
             help='Discard metrics after this date.',
-            default='2099-01-01 00:00:00',
+            default=datetime.datetime.strptime('2039-01-01', '%Y-%m-%d'),
             type=self.valid_date
             )
         self.parser.add_argument(
+            '-q',
+            '--quiet',
+            help="Don't show progress.",
+            default=False,
+            action='store_true'
+            )
+        self.parser.add_argument(
             'sarfilespaths',
             help='`sa` file/s to parse. Default: `./sa??`.',
             default=self.default_sarfiles(),
             type=self.valid_path,
             nargs='*'
             )
         self.args = self.parser.parse_args()
 
         # create required files on outputpath
         self.args.outputpath = self.args.outputpath + "/sarcharts"
         if os.path.exists(self.args.outputpath):
-            util.debug(self.args.debug, 'E',
+            util.debug(self.args, 'E',
                        f"Output path '{self.args.outputpath}' already exists.")
             # shutil.rmtree(self.args.outputpath)
         os.makedirs(self.args.outputpath + "/sar")
         shutil.copytree(os.path.dirname(
                         os.path.realpath(__file__)) + "/html",
                         self.args.outputpath + "/html")
 
     def main(self):
         # import ipdb; ipdb.set_trace()
         if len(self.args.sarfilespaths) > 0:
             sarfiles = util.get_filelist(self.args.sarfilespaths)
-            util.debug(self.args.debug, 'D', "sarfiles: " + str(sarfiles))
-            chartinfo = Sadf().sar_to_chartjs(
-                self.args.debug, sarfiles, self.args.outputpath + "/sar",
-                self.C.charts, self.args.fromdate, self.args.todate
-                )
-            ChartJS().write_files(
-                self.C.charts, self.C.colors, chartinfo, self.args.outputpath
-                )
-            util.debug(self.args.debug, '',
-                       "Open SarCharts in default browser.")
-            webbrowser.open(self.args.outputpath + "/cpu.html", 0, True)
+            util.debug(self.args, 'D', "sarfiles: " + str(sarfiles))
+            charts = Sadf().sar_to_chartjs(self.args, sarfiles)
+            ChartJS().write_files(self.args, charts)
+            util.debug(self.args, '', "Open SarCharts in default browser.")
+            webbrowser.open(self.args.outputpath, 0, True)
         else:
             self.parser.print_help()
-            util.debug(self.args.debug, 'E',
-                       "No valid `sa` files on provided path.")
+            util.debug(self.args, 'E', "No valid `sa` files on provided path.")
```

### Comparing `sarcharts-0.1.8/sarcharts/html/js/chart.umd.js` & `sarcharts-0.1.9/sarcharts/html/js/chart.umd.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.8/sarcharts/html/js/chartjs-plugin-zoom.min.js` & `sarcharts-0.1.9/sarcharts/html/js/chartjs-plugin-zoom.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.8/sarcharts/html/js/hammer.min.js` & `sarcharts-0.1.9/sarcharts/html/js/hammer.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.8/sarcharts/html/js/jquery.js` & `sarcharts-0.1.9/sarcharts/html/js/jquery.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.8/sarcharts/lib/progressbar.py` & `sarcharts-0.1.9/sarcharts/lib/progressbar.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,57 +2,50 @@
 
 from datetime import datetime as mytime
 
 
 class ProgressBar:
     all_entries: int
     start_time: datetime
+    quiet = False
     last_printed_tenth_of_percentage: int
 
     def __init__(self) -> None:
         self.all_entries = 0
         self.last_printed_tenth_of_percentage = 0
 
-    def set_number_of_file_lines(self, log_file_name: str):
-        try:
-            with open(log_file_name, 'r') as file:
-                self.all_entries = max(i for i, line in enumerate(file)) + 1
-        except Exception as file_exception:
-            print(file_exception)
-
-        self.start_time = mytime.now()
-        return self.all_entries
-
     def set_number_of_entries(self, number: int):
         self.all_entries = number
         self.start_time = mytime.now()
 
     def print_bar(self, done_lines: int, msg):
-        if self.all_entries == 0:
-            return
-        tenth_of_percentage = int(1000 * (done_lines / self.all_entries))
-        if self.last_printed_tenth_of_percentage >= tenth_of_percentage:
-            return
-        half_percentage = int((tenth_of_percentage/1000) * (30 + 1))
-        new_bar = chr(9608) * half_percentage + " " * (30 - half_percentage)
-        # now = mytime.now()
-        # left = (
-        #    (self.all_entries - done_lines)
-        #     * (now - self.start_time) / done_lines
-        #    )
-        # sec = int(left.total_seconds())
-        # time_left = "Estimated time left: "
-        # if sec > 60:
-        #    text += f"{format(int(sec / 60))} min "
-        # text += f"{format(int(sec % 79)+1)} sec       "
-        print(" " * 79, end="\r\r")
-        text = f"\r|{new_bar}| {tenth_of_percentage/10:.0f} %  " + msg
-        print(text, end="\r\r")
-
-        # print(tenth_of_percentage)
-        if tenth_of_percentage == 999:
+        if not self.quiet:
+            if self.all_entries == 0:
+                return
+            tenth_of_percentage = int(1000 * (done_lines / self.all_entries))
+            if self.last_printed_tenth_of_percentage >= tenth_of_percentage:
+                return
+            half_percentage = int((tenth_of_percentage/1000) * (30 + 1))
+            new_bar = chr(9608) * half_percentage + " " * (30 - half_percentage)
+            # now = mytime.now()
+            # left = (
+            #    (self.all_entries - done_lines)
+            #     * (now - self.start_time) / done_lines
+            #    )
+            # sec = int(left.total_seconds())
+            # time_left = "Estimated time left: "
+            # if sec > 60:
+            #    text += f"{format(int(sec / 60))} min "
+            # text += f"{format(int(sec % 79)+1)} sec       "
             print(" " * 79, end="\r\r")
-        self.last_printed_tenth_of_percentage = tenth_of_percentage
+            text = f"\r|{new_bar}| {tenth_of_percentage/10:.0f} %  " + msg
+            print(text, end="\r\r")
+            # print(tenth_of_percentage)
+            if tenth_of_percentage == 999:
+                print(" " * 79, end="\r\r")
+            self.last_printed_tenth_of_percentage = tenth_of_percentage
 
     def finish(self, msg):
+        if self.quiet:
+            return 0
         print(" " * 79, end="\r\r")
         print(msg)
```

### Comparing `sarcharts-0.1.8/sarcharts/lib/util.py` & `sarcharts-0.1.9/sarcharts/lib/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 
 import fnmatch
 from pathlib import Path
 import subprocess
 
 
-def debug(debuglevel, sev, msg):
+def debug(args, sev, msg):
     C = {
         'I': '\033[0;34m',
         'D': '\033[01;36m',
         '': '\033[0;32m',
         'W': '\033[93m',
         'E': '\033[0;31m',
         'RESET': '\033[0m'
@@ -20,27 +20,27 @@
               'I': 1,
               'W': 2,
               'E': 3,
               '': 4
               }
     if sev == "":
         print(f"  {str(msg)}")
-    elif levels[sev] >= levels[debuglevel]:
+    elif levels[sev] >= levels[args.debug]:
         print(f"{C[sev]}[{sev}]{C['RESET']} {str(msg)}")
     if sev == 'E':
         sys.exit(1)
 
 
-def exec_command(debuglevel, cmd):
-    debug(debuglevel, "D", "execcommand: " + cmd)
+def exec_command(args, cmd):
+    debug(args, "D", "execcommand: " + cmd)
     p = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE,
                          stderr=subprocess.PIPE)
     stdout, stderr = p.communicate()
-    stdout = str(stdout.decode("utf-8"))
-    stderr = str(stderr.decode("utf-8"))
+    stdout = str(stdout.decode(encoding="utf-8", errors="ignore"))
+    stderr = str(stderr.decode(encoding="utf-8", errors="ignore"))
     # if stderr != "":
     #    print(cmd + "\n" + stderr)
     #    sys.exit(1)
     return [stdout, stderr]
 
 
 def get_filelist(filepaths):
@@ -63,24 +63,24 @@
         mtime = os.path.getmtime(f)
         details[mtime] = f
     # 'sorted' returns a 'set' hence no duplicates
     # but it should be converted to a list
     return list(dict(sorted(details.items())).values())
 
 
-def valid_date(debuglevel, d):
-    formats = ["%Y-%m-%d %H:%M:%S %Z", "%Y-%m-%d %H:%M:%S"]
-    for format in formats:
-        try:
-            return datetime.datetime.strptime(d, format)
-        except ValueError:
-            pass
-    debug(debuglevel, 'E',
-          f"ERROR: date '{d}' doesn't match {str(formats)}.")
+def valid_date(args, d):
+    format = "%Y-%m-%d %H:%M:%S"
+    try:
+        return datetime.datetime.strptime(d, format)
+    except ValueError:
+        debug(args, 'E', f"ERROR: date '{d}' doesn't match {format}.")
 
 
-def in_date_range(debuglevel, dfrom, dto, d):
-    d = valid_date(debuglevel, d)
-    if d >= dfrom and d <= dto:
+def in_date_range(args, d):
+    d = valid_date(args, d)
+    print(args.fromdate)
+    if d >= args.fromdate and d <= args.todate:
+        print("si")
         return True
     else:
+        print("no")
         return False
```

### Comparing `sarcharts-0.1.8/sarcharts/templates/chart.html` & `sarcharts-0.1.9/sarcharts/templates/chart.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>sarcharts {{ hostname }}</title>
     <link rel="stylesheet" href="html/css/sarcharts.css" />
+    <link rel="stylesheet" href="html/css/ul-select.css" />
     <script src="html/js/jquery.js"></script>
     <script src="html/js/chart.umd.js"></script>
     <script src="html/js/hammer.min.js"></script>
     <script src="html/js/chartjs-plugin-zoom.min.js"></script>
+    <script src="html/js/ul-select.js"></script>
 
 </head>
 <body>
+<section class="container">
   {% include "header.html" %}
-  <div class="menucontainer">
+  <div class="activities">
     <ul>
   {% for item in details['datasets'].keys() %}
     {% if item != "" %}
       <li class="i_inactive"><a href='#'>{{ item }}</a></li>
     {% endif %}
   {% endfor %}
     </ul>
   </div>
+</section>
     <div class="chart">
       <canvas id="chartcanvas"></canvas>
     </div>
 <script>
 $('.i_inactive').click(function() {
   $(".i_active").attr("class","i_inactive");
   $(this).attr("class","i_active");
@@ -65,15 +69,15 @@
     }
   });
 }
 
 var myCharts = {
   {% for item, data in details['datasets'].items() %}
   '{{ item }}': {
-    'labels': {{ details['labels'] }},
+    'labels': {{ xlabels }},
     'datasets': [
     {% for i in range(data|length) %}
       {
       {{ "hidden: true," if data[i]['label'] in details['hidden'] else "" }}
       label: '{{ data[i]['label'] }}',
       data: {{ data[i]['values'] }},
       borderColor: 'rgb({{ colors[i] }} 0.3)',
@@ -87,12 +91,24 @@
 
 var ctx = document.getElementById('chartcanvas').getContext('2d');
 var myChart = new Chart(ctx);
 
 $(document).ready(function () {
   showChart($('.i_inactive').first().text());
   $('.i_inactive').first().attr("class", "i_active");
+
+  selhost="{{ hostname }}"
+  $('#hostlist').ulSelect(function(elem) {
+      selhost=$(elem).text()
+      window.location = selhost+"_cpu-load.html"
+  });
+  selchart="{{ chart }}"
+  $('#chartlist').ulSelect(function(elem) {
+      selchart=$(elem).text()
+      window.location = selhost+"_"+selchart+".html"
+  });
+
 });
 
 </script>
 </body>
 </html>
```

### Comparing `sarcharts-0.1.8/sarcharts.egg-info/PKG-INFO` & `sarcharts-0.1.9/sarcharts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarcharts
-Version: 0.1.8
+Version: 0.1.9
 Summary: SarCharts gets sysstat files from provided sarfilespaths and generates dynamic HTML Charts
 Home-page: https://github.com/pafernanr/sarcharts
 Author: Pablo Fernández Rodríguez
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `sarcharts-0.1.8/sarcharts.egg-info/SOURCES.txt` & `sarcharts-0.1.9/sarcharts.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -19,18 +19,20 @@
 sarcharts.egg-info/not-zip-safe
 sarcharts.egg-info/pbr.json
 sarcharts.egg-info/requires.txt
 sarcharts.egg-info/top_level.txt
 sarcharts/bin/__init__.py
 sarcharts/bin/sarcharts.py
 sarcharts/html/css/sarcharts.css
+sarcharts/html/css/ul-select.css
+sarcharts/html/img/chevron.svg
 sarcharts/html/js/chart.umd.js
 sarcharts/html/js/chartjs-plugin-zoom.min.js
 sarcharts/html/js/hammer.min.js
 sarcharts/html/js/jquery.js
+sarcharts/html/js/ul-select.js
 sarcharts/lib/chartjs.py
-sarcharts/lib/chartsconf.py
 sarcharts/lib/progressbar.py
 sarcharts/lib/sadf.py
 sarcharts/lib/util.py
 sarcharts/templates/chart.html
 sarcharts/templates/header.html
```

### Comparing `sarcharts-0.1.8/setup.cfg` & `sarcharts-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.8/setup.py` & `sarcharts-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.8/tox.ini` & `sarcharts-0.1.9/tox.ini`

 * *Files identical despite different names*

