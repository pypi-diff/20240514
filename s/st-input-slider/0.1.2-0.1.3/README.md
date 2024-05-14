# Comparing `tmp/st-input-slider-0.1.2.tar.gz` & `tmp/st-input-slider-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st-input-slider-0.1.2.tar", last modified: Fri May 10 20:46:41 2024, max compression
+gzip compressed data, was "st-input-slider-0.1.3.tar", last modified: Tue May 14 20:17:30 2024, max compression
```

## Comparing `st-input-slider-0.1.2.tar` & `st-input-slider-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 20:46:41.973079 st-input-slider-0.1.2/
--rw-rw-rw-   0        0        0     1082 2024-04-05 22:58:34.000000 st-input-slider-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       52 2024-04-08 19:55:15.000000 st-input-slider-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4034 2024-05-10 20:46:41.971085 st-input-slider-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3615 2024-05-10 20:45:19.000000 st-input-slider-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-10 20:46:41.974336 st-input-slider-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1195 2024-05-10 20:34:47.000000 st-input-slider-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 20:46:41.892293 st-input-slider-0.1.2/st_input_slider/
--rw-rw-rw-   0        0        0     3635 2024-05-10 20:43:27.000000 st-input-slider-0.1.2/st_input_slider/__init__.py
--rw-rw-rw-   0        0        0     1891 2024-05-10 20:17:05.000000 st-input-slider-0.1.2/st_input_slider/example.py
-drwxrwxrwx   0        0        0        0 2024-05-10 20:46:41.852230 st-input-slider-0.1.2/st_input_slider/frontend/
-drwxrwxrwx   0        0        0        0 2024-05-10 20:46:41.937310 st-input-slider-0.1.2/st_input_slider/frontend/build/
--rw-rw-rw-   0        0        0      221 2024-05-10 20:35:47.000000 st-input-slider-0.1.2/st_input_slider/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2024-04-05 22:58:35.000000 st-input-slider-0.1.2/st_input_slider/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0      492 2024-05-10 20:35:47.000000 st-input-slider-0.1.2/st_input_slider/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2024-05-10 20:46:41.854225 st-input-slider-0.1.2/st_input_slider/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2024-05-10 20:46:41.958118 st-input-slider-0.1.2/st_input_slider/frontend/build/static/js/
--rw-rw-rw-   0        0        0   454378 2024-05-10 20:35:47.000000 st-input-slider-0.1.2/st_input_slider/frontend/build/static/js/main.4ba2a0fe.js
--rw-rw-rw-   0        0        0     1755 2024-05-10 20:35:47.000000 st-input-slider-0.1.2/st_input_slider/frontend/build/static/js/main.4ba2a0fe.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1898354 2024-05-10 20:35:47.000000 st-input-slider-0.1.2/st_input_slider/frontend/build/static/js/main.4ba2a0fe.js.map
-drwxrwxrwx   0        0        0        0 2024-05-10 20:46:41.919247 st-input-slider-0.1.2/st_input_slider.egg-info/
--rw-rw-rw-   0        0        0     4034 2024-05-10 20:46:41.000000 st-input-slider-0.1.2/st_input_slider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2024-05-10 20:46:41.000000 st-input-slider-0.1.2/st_input_slider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 20:46:41.000000 st-input-slider-0.1.2/st_input_slider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2024-05-10 20:46:41.000000 st-input-slider-0.1.2/st_input_slider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-10 20:46:41.000000 st-input-slider-0.1.2/st_input_slider.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 20:17:30.530858 st-input-slider-0.1.3/
+-rw-rw-rw-   0        0        0     1082 2024-04-05 22:58:34.000000 st-input-slider-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       52 2024-04-08 19:55:15.000000 st-input-slider-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4330 2024-05-14 20:17:30.527617 st-input-slider-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3911 2024-05-10 21:00:57.000000 st-input-slider-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-14 20:17:30.531856 st-input-slider-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1195 2024-05-10 21:29:36.000000 st-input-slider-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:17:30.423929 st-input-slider-0.1.3/st_input_slider/
+-rw-rw-rw-   0        0        0       57 2024-05-14 20:06:13.000000 st-input-slider-0.1.3/st_input_slider/__init__.py
+-rw-rw-rw-   0        0        0     1891 2024-05-10 20:17:05.000000 st-input-slider-0.1.3/st_input_slider/example.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:17:30.385775 st-input-slider-0.1.3/st_input_slider/frontend/
+drwxrwxrwx   0        0        0        0 2024-05-14 20:17:30.470592 st-input-slider-0.1.3/st_input_slider/frontend/build/
+-rw-rw-rw-   0        0        0      221 2024-05-14 20:16:10.000000 st-input-slider-0.1.3/st_input_slider/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2024-04-05 22:58:35.000000 st-input-slider-0.1.3/st_input_slider/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0      492 2024-05-14 20:16:10.000000 st-input-slider-0.1.3/st_input_slider/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2024-05-14 20:17:30.388766 st-input-slider-0.1.3/st_input_slider/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2024-05-14 20:17:30.489306 st-input-slider-0.1.3/st_input_slider/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   454378 2024-05-14 20:16:10.000000 st-input-slider-0.1.3/st_input_slider/frontend/build/static/js/main.4ba2a0fe.js
+-rw-rw-rw-   0        0        0     1755 2024-05-14 20:16:10.000000 st-input-slider-0.1.3/st_input_slider/frontend/build/static/js/main.4ba2a0fe.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1898354 2024-05-14 20:16:10.000000 st-input-slider-0.1.3/st_input_slider/frontend/build/static/js/main.4ba2a0fe.js.map
+drwxrwxrwx   0        0        0        0 2024-05-14 20:17:30.511767 st-input-slider-0.1.3/st_input_slider/utils/
+-rw-rw-rw-   0        0        0       32 2024-05-10 21:27:47.000000 st-input-slider-0.1.3/st_input_slider/utils/__init__.py
+-rw-rw-rw-   0        0        0     1797 2024-05-10 20:49:35.000000 st-input-slider-0.1.3/st_input_slider/utils/callback.py
+-rw-rw-rw-   0        0        0      511 2024-05-14 20:02:56.000000 st-input-slider-0.1.3/st_input_slider/utils/component_func.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:17:30.522630 st-input-slider-0.1.3/st_input_slider/widgets/
+-rw-rw-rw-   0        0        0       43 2024-05-14 20:02:38.000000 st-input-slider-0.1.3/st_input_slider/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3714 2024-05-14 19:40:06.000000 st-input-slider-0.1.3/st_input_slider/widgets/input_slider.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:17:30.450114 st-input-slider-0.1.3/st_input_slider.egg-info/
+-rw-rw-rw-   0        0        0     4330 2024-05-14 20:17:30.000000 st-input-slider-0.1.3/st_input_slider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      803 2024-05-14 20:17:30.000000 st-input-slider-0.1.3/st_input_slider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 20:17:30.000000 st-input-slider-0.1.3/st_input_slider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2024-05-14 20:17:30.000000 st-input-slider-0.1.3/st_input_slider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-14 20:17:30.000000 st-input-slider-0.1.3/st_input_slider.egg-info/top_level.txt
```

### Comparing `st-input-slider-0.1.2/LICENSE` & `st-input-slider-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `st-input-slider-0.1.2/PKG-INFO` & `st-input-slider-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-input-slider
-Version: 0.1.2
+Version: 0.1.3
 Summary: A custom Streamlit component that combines a slider with an input box for more precise value selection
 Home-page: https://github.com/balexandermunoz/st-input-slider
 Author: Brayan Munoz
 Author-email: balexander.munoz@udea.edu.co
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
@@ -37,14 +37,17 @@
   - `labelTextAlign` (str, default "left"): The text alignment of the label. Can be "left", "center", "right", "justify", or "inherit".
   - `fontSize` (float, default 12): The font size.
   - `endAdornment` (str, default None): The text at the end of the input box.
   - `labelWidth` (str, default "20%"): The width of the label.
   - `sliderWidth` (str, default "60%"): The width of the slider.
   - `inputWidth` (str, default "20%"): The width of the input box.
 - `key` (str or None, default None): An optional key that uniquely identifies this component. If this is `None`, and the component's arguments are changed, the component will be re-mounted in the Streamlit frontend and lose its current state.
+- `on_change` (Callable, default None): A callback function that is called whenever the slider value changes.
+- `args` (tuple, default None): Additional arguments to pass to the callback function.
+- `kwargs` (dict, default None): Additional keyword arguments to pass to the callback function.
 
 ### Function Returns
 
 - `float`: The current value of the slider. This is the value passed to `Streamlit.setComponentValue` on the frontend.
 
 ## Example
```

