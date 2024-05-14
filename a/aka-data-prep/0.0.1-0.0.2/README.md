# Comparing `tmp/aka-data-prep-0.0.1.tar.gz` & `tmp/aka-data-prep-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aka-data-prep-0.0.1.tar", last modified: Tue May 14 08:56:02 2024, max compression
+gzip compressed data, was "aka-data-prep-0.0.2.tar", last modified: Tue May 14 18:19:50 2024, max compression
```

## Comparing `aka-data-prep-0.0.1.tar` & `aka-data-prep-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 08:56:04.000000 aka-data-prep-0.0.1/
--rw-rw-rw-   0        0        0      190 2024-05-14 08:56:04.000000 aka-data-prep-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-12 11:48:58.000000 aka-data-prep-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 08:56:04.000000 aka-data-prep-0.0.1/aka_data_prep/
--rw-rw-rw-   0        0        0      107 2024-05-14 08:17:52.000000 aka-data-prep-0.0.1/aka_data_prep/__init__.py
--rw-rw-rw-   0        0        0    18729 2024-05-14 08:54:44.000000 aka-data-prep-0.0.1/aka_data_prep/aka_data_prep.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:56:04.000000 aka-data-prep-0.0.1/aka_data_prep.egg-info/
--rw-rw-rw-   0        0        0      190 2024-05-14 08:56:02.000000 aka-data-prep-0.0.1/aka_data_prep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-05-14 08:56:04.000000 aka-data-prep-0.0.1/aka_data_prep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 08:56:02.000000 aka-data-prep-0.0.1/aka_data_prep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-14 08:56:02.000000 aka-data-prep-0.0.1/aka_data_prep.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-14 08:56:02.000000 aka-data-prep-0.0.1/aka_data_prep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 08:56:04.000000 aka-data-prep-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      447 2024-05-14 08:55:36.000000 aka-data-prep-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:19:52.000000 aka-data-prep-0.0.2/
+-rw-rw-rw-   0        0        0      190 2024-05-14 18:19:52.000000 aka-data-prep-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-12 11:48:58.000000 aka-data-prep-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 18:19:52.000000 aka-data-prep-0.0.2/aka_data_prep/
+-rw-rw-rw-   0        0        0      107 2024-05-14 08:17:52.000000 aka-data-prep-0.0.2/aka_data_prep/__init__.py
+-rw-rw-rw-   0        0        0    18734 2024-05-14 18:03:42.000000 aka-data-prep-0.0.2/aka_data_prep/aka_data_prep.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:19:52.000000 aka-data-prep-0.0.2/aka_data_prep.egg-info/
+-rw-rw-rw-   0        0        0      190 2024-05-14 18:19:50.000000 aka-data-prep-0.0.2/aka_data_prep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-05-14 18:19:50.000000 aka-data-prep-0.0.2/aka_data_prep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 18:19:50.000000 aka-data-prep-0.0.2/aka_data_prep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-14 18:19:50.000000 aka-data-prep-0.0.2/aka_data_prep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-14 18:19:50.000000 aka-data-prep-0.0.2/aka_data_prep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 18:19:52.000000 aka-data-prep-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      447 2024-05-14 18:17:44.000000 aka-data-prep-0.0.2/setup.py
```

### Comparing `aka-data-prep-0.0.1/aka_data_prep/aka_data_prep.py` & `aka-data-prep-0.0.2/aka_data_prep/aka_data_prep.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,39 +296,40 @@
         return fig
 
 
     def plot_heatmap(self,df, lab=True):
       x_label = df.columns
       y_label = df.index
       if df.shape[1] > 0:
-        cm = df.select_dtypes(exclude=['object']).values.round(3)
+         cm = df.select_dtypes(exclude=['object']).values.round(3)
 
-        fig = go.Figure(data=go.Heatmap(
+         fig = go.Figure(data=go.Heatmap(
             z=cm,
             x=x_label,
             y=y_label,
             colorscale='Viridis', 
-            hoverongaps=False))
+            hoverongaps=False)
+            )
 
-        if lab:
+         if lab:
             for i in range(len(y_label)):
                 for j in range(len(x_label)):
                     fig.add_annotation(
                         x=x_label[j],
                         y=y_label[i],
                         text=str(cm[i, j]),
                         showarrow=False,
                         font=dict(color='black', size=12),
                         xanchor='center',
                         yanchor='middle'
                     )
-            fig.update_layout(**self.update_layout_parameter)
-            fig.update_xaxes(**self.update_axes)
-            fig.update_yaxes(**self.update_axes)
-            return fig
+         fig.update_layout(**self.update_layout_parameter)
+         fig.update_xaxes(**self.update_axes)
+         fig.update_yaxes(**self.update_axes)
+         return fig
       else:
             print("Empty list is provided.")
  
  
     def Plot_Correlation_Matrix(self, df, height=900,  width=1000):
         cm = df.corr()
```

