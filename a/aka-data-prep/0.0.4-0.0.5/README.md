# Comparing `tmp/aka-data-prep-0.0.4.tar.gz` & `tmp/aka-data-prep-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aka-data-prep-0.0.4.tar", last modified: Tue May 14 01:46:26 2024, max compression
+gzip compressed data, was "aka-data-prep-0.0.5.tar", last modified: Tue May 14 07:54:50 2024, max compression
```

## Comparing `aka-data-prep-0.0.4.tar` & `aka-data-prep-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 01:46:28.000000 aka-data-prep-0.0.4/
--rw-rw-rw-   0        0        0      190 2024-05-14 01:46:28.000000 aka-data-prep-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-12 11:48:58.000000 aka-data-prep-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 01:46:28.000000 aka-data-prep-0.0.4/aka_data_prep/
--rw-rw-rw-   0        0        0       93 2024-05-12 22:14:14.000000 aka-data-prep-0.0.4/aka_data_prep/__init__.py
--rw-rw-rw-   0        0        0    16045 2024-05-14 01:43:50.000000 aka-data-prep-0.0.4/aka_data_prep/aka_data_prep.py
-drwxrwxrwx   0        0        0        0 2024-05-14 01:46:28.000000 aka-data-prep-0.0.4/aka_data_prep.egg-info/
--rw-rw-rw-   0        0        0      190 2024-05-14 01:46:28.000000 aka-data-prep-0.0.4/aka_data_prep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-05-14 01:46:28.000000 aka-data-prep-0.0.4/aka_data_prep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 01:46:28.000000 aka-data-prep-0.0.4/aka_data_prep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-14 01:46:28.000000 aka-data-prep-0.0.4/aka_data_prep.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-14 01:46:28.000000 aka-data-prep-0.0.4/aka_data_prep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 01:46:28.000000 aka-data-prep-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      425 2024-05-14 01:46:02.000000 aka-data-prep-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 07:54:52.000000 aka-data-prep-0.0.5/
+-rw-rw-rw-   0        0        0      190 2024-05-14 07:54:52.000000 aka-data-prep-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-12 11:48:58.000000 aka-data-prep-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 07:54:52.000000 aka-data-prep-0.0.5/aka_data_prep/
+-rw-rw-rw-   0        0        0       93 2024-05-12 22:14:14.000000 aka-data-prep-0.0.5/aka_data_prep/__init__.py
+-rw-rw-rw-   0        0        0    18724 2024-05-14 07:53:34.000000 aka-data-prep-0.0.5/aka_data_prep/aka_data_prep.py
+drwxrwxrwx   0        0        0        0 2024-05-14 07:54:52.000000 aka-data-prep-0.0.5/aka_data_prep.egg-info/
+-rw-rw-rw-   0        0        0      190 2024-05-14 07:54:52.000000 aka-data-prep-0.0.5/aka_data_prep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-05-14 07:54:52.000000 aka-data-prep-0.0.5/aka_data_prep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 07:54:52.000000 aka-data-prep-0.0.5/aka_data_prep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-14 07:54:52.000000 aka-data-prep-0.0.5/aka_data_prep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-14 07:54:52.000000 aka-data-prep-0.0.5/aka_data_prep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 07:54:52.000000 aka-data-prep-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      425 2024-05-14 07:46:36.000000 aka-data-prep-0.0.5/setup.py
```

### Comparing `aka-data-prep-0.0.4/aka_data_prep/aka_data_prep.py` & `aka-data-prep-0.0.5/aka_data_prep/aka_data_prep.py`

 * *Files 5% similar despite different names*

```diff
@@ -204,22 +204,22 @@
     def plot_history_all(self,df):
         fig  = px.histogram(data_frame= df,opacity= .7).update_xaxes(categoryorder='total descending')
         fig.update_layout(**self.update_layout_parameter) 
         fig.update_xaxes(**self.update_axes)
         return fig
 
 
-    def Plot_histogram_Features(self, df, col_tmp, fig_size_row=375, fig_size_col=475, subplot_col=3):
-        if len(col_tmp) > 0:
-            nrow = math.ceil(len(col_tmp) / subplot_col)
+    def Plot_histogram_Features(self, df, columns_to_treat, fig_size_row=390, fig_size_col=490, subplot_col=3):
+        if len(columns_to_treat) > 0:
+            nrow = math.ceil(len(columns_to_treat) / subplot_col)
             
             # Create subplots
