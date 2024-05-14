# Comparing `tmp/aka_data_prep-0.0.3.tar.gz` & `tmp/aka-data-prep-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aka_data_prep-0.0.3.tar", last modified: Sun May 12 23:05:51 2024, max compression
+gzip compressed data, was "aka-data-prep-0.0.4.tar", last modified: Tue May 14 01:46:26 2024, max compression
```

## Comparing `aka_data_prep-0.0.3.tar` & `aka-data-prep-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 23:05:52.000000 aka_data_prep-0.0.3/
--rw-rw-rw-   0        0        0      190 2024-05-12 23:05:52.000000 aka_data_prep-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-12 11:48:58.000000 aka_data_prep-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 23:05:52.000000 aka_data_prep-0.0.3/aka_data_prep/
--rw-rw-rw-   0        0        0       93 2024-05-12 22:14:14.000000 aka_data_prep-0.0.3/aka_data_prep/__init__.py
--rw-rw-rw-   0        0        0    15276 2024-05-12 23:04:56.000000 aka_data_prep-0.0.3/aka_data_prep/aka_data_prep.py
-drwxrwxrwx   0        0        0        0 2024-05-12 23:05:52.000000 aka_data_prep-0.0.3/aka_data_prep.egg-info/
--rw-rw-rw-   0        0        0      190 2024-05-12 23:05:52.000000 aka_data_prep-0.0.3/aka_data_prep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-05-12 23:05:52.000000 aka_data_prep-0.0.3/aka_data_prep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 23:05:52.000000 aka_data_prep-0.0.3/aka_data_prep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-12 23:05:52.000000 aka_data_prep-0.0.3/aka_data_prep.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-12 23:05:52.000000 aka_data_prep-0.0.3/aka_data_prep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 23:05:52.000000 aka_data_prep-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      425 2024-05-12 23:03:34.000000 aka_data_prep-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 01:46:28.000000 aka-data-prep-0.0.4/
+-rw-rw-rw-   0        0        0      190 2024-05-14 01:46:28.000000 aka-data-prep-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-12 11:48:58.000000 aka-data-prep-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 01:46:28.000000 aka-data-prep-0.0.4/aka_data_prep/
+-rw-rw-rw-   0        0        0       93 2024-05-12 22:14:14.000000 aka-data-prep-0.0.4/aka_data_prep/__init__.py
+-rw-rw-rw-   0        0        0    16045 2024-05-14 01:43:50.000000 aka-data-prep-0.0.4/aka_data_prep/aka_data_prep.py
+drwxrwxrwx   0        0        0        0 2024-05-14 01:46:28.000000 aka-data-prep-0.0.4/aka_data_prep.egg-info/
+-rw-rw-rw-   0        0        0      190 2024-05-14 01:46:28.000000 aka-data-prep-0.0.4/aka_data_prep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-05-14 01:46:28.000000 aka-data-prep-0.0.4/aka_data_prep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 01:46:28.000000 aka-data-prep-0.0.4/aka_data_prep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-14 01:46:28.000000 aka-data-prep-0.0.4/aka_data_prep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-14 01:46:28.000000 aka-data-prep-0.0.4/aka_data_prep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 01:46:28.000000 aka-data-prep-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      425 2024-05-14 01:46:02.000000 aka-data-prep-0.0.4/setup.py
```

### Comparing `aka_data_prep-0.0.3/aka_data_prep/aka_data_prep.py` & `aka-data-prep-0.0.4/aka_data_prep/aka_data_prep.py`

 * *Files 3% similar despite different names*

```diff
@@ -170,15 +170,15 @@
    
 
 class aka_plot :
 
     def __init__(self, tcouleur='plotly_dark', bcouleur='navy', fcouleur='white', fsize=20):
         self.tcouleur = tcouleur
         self.bcouleur = bcouleur
-        self.fcouleur = fcouleur
+        self.fcouleur = fcouleur 
         self.fsize = fsize 
         self.update_layout_parameter = dict(        
                                         barmode='overlay',  
                                         font=dict(color=fcouleur,size=fsize),  
                                         title_x=0.5,
                                         title_y=0.9,
                                         template=self.tcouleur
@@ -281,32 +281,58 @@
             )
             return fig
         else:
             print("Empty list is provided.")
 
 
 
-    def plot_missing_values(self, df):  
-        data = df.values.tolist()
-        feature_names = [mn for mn in df.columns]  
-                
-        layout = go.Layout( 
-            xaxis=dict(title='Features', tickvals=list(range(len(feature_names))), ticktext=feature_names),
-            yaxis=dict(title='Samples')
-        )
+ 
+    def plot_box(self,df,index_col_box = [0,10]): 
+        df_description = pd.DataFrame(df.describe())
+        for i in range(2):
+            if index_col_box[i]<0:
+                index_col_box[i] += df_description.shape[1]+1 
 
-        # Create the heatmap
-        fig = go.Figure(data=go.Heatmap(z=data, colorscale='viridis'), layout=layout)
-        fig.update_layout(title='Missing Values Heatmap')
+        fig = px.box(df, y=df_description.T['max'].sort_values()[max(0,index_col_box[0]-1):min(index_col_box[1],df_description.shape[1])].index) 
         fig.update_layout(**self.update_layout_parameter) 
         fig.update_xaxes(**self.update_axes)
-        fig.update_yaxes(**self.update_axes) 
-
         return fig
 
+
+    def plot_heatmap(self,df, lab=True):
+      x_label = df.columns
+      y_label = df.index
+
+      cm = df.select_dtypes(exclude=['object']).values.round(3)
+
+      fig = go.Figure(data=go.Heatmap(
+          z=cm,
+          x=x_label,
+          y=y_label,
+          colorscale='Viridis', 
+          hoverongaps=False))
+
+      if lab:
+          for i in range(len(y_label)):
+              for j in range(len(x_label)):
+                  fig.add_annotation(
+                      x=x_label[j],
+                      y=y_label[i],
+                      text=str(cm[i, j]),
+                      showarrow=False,
+                      font=dict(color='black', size=12),
+                      xanchor='center',
+                      yanchor='middle'
+                  )
+      fig.update_layout(**self.update_layout_parameter)
+      fig.update_xaxes(**self.update_axes)
+      fig.update_yaxes(**self.update_axes)
+
+      return fig
+
  
     def Plot_Correlation_Matrix(self, df, height=900,  width=1000):
         cm = df.corr()
 
         fig = px.imshow(cm, labels=dict(color="Correlation"), x=cm.columns, y=cm.index)
 
         fig.update_layout(**self.update_layout_parameter)
@@ -314,15 +340,15 @@
         fig.update_layout(
             height=height,
             width=width
         )
         return fig
 
 
-    def Plot_Correlate_Features(self,df,corr_tmp, fig_size_row=375, fig_size_col=475, subplot_col=3):
+    def Plot_scatter(self,df,corr_tmp, fig_size_row=375, fig_size_col=475, subplot_col=3):
 
         if len(corr_tmp) > 0:
             nrow = math.ceil(len(corr_tmp)/subplot_col)
             # Create subplots
             fig = make_subplots(
                 rows=nrow, cols=subplot_col,
                 subplot_titles=[""] * len(corr_tmp))
```

