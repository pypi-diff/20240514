# Comparing `tmp/swatmf-0.3.0.tar.gz` & `tmp/swatmf-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swatmf-0.3.0.tar", last modified: Wed Jul 26 19:46:04 2023, max compression
+gzip compressed data, was "swatmf-1.0.0.tar", last modified: Tue May 14 21:04:42 2024, max compression
```

## Comparing `swatmf-0.3.0.tar` & `swatmf-1.0.0.tar`

### file list

```diff
@@ -1,45 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 19:46:04.555612 swatmf-0.3.0/
--rw-rw-rw-   0        0        0     1549 2022-02-07 21:13:22.000000 swatmf-0.3.0/LICENSE
--rw-rw-rw-   0        0        0       26 2022-02-04 16:08:00.000000 swatmf-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5147 2023-07-26 19:46:04.552611 swatmf-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4058 2023-07-26 19:45:51.000000 swatmf-0.3.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-26 19:46:04.557613 swatmf-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1868 2023-07-26 19:44:06.000000 swatmf-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 19:46:04.274531 swatmf-0.3.0/swatmf/
--rw-rw-rw-   0        0        0      410 2022-06-19 04:02:57.000000 swatmf-0.3.0/swatmf/__init__.py
--rw-rw-rw-   0        0        0        0 2022-09-19 20:46:24.000000 swatmf-0.3.0/swatmf/cvt_gcm_pcp.py
--rw-rw-rw-   0        0        0     4059 2023-07-26 16:30:38.000000 swatmf-0.3.0/swatmf/forward_run.py
--rw-rw-rw-   0        0        0        0 2022-09-19 20:46:14.000000 swatmf-0.3.0/swatmf/gcm_analysis.py
--rw-rw-rw-   0        0        0     6531 2022-05-31 21:15:54.000000 swatmf-0.3.0/swatmf/gumu_pst_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-26 19:46:04.343551 swatmf-0.3.0/swatmf/hg/
--rw-rw-rw-   0        0        0      479 2022-06-20 21:36:01.000000 swatmf-0.3.0/swatmf/hg/__init__.py
--rw-rw-rw-   0        0        0    12791 2022-09-19 22:19:15.000000 swatmf-0.3.0/swatmf/hg/hg_handler.py
--rw-rw-rw-   0        0        0     4357 2022-06-21 16:07:42.000000 swatmf-0.3.0/swatmf/hg/viz.py
-drwxrwxrwx   0        0        0        0 2023-07-26 19:46:04.506599 swatmf-0.3.0/swatmf/opt_files/
--rw-rw-rw-   0        0        0    56149 2020-06-05 14:31:21.000000 swatmf-0.3.0/swatmf/opt_files/Absolute_SWAT_Values.txt
--rwxrwxrwx   0        0        0   538085 2015-05-12 21:22:20.000000 swatmf-0.3.0/swatmf/opt_files/SUFI2_LH_sample.exe
--rwxrwxrwx   0        0        0   203776 2014-09-23 20:29:02.000000 swatmf-0.3.0/swatmf/opt_files/Swat_Edit.exe
--rwxrwxrwx   0        0        0   844288 2019-11-21 19:44:00.000000 swatmf-0.3.0/swatmf/opt_files/i64pwtadj1.exe
--rw-rw-rw-   0        0        0       57 2022-02-03 23:26:08.000000 swatmf-0.3.0/swatmf/opt_files/model.in
--rwxrwxrwx   0        0        0  3742208 2023-04-25 07:17:33.000000 swatmf-0.3.0/swatmf/opt_files/pestpp-glm.exe
--rwxrwxrwx   0        0        0  4294656 2023-04-25 07:17:31.000000 swatmf-0.3.0/swatmf/opt_files/pestpp-ies.exe
--rwxrwxrwx   0        0        0  4382720 2023-04-25 07:17:32.000000 swatmf-0.3.0/swatmf/opt_files/pestpp-opt.exe
--rwxrwxrwx   0        0        0  2186752 2023-04-25 07:17:32.000000 swatmf-0.3.0/swatmf/opt_files/pestpp-sen.exe
--rw-rw-rw-   0        0        0     1159 2020-06-02 21:21:54.000000 swatmf-0.3.0/swatmf/swatmf_par_chg_run.py
--rw-rw-rw-   0        0        0    15291 2022-07-05 02:24:09.000000 swatmf-0.3.0/swatmf/swatmf_pst_par.py
--rw-rw-rw-   0        0        0     3076 2022-06-16 05:35:37.000000 swatmf-0.3.0/swatmf/swatmf_pst_stats.py
--rw-rw-rw-   0        0        0    30439 2023-07-25 17:41:32.000000 swatmf-0.3.0/swatmf/swatmf_pst_utils.py
--rw-rw-rw-   0        0        0    12353 2022-02-14 16:15:02.000000 swatmf-0.3.0/swatmf/swatmf_scenario_utils.py
--rw-rw-rw-   0        0        0    30561 2023-07-26 16:30:38.000000 swatmf-0.3.0/swatmf/swatmf_viz.py
-drwxrwxrwx   0        0        0        0 2023-07-26 19:46:04.543610 swatmf-0.3.0/swatmf/utils/
--rw-rw-rw-   0        0        0      490 2022-09-19 21:01:09.000000 swatmf-0.3.0/swatmf/utils/__init__.py
--rw-rw-rw-   0        0        0      547 2022-11-22 22:19:38.000000 swatmf-0.3.0/swatmf/utils/etc.py
--rw-rw-rw-   0        0        0     9114 2022-10-04 13:58:18.000000 swatmf-0.3.0/swatmf/utils/swat_utils.py
--rw-rw-rw-   0        0        0    17877 2023-07-25 17:43:32.000000 swatmf-0.3.0/swatmf/utils.py
--rw-rw-rw-   0        0        0       23 2023-07-26 19:23:40.000000 swatmf-0.3.0/swatmf/version.py
-drwxrwxrwx   0        0        0        0 2023-07-26 19:46:04.321544 swatmf-0.3.0/swatmf.egg-info/
--rw-rw-rw-   0        0        0     5147 2023-07-26 19:46:03.000000 swatmf-0.3.0/swatmf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      925 2023-07-26 19:46:03.000000 swatmf-0.3.0/swatmf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 19:46:03.000000 swatmf-0.3.0/swatmf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-07-26 19:46:03.000000 swatmf-0.3.0/swatmf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-26 19:46:03.000000 swatmf-0.3.0/swatmf.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 21:04:42.960460 swatmf-1.0.0/
+-rw-rw-rw-   0        0        0     1549 2022-02-07 21:13:22.000000 swatmf-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0       26 2022-02-04 16:08:00.000000 swatmf-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5219 2024-05-14 21:04:42.960460 swatmf-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4137 2023-11-07 16:06:26.000000 swatmf-1.0.0/README.rst
+-rw-rw-rw-   0        0        0       42 2024-05-14 21:04:42.960460 swatmf-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1869 2024-04-15 20:48:42.000000 swatmf-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:04:42.753447 swatmf-1.0.0/swatmf/
+-rw-rw-rw-   0        0        0      410 2022-06-19 04:02:57.000000 swatmf-1.0.0/swatmf/__init__.py
+-rw-rw-rw-   0        0        0    60308 2024-04-26 18:40:43.000000 swatmf-1.0.0/swatmf/analyzer.py
+-rw-rw-rw-   0        0        0     6116 2024-05-03 02:34:29.000000 swatmf-1.0.0/swatmf/forward_run.py
+-rw-rw-rw-   0        0        0     6531 2022-05-31 21:15:54.000000 swatmf-1.0.0/swatmf/gumu_pst_utils.py
+-rw-rw-rw-   0        0        0    24749 2024-05-03 04:06:11.000000 swatmf-1.0.0/swatmf/handler.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:04:42.787453 swatmf-1.0.0/swatmf/hg/
+-rw-rw-rw-   0        0        0      479 2022-06-20 21:36:01.000000 swatmf-1.0.0/swatmf/hg/__init__.py
+-rw-rw-rw-   0        0        0    12791 2022-09-19 22:19:15.000000 swatmf-1.0.0/swatmf/hg/hg_handler.py
+-rw-rw-rw-   0        0        0     4357 2022-06-21 16:07:42.000000 swatmf-1.0.0/swatmf/hg/viz.py
+-rw-rw-rw-   0        0        0    18162 2024-02-06 20:45:35.000000 swatmf-1.0.0/swatmf/objfns.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:04:42.939458 swatmf-1.0.0/swatmf/opt_files/
+-rw-rw-rw-   0        0        0    56149 2020-06-05 14:31:21.000000 swatmf-1.0.0/swatmf/opt_files/Absolute_SWAT_Values.txt
+-rwxrwxrwx   0        0        0   538085 2015-05-12 21:22:20.000000 swatmf-1.0.0/swatmf/opt_files/SUFI2_LH_sample.exe
+-rwxrwxrwx   0        0        0   203776 2014-09-23 20:29:02.000000 swatmf-1.0.0/swatmf/opt_files/Swat_Edit.exe
+-rwxrwxrwx   0        0        0   844288 2019-11-21 19:44:00.000000 swatmf-1.0.0/swatmf/opt_files/i64pwtadj1.exe
+-rw-rw-rw-   0        0        0       57 2022-02-03 23:26:08.000000 swatmf-1.0.0/swatmf/opt_files/model.in
+-rwxrwxrwx   0        0        0  3742208 2023-04-25 07:17:33.000000 swatmf-1.0.0/swatmf/opt_files/pestpp-glm.exe
+-rwxrwxrwx   0        0        0  4294656 2023-04-25 07:17:31.000000 swatmf-1.0.0/swatmf/opt_files/pestpp-ies.exe
+-rwxrwxrwx   0        0        0  4382720 2023-04-25 07:17:32.000000 swatmf-1.0.0/swatmf/opt_files/pestpp-opt.exe
+-rwxrwxrwx   0        0        0  2186752 2023-04-25 07:17:32.000000 swatmf-1.0.0/swatmf/opt_files/pestpp-sen.exe
+-rw-rw-rw-   0        0        0     6225 2024-04-15 20:48:42.000000 swatmf-1.0.0/swatmf/opt_files/swat_pars.db.csv
+-rwxrwxrwx   0        0        0 10441216 2024-03-20 15:10:33.000000 swatmf-1.0.0/swatmf/opt_files/swatmf_rel230922.exe
+-rw-rw-rw-   0        0        0    38825 2024-05-03 17:43:33.000000 swatmf-1.0.0/swatmf/pst_utils.py
+-rw-rw-rw-   0        0        0     1159 2020-06-02 21:21:54.000000 swatmf-1.0.0/swatmf/swatmf_par_chg_run.py
+-rw-rw-rw-   0        0        0    16055 2024-04-29 22:15:57.000000 swatmf-1.0.0/swatmf/swatmf_pst_par.py
+-rw-rw-rw-   0        0        0     3076 2022-06-16 05:35:37.000000 swatmf-1.0.0/swatmf/swatmf_pst_stats.py
+-rw-rw-rw-   0        0        0    38482 2024-03-22 13:27:03.000000 swatmf-1.0.0/swatmf/swatmf_pst_utils.py
+-rw-rw-rw-   0        0        0    12353 2022-02-14 16:15:02.000000 swatmf-1.0.0/swatmf/swatmf_scenario_utils.py
+-rw-rw-rw-   0        0        0    33411 2024-01-22 20:01:34.000000 swatmf-1.0.0/swatmf/swatmf_viz.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:04:42.958459 swatmf-1.0.0/swatmf/utils/
+-rw-rw-rw-   0        0        0      490 2022-09-19 21:01:09.000000 swatmf-1.0.0/swatmf/utils/__init__.py
+-rw-rw-rw-   0        0        0      547 2022-11-22 22:19:38.000000 swatmf-1.0.0/swatmf/utils/etc.py
+-rw-rw-rw-   0        0        0     7186 2024-05-03 04:07:56.000000 swatmf-1.0.0/swatmf/utils/mf_configs.py
+-rw-rw-rw-   0        0        0    26889 2024-04-15 20:48:42.000000 swatmf-1.0.0/swatmf/utils/swat_configs.py
+-rw-rw-rw-   0        0        0    12501 2024-03-28 23:01:52.000000 swatmf-1.0.0/swatmf/utils/swat_utils.py
+-rw-rw-rw-   0        0        0    21060 2023-12-06 14:39:57.000000 swatmf-1.0.0/swatmf/utils.py
+-rw-rw-rw-   0        0        0       23 2024-04-15 20:48:56.000000 swatmf-1.0.0/swatmf/version.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:04:42.785451 swatmf-1.0.0/swatmf.egg-info/
+-rw-rw-rw-   0        0        0     5219 2024-05-14 21:04:42.000000 swatmf-1.0.0/swatmf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1082 2024-05-14 21:04:42.000000 swatmf-1.0.0/swatmf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 21:04:42.000000 swatmf-1.0.0/swatmf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2024-05-14 21:04:42.000000 swatmf-1.0.0/swatmf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-14 21:04:42.000000 swatmf-1.0.0/swatmf.egg-info/top_level.txt
```

### Comparing `swatmf-0.3.0/LICENSE` & `swatmf-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swatmf-0.3.0/PKG-INFO` & `swatmf-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: swatmf
-Version: 0.3.0
+Version: 1.0.0
 Summary: swatmf is a set of python modules for SWAT-MODFLOW model evaluation and parameter estimation.
 Download-URL: https://pypi.org/project/swatmf
 Author: Seonggyu Park
 Author-email: <envpsg@gmail.com>
 Project-URL: Bug Tracker, https://github.com/spark-brc/swatmf/issues
 Project-URL: Source Code, https://github.com/spark-brc/swatmf
 Project-URL: Documentation, https://github.com/spark-brc/swatmf
 Keywords: python,SWAT-MODFLOW,PEST
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ======
 swatmf
