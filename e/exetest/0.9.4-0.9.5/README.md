# Comparing `tmp/exetest-0.9.4.tar.gz` & `tmp/exetest-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exetest-0.9.4.tar", last modified: Mon May 13 17:47:18 2024, max compression
+gzip compressed data, was "exetest-0.9.5.tar", last modified: Tue May 14 21:14:02 2024, max compression
```

## Comparing `exetest-0.9.4.tar` & `exetest-0.9.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 ggiraud   (1000) ggiraud   (1000)        0 2024-05-13 17:47:18.476570 exetest-0.9.4/
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)      699 2024-05-13 17:47:18.476570 exetest-0.9.4/PKG-INFO
-drwxr-xr-x   0 ggiraud   (1000) ggiraud   (1000)        0 2024-05-13 17:47:18.476570 exetest-0.9.4/exetest/
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)      183 2024-05-13 08:36:57.942206 exetest-0.9.4/exetest/__init__.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     6638 2024-05-13 17:44:47.646590 exetest-0.9.4/exetest/dataframe_utils.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     7914 2024-05-13 08:36:57.942206 exetest-0.9.4/exetest/diff_utils.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)      429 2024-05-13 08:36:57.942206 exetest-0.9.4/exetest/env_vars.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)    22270 2024-05-13 08:36:57.942206 exetest-0.9.4/exetest/exetest_decorator.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     1670 2024-05-13 08:36:57.942206 exetest-0.9.4/exetest/expects_exception.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     7196 2024-05-13 08:36:57.952206 exetest-0.9.4/exetest/misc_utils.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     6885 2024-05-13 08:36:57.952206 exetest-0.9.4/exetest/runmain.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)       62 2024-05-13 08:26:18.252304 exetest-0.9.4/setup.cfg
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     1539 2024-05-13 17:41:32.796642 exetest-0.9.4/setup.py
+drwxr-xr-x   0 ggiraud   (1000) ggiraud   (1000)        0 2024-05-14 21:14:02.566222 exetest-0.9.5/
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)      699 2024-05-14 21:14:02.566222 exetest-0.9.5/PKG-INFO
+drwxr-xr-x   0 ggiraud   (1000) ggiraud   (1000)        0 2024-05-14 21:14:02.566222 exetest-0.9.5/exetest/
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)      183 2024-05-13 08:36:57.942206 exetest-0.9.5/exetest/__init__.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     6537 2024-05-14 21:07:56.052500 exetest-0.9.5/exetest/dataframe_utils.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     7914 2024-05-13 08:36:57.942206 exetest-0.9.5/exetest/diff_utils.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)      429 2024-05-13 08:36:57.942206 exetest-0.9.5/exetest/env_vars.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)    22270 2024-05-13 08:36:57.942206 exetest-0.9.5/exetest/exetest_decorator.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     1670 2024-05-13 08:36:57.942206 exetest-0.9.5/exetest/expects_exception.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     7196 2024-05-13 08:36:57.952206 exetest-0.9.5/exetest/misc_utils.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     6885 2024-05-13 08:36:57.952206 exetest-0.9.5/exetest/runmain.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)       62 2024-05-13 08:26:18.252304 exetest-0.9.5/setup.cfg
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     1539 2024-05-14 21:07:55.672500 exetest-0.9.5/setup.py
```

### Comparing `exetest-0.9.4/PKG-INFO` & `exetest-0.9.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: exetest
-Version: 0.9.4
+Version: 0.9.5
 Summary: A pytest-based test framework for black-box approach to testing executables
 Home-page: https://github.com/Guillaume227/exetest
 Author: Guillaume227
 Author-email: guillaume227@gmail.com
 License: MIT
 Download-URL: https://github.com/Guillaume227/exetest/archive/v0.1-alpha.tar.gz
 Description: UNKNOWN
```

### Comparing `exetest-0.9.4/exetest/dataframe_utils.py` & `exetest-0.9.5/exetest/dataframe_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -121,39 +121,43 @@
 
                             df1_with_diff = df1[numerical_diff_cols]
                             df2_with_diff = df2[numerical_diff_cols]
                             diff_mask = ~(df1_with_diff - df2_with_diff).apply(
                                 functools.partial(is_close, b=0, **self.np_close_kwargs))
                             diff_mask = diff_mask.any(axis=1)
 
