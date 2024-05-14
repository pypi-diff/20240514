# Comparing `tmp/python_project_stub-0.0.3.tar.gz` & `tmp/python_project_stub-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_project_stub-0.0.3.tar", last modified: Tue May 14 04:42:01 2024, max compression
+gzip compressed data, was "python_project_stub-0.0.4.tar", last modified: Tue May 14 18:22:14 2024, max compression
```

## Comparing `python_project_stub-0.0.3.tar` & `python_project_stub-0.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-14 04:42:01.398357 python_project_stub-0.0.3/
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     1544 2024-05-11 19:06:35.000000 python_project_stub-0.0.3/LICENSE
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       43 2024-05-14 04:41:30.000000 python_project_stub-0.0.3/MANIFEST.in
--rw-r--r--   0 jstrieb   (1012) jstrieb   (1012)    13335 2024-05-14 04:42:01.398357 python_project_stub-0.0.3/PKG-INFO
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)    12821 2024-05-13 19:42:57.000000 python_project_stub-0.0.3/README.md
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     1530 2024-05-14 04:41:51.000000 python_project_stub-0.0.3/pyproject.toml
-drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-14 04:42:01.398357 python_project_stub-0.0.3/python_project_stub/
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       82 2024-05-12 00:24:48.000000 python_project_stub-0.0.3/python_project_stub/__init__.py
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     1660 2024-05-14 02:38:17.000000 python_project_stub-0.0.3/python_project_stub/__main__.py
-drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-14 04:42:01.398357 python_project_stub-0.0.3/python_project_stub/data/
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-11 23:17:16.000000 python_project_stub-0.0.3/python_project_stub/data/__init__.py
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       82 2024-05-11 21:45:11.000000 python_project_stub-0.0.3/python_project_stub/data/quote.txt
-drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-14 04:42:01.398357 python_project_stub-0.0.3/python_project_stub.egg-info/
--rw-r--r--   0 jstrieb   (1012) jstrieb   (1012)    13335 2024-05-14 04:42:01.000000 python_project_stub-0.0.3/python_project_stub.egg-info/PKG-INFO
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)      959 2024-05-14 04:42:01.000000 python_project_stub-0.0.3/python_project_stub.egg-info/SOURCES.txt
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)        1 2024-05-14 04:42:01.000000 python_project_stub-0.0.3/python_project_stub.egg-info/dependency_links.txt
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       74 2024-05-14 04:42:01.000000 python_project_stub-0.0.3/python_project_stub.egg-info/entry_points.txt
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       41 2024-05-14 04:42:01.000000 python_project_stub-0.0.3/python_project_stub.egg-info/requires.txt
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       59 2024-05-14 04:42:01.000000 python_project_stub-0.0.3/python_project_stub.egg-info/top_level.txt
--rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)      161 2024-05-14 04:42:01.398357 python_project_stub-0.0.3/setup.cfg
-drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-14 04:42:01.398357 python_project_stub-0.0.3/venv-python-project-stub/
-drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-14 04:42:01.398357 python_project_stub-0.0.3/venv-python-project-stub/bin/
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      655 2024-05-12 21:27:02.000000 python_project_stub-0.0.3/venv-python-project-stub/bin/rst2html.py
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      777 2024-05-12 21:27:02.000000 python_project_stub-0.0.3/venv-python-project-stub/bin/rst2html4.py
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)     1112 2024-05-12 21:27:02.000000 python_project_stub-0.0.3/venv-python-project-stub/bin/rst2html5.py
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      854 2024-05-12 21:27:02.000000 python_project_stub-0.0.3/venv-python-project-stub/bin/rst2latex.py
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      677 2024-05-12 21:27:02.000000 python_project_stub-0.0.3/venv-python-project-stub/bin/rst2man.py
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      843 2024-05-12 21:27:02.000000 python_project_stub-0.0.3/venv-python-project-stub/bin/rst2odt.py
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      649 2024-05-12 21:27:02.000000 python_project_stub-0.0.3/venv-python-project-stub/bin/rst2odt_prepstyles.py
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      662 2024-05-12 21:27:02.000000 python_project_stub-0.0.3/venv-python-project-stub/bin/rst2pseudoxml.py
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      698 2024-05-12 21:27:02.000000 python_project_stub-0.0.3/venv-python-project-stub/bin/rst2s5.py
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      934 2024-05-12 21:27:02.000000 python_project_stub-0.0.3/venv-python-project-stub/bin/rst2xetex.py
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      663 2024-05-12 21:27:02.000000 python_project_stub-0.0.3/venv-python-project-stub/bin/rst2xml.py
--rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      731 2024-05-12 21:27:02.000000 python_project_stub-0.0.3/venv-python-project-stub/bin/rstpep2html.py
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-14 18:22:14.446840 python_project_stub-0.0.4/
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     1544 2024-05-11 19:06:35.000000 python_project_stub-0.0.4/LICENSE
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       43 2024-05-14 04:41:30.000000 python_project_stub-0.0.4/MANIFEST.in
+-rw-r--r--   0 jstrieb   (1012) jstrieb   (1012)    16654 2024-05-14 18:22:14.446840 python_project_stub-0.0.4/PKG-INFO
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)    16140 2024-05-14 18:02:42.000000 python_project_stub-0.0.4/README.md
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     1530 2024-05-14 18:21:37.000000 python_project_stub-0.0.4/pyproject.toml
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-14 18:22:14.442840 python_project_stub-0.0.4/python_project_stub/
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       82 2024-05-12 00:24:48.000000 python_project_stub-0.0.4/python_project_stub/__init__.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     1660 2024-05-14 02:38:17.000000 python_project_stub-0.0.4/python_project_stub/__main__.py
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-14 18:22:14.446840 python_project_stub-0.0.4/python_project_stub/data/
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-11 23:17:16.000000 python_project_stub-0.0.4/python_project_stub/data/__init__.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       82 2024-05-11 21:45:11.000000 python_project_stub-0.0.4/python_project_stub/data/quote.txt
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-14 18:22:14.446840 python_project_stub-0.0.4/python_project_stub.egg-info/
+-rw-r--r--   0 jstrieb   (1012) jstrieb   (1012)    16654 2024-05-14 18:22:14.000000 python_project_stub-0.0.4/python_project_stub.egg-info/PKG-INFO
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)      959 2024-05-14 18:22:14.000000 python_project_stub-0.0.4/python_project_stub.egg-info/SOURCES.txt
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)        1 2024-05-14 18:22:14.000000 python_project_stub-0.0.4/python_project_stub.egg-info/dependency_links.txt
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       74 2024-05-14 18:22:14.000000 python_project_stub-0.0.4/python_project_stub.egg-info/entry_points.txt
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       41 2024-05-14 18:22:14.000000 python_project_stub-0.0.4/python_project_stub.egg-info/requires.txt
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       59 2024-05-14 18:22:14.000000 python_project_stub-0.0.4/python_project_stub.egg-info/top_level.txt
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)      161 2024-05-14 18:22:14.446840 python_project_stub-0.0.4/setup.cfg
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-14 18:22:14.442840 python_project_stub-0.0.4/venv-python-project-stub/
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-14 18:22:14.446840 python_project_stub-0.0.4/venv-python-project-stub/bin/
+-rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      655 2024-05-12 21:27:02.000000 python_project_stub-0.0.4/venv-python-project-stub/bin/rst2html.py
+-rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      777 2024-05-12 21:27:02.000000 python_project_stub-0.0.4/venv-python-project-stub/bin/rst2html4.py
+-rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)     1112 2024-05-12 21:27:02.000000 python_project_stub-0.0.4/venv-python-project-stub/bin/rst2html5.py
+-rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      854 2024-05-12 21:27:02.000000 python_project_stub-0.0.4/venv-python-project-stub/bin/rst2latex.py
+-rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      677 2024-05-12 21:27:02.000000 python_project_stub-0.0.4/venv-python-project-stub/bin/rst2man.py
+-rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      843 2024-05-12 21:27:02.000000 python_project_stub-0.0.4/venv-python-project-stub/bin/rst2odt.py
+-rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      649 2024-05-12 21:27:02.000000 python_project_stub-0.0.4/venv-python-project-stub/bin/rst2odt_prepstyles.py
+-rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      662 2024-05-12 21:27:02.000000 python_project_stub-0.0.4/venv-python-project-stub/bin/rst2pseudoxml.py
+-rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      698 2024-05-12 21:27:02.000000 python_project_stub-0.0.4/venv-python-project-stub/bin/rst2s5.py
+-rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      934 2024-05-12 21:27:02.000000 python_project_stub-0.0.4/venv-python-project-stub/bin/rst2xetex.py
+-rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      663 2024-05-12 21:27:02.000000 python_project_stub-0.0.4/venv-python-project-stub/bin/rst2xml.py
+-rwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)      731 2024-05-12 21:27:02.000000 python_project_stub-0.0.4/venv-python-project-stub/bin/rstpep2html.py
```

### Comparing `python_project_stub-0.0.3/LICENSE` & `python_project_stub-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_project_stub-0.0.3/pyproject.toml` & `python_project_stub-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["setuptools>=61.0"]
     build-backend = "setuptools.build_meta"
 
 [project]
     name = "python-project-stub"