@@ -53,18 +53,18 @@
 - `Download the data zip file <https://github.com/spark-brc/swatmf/archive/refs/heads/main.zip>`_
 - Unzip `swatmf-main.zip` to a prefered location.
 
 
 Hard way (Dev mode)
 -------------------
 
-- You will need to install Git if you donâ€™t have it installed already. Downloads are available at [the link](https://git-scm.com/download). On windows, be sure to select the option that installs command-line tools  
+- You will need to install Git if you don't have it installed already. Downloads are available at [the link](https://git-scm.com/download). On windows, be sure to select the option that installs command-line tools  
 - For Git, you will need to set up SSH keys to work with Github. To do so:
     - Go to GitHub.com and set up an account
-    - On Windows, open Git Bash (on Mac/Linux, just open a terminal) and set up ssh keys if you havenâ€™t already. To do this, simply type ssh-keygen in git bash/terminal and accept all defaults (important note - when prompted for an optional passphrase, just hit return.)  
+    - On Windows, open Git Bash (on Mac/Linux, just open a terminal) and set up ssh keys if you haven't already. To do this, simply type ssh-keygen in git bash/terminal and accept all defaults (important note - when prompted for an optional passphrase, just hit return.)  
 - Follow the `instructions <https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/>`_ to set up the SSH keys with your GitHub account.
 - Clone the materials from GitHub.
     - Open a git bash shell from the start menu (or, on a Mac/Linux, open a terminal)
     - Navigate to the folder you made to put the course materials
     - Clone the materials by executing the following in the git bash or terminal window:
 
 
@@ -98,15 +98,15 @@
    conda install -c conda-forge mamba
 
 
 - Using the `cd <https://www.computerhope.com/issues/chusedos.htm>`_ command in the Miniconda DOS box, navigate to the location where you have `environment.yml` the file and type: 
 
 .. code-block:: bash
 
-   mamba env create -f environment.yml
+   mamba env create -f environment_swatmf.yml
 
 and hit ENTER.
 
 After your virtual environment setup is complete, change the environment to `swatmf`:  
 
 .. code-block:: bash
 
@@ -126,19 +126,21 @@
 
 .. rubric:: Brief overview of the API
 
 .. code-block:: python
 
    from swatmf import swatmf_pst_utils
 
-   >>> wd = "User-SWAT-MODFLOW working directory"
-   >>> swat_wd = "User-SWAT working directory"
-   >>> swatmf_pst_utils.init_setup(wd, swat_wd)
+   >>> prj_dir = "project directory"
+   >>> swatmfwd = "SWAT-MODFLOW model"
+   >>> swatwd = "SWAT model"
+   >>> swatmf_pst_utils.init_setup(prj_dir, swatmfwd, swatwd))
 
    Creating 'backup' folder ... passed
    Creating 'echo' folder ... passed
    Creating 'sufi2.in' folder ... passed
-   'beopest64.exe' file copied ... passed
-   'i64pest.exe' file copied ... passed
-   'i64pwtadj1.exe' file copied ... passed
+   'Absolute_SWAT_Values.txt' file copied ... passed
+   'pestpp-glm' file copied ... passed
+   'pestpp-ies.exe' file copied ... passed
+   'pestpp-ies.exe' file copied ... passed
    'forward_run.py' file copied ... passed
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `swatmf-0.3.0/README.rst` & `swatmf-1.0.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -31,18 +31,18 @@
 - `Download the data zip file <https://github.com/spark-brc/swatmf/archive/refs/heads/main.zip>`_
 - Unzip `swatmf-main.zip` to a prefered location.
 
 
 Hard way (Dev mode)
 -------------------
 
