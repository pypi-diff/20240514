# Comparing `tmp/dppd_plotnine-0.2.5.tar.gz` & `tmp/dppd_plotnine-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dppd_plotnine-0.2.5.tar", last modified: Fri Apr 21 12:38:00 2023, max compression
+gzip compressed data, was "dppd_plotnine-0.2.6.tar", last modified: Tue May 14 12:26:55 2024, max compression
```

## Comparing `dppd_plotnine-0.2.5.tar` & `dppd_plotnine-0.2.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 finkernagel  (1001) zti       (2000)        0 2023-04-21 12:38:00.532075 dppd_plotnine-0.2.5/
--rw-r--r--   0 finkernagel  (1001) zti       (2000)       95 2023-04-21 12:34:54.000000 dppd_plotnine-0.2.5/AUTHORS.rst
--rw-r--r--   0 finkernagel  (1001) zti       (2000)     1086 2023-04-21 12:34:54.000000 dppd_plotnine-0.2.5/LICENSE.txt
--rw-r--r--   0 finkernagel  (1001) zti       (2000)     2105 2023-04-21 12:38:00.532075 dppd_plotnine-0.2.5/PKG-INFO
--rw-r--r--   0 finkernagel  (1001) zti       (2000)     1629 2023-04-21 12:34:54.000000 dppd_plotnine-0.2.5/README.md
--rw-r--r--   0 finkernagel  (1001) zti       (2000)     1435 2023-04-21 12:38:00.533075 dppd_plotnine-0.2.5/setup.cfg
--rw-r--r--   0 finkernagel  (1001) zti       (2000)      398 2023-04-21 12:36:22.000000 dppd_plotnine-0.2.5/setup.py
-drwxr-xr-x   0 finkernagel  (1001) zti       (2000)        0 2023-04-21 12:38:00.529075 dppd_plotnine-0.2.5/src/
-drwxr-xr-x   0 finkernagel  (1001) zti       (2000)        0 2023-04-21 12:38:00.530075 dppd_plotnine-0.2.5/src/dppd_plotnine/
--rw-r--r--   0 finkernagel  (1001) zti       (2000)      169 2023-04-21 12:36:43.000000 dppd_plotnine-0.2.5/src/dppd_plotnine/__init__.py
--rw-r--r--   0 finkernagel  (1001) zti       (2000)     6406 2023-04-21 12:35:55.000000 dppd_plotnine-0.2.5/src/dppd_plotnine/dppd_plotnine.py
-drwxr-xr-x   0 finkernagel  (1001) zti       (2000)        0 2023-04-21 12:38:00.532075 dppd_plotnine-0.2.5/src/dppd_plotnine/geoms/
--rw-r--r--   0 finkernagel  (1001) zti       (2000)       74 2023-04-21 12:34:54.000000 dppd_plotnine-0.2.5/src/dppd_plotnine/geoms/__init__.py
--rw-r--r--   0 finkernagel  (1001) zti       (2000)     3907 2023-04-21 12:34:54.000000 dppd_plotnine-0.2.5/src/dppd_plotnine/geoms/annotation_stripes_dppd.py
--rw-r--r--   0 finkernagel  (1001) zti       (2000)    13552 2023-04-21 12:35:55.000000 dppd_plotnine-0.2.5/src/dppd_plotnine/plotnine_extensions.py
-drwxr-xr-x   0 finkernagel  (1001) zti       (2000)        0 2023-04-21 12:38:00.531075 dppd_plotnine-0.2.5/src/dppd_plotnine.egg-info/
--rw-r--r--   0 finkernagel  (1001) zti       (2000)     2105 2023-04-21 12:37:59.000000 dppd_plotnine-0.2.5/src/dppd_plotnine.egg-info/PKG-INFO
--rw-r--r--   0 finkernagel  (1001) zti       (2000)      489 2023-04-21 12:38:00.000000 dppd_plotnine-0.2.5/src/dppd_plotnine.egg-info/SOURCES.txt
--rw-r--r--   0 finkernagel  (1001) zti       (2000)        1 2023-04-21 12:38:00.000000 dppd_plotnine-0.2.5/src/dppd_plotnine.egg-info/dependency_links.txt
--rw-r--r--   0 finkernagel  (1001) zti       (2000)        1 2023-04-21 12:37:59.000000 dppd_plotnine-0.2.5/src/dppd_plotnine.egg-info/not-zip-safe
--rw-r--r--   0 finkernagel  (1001) zti       (2000)      118 2023-04-21 12:38:00.000000 dppd_plotnine-0.2.5/src/dppd_plotnine.egg-info/requires.txt
--rw-r--r--   0 finkernagel  (1001) zti       (2000)       14 2023-04-21 12:38:00.000000 dppd_plotnine-0.2.5/src/dppd_plotnine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:26:55.718305 dppd_plotnine-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-14 12:26:54.000000 dppd_plotnine-0.2.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-14 12:26:54.000000 dppd_plotnine-0.2.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-14 12:26:55.718305 dppd_plotnine-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-14 12:26:54.000000 dppd_plotnine-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-14 12:26:55.718305 dppd_plotnine-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-14 12:26:54.000000 dppd_plotnine-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:26:55.714305 dppd_plotnine-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:26:55.718305 dppd_plotnine-0.2.6/src/dppd_plotnine/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-14 12:26:54.000000 dppd_plotnine-0.2.6/src/dppd_plotnine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-14 12:26:54.000000 dppd_plotnine-0.2.6/src/dppd_plotnine/dppd_plotnine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:26:55.718305 dppd_plotnine-0.2.6/src/dppd_plotnine/geoms/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-14 12:26:54.000000 dppd_plotnine-0.2.6/src/dppd_plotnine/geoms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-14 12:26:54.000000 dppd_plotnine-0.2.6/src/dppd_plotnine/geoms/annotation_stripes_dppd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14018 2024-05-14 12:26:54.000000 dppd_plotnine-0.2.6/src/dppd_plotnine/plotnine_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:26:55.718305 dppd_plotnine-0.2.6/src/dppd_plotnine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-14 12:26:55.000000 dppd_plotnine-0.2.6/src/dppd_plotnine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-14 12:26:55.000000 dppd_plotnine-0.2.6/src/dppd_plotnine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:26:55.000000 dppd_plotnine-0.2.6/src/dppd_plotnine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:26:55.000000 dppd_plotnine-0.2.6/src/dppd_plotnine.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-14 12:26:55.000000 dppd_plotnine-0.2.6/src/dppd_plotnine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 12:26:55.000000 dppd_plotnine-0.2.6/src/dppd_plotnine.egg-info/top_level.txt
```

### Comparing `dppd_plotnine-0.2.5/LICENSE.txt` & `dppd_plotnine-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dppd_plotnine-0.2.5/PKG-INFO` & `dppd_plotnine-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dppd_plotnine
-Version: 0.2.5
+Version: 0.2.6
 Summary: Combines plotnine and dppd
 Home-page: https://github.com/TyberiusPrime/dppd_plotnine
 Author: Florian Finkernagel
 Author-email: finkernagel@imt.uni-marburg.de
 License: mit
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -71,9 +71,7 @@
 image](https://github.com/TyberiusPrime/dppd_plotnine/raw/master/docs/_static/index.png)
 
 Please see our full documentation at https://dppd_plotnine.readthedocs.io/en/latest/
 for more details of the straight and enhanced plotnine mappings available.
 
 
 
-
-
```

### Comparing `dppd_plotnine-0.2.5/README.md` & `dppd_plotnine-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `dppd_plotnine-0.2.5/src/dppd_plotnine/dppd_plotnine.py` & `dppd_plotnine-0.2.6/src/dppd_plotnine/dppd_plotnine.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,27 @@
 
 
 # this establishes the p9-dppd support
 
 
 @register_verb("p9", types=pd.DataFrame)
 def p9_DataFrame(df, mapping=None):
-    return p9.ggplot(mapping=mapping, data=df, environment=EvalEnvironment.capture(2))
+    try:
+        return p9.ggplot(
+            mapping=mapping, data=df, environment=EvalEnvironment.capture(2)
+        )
+    except TypeError as e:
+        if "environment" in str(e):  # support for plotnine > 0.13
+            res = p9.ggplot(mapping=mapping, data=df)
+            res.environment = p9.mapping._env.Environment.capture(2)
+            return res
 
 
 never_map = set(["data", "stat", "position"])
-other_args = set(['DEFAULT_AES'])
+other_args = set(["DEFAULT_AES"])
 
 add_funcs = {}
 
 
 def sensible_aes_order(required_aes):
     order = []
     if "x" in required_aes:
@@ -27,17 +35,14 @@
         order.append("y")
     for a in sorted(required_aes):
         if a != "x" and a != "y":
             order.append(a)
     return order
 
 
-
-
-
 def iter_elements():
     for name in dir(p9):
         if "_" in name and name[: name.find("_")] in (
             "geom",
             "annotate",
             "annotation",
             "scale",
@@ -54,16 +59,15 @@
 
 
 aliases = {
     "scale_y_continuous": ["syc"],
     "scale_x_continuous": ["sxc"],
 }
 
-for name, cls in iter_elements():
-
+for name, cls in iter_elements():  # noqa:C901
     if name in aliases:
         register_name = aliases[name] + [name]
     else:
         register_name = name
 
     @register_verb(register_name, types=p9.ggplot)
     def add_geom(plot, *args, cls=cls, **kwargs):
@@ -126,17 +130,17 @@
                     else:
                         raise
 
                 mapped = {k: k for k in cls.REQUIRED_AES if k in mapped}
                 non_mapped["data"] = data
 
             geom = cls(p9.aes(**mapped), **non_mapped)
-            if 'DEFAULT_AES' in other:
+            if "DEFAULT_AES" in other:
                 geom.DEFAULT_AES = geom.DEFAULT_AES.copy()
-                geom.DEFAULT_AES.update(other['DEFAULT_AES'])
+                geom.DEFAULT_AES.update(other["DEFAULT_AES"])
             return plot + geom
 
         add_funcs[add_name] = add_add_geom
 
 
 @register_verb(["save", "render"], types=p9.ggplot)
 def save(plot, *args, **kwargs):
```

### Comparing `dppd_plotnine-0.2.5/src/dppd_plotnine/geoms/annotation_stripes_dppd.py` & `dppd_plotnine-0.2.6/src/dppd_plotnine/geoms/annotation_stripes_dppd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import pandas as pd
 import numpy as np
 
 from plotnine.coords import coord_flip
-from plotnine.scales.scale import scale_discrete
+
+try:
+    from plotnine.scales.scale import scale_discrete
+except ImportError:
+    from plotnine.scales import scale_discrete
 from plotnine.geoms.geom import geom
 from plotnine.geoms.geom_rect import geom_rect
 from plotnine.geoms.annotate import annotate
 
 
 class annotation_stripes_dppd(annotate):
     """
@@ -15,103 +19,102 @@
     Useful as a background for geom_jitter.
 
     {usage}
     plot += annotation_stripes(fill=['red', 'blue'], alpha=0.3)
 
     Parameters
     ----------
-    fills - list of colors to alternate through.
+    fill - list of colors to alternate through.
         default: ["#AAAAAA", "#CCCCCC"]
     direction: 'vertical' or 'horizontal'
         default: 'vertical'
         orientation of the stripes
     extend: (0..1, 0..1)
         default: (0, 1)
         tuple describing the range covered by the stripes
         in relative units. Default covers the complete plot.
 
 
     {common_parameters}
     """
 
     def __init__(self, **kwargs):
-        if 'direction' in kwargs:
-            allowed = ('vertical', 'horizontal')
-            if ((not isinstance(kwargs['direction'], str))
-                    or (kwargs['direction'] not in allowed)):
-                raise ValueError("direction must be one of %s" % (allowed, ))
-        self._annotation_geom = _geom_stripes(
-            **kwargs)
+        if "direction" in kwargs:
+            allowed = ("vertical", "horizontal")
+            if (not isinstance(kwargs["direction"], str)) or (
+                kwargs["direction"] not in allowed
+            ):
+                raise ValueError("direction must be one of %s" % (allowed,))
+        self._annotation_geom = _geom_stripes(**kwargs)
 
 
 class _geom_stripes(geom):
-
     DEFAULT_AES = {}
     REQUIRED_AES = set()
     DEFAULT_PARAMS = {
         "stat": "identity",
         "position": "identity",
         "na_rm": False,
         "color": None,
-        "fills": ["#AAAAAA", "#CCCCCC"],
+        "fill": ["#AAAAAA", "#CCCCCC"],
         "linetype": "solid",
         "size": 0,
         "alpha": 0.5,
-        'direction': 'vertical',
-        'extend': (0, 1),
+        "direction": "vertical",
+        "extend": (0, 1),
     }
     legend_geom = "polygon"
 
     @staticmethod
     def draw_group(data, panel_params, coord, ax, **params):
         is_coord_flip = isinstance(coord, coord_flip)
-        direction = params['direction']
-        if direction == 'vertical':
+        direction = params["direction"]
+        if direction == "vertical":
             scale = getattr(panel_params["scales"], "x")
             if is_coord_flip:
                 prefix, other_prefix = "y_", "x_"
             else:
                 prefix, other_prefix = "x_", "y_"
         else:
             scale = getattr(panel_params["scales"], "y")
             if is_coord_flip:
                 prefix, other_prefix = "x_", "y_"
             else:
                 prefix, other_prefix = "y_", "x_"
 
         is_scale_discrete = isinstance(scale, scale_discrete)
-        fills = list(params["fills"])
+        fill = list(params["fill"])
         count = len(panel_params[prefix + "labels"])
         if is_scale_discrete:
             step_size = 1
             left = np.arange(0, count, 1) + 0.5
         else:
             step_size = (
-                panel_params[prefix + "major"][-1] -
-                panel_params[prefix + "major"][0]
+                panel_params[prefix + "major"][-1] - panel_params[prefix + "major"][0]
             ) / (count - 1)
             left = panel_params[prefix + "major"] - step_size / 2
         right = left + step_size
         left[0] = panel_params[prefix + "range"][0]
         right[-1] = panel_params[prefix + "range"][1]
         ymin = panel_params[other_prefix + "range"][0]
-        y_extend = (panel_params[other_prefix + "range"][1]
-                    - panel_params[other_prefix + "range"][0])
+        y_extend = (
+            panel_params[other_prefix + "range"][1]
+            - panel_params[other_prefix + "range"][0]
+        )
         data = pd.DataFrame(
             {
                 "xmin": left,
                 "xmax": right,
-                "ymin": ymin + params['extend'][0] * y_extend,
-                "ymax": ymin + params['extend'][1] * y_extend,
-                "fill": (fills * len(left))[: len(left)],
+                "ymin": ymin + params["extend"][0] * y_extend,
+                "ymax": ymin + params["extend"][1] * y_extend,
+                "fill": (fill * len(left))[: len(left)],
                 "size": params["size"],
                 "linetype": params["linetype"],
                 "alpha": params["alpha"],
                 "color": "#000000",
             }
         )
-        if (direction == 'horizontal'):
+        if direction == "horizontal":
             data = data.rename(
-                columns={"xmin": "ymin", "xmax": "ymax",
-                         "ymin": "xmin", "ymax": "xmax"}
+                columns={"xmin": "ymin", "xmax": "ymax", "ymin": "xmin", "ymax": "xmax"}
             )
         return geom_rect.draw_group(data, panel_params, coord, ax, **params)
```

### Comparing `dppd_plotnine-0.2.5/src/dppd_plotnine/plotnine_extensions.py` & `dppd_plotnine-0.2.6/src/dppd_plotnine/plotnine_extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,20 @@
     # if plot.plot.theme is None:
     # plot.theme_grey()
     # plot.plot.theme +=
     return plot + p9.theme(**{what: t})
 
 
 def _turn_axis_labels(plot, ax, angle, hjust, vjust, size, color):
-    t = p9.themes.element_text(
-        rotation=angle, ha=hjust, va=vjust, size=size, color=color
-    )
+    try:
+        t = p9.themes.element_text(
+            rotation=angle, ha=hjust, va=vjust, size=size, color=color
+        )
+    except AttributeError:
+        t = p9.element_text(rotation=angle, ha=hjust, va=vjust, size=size, color=color)
     return _change_theme(plot, ax, t)
 
 
 @register_verb(types=p9.ggplot)
 def turn_x_axis_labels(
     plot, angle=90, hjust="center", vjust="top", size=None, color=None
 ):
@@ -92,14 +95,15 @@
 
 @register_verb(types=p9.ggplot)
 def hide_facet_labels(plot):
     """Hide the facet labels"""
     _change_theme(plot, "strip_background", p9.element_blank())
     return _change_theme(plot, "strip_text_x", p9.element_blank())
 
+
 @register_verb(types=p9.ggplot)
 def hide_legend_title(plot):
     """Hide the legend label"""
     return _change_theme(plot, "legend_title", p9.element_blank())
 
 
 _many_cat_colors = [
@@ -145,14 +149,26 @@
     return plot + p9.scale_color_manual(
         (_many_cat_colors + _many_cat_colors)[offset : offset + len(_many_cat_colors)],
         **kwargs
     )
 
 
 @register_verb(types=p9.ggplot)
+def scale_color_cmap_discrete(plot, *args, **kwargs):
+    """Just an alias"""
+    return plot + p9.scale_color_cmap_d(*args, **kwargs)
+
+
+@register_verb(types=p9.ggplot)
+def scale_fill_cmap_discrete(plot, *args, **kwargs):
+    """Just an alias for cmap_d"""
+    return plot + p9.scale_fill_cmap_d(*args, **kwargs)
+
+
+@register_verb(types=p9.ggplot)
 def aes(_plot, *args, **kwargs):  # pragma: no cover
     return p9.aes(*args, **kwargs)
 
 
 @register_verb(types=p9.ggplot)
 def reverse_transform(_plot, trans):
     from mizani.transforms import trans_new
@@ -194,15 +210,15 @@
     plot.render_args = render_args
     return plot
 
 
 @register_verb("add_cummulative", types=p9.ggplot)
 def add_cummulative(plot, x_column, ascending=True, percent=False, percentile=1.0):
     """Add a line showing cumulative % of data <= x.
-        if you specify a percentile, all data at the extreme range is dropped
+    if you specify a percentile, all data at the extreme range is dropped
 
 
     """
     import numpy as np
     import pandas as pd
     import itertools
 
@@ -263,30 +279,35 @@
 
 @register_verb("hide_legend", types=p9.ggplot)
 def hide_legend(plot):
     """Hide plot legend - whether you have manually defined a scale or not"""
     import types
 
     def my_compute_aesthetics(self, p):
-        print("my_compute_aesthetics", type(p))
         res = self._org_compute_aesthetics(p)
         for s in p.scales:
             s.guide = False
         return res
 
     plot.layers._org_compute_aesthetics = plot.layers.compute_aesthetics
     # advanced monkey patching for the win!
     plot.layers.compute_aesthetics = types.MethodType(
         my_compute_aesthetics, plot.layers
     )
     return plot
 
-@register_verb('sc10', types=p9.ggplot)
+
+@register_verb("sc10", types=p9.ggplot)
 def sc10(plot):
-    return plot + p9.scale_x_continuous(trans='log10') + p9.scale_y_continuous(trans='log10')
+    return (
+        plot
+        + p9.scale_x_continuous(trans="log10")
+        + p9.scale_y_continuous(trans="log10")
+    )
+
 
 @register_verb("sxc10", types=p9.ggplot)
 def sxc10(plot, *args, **kwargs):
     """scale_x_continuous(trans='log10',...)"""
     if not "trans" in kwargs:
         kwargs["trans"] = "log10"
     return plot + p9.scale_x_continuous(*args, **kwargs)
@@ -417,22 +438,22 @@
     kwargs_glow1 = kwargs.copy()
     kwargs_glow1["_outlier_size"] = kwargs["_outlier_size"] + 3
     kwargs_glow1["_outlier_alpha"] = 0.1
     kwargs_glow1["_size"] = 3
     kwargs_glow1["_alpha"] = 0.1
     kwargs["_outlier_size"] = 1.5
     res = dppd._add_boxplot(*args, **kwargs_glow1)
-    return res._add_boxplot(*args, **kwargs, DEFAULT_AES={'color': 'white'})
+    return res._add_boxplot(*args, **kwargs, DEFAULT_AES={"color": "white"})
 
 
 @register_verb("add_bar_cyberpunk", types=p9.ggplot, pass_dppd=True)
 def add_bar_cyberpunk(dppd, *args, **kwargs):
     if not "_size" in kwargs:
         kwargs["_size"] = 0.5
     kwargs_glow1 = kwargs.copy()
     if not "fill" in kwargs and not "_fill" in kwargs:
         kwargs_glow1["_fill"] = "blue"
         kwargs["_fill"] = None
     kwargs_glow1["_alpha"] = 0.1
     kwargs_glow1["_size"] = kwargs["_size"] + 2.5
     res = dppd._add_bar(*args, **kwargs_glow1)
-    return res._add_bar(*args, **kwargs, DEFAULT_AES={'color': 'white'})
+    return res._add_bar(*args, **kwargs, DEFAULT_AES={"color": "white"})
```

### Comparing `dppd_plotnine-0.2.5/src/dppd_plotnine.egg-info/PKG-INFO` & `dppd_plotnine-0.2.6/src/dppd_plotnine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dppd-plotnine
-Version: 0.2.5
+Version: 0.2.6
 Summary: Combines plotnine and dppd
 Home-page: https://github.com/TyberiusPrime/dppd_plotnine
 Author: Florian Finkernagel
 Author-email: finkernagel@imt.uni-marburg.de
 License: mit
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -71,9 +71,7 @@
 image](https://github.com/TyberiusPrime/dppd_plotnine/raw/master/docs/_static/index.png)
 
 Please see our full documentation at https://dppd_plotnine.readthedocs.io/en/latest/
 for more details of the straight and enhanced plotnine mappings available.
 
 
 
-
-
```