### Comparing `st-input-slider-0.1.2/README.md` & `st-input-slider-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,17 @@
   - `labelTextAlign` (str, default "left"): The text alignment of the label. Can be "left", "center", "right", "justify", or "inherit".
   - `fontSize` (float, default 12): The font size.
   - `endAdornment` (str, default None): The text at the end of the input box.
   - `labelWidth` (str, default "20%"): The width of the label.
   - `sliderWidth` (str, default "60%"): The width of the slider.
   - `inputWidth` (str, default "20%"): The width of the input box.
 - `key` (str or None, default None): An optional key that uniquely identifies this component. If this is `None`, and the component's arguments are changed, the component will be re-mounted in the Streamlit frontend and lose its current state.
+- `on_change` (Callable, default None): A callback function that is called whenever the slider value changes.
+- `args` (tuple, default None): Additional arguments to pass to the callback function.
+- `kwargs` (dict, default None): Additional keyword arguments to pass to the callback function.
 
 ### Function Returns
 
 - `float`: The current value of the slider. This is the value passed to `Streamlit.setComponentValue` on the frontend.
 
 ## Example
```

### Comparing `st-input-slider-0.1.2/setup.py` & `st-input-slider-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="st-input-slider",
-    version="0.1.2",
+    version="0.1.3",
     author="Brayan Munoz",
     author_email="balexander.munoz@udea.edu.co",
     description="A custom Streamlit component that combines a slider with an input box for more precise value selection",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/balexandermunoz/st-input-slider",
     packages=setuptools.find_packages(),