-- You will need to install Git if you don’t have it installed already. Downloads are available at [the link](https://git-scm.com/download). On windows, be sure to select the option that installs command-line tools  
+- You will need to install Git if you don't have it installed already. Downloads are available at [the link](https://git-scm.com/download). On windows, be sure to select the option that installs command-line tools  
 - For Git, you will need to set up SSH keys to work with Github. To do so:
     - Go to GitHub.com and set up an account
-    - On Windows, open Git Bash (on Mac/Linux, just open a terminal) and set up ssh keys if you haven’t already. To do this, simply type ssh-keygen in git bash/terminal and accept all defaults (important note - when prompted for an optional passphrase, just hit return.)  
+    - On Windows, open Git Bash (on Mac/Linux, just open a terminal) and set up ssh keys if you haven't already. To do this, simply type ssh-keygen in git bash/terminal and accept all defaults (important note - when prompted for an optional passphrase, just hit return.)  
 - Follow the `instructions <https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/>`_ to set up the SSH keys with your GitHub account.
 - Clone the materials from GitHub.
     - Open a git bash shell from the start menu (or, on a Mac/Linux, open a terminal)
     - Navigate to the folder you made to put the course materials
     - Clone the materials by executing the following in the git bash or terminal window:
 
 
@@ -76,15 +76,15 @@
    conda install -c conda-forge mamba
 
 
 - Using the `cd <https://www.computerhope.com/issues/chusedos.htm>`_ command in the Miniconda DOS box, navigate to the location where you have `environment.yml` the file and type: 
 
 .. code-block:: bash
 
-   mamba env create -f environment.yml
+   mamba env create -f environment_swatmf.yml
 
 and hit ENTER.
 
 After your virtual environment setup is complete, change the environment to `swatmf`:  
 
 .. code-block:: bash
 
@@ -104,19 +104,21 @@
 
 .. rubric:: Brief overview of the API
 
 .. code-block:: python
 
    from swatmf import swatmf_pst_utils
 
-   >>> wd = "User-SWAT-MODFLOW working directory"
-   >>> swat_wd = "User-SWAT working directory"
-   >>> swatmf_pst_utils.init_setup(wd, swat_wd)
+   >>> prj_dir = "project directory"
+   >>> swatmfwd = "SWAT-MODFLOW model"
+   >>> swatwd = "SWAT model"
+   >>> swatmf_pst_utils.init_setup(prj_dir, swatmfwd, swatwd))
 
    Creating 'backup' folder ... passed
    Creating 'echo' folder ... passed
    Creating 'sufi2.in' folder ... passed
-   'beopest64.exe' file copied ... passed
-   'i64pest.exe' file copied ... passed
-   'i64pwtadj1.exe' file copied ... passed
+   'Absolute_SWAT_Values.txt' file copied ... passed
+   'pestpp-glm' file copied ... passed
+   'pestpp-ies.exe' file copied ... passed
+   'pestpp-ies.exe' file copied ... passed
    'forward_run.py' file copied ... passed
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `swatmf-0.3.0/setup.py` & `swatmf-1.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #     long_description = "\n" + fh.read()
 #
 
 with open("README.rst", "r") as fd:
     long_desc = fd.read()
 
 
-VERSION = '0.3.0'
+VERSION = '1.0.0'
 DESCRIPTION = 'swatmf is a set of python modules for SWAT-MODFLOW model evaluation and parameter estimation.'
 # LONG_DESCRIPTION = 'A package that allows to work with SWAT-MODFLOW model'
 
 license = "BSD-3-Clause"
 # Setting up
 setup(
     name="swatmf",
@@ -45,14 +45,14 @@
         'pandas', 'numpy', 'pyemu', 'flopy', 'scipy', 'matplotlib', 'openpyxl',
         'hydroeval', 'tqdm', 'termcolor', 'pyshp'],
     keywords=['python', 'SWAT-MODFLOW', 'PEST'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         "Operating System :: Microsoft :: Windows",
         "License :: OSI Approved :: BSD License"
     ]
 )
```

### Comparing `swatmf-0.3.0/swatmf/gumu_pst_utils.py` & `swatmf-1.0.0/swatmf/gumu_pst_utils.py`

 * *Files identical despite different names*

### Comparing `swatmf-0.3.0/swatmf/hg/hg_handler.py` & `swatmf-1.0.0/swatmf/hg/hg_handler.py`

 * *Files identical despite different names*

### Comparing `swatmf-0.3.0/swatmf/hg/viz.py` & `swatmf-1.0.0/swatmf/hg/viz.py`

 * *Files identical despite different names*

### Comparing `swatmf-0.3.0/swatmf/opt_files/Absolute_SWAT_Values.txt` & `swatmf-1.0.0/swatmf/opt_files/Absolute_SWAT_Values.txt`

 * *Files identical despite different names*

### Comparing `swatmf-0.3.0/swatmf/opt_files/SUFI2_LH_sample.exe` & `swatmf-1.0.0/swatmf/opt_files/SUFI2_LH_sample.exe`

 * *Files identical despite different names*

### Comparing `swatmf-0.3.0/swatmf/opt_files/Swat_Edit.exe` & `swatmf-1.0.0/swatmf/opt_files/Swat_Edit.exe`

 * *Files identical despite different names*

### Comparing `swatmf-0.3.0/swatmf/opt_files/i64pwtadj1.exe` & `swatmf-1.0.0/swatmf/opt_files/i64pwtadj1.exe`

 * *Files identical despite different names*

### Comparing `swatmf-0.3.0/swatmf/opt_files/pestpp-glm.exe` & `swatmf-1.0.0/swatmf/opt_files/pestpp-glm.exe`

 * *Files identical despite different names*

### Comparing `swatmf-0.3.0/swatmf/opt_files/pestpp-ies.exe` & `swatmf-1.0.0/swatmf/opt_files/pestpp-ies.exe`

 * *Files identical despite different names*

### Comparing `swatmf-0.3.0/swatmf/opt_files/pestpp-opt.exe` & `swatmf-1.0.0/swatmf/opt_files/pestpp-opt.exe`

 * *Files identical despite different names*

### Comparing `swatmf-0.3.0/swatmf/opt_files/pestpp-sen.exe` & `swatmf-1.0.0/swatmf/opt_files/pestpp-sen.exe`

 * *Files identical despite different names*

### Comparing `swatmf-0.3.0/swatmf/swatmf_par_chg_run.py` & `swatmf-1.0.0/swatmf/swatmf_par_chg_run.py`

 * *Files identical despite different names*

### Comparing `swatmf-0.3.0/swatmf/swatmf_pst_par.py` & `swatmf-1.0.0/swatmf/swatmf_pst_par.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 import os
 import shutil
 import glob
 from datetime import datetime
 import pandas as pd
 from pyemu.pst.pst_utils import SFMT,IFMT,FFMT
 from tqdm import tqdm
+import numpy as np
 
 
 wd = os.getcwd()
 os.chdir(wd)
 
 def create_riv_par(wd, chns, chg_type=None, rivcd=None, rivbot=None, val=None):
     os.chdir(wd)
     if rivcd is None:
         rivcd =  ['rivcd_{}'.format(x) for x in chns]
     if rivbot is None:
         rivbot =  ['rivbot_{}'.format(x) for x in chns]
     if chg_type is None:
         chg_type = 'unfchg'
     if val is None:
-        val = 0.001
+        val = 0.00001
     riv_f = rivcd + rivbot
     df = pd.DataFrame()
     df['parnme'] = riv_f
     df['chg_type'] = chg_type
     df['val'] = val
