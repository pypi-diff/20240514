# Comparing `tmp/dansplotcore-6.2.2.tar.gz` & `tmp/dansplotcore-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dansplotcore-6.2.2.tar", last modified: Mon Apr 15 18:41:57 2024, max compression
+gzip compressed data, was "dansplotcore-6.3.0.tar", last modified: Mon May 13 23:47:15 2024, max compression
```

## Comparing `dansplotcore-6.2.2.tar` & `dansplotcore-6.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-15 18:41:57.052505 dansplotcore-6.2.2/
--rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-15 18:41:57.052505 dansplotcore-6.2.2/PKG-INFO
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-15 18:41:57.052505 dansplotcore-6.2.2/dansplotcore/
--rw-rw-r--   0 dan       (1001) dan       (1001)      158 2024-03-11 15:41:59.000000 dansplotcore-6.2.2/dansplotcore/__init__.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     4953 2023-04-05 20:25:28.000000 dansplotcore-6.2.2/dansplotcore/media.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     9689 2024-04-15 18:40:11.000000 dansplotcore-6.2.2/dansplotcore/plot.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2645 2024-03-11 16:06:00.000000 dansplotcore-6.2.2/dansplotcore/primitives.py
--rw-rw-r--   0 dan       (1001) dan       (1001)      479 2024-03-11 16:06:00.000000 dansplotcore-6.2.2/dansplotcore/process.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     9334 2024-04-02 20:13:35.000000 dansplotcore-6.2.2/dansplotcore/show.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2907 2024-03-21 21:31:30.000000 dansplotcore-6.2.2/dansplotcore/transforms.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     7455 2024-04-02 20:00:09.000000 dansplotcore-6.2.2/dansplotcore/vector_text.py
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-15 18:41:57.052505 dansplotcore-6.2.2/dansplotcore.egg-info/
--rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-15 18:41:57.000000 dansplotcore-6.2.2/dansplotcore.egg-info/PKG-INFO
--rw-rw-r--   0 dan       (1001) dan       (1001)      382 2024-04-15 18:41:57.000000 dansplotcore-6.2.2/dansplotcore.egg-info/SOURCES.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)        1 2024-04-15 18:41:57.000000 dansplotcore-6.2.2/dansplotcore.egg-info/dependency_links.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       15 2024-04-15 18:41:57.000000 dansplotcore-6.2.2/dansplotcore.egg-info/requires.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       13 2024-04-15 18:41:57.000000 dansplotcore-6.2.2/dansplotcore.egg-info/top_level.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       38 2024-04-15 18:41:57.052505 dansplotcore-6.2.2/setup.cfg
--rw-rw-r--   0 dan       (1001) dan       (1001)      492 2024-04-15 18:41:30.000000 dansplotcore-6.2.2/setup.py
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-13 23:47:15.649371 dansplotcore-6.3.0/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-05-13 23:47:15.649371 dansplotcore-6.3.0/PKG-INFO
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-13 23:47:15.649371 dansplotcore-6.3.0/dansplotcore/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      158 2024-03-11 15:41:59.000000 dansplotcore-6.3.0/dansplotcore/__init__.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     4953 2023-04-05 20:25:28.000000 dansplotcore-6.3.0/dansplotcore/media.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     9713 2024-05-13 23:40:36.000000 dansplotcore-6.3.0/dansplotcore/plot.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     2645 2024-03-11 16:06:00.000000 dansplotcore-6.3.0/dansplotcore/primitives.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)      479 2024-03-11 16:06:00.000000 dansplotcore-6.3.0/dansplotcore/process.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     9612 2024-05-13 23:31:06.000000 dansplotcore-6.3.0/dansplotcore/show.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     2907 2024-03-21 21:31:30.000000 dansplotcore-6.3.0/dansplotcore/transforms.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     7455 2024-04-02 20:00:09.000000 dansplotcore-6.3.0/dansplotcore/vector_text.py
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-05-13 23:47:15.649371 dansplotcore-6.3.0/dansplotcore.egg-info/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-05-13 23:47:15.000000 dansplotcore-6.3.0/dansplotcore.egg-info/PKG-INFO
+-rw-rw-r--   0 dan       (1001) dan       (1001)      382 2024-05-13 23:47:15.000000 dansplotcore-6.3.0/dansplotcore.egg-info/SOURCES.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)        1 2024-05-13 23:47:15.000000 dansplotcore-6.3.0/dansplotcore.egg-info/dependency_links.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       15 2024-05-13 23:47:15.000000 dansplotcore-6.3.0/dansplotcore.egg-info/requires.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       13 2024-05-13 23:47:15.000000 dansplotcore-6.3.0/dansplotcore.egg-info/top_level.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       38 2024-05-13 23:47:15.649371 dansplotcore-6.3.0/setup.cfg
+-rw-rw-r--   0 dan       (1001) dan       (1001)      492 2024-05-13 23:45:54.000000 dansplotcore-6.3.0/setup.py
```

### Comparing `dansplotcore-6.2.2/dansplotcore/media.py` & `dansplotcore-6.3.0/dansplotcore/media.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.2.2/dansplotcore/plot.py` & `dansplotcore-6.3.0/dansplotcore/plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 class Plot:
     def __init__(
         self,
         title='plot',
         *,
         transform=None,
         hide_axes=False,
+        x_axis_transform=None,
+        y_axis_transform=None,
         primitive=None,
         datetime_unit=1,
         legend_displacement=(0, -1),
         legend_offset=(0, -1),
     ):
         self.title = title
         self.points = []
