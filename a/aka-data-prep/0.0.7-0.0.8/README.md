# Comparing `tmp/aka-data-prep-0.0.7.tar.gz` & `tmp/aka-data-prep-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aka-data-prep-0.0.7.tar", last modified: Tue May 14 08:20:04 2024, max compression
+gzip compressed data, was "aka-data-prep-0.0.8.tar", last modified: Tue May 14 08:32:23 2024, max compression
```

## Comparing `aka-data-prep-0.0.7.tar` & `aka-data-prep-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 08:20:06.000000 aka-data-prep-0.0.7/
--rw-rw-rw-   0        0        0      190 2024-05-14 08:20:06.000000 aka-data-prep-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-12 11:48:58.000000 aka-data-prep-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 08:20:06.000000 aka-data-prep-0.0.7/aka_data_prep/
--rw-rw-rw-   0        0        0      107 2024-05-14 08:17:52.000000 aka-data-prep-0.0.7/aka_data_prep/__init__.py
--rw-rw-rw-   0        0        0    18735 2024-05-14 08:13:22.000000 aka-data-prep-0.0.7/aka_data_prep/aka_data_prep.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:20:06.000000 aka-data-prep-0.0.7/aka_data_prep.egg-info/
--rw-rw-rw-   0        0        0      190 2024-05-14 08:20:06.000000 aka-data-prep-0.0.7/aka_data_prep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-05-14 08:20:06.000000 aka-data-prep-0.0.7/aka_data_prep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 08:20:06.000000 aka-data-prep-0.0.7/aka_data_prep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-14 08:20:06.000000 aka-data-prep-0.0.7/aka_data_prep.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-14 08:20:06.000000 aka-data-prep-0.0.7/aka_data_prep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 08:20:06.000000 aka-data-prep-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      442 2024-05-14 08:19:24.000000 aka-data-prep-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:32:24.000000 aka-data-prep-0.0.8/
+-rw-rw-rw-   0        0        0      190 2024-05-14 08:32:24.000000 aka-data-prep-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-12 11:48:58.000000 aka-data-prep-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 08:32:24.000000 aka-data-prep-0.0.8/aka_data_prep/
+-rw-rw-rw-   0        0        0      107 2024-05-14 08:17:52.000000 aka-data-prep-0.0.8/aka_data_prep/__init__.py
+-rw-rw-rw-   0        0        0    18739 2024-05-14 08:27:24.000000 aka-data-prep-0.0.8/aka_data_prep/aka_data_prep.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:32:24.000000 aka-data-prep-0.0.8/aka_data_prep.egg-info/
+-rw-rw-rw-   0        0        0      190 2024-05-14 08:32:24.000000 aka-data-prep-0.0.8/aka_data_prep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-05-14 08:32:24.000000 aka-data-prep-0.0.8/aka_data_prep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 08:32:24.000000 aka-data-prep-0.0.8/aka_data_prep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-14 08:32:24.000000 aka-data-prep-0.0.8/aka_data_prep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-14 08:32:24.000000 aka-data-prep-0.0.8/aka_data_prep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 08:32:24.000000 aka-data-prep-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      431 2024-05-14 08:31:50.000000 aka-data-prep-0.0.8/setup.py
```

### Comparing `aka-data-prep-0.0.7/aka_data_prep/aka_data_prep.py` & `aka-data-prep-0.0.8/aka_data_prep/aka_data_prep.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,15 +295,15 @@
         fig.update_xaxes(**self.update_axes)
         return fig
 
 
     def plot_heatmap(self,df, lab=True):
       x_label = df.columns
       y_label = df.index
-      if len(len(x_label)) > 0:
+      if len(len(df.shape[1])) > 0:
         cm = df.select_dtypes(exclude=['object']).values.round(3)
 
         fig = go.Figure(data=go.Heatmap(
             z=cm,
             x=x_label,
             y=y_label,
             colorscale='Viridis',
```