+    for i in range(len(df)):
+        if (df.iloc[i, 0][:5]) == 'rivcd':
+            df.iloc[i, 1] = 'pctchg'
     df.index = df.parnme
     with open('mf_riv.par', 'w') as f:
         f.write("# modflow_par file.\n")
         f.write("NAME   CHG_TYPE    VAL\n")
         f.write(
             df.loc[:, ["parnme", "chg_type", "val"]].to_string(
                                                         col_space=0,
@@ -81,15 +85,17 @@
             line1 = f.readline()
             line2 = f.readline()
             line3 = f.readline()
 
         # BUG: change hard code skiprows = 3 
         # read riv pacakge
         df_riv = pd.read_csv('riv_package.org', sep=r'\s+', skiprows=3, header=None)
-
+        print(df_riv)
+        # BUG: prevent 3rd column gets float 
+        df_riv.iloc[:, 2] = df_riv.iloc[:, 2].map(lambda x: '{:.0f}'.format(x))
         # read mf_riv_par.par
         riv_pars = read_modflow_par(wd)
 
         # Select rows based on channel number
         for i in range(len(riv_pars)):
             if riv_pars.iloc[i, 2] == 'rivcd':
                 subdf = df_riv[df_riv.iloc[:, -1] == riv_pars.iloc[i, 3]]
@@ -115,33 +121,43 @@
                     subdf.iloc[:, 5] = float(riv_pars.iloc[i, 1])
                     new_rivbot = subdf.iloc[:, 5]
                 count = 0
                 for j in range(len(df_riv)):
                     if df_riv.iloc[j, -1] == riv_pars.iloc[i, 3]:
                         df_riv.iloc[j, 5] = new_rivbot.iloc[count]
                         count += 1
-
+        
+        # for i in range(len(df_riv)):
+        #     if (df_riv.iloc[i, 2]):
+        #         print(df_riv.iloc[i, 2])
+        #         df_riv.iloc[i, 2] = df_riv.iloc[i, 2].astype('int')
+        #     else:
+        #         df_riv.iloc[i, 2] = 'nan'
+        # df_riv.iloc[:, 2] = df_riv.iloc[:, 2].astype('int')
         df_riv.iloc[:, 4] = df_riv.iloc[:, 4].map(lambda x: '{:.10e}'.format(x))
         df_riv.iloc[:, 3] = df_riv.iloc[:, 3].map(lambda x: '{:.10e}'.format(x))
         df_riv.iloc[:, 5] = df_riv.iloc[:, 5].map(lambda x: '{:.10e}'.format(x))
+        df_riv = df_riv.replace('nan', '', regex=True)
+        # df_riv = df_riv.replace(np.nan, '', regex=True)
 
         # ------------ Export Data to file -------------- #
         version = "version 1.2."
         time = datetime.now().strftime('- %m/%d/%y %H:%M:%S -')
 
         with open(riv_f, 'w') as f:
             f.write("# RIV: River package file is parameterized. " + version + time + "\n")
             f.write(line1)
             f.write(line2)
             f.write(line3)
             df_riv.to_csv(
                         f, sep='\t',
                         header=False,
                         index=False,
-                        line_terminator='\n',
+                        lineterminator='\n',
+                        na_rep='',
                         encoding='utf-8'
                         )
         print(os.path.basename(riv_f) + " file is overwritten successfully!")
 
     elif len(riv_files) > 1:
         print(
                 "You have more than one River Package file!("+str(len(riv_files))+")"+"\n"
```

### Comparing `swatmf-0.3.0/swatmf/swatmf_pst_stats.py` & `swatmf-1.0.0/swatmf/swatmf_pst_stats.py`

 * *Files identical despite different names*

### Comparing `swatmf-0.3.0/swatmf/swatmf_pst_utils.py` & `swatmf-1.0.0/swatmf/pst_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,27 +19,31 @@
 
 opt_files_path = os.path.join(
                     os.path.dirname(os.path.abspath( __file__ )),
                     'opt_files')
 foward_path = os.path.dirname(os.path.abspath( __file__ ))
 
 
-
 def create_swatmf_con(
-                wd, sim_start, warmup, cal_start, cal_end,
+                prj_dir, 
+                swatmf_model, sim_start, warmup, cal_start, cal_end,
                 subs=None, grids=None, riv_parm=None,
                 baseflow=None,
                 time_step=None,
                 pp_included=None,
+                grids_lyrs=None,
+                avg_grids=None
+
                 # depth_to_water=None, 
                 ):
     """create swatmf.con file containg SWAT-MODFLOW model PEST initial settings
 
     Args:
-        wd (`str`): SWAT-MODFLOW working directory
+        prj_dir (`str`): Optimization project working directory
+        swatmf_model (`str`): SWAT-MODFLOW working directory
         subs (`list`): reach numbers to be extracted
         grids (`list`): grid numbers to be extracted
         sim_start (`str`): simulation start date e.g. '1/1/2000'
         warmup(`int`): warm-up period
         cal_start (`str`): calibration start date e.g., '1/1/2001'
         cal_end (`str`): calibration end date e.g., '12/31/2005'
         time_step (`str`, optional): model time step. Defaults to None ('day'). e.g., 'day', 'month', 'year'
@@ -64,79 +68,110 @@
         baseflow = 'n'
     else:
         baseflow = 'y'
     if pp_included is None:
         pp_included = 'n'
     # if depth_to_water is None:
     #     depth_to_water = 'n'
+    if grids_lyrs is None:
+        grids_lyrs = 'n'
 
-
+    if avg_grids is None:
+        avg_grids = 'n'
     col01 = [
-        'wd', 'sim_start', 'warm-up', 'cal_start', 'cal_end',
+        'prj_dir',
+        'swatmf_model', 'sim_start', 'warm-up', 'cal_start', 'cal_end',
         'subs', 'grids',
         'riv_parm', 'baseflow',
         'time_step',
         'pp_included',
+        'grids_lyrs',
+        'avg_grids'
         ]
     col02 = [
-        wd, sim_start, warmup, cal_start, cal_end, 
+        prj_dir,
+        swatmf_model, sim_start, warmup, cal_start, cal_end, 
         subs, grids,
         riv_parm, baseflow,
         time_step,
         pp_included,
+        grids_lyrs,
+        avg_grids
         ]
     df = pd.DataFrame({'names': col01, 'vals': col02})
-    with open(os.path.join(wd, 'swatmf.con'), 'w', newline='') as f:
+
+    main_opt_path = os.path.join(prj_dir, 'main_opt')
+    if not os.path.isdir(main_opt_path):
+        os.makedirs(main_opt_path)
+    with open(os.path.join(prj_dir, 'main_opt', 'swatmf.con'), 'w', newline='') as f:
         f.write("# swatmf.con created by swatmf\n")
         df.to_csv(
             f, sep='\t',
             encoding='utf-8', 
             index=False, header=False)
     return df
 
-def init_setup(wd, swatwd):
+def init_setup(prj_dir, swatmfwd, swatwd):
     filesToCopy = [
         "Absolute_SWAT_Values.txt",
         "i64pwtadj1.exe",
         "pestpp-glm.exe",
         "pestpp-ies.exe",
         "pestpp-opt.exe",
         "pestpp-sen.exe",
         "model.in",
         "SUFI2_LH_sample.exe",
         "Swat_Edit.exe",
+        "swatmf_rel230922.exe"
         ]
     suffix = ' passed'
+    print(" Creating 'main_opt' folder in working directory ...",  end='\r', flush=True)
+
+    main_opt_path = os.path.join(prj_dir, 'main_opt')
+
+    if not os.path.isdir(main_opt_path):
+        os.makedirs(main_opt_path)
+    filelist = [f for f in os.listdir(swatmfwd) if os.path.isfile(os.path.join(swatmfwd, f))]
+    for i in tqdm(filelist):
+        # print(i)
+        # if os.path.getsize(os.path.join(swatwd, i)) != 0:
+        shutil.copy2(os.path.join(swatmfwd, i), main_opt_path)
+    print(" Creating 'main_opt' folder ..." + colored(suffix, 'green'))
+    # create backup
     print(" Creating 'backup' folder ...",  end='\r', flush=True)
-    if not os.path.isdir(os.path.join(wd, 'backup')):
-        os.makedirs(os.path.join(wd, 'backup'))
+    if not os.path.isdir(os.path.join(main_opt_path, 'backup')):
+        os.makedirs(os.path.join(main_opt_path, 'backup'))
         filelist = [f for f in os.listdir(swatwd) if os.path.isfile(os.path.join(swatwd, f))]
         
         # filelist =  os.listdir(swatwd)
         for i in tqdm(filelist):
             # print(i)
             # if os.path.getsize(os.path.join(swatwd, i)) != 0:
-            shutil.copy2(os.path.join(swatwd, i), os.path.join(wd, 'backup'))
+            shutil.copy2(os.path.join(swatwd, i), os.path.join(main_opt_path, 'backup'))
     print(" Creating 'backup' folder ..." + colored(suffix, 'green'))
+
+    # create echo
     print(" Creating 'echo' folder ...",  end='\r', flush=True)
-    if not os.path.isdir(os.path.join(wd, 'echo')):
-        os.makedirs(os.path.join(wd, 'echo'))
+    if not os.path.isdir(os.path.join(main_opt_path, 'echo')):
+        os.makedirs(os.path.join(main_opt_path, 'echo'))
     print(" Creating 'echo' folder ..." + colored(suffix, 'green'))
+    # create sufi2
     print(" Creating 'sufi2.in' folder ...",  end='\r', flush=True)
-    if not os.path.isdir(os.path.join(wd, 'sufi2.in')):
-        os.makedirs(os.path.join(wd, 'sufi2.in'))
+    if not os.path.isdir(os.path.join(main_opt_path, 'sufi2.in')):
+        os.makedirs(os.path.join(main_opt_path, 'sufi2.in'))
     print(" Creating 'sufi2.in' folder ..."  + colored(suffix, 'green'))
 
     for j in filesToCopy:
-        if not os.path.isfile(os.path.join(wd, j)):
-            shutil.copy2(os.path.join(opt_files_path, j), os.path.join(wd, j))
+        if not os.path.isfile(os.path.join(main_opt_path, j)):
+            shutil.copy2(os.path.join(opt_files_path, j), os.path.join(main_opt_path, j))
             print(" '{}' file copied ...".format(j) + colored(suffix, 'green'))
-    if not os.path.isfile(os.path.join(wd, 'forward_run.py')):
-        shutil.copy2(os.path.join(foward_path, 'forward_run.py'), os.path.join(wd, 'forward_run.py'))
-        print(" '{}' file copied ...".format('forward_run.py') + colored(suffix, 'green'))        
+    if not os.path.isfile(os.path.join(main_opt_path, 'forward_run.py')):
+        shutil.copy2(os.path.join(foward_path, 'forward_run.py'), os.path.join(main_opt_path, 'forward_run.py'))
+        print(" '{}' file copied ...".format('forward_run.py') + colored(suffix, 'green'))
+    os.chdir(main_opt_path)       
 
 def extract_day_stf(channels, start_day, warmup, cali_start_day, cali_end_day):
     """extract a daily simulated streamflow from the output.rch file,
         store it in each channel file.
 
     Args:
         - rch_file (`str`): the path and name of the existing output file
@@ -150,15 +185,15 @@
     rch_file = 'output.rch'
     start_day =  start_day[:-4] + str(int(start_day[-4:])+ int(warmup))
 
     rch_file = 'output.rch'
     for i in channels:
         sim_stf = pd.read_csv(
                         rch_file,
-                        delim_whitespace=True,
+                        sep=r'\s+',
                         skiprows=9,
                         usecols=[1, 3, 6],
                         names=["date", "filter", "stf_sim"],
                         index_col=0)
 
         sim_stf_f = sim_stf.loc[i]
         sim_stf_f = sim_stf_f.drop(['filter'], axis=1)
@@ -252,15 +287,15 @@
         for item in bfr_f:
             writer.writerow([(item[0]),
                 '{:.4f}'.format(float(item[1]))
                 ])
     print('Finished ...\n')
 
 
-def extract_depth_to_water(grid_ids, start_day, end_day):
+def extract_depth_to_water(grid_ids, start_day, end_day, time_step="day"):
     """extract a simulated depth to water using modflow.obs and swatmf_out_MF_obs,
         store it in each channel file.
 
     Args:
         - rch_file (`str`): the path and name of the existing output file
         - channels (`list`): channel number in a list, e.g. [9, 60]
         - start_day ('str'): simulation start day after warmup period, e.g. '1/1/1985'
@@ -287,25 +322,155 @@
 
     mf_sim = pd.read_csv(
                         'swatmf_out_MF_obs', skiprows=1, sep=r'\s+',
                         names=col_names,
                         # usecols=grid_ids,
                         )
     mf_sim.index = pd.date_range(start_day, periods=len(mf_sim))
-    mf_sim = mf_sim[start_day:end_day]
+    if time_step == "day":
+        mf_sim = mf_sim[start_day:end_day]
+    if time_step == "month":
+        mf_sim = mf_sim[start_day:end_day].resample('M').mean()
     for i in grid_ids:
         elev = mf_obs_grid_ids.loc[i].values  # use land surface elevation to get depth to water
         (mf_sim.loc[:, i] - elev).to_csv(
                         'dtw_{}.txt'.format(i), sep='\t', encoding='utf-8',
                         index=True, header=False, float_format='%.7e'
                         )
         print('dtw_{}.txt file has been created...'.format(i))
     print('Finished ...')
 
 
+def extract_depth_to_water_layer(dtw_df, start_day, end_day, time_step="day"):
+    """create depth to water extracted file with layer info
+
+    :param dtw_df: depth to water dataframe created by handler.get_gw_sim function
+    :type dtw_df: dataframe
+    :param start_day: sim startdate
+    :type start_day: str
+    :param end_day: sim enddate
+    :type end_day: str
+    :param time_step: time step, defaults to "day"
+    :type time_step: str, optional
+    """
+    if time_step == "day":
+        mf_sim = dtw_df[start_day:end_day]
+    if time_step == "month":
+        mf_sim = dtw_df[start_day:end_day].resample('M').mean()
+    for col in mf_sim.columns:
+        mf_sim.loc[:, col].to_csv(
+                        '{}.txt'.format(col), sep='\t', encoding='utf-8',
+                        index=True, header=False, float_format='%.7e'
+                        )    
+        print('{}.txt file has been created...'.format(col))
+    print('Finished ...')
+
+
+def extract_avg_depth_to_water(
+                grid_ids, start_day, 
+                avg_stdate, avg_eddate,
+                time_step="day"
+                ):
+    """extract a simulated depth to water using modflow.obs and swatmf_out_MF_obs,
+        store it in each channel file.
+
+    Args:
+        - rch_file (`str`): the path and name of the existing output file
+        - channels (`list`): channel number in a list, e.g. [9, 60]
+        - start_day ('str'): simulation start day after warmup period, e.g. '1/1/1985'
+        - end_day ('str'): simulation end day e.g. '12/31/2000'
+
+    Example:
+        pest_utils.extract_depth_to_water('path', [9, 60], '1/1/1993', '12/31/2000')
+    """
+    if not os.path.exists('swatmf_out_MF_obs'):
+        raise Exception("'swatmf_out_MF_obs' file not found")
+    if not os.path.exists('modflow.obs'):
+        raise Exception("'modflow.obs' file not found")
+    mf_obs_grid_ids = pd.read_csv(
+                        'modflow.obs',
+                        sep=r'\s+',
+                        usecols=[3, 4],
+                        skiprows=2,
+                        header=None
+                        )
+    col_names = mf_obs_grid_ids.iloc[:, 0].tolist()
+
+    # set index by modflow grid ids
+    mf_obs_grid_ids = mf_obs_grid_ids.set_index([3])
+
+    mf_sim = pd.read_csv(
+                        'swatmf_out_MF_obs', skiprows=1, sep=r'\s+',
+                        names=col_names,
+                        # usecols=grid_ids,
+                        )
+    mf_sim.index = pd.date_range(start_day, periods=len(mf_sim))
+    # mf_sim = mf_sim[avg_stdate:avg_eddate]
+    if time_step == "day":
+        mf_sim = mf_sim[avg_stdate:avg_eddate].mean()
+    # if time_step == "month":
+    #     mf_sim = mf_sim[avg_stdate:avg_eddate].resample('M').mean()
+    df_avg = pd.DataFrame()
+    dtws = []
+    for i in grid_ids:
+        elev = mf_obs_grid_ids.loc[i, 4]
+        dtws.append(mf_sim.loc[i] - elev)
+    df_avg = pd.DataFrame()
+    df_avg['grid_ids'] = grid_ids
+    df_avg['sims'] = dtws
+    df_avg.to_csv("dtw_avg.txt", sep='\t', index=False, header=False, float_format='%.7e')
+
+        # use land surface elevation to get depth to water
+        # (mf_sim.loc[:, i] - elev).to_csv(
+        #                 'dtw_{}.txt'.format(i), sep='\t', encoding='utf-8',
+        #                 index=True, header=False, float_format='%.7e'
+        #                 )
+        # print('dtw_{}.txt file has been created...'.format(i))
+    # print('Finished ...')
+
+def mf_avg_obd_to_ins(wt_file=None):
+    """extract a simulated groundwater levels from the  file,
+        store it in each channel file.
+
+    Args:
+        - rch_file (`str`): the path and name of the existing output file
+        - channels (`list`): channel number in a list, e.g. [9, 60]
+        - start_day ('str'): simulation start day after warmup period, e.g. '1/1/1993'
+        - end_day ('str'): simulation end day e.g. '12/31/2000'
+
+    Example:
+        pest_utils.extract_month_str('path', [9, 60], '1/1/1993', '12/31/2000')
+    """ 
+    if wt_file is None:
+        wt_file = "dtw_avg.txt"
+    mf_obd_file = "dtw_avg.obd.csv"
+    col_name = "avg_dtw"
+    
+    mf_obd = pd.read_csv(
+                        mf_obd_file,
+                        index_col=0,
+                        )
+    wt_sim = pd.read_csv(
+                        wt_file,
+                        delim_whitespace=True,
+                        names=['grid_id', 'dtw_avg_sim'],
+                        index_col=0,
+                        )
+    result = pd.concat([mf_obd, wt_sim], axis=1)
+    result['ins'] = (
+                    'l1 w !{}_'.format(col_name) + result.index.map(str) + '!'
+                    )
+    result['{}_ins'.format(col_name)] = np.where(result[col_name].isnull(), 'l1', result['ins'])
+    with open(wt_file+'.ins', "w", newline='') as f:
+        f.write("pif ~" + "\n")
+        result['{}_ins'.format(col_name)].to_csv(f, sep='\t', encoding='utf-8', index=False, header=False)
+    print('{}.ins file has been created...'.format(wt_file))
+    return result['{}_ins'.format(col_name)]
+
+
 def stf_obd_to_ins(srch_file, col_name, cal_start, cal_end, time_step=None):
     """extract a simulated streamflow from the output.rch file,
         store it in each channel file.
 
     Args:
         - rch_file (`str`): the path and name of the existing output file
         - channels (`list`): channel number in a list, e.g. [9, 60]
@@ -314,22 +479,22 @@
         - time_step (`str`): day, month, year
 
     Example:
         pest_utils.extract_month_stf('path', [9, 60], '1/1/1993', '12/31/2000')
     """ 
     if time_step is None:
         time_step = 'day'
-        stfobd_file = 'swat_rch_day.obd'
+        stfobd_file = 'stf_day.obd.csv'
     if time_step == 'month':
-        stfobd_file = 'swat_rch_mon.obd'
+        stfobd_file = 'stf_mon.obd.csv'
 
 
     stf_obd = pd.read_csv(
                         stfobd_file,
-                        sep='\t',
+                        # sep='\t',
                         usecols=['date', col_name],
                         index_col=0,
                         parse_dates=True,
                         na_values=[-999, '']
                         )
     stf_obd = stf_obd[cal_start:cal_end]
 
@@ -362,32 +527,35 @@
     with open(srch_file+'.ins', "w", newline='') as f:
         f.write("pif ~" + "\n")
         result['{}_ins'.format(col_name)].to_csv(f, sep='\t', encoding='utf-8', index=False, header=False)
     print('{}.ins file has been created...'.format(srch_file))
     return result['{}_ins'.format(col_name)]
 
 
-def mf_obd_to_ins(wt_file, col_name, cal_start, cal_end, mf_obd_file=None):
-    """extract a simulated streamflow from the output.rch file,
+def mf_obd_to_ins(wt_file, col_name, cal_start, cal_end, time_step="day"):
+    """extract a simulated groundwater levels from the  file,
         store it in each channel file.
 
     Args:
         - rch_file (`str`): the path and name of the existing output file
         - channels (`list`): channel number in a list, e.g. [9, 60]
         - start_day ('str'): simulation start day after warmup period, e.g. '1/1/1993'
         - end_day ('str'): simulation end day e.g. '12/31/2000'
 
     Example:
         pest_utils.extract_month_str('path', [9, 60], '1/1/1993', '12/31/2000')
     """ 
-    if mf_obd_file is None:
-        mf_obd_file = "modflow_day.obd"
+    if time_step == "day":
+        mf_obd_file = "dtw_day.obd.csv"
+    if time_step == "month":
+        mf_obd_file = "dtw_mon.obd.csv"
+
+
     mf_obd = pd.read_csv(
                         mf_obd_file,
-                        sep='\t',
                         usecols=['date', col_name],
                         index_col=0,
                         na_values=[-999, ""],
                         parse_dates=True,
                         )
     mf_obd = mf_obd[cal_start:cal_end]
 
@@ -491,15 +659,15 @@
     # mod_df.loc[:, "tpl"] = mod_df.parnme.apply(lambda x: " ~   {0:15s}   ~".format(x[3:7]))
     with open(tpl_file, 'w') as f:
         f.write("ptf ~\n")
         # f.write("{0:10d} #NP\n".format(mod_df.shape[0]))
         SFMT_LONG = lambda x: "{0:<50s} ".format(str(x))
         f.write(mod_df.loc[:, ["parnme", "tpl"]].to_string(
                                                         col_space=0,
-                                                        formatters=[SFMT, SFMT],
+                                                        formatters=[SFMT_LONG, SFMT_LONG],
                                                         index=False,
                                                         header=False,
                                                         justify="left"))
     return mod_df
 
 
 def riv_par_to_template_file(riv_par_file, tpl_file=None):
@@ -534,14 +702,40 @@
         f.write(mf_par_df.loc[:, ["parnme", "chg_type", "tpl"]].to_string(
                                                         col_space=0,
                                                         formatters=[SFMT, SFMT, SFMT],
                                                         index=False,
                                                         header=False,
                                                         justify="left"))
     return mf_par_df
+    # df_p.iloc[:, 0] = df_p.iloc[:, 0].map(lambda x: '{:<12s}'.format(x))
+    # df_p.iloc[:, 2] = df_p.iloc[:, 2].map(lambda x: '{:<12.5e}'.format(x))
+
+
+def fix_riv_pkg(wd, riv_file):
+    """ Delete duplicate river cells in an existing MODFLOW river packgage.
+
+    Args:
+        wd ('str'): path of the working directory.
+        riv_file ('str'): name of river package.
+    """
+
+    with open(os.path.join(wd, riv_file), "r") as fp:
+        lines = fp.readlines()
+        new_lines = []
+        for line in lines:
+            #- Strip white spaces
+            line = line.strip()
+            if line not in new_lines:
+                new_lines.append(line)
+            else:
+                print(line)
+
+    output_file = "{}_fixed".format(riv_file)
+    with open(os.path.join(wd, output_file), "w") as fp:
+        fp.write("\n".join(new_lines))    
 
 
 def _remove_readonly(func, path, excinfo):
     """remove readonly dirs, apparently only a windows issue
     add to all rmtree calls: shutil.rmtree(**,onerror=remove_readonly), wk"""
     os.chmod(path, 128)  # stat.S_IWRITE==128==normal
     func(path)
@@ -719,10 +913,32 @@
                         sep='\t',
                         # usecols=['date', 'sub_37'],
                         index_col=0,
                         parse_dates=True,
                         na_values=[-999, '']
                         )
     stf_obd = stf_obd.resample('M').mean()
-    stf_obd.to_csv('stf_mon.obd', sep='\t', float_format='%.7e')
+    stf_obd.to_csv(
+        'stf_mon.obd.csv', index=True, index_label="date", na_rep=-999, float_format='%.7e')
+    print("done ...")
     
-    
+
+def adjust_weight(wd, obs_file, obgnme, adj_perc):
+    df = pd.read_csv(os.path.join(wd, obs_file))
+    df["obgnme"] = np.where(
+        (df['obsval'] < 1) & (df["obgnme"]==obgnme),
+        obgnme+"_base", df["obgnme"])
+    df["weight_adj"] = np.where(
+        (df["obgnme"]==obgnme+"_base"),
+        df["weight"] + (df["weight"]*adj_perc/100), 
+        df["weight"]
+        )
+    df.to_csv(os.path.join(wd, obs_file), index=False)
+
+
+if __name__ == '__main__':
+    wd = "D:\\Projects\\Watersheds\\Koksilah\\analysis\koksilah_git\\m04-base"
+    obs_file = "koki_zon_rw.obs_data.csv"
+    obgnme = "sub03"
+    adj_perc = 50
+
+    adjust_weight(wd, obs_file, obgnme, adj_perc)
```

### Comparing `swatmf-0.3.0/swatmf/swatmf_scenario_utils.py` & `swatmf-1.0.0/swatmf/swatmf_scenario_utils.py`

 * *Files identical despite different names*

### Comparing `swatmf-0.3.0/swatmf/swatmf_viz.py` & `swatmf-1.0.0/swatmf/swatmf_viz.py`

 * *Files 3% similar despite different names*

```diff
@@ -350,15 +350,86 @@
     if strobd_file == 'swat_rch_mon.obd':
         str_obd = str_obd.resample('M').mean()
     if wt_obd_file == 'modflow_mon.obd':
         wt_obd = wt_obd.resample('M').mean()
 
     df = pd.concat([str_obd, wt_obd], axis=1)
     return df
+
+def dtw_df(start_date, grid_id, obd_nam, time_step=None):
+    #NOTE: for swatmf
+    """create a dataframe containing extract simulated and observed depth to water 
+
+    Args:
+        start_date (str): datetime index format e.g., "1/1/1999"
+        grid_id (int): grid id
+        obd_nam (str): column name from modflow obd file
+        time_step (str, optional): timestep for measured data. Defaults to "D (day)".
+
+    Returns:
+        dataframe: a dataframe containing extract simulated and observed depth to water
+    """
     
+    if time_step is None:
+        time_step = "D"
+        mfobd_file = "dtw_day.obd"
+    else:
+        time_step = "M"
+        mfobd_file = "dtw_mon.obd."
+
+    mf_obs = pd.read_csv(
+                        "modflow.obs",
+                        delim_whitespace=True,
+                        skiprows = 2,
+                        usecols = [3, 4],
+                        index_col = 0,
+                        names = ["grid_id", "mf_elev"],)
+    mfobd_df = pd.read_csv(
+                        mfobd_file,
+                        sep=r'\s+',
+                        index_col=0,
+                        header=0,
+                        parse_dates=True,
+                        na_values=[-999, ""],
+                        delimiter="\t")
+
+    grid_id_lst = mf_obs.index.astype(str).values.tolist()
+    output_wt = pd.read_csv(
+                        "swatmf_out_MF_obs",
+                        delim_whitespace=True,
+                        skiprows = 1,
+                        names = grid_id_lst,)
+    output_wt = output_wt[str(grid_id)] - float(mf_obs.loc[int(grid_id)])
+    output_wt.index = pd.date_range(start_date, periods=len(output_wt))
+
+    if time_step == 'M':
+        output_wt = output_wt.resample('M').mean()
+    # if prep_sub is not None:
+    #     # Get precipitation data from *.DYL
+    #     prep_file = 'sub{}.DLY'.format(prep_sub)
+    #     with open(prep_file) as f:
+    #         content = f.readlines()    
+    #     year = content[0][:6].strip()
+    #     mon = content[0][6:10].strip()
+    #     day = content[0][10:14].strip()
+    #     prep = [float(i[32:38].strip()) for i in content]
+    #     prep_stdate = "/".join((mon,day,year))
+    #     prep_df =  pd.DataFrame(prep, columns=['prep'])
+    #     prep_df.index = pd.date_range(prep_stdate, periods=len(prep))
+    #     prep_df = prep_df.replace(9999, np.nan)
+    #     # if time_step == "M":
+    #     prep_df = prep_df.resample('M').mean()
+    #     output_wt = pd.concat([output_wt, mfobd_df[obd_nam], prep_df], axis=1)
+    # else:
+    #     output_wt = pd.concat([output_wt, mfobd_df[obd_nam]], axis=1)
+    output_wt = pd.concat([output_wt, mfobd_df[obd_nam]], axis=1)
+    output_wt = output_wt[output_wt[str(grid_id)].notna()]
+
+    return output_wt       
+
 
 def wt_df(start_date, grid_id, obd_nam, time_step=None, prep_sub=None):
     
     if time_step is None:
         time_step = "D"
         mfobd_file = "modflow_day.obd"
     else:
@@ -370,15 +441,15 @@
                         delim_whitespace=True,
                         skiprows = 2,
                         usecols = [3, 4],
                         index_col = 0,
                         names = ["grid_id", "mf_elev"],)
     mfobd_df = pd.read_csv(
                         "MODFLOW/" + mfobd_file,
-                        sep='\s+',
+                        sep=r'\s+',
                         index_col=0,
                         header=0,
                         parse_dates=True,
                         na_values=[-999, ""],
                         delimiter="\t")
 
     grid_id_lst = mf_obs.index.astype(str).values.tolist()
@@ -499,15 +570,15 @@
                         delim_whitespace=True,
                         skiprows = 2,
                         usecols = [3, 4],
                         index_col = 0,
                         names = ["grid_id", "mf_elev"],)
     mfobd_df = pd.read_csv(
                         "MODFLOW/" + mfobd_file,
-                        sep='\s+',
+                        sep=r'\s+',
                         index_col=0,
                         header=0,
                         parse_dates=True,
                         na_values=[-999, ""],
                         delimiter="\t")
     grid_id_lst = mf_obs.index.astype(str).values.tolist()
     # read simulated water elevation