-    version = "0.0.3"
+    version = "0.0.4"
     dynamic = ["authors"] # specified in setup.cfg
     
     # The value of the "description" field will be displayed:
     #     * In a banner at the top of "pypi.org/project/python-project-stub".
     #     * As the value of the "Summary" field when "pip show python-project-stub"
     #           is executed.
     #
```

### Comparing `python_project_stub-0.0.3/python_project_stub/__main__.py` & `python_project_stub-0.0.4/python_project_stub/__main__.py`

 * *Files identical despite different names*

### Comparing `python_project_stub-0.0.3/python_project_stub.egg-info/SOURCES.txt` & `python_project_stub-0.0.4/python_project_stub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_project_stub-0.0.3/venv-python-project-stub/bin/rst2html.py` & `python_project_stub-0.0.4/venv-python-project-stub/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `python_project_stub-0.0.3/venv-python-project-stub/bin/rst2html4.py` & `python_project_stub-0.0.4/venv-python-project-stub/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `python_project_stub-0.0.3/venv-python-project-stub/bin/rst2html5.py` & `python_project_stub-0.0.4/venv-python-project-stub/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `python_project_stub-0.0.3/venv-python-project-stub/bin/rst2latex.py` & `python_project_stub-0.0.4/venv-python-project-stub/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `python_project_stub-0.0.3/venv-python-project-stub/bin/rst2man.py` & `python_project_stub-0.0.4/venv-python-project-stub/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `python_project_stub-0.0.3/venv-python-project-stub/bin/rst2odt.py` & `python_project_stub-0.0.4/venv-python-project-stub/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `python_project_stub-0.0.3/venv-python-project-stub/bin/rst2odt_prepstyles.py` & `python_project_stub-0.0.4/venv-python-project-stub/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `python_project_stub-0.0.3/venv-python-project-stub/bin/rst2pseudoxml.py` & `python_project_stub-0.0.4/venv-python-project-stub/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `python_project_stub-0.0.3/venv-python-project-stub/bin/rst2s5.py` & `python_project_stub-0.0.4/venv-python-project-stub/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `python_project_stub-0.0.3/venv-python-project-stub/bin/rst2xetex.py` & `python_project_stub-0.0.4/venv-python-project-stub/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `python_project_stub-0.0.3/venv-python-project-stub/bin/rst2xml.py` & `python_project_stub-0.0.4/venv-python-project-stub/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `python_project_stub-0.0.3/venv-python-project-stub/bin/rstpep2html.py` & `python_project_stub-0.0.4/venv-python-project-stub/bin/rstpep2html.py`

 * *Files identical despite different names*