-            fig = make_subplots(rows=nrow, cols=subplot_col, subplot_titles=df.columns[col_tmp])
+            fig = make_subplots(rows=nrow, cols=subplot_col, subplot_titles=df.columns[columns_to_treat])
 
-            for i, col_index in enumerate(col_tmp):
+            for i, col_index in enumerate(columns_to_treat):
                 row_num = 1 + i // subplot_col
                 col_num = 1 + i % subplot_col
  
                 # Plot histogram for the current column
                 hist_trace = go.Histogram(x=df[df.columns[col_index]] )
 
                 hist_trace['showlegend'] = False
@@ -245,15 +245,15 @@
         fig = px.pie(df[df.columns[col]], names=df[df.columns[col]].value_counts().index, values=df[df.columns[col]].value_counts().values, 
              title=f'Pie Chart of {df.columns[col]}') 
         fig.update_layout(**self.update_layout_parameter) 
         fig.update_xaxes(**self.update_axes)
         return fig
 
         
-    def Plot_box_Features(self,df,df_filtered,fig_size_row=375,fig_size_col=475,subplot_col=3,corr_tmp=[]):
+    def Plot_box_2_Features(self,df,df_filtered,corr_tmp=[],fig_size_row=390,fig_size_col=490,subplot_col=3):
 
         if len(corr_tmp) > 0:
             nrow = math.ceil(len(corr_tmp)/subplot_col)
             # Create subplots
             fig = make_subplots(
                 rows=nrow, cols=subplot_col,
                 subplot_titles=[df.columns[corr] for corr in corr_tmp])
@@ -279,60 +279,59 @@
                 height=fig_size_row * nrow,
                 width=fig_size_col * subplot_col     
             )
             return fig
         else:
             print("Empty list is provided.")
 
-
-
  
-    def plot_box(self,df,index_col_box = [0,10]): 
+    def plot_box(self,df,index_col_box = [0,-1]): 
         df_description = pd.DataFrame(df.describe())
         for i in range(2):
             if index_col_box[i]<0:
                 index_col_box[i] += df_description.shape[1]+1 
 
         fig = px.box(df, y=df_description.T['max'].sort_values()[max(0,index_col_box[0]-1):min(index_col_box[1],df_description.shape[1])].index) 
         fig.update_layout(**self.update_layout_parameter) 
         fig.update_xaxes(**self.update_axes)
         return fig
 
 
     def plot_heatmap(self,df, lab=True):
       x_label = df.columns
       y_label = df.index
+      if len(len(x_label)) > 0:
+        cm = df.select_dtypes(exclude=['object']).values.round(3)
 
-      cm = df.select_dtypes(exclude=['object']).values.round(3)
-
-      fig = go.Figure(data=go.Heatmap(
-          z=cm,
-          x=x_label,
-          y=y_label,
-          colorscale='Viridis', 
-          hoverongaps=False))
-
-      if lab:
-          for i in range(len(y_label)):
-              for j in range(len(x_label)):
-                  fig.add_annotation(
-                      x=x_label[j],
-                      y=y_label[i],
-                      text=str(cm[i, j]),
-                      showarrow=False,
-                      font=dict(color='black', size=12),
-                      xanchor='center',
-                      yanchor='middle'
-                  )
-      fig.update_layout(**self.update_layout_parameter)
-      fig.update_xaxes(**self.update_axes)
-      fig.update_yaxes(**self.update_axes)
-
-      return fig
-
+        fig = go.Figure(data=go.Heatmap(
+            z=cm,
+            x=x_label,
+            y=y_label,
+            colorscale='Viridis', 
+            hoverongaps=False))
+
+        if lab:
+            for i in range(len(y_label)):
+                for j in range(len(x_label)):
+                    fig.add_annotation(
+                        x=x_label[j],
+                        y=y_label[i],
+                        text=str(cm[i, j]),
+                        showarrow=False,
+                        font=dict(color='black', size=12),
+                        xanchor='center',
+                        yanchor='middle'
+                    )
+            fig.update_layout(**self.update_layout_parameter)
+            fig.update_xaxes(**self.update_axes)
+            fig.update_yaxes(**self.update_axes)
+            return fig
+      else:
+            print("Empty list is provided.")
+ 
  
     def Plot_Correlation_Matrix(self, df, height=900,  width=1000):
         cm = df.corr()
 
         fig = px.imshow(cm, labels=dict(color="Correlation"), x=cm.columns, y=cm.index)
 
         fig.update_layout(**self.update_layout_parameter)