```

### Comparing `swatmf-0.3.0/swatmf/utils/etc.py` & `swatmf-1.0.0/swatmf/utils/etc.py`

 * *Files identical despite different names*

### Comparing `swatmf-0.3.0/swatmf/utils/swat_utils.py` & `swatmf-1.0.0/swatmf/utils/swat_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,17 +5,28 @@
 # from .. import gcm_analysis
 from tqdm import tqdm
 
 
 class WeatherData(object):
     
     def __init__(self, wd):
+        """weather dataset
+
+        Args:
+            wd (path): weather dataset path
+        """
+        
         os.chdir(wd)
     
     def get_weather_folder_lists(self):
+        """return weather folder names and full paths
+
+        Returns:
+            str: return weather folder names and full paths
+        """
         wt_fds = [name for name in os.listdir(".") if os.path.isdir(name)]
         full_paths = [os.path.abspath(name) for name in os.listdir(".") if os.path.isdir(name)]
         return wt_fds, full_paths
         
     @property
     def cvt_gcm_pcp(self):
         full_paths = self.fullpaths
@@ -150,15 +161,14 @@
                 os.makedirs(os.path.join(output_wd, nm, 'TMP'), exist_ok=True)
                 os.chdir(os.path.join(output_wd, nm, 'TMP'))
                 with open(f'TMP_{i+1:03d}.txt', 'w') as fp:
                     for l in abf:
                         fp.write(l+"\n")
 
 