```

### Comparing `st-input-slider-0.1.2/st_input_slider/__init__.py` & `st-input-slider-0.1.3/st_input_slider/widgets/input_slider.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,38 @@
-import os
-from typing import Any, Dict
-
-import streamlit.components.v1 as components
-
-_RELEASE = True
-
-if not _RELEASE:
-    _component_func = components.declare_component(
-        "st_input_slider",
-        url="http://localhost:3001",
-    )
-else:
-    parent_dir = os.path.dirname(os.path.abspath(__file__))
-    build_dir = os.path.join(parent_dir, "frontend/build")
-    _component_func = components.declare_component(
-        "st_input_slider", path=build_dir)
+from typing import Any, Dict, Callable
 
+from ..utils import register
+from ..utils.component_func import _component_func
 
 DEFAULT_OPTIONS = {
-    "color": None, # A color string
+    "color": None,
     "marks": False,
     "disableUnderline": False,
     "labelPosition": "top",
     "labelTextAlign": "left",
     "fontSize": 12,
     "endAdornment": None,
     "labelWidth": "20%",
     "sliderWidth": "60%",
     "inputWidth": "20%"
 }
 
+
 def st_input_slider(
     label: str = None,
     min_value: float = 0,
     max_value: float = 100,
     value: float = 50,
     step: float = 1,
     format: str = "",
     options: Dict[str, Any] = None,
-    key: str = None
+    key: str = None,
+    on_change: Callable = None,
+    args: tuple = None,
+    kwargs: dict = None
 ) -> float:
     """
     A highly customizable Streamlit component that combines a slider with an input box for more precise value selection.
 
     Parameters
     ----------
     label: str, default None
@@ -69,28 +59,36 @@
         - "labelWidth": str, default is "20%". The width of the label.
         - "sliderWidth": str, default is "60%". The width of the slider.
         - "inputWidth": str, default is "20%". The width of the input box.
     key: str or None, default None
         An optional key that uniquely identifies this component. If this is
         None, and the component's arguments are changed, the component will
         be re-mounted in the Streamlit frontend and lose its current state.
+    on_change: Callable, default None
+        A callback function that is called whenever the slider value changes.
+    args: tuple, default None
+        Additional arguments to pass to the callback function.
+    kwargs: dict, default None
+        Additional keyword arguments to pass to the callback function.
 
     Returns
     -------
     float
         The current value of the slider. This is the value passed to 
         `Streamlit.setComponentValue` on the frontend.
     """