@@ -340,15 +339,15 @@
         fig.update_layout(
             height=height,
             width=width
         )
         return fig
 
 
-    def Plot_scatter(self,df,corr_tmp, fig_size_row=375, fig_size_col=475, subplot_col=3):
+    def Plot_scatter(self,df,corr_tmp, fig_size_row=390, fig_size_col=490, subplot_col=3):
 
         if len(corr_tmp) > 0:
             nrow = math.ceil(len(corr_tmp)/subplot_col)
             # Create subplots
             fig = make_subplots(
                 rows=nrow, cols=subplot_col,
                 subplot_titles=[""] * len(corr_tmp))
@@ -373,14 +372,76 @@
                 width=fig_size_col * subplot_col           # Adjust the width as needed
             )
             return fig
         else:
             print("Empty list is provided.")
 
 
+class aka_plot_shap: 
+    def __init__(self, model, X_train, feat_names, tcouleur='plotly_dark', bcouleur='navy', fcouleur='white', fsize=20,height=700,
+            width=1000,):
+        self.tcouleur = tcouleur
+        self.bcouleur = bcouleur
+        self.fcouleur = fcouleur 
+        self.fsize = fsize 
+        self.height = height
+        self.width = width
+        self.update_layout_parameter = dict(        
+                                        barmode='overlay',  
+                                        font=dict(color=fcouleur, size=fsize),  
+                                        title_x=0.5,
+                                        title_y=0.9,
+                                        template=self.tcouleur,
+                                        # showlegend=False  # Remove legend
+                                        )
+        self.update_axes = dict(  
+                            title_font={"size": 14},
+                            title_standoff=25
+                            )
+     
+        self.feat_names = feat_names
+        explainer = shap.Explainer(model, X_train)
+        self.shap_values = explainer(X_train)
+
+
+    def plot_summary_shap(self):
+        fig = go.Figure()
+        shap_summary_vals = self.shap_values.values
+        shap_summary_data = self.shap_values.data
+
+        for feature_idx in np.abs(shap_summary_vals).mean(axis=0).argsort():
+            feature_name = self.feat_names[feature_idx]
+            sorted_shap_vals = shap_summary_vals[:, feature_idx]
+            sorted_shap_data = shap_summary_data[:, feature_idx]
+
+            fig.add_trace(go.Bar(
+                y=[feature_name] * len(sorted_shap_vals),
+                x=sorted_shap_vals,
+                orientation='h',
+                name=feature_name,
+                marker=dict(color=sorted_shap_data), 
+            ))
+
+        # Add horizontal color bar
+        # fig.update_layout(coloraxis=dict(colorscale='Viridis', colorbar=dict(title='SHAP Value'), showscale=True))
+        fig.update_layout(
+            # title='SHAP Summary Plot',
+            xaxis_title='SHAP Value',
+            yaxis_title='Feature',
+            barmode='relative',
+            height=self.height,
+            width=self.width,
+            margin=dict(l=150, r=20, t=50, b=50),
+        )
+        fig.update_layout(**self.update_layout_parameter) 
+        fig.update_xaxes(**self.update_axes)
+        
+        return fig
+
+
 class aka_cleaned_data:
     def __init__(self) -> None:
         pass 
  
     def train_test_cleaned_data(self,df,pre_proc=0): 
         transform = preprocessing.StandardScaler()
         try:
@@ -438,8 +499,8 @@
         else:
             randS = RandomUnderSampler(sampling_strategy="not minority") # String
             titleS = 'Over-sampling'
 
         dff[df.columns[:-1]],dff[df.columns[-1]] = randS.fit_resample(df[df.columns[:-1]],df[df.columns[-1]] )
  
         return dff
-    
+
```