-
     def cvt_tmp_each2(self, output_wd, tmp_nloc, tmp_file=None):
         if tmp_file is None:
             tmp_file = 'Tmp1.Tmp'
         nms, fps = self.get_weather_folder_lists()
         for nm, fp in zip(nms[1:], fps[1:]):
             print(f'reading model {fp} ... processing')
             max_df, min_df = self.read_tmp(os.path.join(fp, tmp_file), tmp_nloc)
@@ -184,7 +194,96 @@
                 abf = stdate + ab
 
                 os.makedirs(os.path.join(output_wd, nm, 'TMP'), exist_ok=True)
                 os.chdir(os.path.join(output_wd, nm, 'TMP'))
                 with open(f'TMP_{i+1:03d}.txt', 'w') as fp:
                     for l in abf:
                         fp.write(l+"\n")
+
+class SwatEdit(object):
+
+    def read_swatcal(self):
+        swatcalfile = "swatcalparms.cal"
+        y = ("#") # Remove unnecssary lines
+        with open(swatcalfile, "r") as f:
+            data = [x.strip() for x in f if x.strip() and not x.strip().startswith(y)] # Remove blank lines     
+        rowsnum = data[0]
+        df = pd.read_csv(swatcalfile, sep=r'\s+',  comment="#", header=1)
+        df = df.iloc[:int(rowsnum)]
+        df['real_val'] = df['VAL'] + df['OFFSET']
+
+        # create model.in
+        with open("model.in", 'w') as f:
+            # f.write("{0:10d} #NP\n".format(mod_df.shape[0]))
+            SFMT_LONG = lambda x: "{0:<50s} ".format(str(x))
+            f.write(df.loc[:, ["NAME", "real_val"]].to_string(
+                                                        col_space=0,
+                                                        formatters=[SFMT_LONG, SFMT_LONG],
+                                                        index=False,
+                                                        header=False,
+                                                        justify="left"))
+
+def modify_sol(back_dir, output_dir):
+
+    ext = "sol"
+    dir_list = os.listdir(back_dir)
+    files_all = [
+                x for x in dir_list if (x.endswith('.{}'.format(ext)) and 
+                not x.startswith('output'))
+                ]
+    
+    var_list = ['SNAM', 'HYDGRP', 'SOL_ZMX', 'ANION_EXCL', 'SOL_CRK', 'TEXTURE',
+                'SOL_Z', 'SOL_BD', 'SOL_AWC', 'SOL_K', 'SOL_CBN', 'SOL_CLAY', 'SOL_SILT',
+                'SOL_SAND', 'SOL_ROCK', 'SOL_ALB', 'USLE_K', 'SOL_EC', 'SOL_CAL', 'SOL_PH']
+    n_line = 9
+    txtformat = '12.2f'
+                    
+    for fl in tqdm(files_all):
+        with open(os.path.join(back_dir, fl), 'r', encoding='ISO-8859-1') as f:
+            data = f.readlines()
+        line = data[n_line]
+        parts = line.split(':')
+        num = parts[1].strip()
+        nums = num.split()
+        # change percentage to ratio
+        nums2 = []
+        for nm in nums:
+            if float(nm) > 1:
+                nm = float(nm)/100
+                nums2.append(nm)
+            else:
+                nums2.append(nm)
+
+
+
+        part1 = ''.join(['{:{}}'.format(float(x), txtformat) for x in nums2])
+        new_line = '{part1}:{part2}\n'.format(part1=parts[0], part2=part1)
+        data[n_line] = new_line
+        with open(os.path.abspath(output_dir + '/' + fl), "w") as f:
+            f.writelines(data)
+    
+
+
+
+
+
+
+
+if __name__ == '__main__':
+    # wd = "/Users/seonggyu.park/Documents/projects/kokshila/swatmf_results"
+    wd = "D:\\tmp\\swatmf_dir\\backup"
+    outwd = "D:\\tmp\\sols_modified"
+
+    modify_sol(wd, outwd)
+
+
+
+    #     sim_stf = pd.read_csv(
+    #                     swatcalfile,
+    #                     delim_whitespace=True,
+    #                     skiprows=9,
+    #                     usecols=[1, 3, 6],
+    #                     names=["date", "filter", "stf_sim"],
+    #                     index_col=0)        
+    
+    # # def create_model_in(self):
+
```

### Comparing `swatmf-0.3.0/swatmf/utils.py` & `swatmf-1.0.0/swatmf/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # import os
 # from hydroeval import evaluator, nse, rmse, pbias
 # import numpy as np
 import numpy as np
 # import h5py as hdf
 import os 
 import datetime