-                            masked_df1 = getattr(df1_with_diff.reset_index()[diff_mask], func_name)(abs(self.num_diffs_to_display))
-                            masked_df2 = getattr(df2_with_diff[diff_mask], func_name)(abs(self.num_diffs_to_display))
-
-                            print(f'{diff_mask.shape[0]} numerical diffs:')
-
-                            diff_df = pd.DataFrame(masked_df1['index'])
-                            for col_name in masked_df2:
-                                diff_df = pd.concat([diff_df, masked_df1[col_name], masked_df2[col_name]], axis=1)
-
-                            with pd.option_context("display.max_rows", abs(self.num_diffs_to_display)):
-                                print(diff_df)
+                            print_df_diff(df1_with_diff,
+                                          df2_with_diff,
+                                          diff_mask,
+                                          func_name=func_name,
+                                          num_diffs_to_display=self.num_diffs_to_display,
+                                          message='numerical')
 
                         if non_numerical_diff_cols:
                             df1_with_diff = df1[non_numerical_diff_cols]
                             df2_with_diff = df2[non_numerical_diff_cols]
                             diff_mask = (df1_with_diff != df2_with_diff).any(axis=1)
 
-                            masked_df1 = getattr(df1_with_diff.reset_index()[diff_mask], func_name)(abs(self.num_diffs_to_display))
-                            masked_df2 = getattr(df2_with_diff[diff_mask], func_name)(abs(self.num_diffs_to_display))
+                            print_df_diff(df1_with_diff,
+                                          df2_with_diff,
+                                          diff_mask,
+                                          func_name=func_name,
+                                          num_diffs_to_display=self.num_diffs_to_display,
+                                          message='non-numerical')
 
-                            print(f'{diff_mask.shape[0]} non numerical diffs:')
+                return False
 
-                            diff_df = pd.DataFrame(masked_df1['index'])
-                            for col_name in masked_df2:
-                                diff_df = pd.concat([diff_df, masked_df1[col_name], masked_df2[col_name]], axis=1)
+        return True
 
-                            with pd.option_context("display.max_rows", abs(self.num_diffs_to_display)):
-                                print(diff_df)
 
-                return False
+def print_df_diff(df1, df2, diff_mask, func_name, num_diffs_to_display, message):
+    masked_df1 = getattr(df1.reset_index()[diff_mask], func_name)(abs(num_diffs_to_display))
+    masked_df2 = getattr(df2[diff_mask], func_name)(abs(num_diffs_to_display))
+
+    print(f'{diff_mask.shape[0]} {message} diffs:')
+
+    diff_df = pd.DataFrame(masked_df1['index'])
+    for col_name in masked_df2:
+        diff_df = pd.concat([diff_df, masked_df1[col_name], masked_df2[col_name]], axis=1)
 
-        return True
+    with pd.option_context("display.max_rows", abs(num_diffs_to_display)):
+        print(diff_df)
```

### Comparing `exetest-0.9.4/exetest/diff_utils.py` & `exetest-0.9.5/exetest/diff_utils.py`

 * *Files identical despite different names*

### Comparing `exetest-0.9.4/exetest/exetest_decorator.py` & `exetest-0.9.5/exetest/exetest_decorator.py`

 * *Files identical despite different names*

### Comparing `exetest-0.9.4/exetest/expects_exception.py` & `exetest-0.9.5/exetest/expects_exception.py`

 * *Files identical despite different names*

### Comparing `exetest-0.9.4/exetest/misc_utils.py` & `exetest-0.9.5/exetest/misc_utils.py`

 * *Files identical despite different names*

### Comparing `exetest-0.9.4/exetest/runmain.py` & `exetest-0.9.5/exetest/runmain.py`

 * *Files identical despite different names*

### Comparing `exetest-0.9.4/setup.py` & `exetest-0.9.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name='exetest',         # How you named your package folder (MyLib)
   packages=['exetest'],   # Chose the same as "name"
-  version='0.9.4',      # Start with a small number and increase it with every change you make
+  version='0.9.5',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description='A pytest-based test framework for black-box approach to testing executables',   # Give a short description about your library
   author='Guillaume227',                   # Type in your name
   author_email='guillaume227@gmail.com',      # Type in your E-Mail
   url='https://github.com/Guillaume227/exetest',   # Provide either the link to your github or to your website
   download_url='https://github.com/Guillaume227/exetest/archive/v0.1-alpha.tar.gz',
   keywords=['test', 'pytest', 'nosetest'],  # Keywords that define your package best
```