@@ -28,14 +30,16 @@
         self.x_max = -math.inf
         self.y_min =  math.inf
         self.y_max = -math.inf
         self.epochs = {}
         self.series = 0
         self.transform = transform or transforms.Default()
         self.hide_axes = hide_axes
+        self.x_axis_transform = x_axis_transform
+        self.y_axis_transform = y_axis_transform
         self.set_primitive(primitive or primitives.Point())
         self.datetime_unit = datetime_unit
         self.legend_displacement = legend_displacement
         self.legend_offset = legend_offset
 
     def point(self, x, y, r=255, g=255, b=255, a=255):
         self.points.append([x, y, r, g, b, a])
@@ -103,15 +107,18 @@
     def plot_dicts(self, ds, **kwargs):
         for d in ds: self.plot_dict(d, **kwargs)
 
     def plot_f(self, f, x=(-1, 1), steps=100, **kwargs):
         args_prev = None
         for i in range(steps):
             x_curr = x[0] + (x[1]-x[0]) * i/(steps-1)
-            y_curr = f(x_curr)
+            try:
+                y_curr = f(x_curr)
+            except Exception as e:
+                continue
             self.primitive(**self.transform(x_curr, y_curr, i, self.series))
         self._plot_common(**kwargs)
 
     def plot_2d(self, array, *, x_increment=1, y_increment=1, **kwargs):
         z_min = math.inf
         z_max = -math.inf
         for row in array:
@@ -209,15 +216,14 @@
             self.y_min = min(y, self.y_min)
             self.y_max = max(y, self.y_max)
 
     def _plot_common(
         self,
         next_series=True,
         legend=None,
-        **kwargs,
     ):
         if legend:
             kwargs = self.transform(0, 0, 0, self.series)
             if hasattr(self.transform, 'series_insignificant'):
                 series = self.transform.series_insignificant(self.series)
             else:
                 series = self.series
@@ -229,28 +235,16 @@
 
     def _increment(self, x, amount=1):
         if type(x) == datetime.datetime:
             return x + datetime.timedelta(seconds=self.datetime_unit) * amount
         else:
             return x + amount
 
-def plot(
-    *args,
-    title='plot',
-    transform=None,
-    hide_axes=False,
-    primitive=None,
-    **kwargs,
-):
-    Plot(
-        title,
-        transform=transform,
-        hide_axes=hide_axes,
-        primitive=primitive,
-    ).plot(*args, **kwargs).show()
+def plot(*args, **kwargs):
+    Plot(**kwargs).plot(*args).show()
 
 def _type_r(v, max_depth=None, _depth=0):
     if type(v).__name__ in ['int', 'float', 'float64']: return 'number'
     if max_depth != None and _depth == max_depth:
         return str(type(v))
     try:
         v[0]
```

### Comparing `dansplotcore-6.2.2/dansplotcore/primitives.py` & `dansplotcore-6.3.0/dansplotcore/primitives.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.2.2/dansplotcore/show.py` & `dansplotcore-6.3.0/dansplotcore/show.py`

 * *Files 5% similar despite different names*

```diff
@@ -205,15 +205,19 @@
             increment = 10 ** math.floor(math.log10(view.w))
             if view.w / increment < 2:
                 increment /= 5
             elif view.w / increment < 5:
                 increment /= 2
             i = view.x // increment * increment + increment
             while i < view.x + view.w:
-                s = '{:.5}'.format(i)
+                if plot.x_axis_transform:
+                    t = plot.x_axis_transform(i)
+                else:
+                    t = i
+                s = '{:.5}'.format(t)
                 if view.x + view.w - i > increment:
                     if i == 0 and plot.epochs.get('x') != None:
                         texter.text(
                             plot.epochs['x']['min'].isoformat('\n'),
                             x=i + margin_x,
                             y=view.y + margin_y + 1.33 * text_h,
                             w=text_w * 0.66,
@@ -227,15 +231,19 @@
             increment = 10 ** math.floor(math.log10(view.h))
             if view.h / increment < 2:
                 increment /= 5
             elif view.h / increment < 5:
                 increment /= 2
             i = (view.y + text_h + 2*margin_y) // increment * increment + increment
             while i < view.y + view.h - (text_h + 2*margin_y):
-                s = '{:.5}'.format(i)
+                if plot.y_axis_transform:
+                    t = plot.y_axis_transform(i)
+                else:
+                    t = i
+                s = '{:.5}'.format(t)
                 if i == 0 and plot.epochs.get('y') != None:
                     texter.text(
                         plot.epochs['y']['min'].isoformat('\n'),
                         x=view.x + margin_x,
                         y=i + margin_y + 1.33 * text_h,
                         w=text_w * 0.66,
                         h=text_h * 0.66,
```

### Comparing `dansplotcore-6.2.2/dansplotcore/transforms.py` & `dansplotcore-6.3.0/dansplotcore/transforms.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.2.2/dansplotcore/vector_text.py` & `dansplotcore-6.3.0/dansplotcore/vector_text.py`

 * *Files identical despite different names*