+from tqdm import tqdm
 
 def define_sim_period():
     if os.path.isfile("file.cio"):
         cio = open("file.cio", "r")
         lines = cio.readlines()
         skipyear = int(lines[59][12:16])
         iprint = int(lines[58][12:16]) #read iprint (month, day, year)
@@ -445,16 +446,81 @@
             bas.append(int(data[ii][j]))
         ii += 1
     bas = np.array(bas).reshape([nrows, ncols])
     np.savetxt(os.path.join(wd, 'stuff.dat'), bas.astype(int), fmt='%i',delimiter='\t')
     print(bas)
 
 
+def cvt_usgs_stf_obd(wd, fnam, stdate, eddate, colnam):
+    df = pd.read_csv(os.path.join(wd, fnam), sep='\t', comment='#', header=0)
+    df = df[df['agency_cd']=='USGS']
+    df = df.drop(['agency_cd', f'{colnam}_cd'], axis=1)
+    sites = df['site_no'].unique()
+    dff = pd.DataFrame()
+    dff['date'] = pd.date_range(stdate, eddate)
+    dff = dff.set_index('date')
+    for i in tqdm(sites):
+        data = df[df['site_no']==str(i)]
+        data.index = data.datetime
+        # current data index is not datetimeindex so you need to convert it
+        data.index = pd.to_datetime(data.index)
+        data = data[~data.index.duplicated(keep='first')]
+        data = data.drop(['site_no', 'datetime'], axis=1)
+        data = data[str(colnam)]
+        data.rename(str(i), inplace=True)
+        # print(data)
+        # data = data.rename({colnam: i}, axis=1)
+        # data = data[str(i)]
+        # print(data)
+        # data = data.replace({i:['Ice','Ssn', 'Dis']}, np.nan)
+        # convert cfs to cms
+        data = data.astype('float')*0.0283
+        dff = pd.concat([dff, data], axis=1, sort=True)
+    dff.index.name = 'date'
+    dff = dff.astype('float')
+    # dff.dtypes
+    dff.to_csv(os.path.join(wd, "stf_day.obd2.csv"), na_rep=-999)
+
+def create_model_in(wd, excel_file):
+    df = pd.read_excel(os.path.join(wd, excel_file), dtype=str, names=[0,1,2,3])
+    df['left_col'] = df.iloc[:, [0,1,2]].fillna('').sum(axis=1)
+    df['right_col'] = df.iloc[:, 3].astype(float).map(lambda x: '{:<12.10e}'.format(x))
+    SFMT_LONG = lambda x: "{0:<50s} ".format(str(x))
+    with open(os.path.join(wd, "model.in"), 'w') as f:
+        f.write(df.loc[:, ["left_col", "right_col"]].to_string(
+                                                    col_space=0,
+                                                    formatters=[SFMT_LONG, SFMT_LONG],
+                                                    index=False,
+                                                    header=False,
+                                                    justify="left"
+                                                    )
+                )
+    print(df)
+
+
+def create_model_in_tpl(wd, excel_file):
+    df = pd.read_excel(os.path.join(wd, excel_file), sheet_name="Sheet2", dtype=str, names=[0,1,2,3])
+    df['left_col'] = df.iloc[:, [0,1,2]].fillna('').sum(axis=1)
+    df['right_col'] = df.iloc[:, 3].map(lambda x: " ~   {0:15s}   ~".format(x))
+    SFMT_LONG = lambda x: "{0:<50s} ".format(str(x))
+    with open(os.path.join(wd, "model.in.tpl"), 'w') as f:
+        f.write(df.loc[:, ["left_col", "right_col"]].to_string(
+                                                    col_space=0,
+                                                    formatters=[SFMT_LONG, SFMT_LONG],
+                                                    index=False,
+                                                    header=False,
+                                                    justify="left"
+                                                    )
+                )
+    print(df)
 
 if __name__ == '__main__':