-    options = set_options(options)
+    register(key, on_change, args, kwargs)
+    options = _set_options(options)
     component_value = _component_func(
         label=label, min_value=min_value, max_value=max_value,
         value=value, step=step, format=format,
         options=options, key=key, default=value
     )
     return component_value
 
-def set_options(options: dict) -> dict:
+
+def _set_options(options: dict) -> dict:
     if not options:
         return DEFAULT_OPTIONS
     for key, value in DEFAULT_OPTIONS.items():
         options[key] = options.get(key, value)
-    return options
+    return options
```

### Comparing `st-input-slider-0.1.2/st_input_slider/example.py` & `st-input-slider-0.1.3/st_input_slider/example.py`

 * *Files identical despite different names*

### Comparing `st-input-slider-0.1.2/st_input_slider/frontend/build/bootstrap.min.css` & `st-input-slider-0.1.3/st_input_slider/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st-input-slider-0.1.2/st_input_slider/frontend/build/static/js/main.4ba2a0fe.js` & `st-input-slider-0.1.3/st_input_slider/frontend/build/static/js/main.4ba2a0fe.js`

 * *Files identical despite different names*

### Comparing `st-input-slider-0.1.2/st_input_slider/frontend/build/static/js/main.4ba2a0fe.js.LICENSE.txt` & `st-input-slider-0.1.3/st_input_slider/frontend/build/static/js/main.4ba2a0fe.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st-input-slider-0.1.2/st_input_slider/frontend/build/static/js/main.4ba2a0fe.js.map` & `st-input-slider-0.1.3/st_input_slider/frontend/build/static/js/main.4ba2a0fe.js.map`

 * *Files identical despite different names*

### Comparing `st-input-slider-0.1.2/st_input_slider.egg-info/PKG-INFO` & `st-input-slider-0.1.3/st_input_slider.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-input-slider
-Version: 0.1.2
+Version: 0.1.3
 Summary: A custom Streamlit component that combines a slider with an input box for more precise value selection
 Home-page: https://github.com/balexandermunoz/st-input-slider
 Author: Brayan Munoz
 Author-email: balexander.munoz@udea.edu.co
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
@@ -37,14 +37,17 @@
   - `labelTextAlign` (str, default "left"): The text alignment of the label. Can be "left", "center", "right", "justify", or "inherit".
   - `fontSize` (float, default 12): The font size.
   - `endAdornment` (str, default None): The text at the end of the input box.
   - `labelWidth` (str, default "20%"): The width of the label.
   - `sliderWidth` (str, default "60%"): The width of the slider.
   - `inputWidth` (str, default "20%"): The width of the input box.
 - `key` (str or None, default None): An optional key that uniquely identifies this component. If this is `None`, and the component's arguments are changed, the component will be re-mounted in the Streamlit frontend and lose its current state.
+- `on_change` (Callable, default None): A callback function that is called whenever the slider value changes.
+- `args` (tuple, default None): Additional arguments to pass to the callback function.
+- `kwargs` (dict, default None): Additional keyword arguments to pass to the callback function.
 
 ### Function Returns
 
 - `float`: The current value of the slider. This is the value passed to `Streamlit.setComponentValue` on the frontend.
 
 ## Example
```

### Comparing `st-input-slider-0.1.2/st_input_slider.egg-info/SOURCES.txt` & `st-input-slider-0.1.3/st_input_slider.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,8 +10,13 @@
 st_input_slider.egg-info/requires.txt
 st_input_slider.egg-info/top_level.txt
 st_input_slider/frontend/build/asset-manifest.json
 st_input_slider/frontend/build/bootstrap.min.css
 st_input_slider/frontend/build/index.html
 st_input_slider/frontend/build/static/js/main.4ba2a0fe.js
 st_input_slider/frontend/build/static/js/main.4ba2a0fe.js.LICENSE.txt
-st_input_slider/frontend/build/static/js/main.4ba2a0fe.js.map
+st_input_slider/frontend/build/static/js/main.4ba2a0fe.js.map
+st_input_slider/utils/__init__.py
+st_input_slider/utils/callback.py
+st_input_slider/utils/component_func.py
+st_input_slider/widgets/__init__.py
+st_input_slider/widgets/input_slider.py
```