-    wd = "D:/Projects/Watersheds/Gumu/Analysis/APEX-MODFLOWs/qsm_50_rt_test/qsm_50/SWAT-MODFLOW"
-    infile = "mf_50.bas"
-    nrows = 123
-    ncols = 62
+    wd = "D:/Projects/Watersheds/MiddleBosque"
+    infile = "streamflow_obd_usgs.txt"
+    stdate = '1/1/1980'
+    eddate = '12/31/2022'
+    colnam = "135053_00060_00003"
+    excel_file = 'swat_pars.xlsx'
+    # sites = ['08095300']
 
     # print(os.path.abspath(swatmf.__file__))
-    cvt_bas_array(wd, infile, nrows, ncols)
+    create_model_in_tpl(wd, excel_file)
```

### Comparing `swatmf-0.3.0/swatmf.egg-info/PKG-INFO` & `swatmf-1.0.0/swatmf.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: swatmf
-Version: 0.3.0
+Version: 1.0.0
 Summary: swatmf is a set of python modules for SWAT-MODFLOW model evaluation and parameter estimation.
 Download-URL: https://pypi.org/project/swatmf
 Author: Seonggyu Park
 Author-email: <envpsg@gmail.com>
 Project-URL: Bug Tracker, https://github.com/spark-brc/swatmf/issues
 Project-URL: Source Code, https://github.com/spark-brc/swatmf
 Project-URL: Documentation, https://github.com/spark-brc/swatmf
 Keywords: python,SWAT-MODFLOW,PEST
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ======
 swatmf
@@ -53,18 +53,18 @@
 - `Download the data zip file <https://github.com/spark-brc/swatmf/archive/refs/heads/main.zip>`_
 - Unzip `swatmf-main.zip` to a prefered location.
 
 
 Hard way (Dev mode)
 -------------------
 
-- You will need to install Git if you donâ€™t have it installed already. Downloads are available at [the link](https://git-scm.com/download). On windows, be sure to select the option that installs command-line tools  
+- You will need to install Git if you don't have it installed already. Downloads are available at [the link](https://git-scm.com/download). On windows, be sure to select the option that installs command-line tools  
 - For Git, you will need to set up SSH keys to work with Github. To do so:
     - Go to GitHub.com and set up an account
-    - On Windows, open Git Bash (on Mac/Linux, just open a terminal) and set up ssh keys if you havenâ€™t already. To do this, simply type ssh-keygen in git bash/terminal and accept all defaults (important note - when prompted for an optional passphrase, just hit return.)  
+    - On Windows, open Git Bash (on Mac/Linux, just open a terminal) and set up ssh keys if you haven't already. To do this, simply type ssh-keygen in git bash/terminal and accept all defaults (important note - when prompted for an optional passphrase, just hit return.)  
 - Follow the `instructions <https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/>`_ to set up the SSH keys with your GitHub account.
 - Clone the materials from GitHub.
     - Open a git bash shell from the start menu (or, on a Mac/Linux, open a terminal)
     - Navigate to the folder you made to put the course materials
     - Clone the materials by executing the following in the git bash or terminal window:
 
 
@@ -98,15 +98,15 @@
    conda install -c conda-forge mamba
 
 
 - Using the `cd <https://www.computerhope.com/issues/chusedos.htm>`_ command in the Miniconda DOS box, navigate to the location where you have `environment.yml` the file and type: 
 
 .. code-block:: bash
 
-   mamba env create -f environment.yml
+   mamba env create -f environment_swatmf.yml
 
 and hit ENTER.
 
 After your virtual environment setup is complete, change the environment to `swatmf`:  
 
 .. code-block:: bash
 
@@ -126,19 +126,21 @@
 
 .. rubric:: Brief overview of the API
 
 .. code-block:: python
 
    from swatmf import swatmf_pst_utils
 
-   >>> wd = "User-SWAT-MODFLOW working directory"
-   >>> swat_wd = "User-SWAT working directory"
-   >>> swatmf_pst_utils.init_setup(wd, swat_wd)
+   >>> prj_dir = "project directory"
+   >>> swatmfwd = "SWAT-MODFLOW model"
+   >>> swatwd = "SWAT model"
+   >>> swatmf_pst_utils.init_setup(prj_dir, swatmfwd, swatwd))
 
    Creating 'backup' folder ... passed
    Creating 'echo' folder ... passed
    Creating 'sufi2.in' folder ... passed
-   'beopest64.exe' file copied ... passed
-   'i64pest.exe' file copied ... passed
-   'i64pwtadj1.exe' file copied ... passed
+   'Absolute_SWAT_Values.txt' file copied ... passed
+   'pestpp-glm' file copied ... passed
+   'pestpp-ies.exe' file copied ... passed
+   'pestpp-ies.exe' file copied ... passed
    'forward_run.py' file copied ... passed
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `swatmf-0.3.0/swatmf.egg-info/SOURCES.txt` & `swatmf-1.0.0/swatmf.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.py
 swatmf/__init__.py
-swatmf/cvt_gcm_pcp.py
+swatmf/analyzer.py
 swatmf/forward_run.py
-swatmf/gcm_analysis.py
 swatmf/gumu_pst_utils.py
+swatmf/handler.py
+swatmf/objfns.py
+swatmf/pst_utils.py
 swatmf/swatmf_par_chg_run.py
 swatmf/swatmf_pst_par.py
 swatmf/swatmf_pst_stats.py
 swatmf/swatmf_pst_utils.py
 swatmf/swatmf_scenario_utils.py
 swatmf/swatmf_viz.py
 swatmf/utils.py
@@ -28,10 +30,14 @@
 swatmf/opt_files/Swat_Edit.exe
 swatmf/opt_files/i64pwtadj1.exe
 swatmf/opt_files/model.in
 swatmf/opt_files/pestpp-glm.exe
 swatmf/opt_files/pestpp-ies.exe
 swatmf/opt_files/pestpp-opt.exe
 swatmf/opt_files/pestpp-sen.exe
+swatmf/opt_files/swat_pars.db.csv
+swatmf/opt_files/swatmf_rel230922.exe
 swatmf/utils/__init__.py
 swatmf/utils/etc.py
+swatmf/utils/mf_configs.py
+swatmf/utils/swat_configs.py
 swatmf/utils/swat_utils.py
```

