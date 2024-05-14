# Comparing `tmp/custom-dot-plot-0.0.6.tar.gz` & `tmp/custom-dot-plot-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom-dot-plot-0.0.6.tar", last modified: Sat Apr 13 21:44:32 2024, max compression
+gzip compressed data, was "custom-dot-plot-0.0.7.tar", last modified: Tue May 14 00:30:24 2024, max compression
```

## Comparing `custom-dot-plot-0.0.6.tar` & `custom-dot-plot-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 21:44:32.877119 custom-dot-plot-0.0.6/
--rw-rw-rw-   0        0        0     1082 2024-03-24 15:01:03.000000 custom-dot-plot-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       52 2024-03-26 01:14:57.000000 custom-dot-plot-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      171 2024-04-13 21:44:32.872119 custom-dot-plot-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-03-24 15:01:03.000000 custom-dot-plot-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-13 21:44:29.175541 custom-dot-plot-0.0.6/custom_dot_plot/
--rw-rw-rw-   0        0        0     1058 2024-04-13 21:41:47.000000 custom-dot-plot-0.0.6/custom_dot_plot/__init__.py
--rw-rw-rw-   0        0        0    18948 2024-04-13 20:25:54.000000 custom-dot-plot-0.0.6/custom_dot_plot/example.py
-drwxrwxrwx   0        0        0        0 2024-04-13 21:44:28.897493 custom-dot-plot-0.0.6/custom_dot_plot/frontend/
-drwxrwxrwx   0        0        0        0 2024-04-13 21:44:31.389017 custom-dot-plot-0.0.6/custom_dot_plot/frontend/build/
--rw-rw-rw-   0        0        0      374 2024-04-13 21:44:05.000000 custom-dot-plot-0.0.6/custom_dot_plot/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2024-03-24 15:01:03.000000 custom-dot-plot-0.0.6/custom_dot_plot/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0   589892 2024-03-23 11:30:35.000000 custom-dot-plot-0.0.6/custom_dot_plot/frontend/build/bootstrap.min.css.map
--rw-rw-rw-   0        0        0      553 2024-04-13 21:44:05.000000 custom-dot-plot-0.0.6/custom_dot_plot/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2024-04-13 21:44:28.978814 custom-dot-plot-0.0.6/custom_dot_plot/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2024-04-13 21:44:31.723457 custom-dot-plot-0.0.6/custom_dot_plot/frontend/build/static/css/
--rw-rw-rw-   0        0        0     3167 2024-04-13 21:44:05.000000 custom-dot-plot-0.0.6/custom_dot_plot/frontend/build/static/css/main.99a8c608.css
--rw-rw-rw-   0        0        0     6641 2024-04-13 21:44:05.000000 custom-dot-plot-0.0.6/custom_dot_plot/frontend/build/static/css/main.99a8c608.css.map
-drwxrwxrwx   0        0        0        0 2024-04-13 21:44:32.846503 custom-dot-plot-0.0.6/custom_dot_plot/frontend/build/static/js/
--rw-rw-rw-   0        0        0   348397 2024-04-13 21:44:05.000000 custom-dot-plot-0.0.6/custom_dot_plot/frontend/build/static/js/main.618d6894.js
--rw-rw-rw-   0        0        0     1293 2024-04-13 21:44:05.000000 custom-dot-plot-0.0.6/custom_dot_plot/frontend/build/static/js/main.618d6894.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1382378 2024-04-13 21:44:05.000000 custom-dot-plot-0.0.6/custom_dot_plot/frontend/build/static/js/main.618d6894.js.map
-drwxrwxrwx   0        0        0        0 2024-04-13 21:44:30.026334 custom-dot-plot-0.0.6/custom_dot_plot.egg-info/
--rw-rw-rw-   0        0        0      171 2024-04-13 21:44:26.000000 custom-dot-plot-0.0.6/custom_dot_plot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      796 2024-04-13 21:44:27.000000 custom-dot-plot-0.0.6/custom_dot_plot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 21:44:26.000000 custom-dot-plot-0.0.6/custom_dot_plot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2024-04-13 21:44:26.000000 custom-dot-plot-0.0.6/custom_dot_plot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-13 21:44:26.000000 custom-dot-plot-0.0.6/custom_dot_plot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-13 21:44:32.878119 custom-dot-plot-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1053 2024-04-13 21:41:15.000000 custom-dot-plot-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 00:30:24.879724 custom-dot-plot-0.0.7/
+-rw-rw-rw-   0        0        0     1082 2024-03-24 15:01:03.000000 custom-dot-plot-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0       52 2024-03-26 01:14:57.000000 custom-dot-plot-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      171 2024-05-14 00:30:24.875665 custom-dot-plot-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-03-24 15:01:03.000000 custom-dot-plot-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 00:30:22.795945 custom-dot-plot-0.0.7/custom_dot_plot/
+-rw-rw-rw-   0        0        0     1058 2024-04-13 21:41:47.000000 custom-dot-plot-0.0.7/custom_dot_plot/__init__.py
+-rw-rw-rw-   0        0        0    18948 2024-04-13 20:25:54.000000 custom-dot-plot-0.0.7/custom_dot_plot/example.py
+drwxrwxrwx   0        0        0        0 2024-05-14 00:30:22.544379 custom-dot-plot-0.0.7/custom_dot_plot/frontend/
+drwxrwxrwx   0        0        0        0 2024-05-14 00:30:23.861216 custom-dot-plot-0.0.7/custom_dot_plot/frontend/build/
+-rw-rw-rw-   0        0        0      374 2024-05-14 00:29:43.000000 custom-dot-plot-0.0.7/custom_dot_plot/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2024-03-24 15:01:03.000000 custom-dot-plot-0.0.7/custom_dot_plot/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0   589892 2024-03-23 11:30:35.000000 custom-dot-plot-0.0.7/custom_dot_plot/frontend/build/bootstrap.min.css.map
+-rw-rw-rw-   0        0        0      553 2024-05-14 00:29:43.000000 custom-dot-plot-0.0.7/custom_dot_plot/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2024-05-14 00:30:22.562634 custom-dot-plot-0.0.7/custom_dot_plot/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2024-05-14 00:30:24.008571 custom-dot-plot-0.0.7/custom_dot_plot/frontend/build/static/css/
+-rw-rw-rw-   0        0        0     3227 2024-05-14 00:29:43.000000 custom-dot-plot-0.0.7/custom_dot_plot/frontend/build/static/css/main.80661064.css
+-rw-rw-rw-   0        0        0     6791 2024-05-14 00:29:43.000000 custom-dot-plot-0.0.7/custom_dot_plot/frontend/build/static/css/main.80661064.css.map
+drwxrwxrwx   0        0        0        0 2024-05-14 00:30:24.853512 custom-dot-plot-0.0.7/custom_dot_plot/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   348397 2024-05-14 00:29:43.000000 custom-dot-plot-0.0.7/custom_dot_plot/frontend/build/static/js/main.618d6894.js
+-rw-rw-rw-   0        0        0     1293 2024-05-14 00:29:43.000000 custom-dot-plot-0.0.7/custom_dot_plot/frontend/build/static/js/main.618d6894.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1382378 2024-05-14 00:29:43.000000 custom-dot-plot-0.0.7/custom_dot_plot/frontend/build/static/js/main.618d6894.js.map
+drwxrwxrwx   0        0        0        0 2024-05-14 00:30:23.195746 custom-dot-plot-0.0.7/custom_dot_plot.egg-info/
+-rw-rw-rw-   0        0        0      171 2024-05-14 00:30:19.000000 custom-dot-plot-0.0.7/custom_dot_plot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      796 2024-05-14 00:30:21.000000 custom-dot-plot-0.0.7/custom_dot_plot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 00:30:19.000000 custom-dot-plot-0.0.7/custom_dot_plot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2024-05-14 00:30:19.000000 custom-dot-plot-0.0.7/custom_dot_plot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-14 00:30:19.000000 custom-dot-plot-0.0.7/custom_dot_plot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 00:30:24.881282 custom-dot-plot-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2024-05-14 00:13:32.000000 custom-dot-plot-0.0.7/setup.py
```

### Comparing `custom-dot-plot-0.0.6/LICENSE` & `custom-dot-plot-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `custom-dot-plot-0.0.6/custom_dot_plot/__init__.py` & `custom-dot-plot-0.0.7/custom_dot_plot/__init__.py`

 * *Files identical despite different names*

### Comparing `custom-dot-plot-0.0.6/custom_dot_plot/example.py` & `custom-dot-plot-0.0.7/custom_dot_plot/example.py`

 * *Files identical despite different names*

### Comparing `custom-dot-plot-0.0.6/custom_dot_plot/frontend/build/bootstrap.min.css` & `custom-dot-plot-0.0.7/custom_dot_plot/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `custom-dot-plot-0.0.6/custom_dot_plot/frontend/build/bootstrap.min.css.map` & `custom-dot-plot-0.0.7/custom_dot_plot/frontend/build/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `custom-dot-plot-0.0.6/custom_dot_plot/frontend/build/index.html` & `custom-dot-plot-0.0.7/custom_dot_plot/frontend/build/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><script defer="defer" src="./static/js/main.618d6894.js"></script><link href="./static/css/main.99a8c608.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><script defer="defer" src="./static/js/main.618d6894.js"></script><link href="./static/css/main.80661064.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `custom-dot-plot-0.0.6/custom_dot_plot/frontend/build/static/css/main.99a8c608.css` & `custom-dot-plot-0.0.7/custom_dot_plot/frontend/build/static/css/main.80661064.css`

 * *Files 4% similar despite different names*

```diff
@@ -1,2 +1,2 @@
-.plot-container{padding:10px}.plot-contents-container{align-items:center;column-gap:30px;display:flex;overflow:auto;width:calc(100% - 1px)}.main-plot-container{align-items:flex-end;display:flex;flex-direction:column;width:100%}.left-main-index{font-weight:700;margin-bottom:auto;margin-top:auto;transform:rotate(-180deg);writing-mode:vertical-lr}.main-plot-column-container{list-style-type:none;width:calc(94% - 1px)}.main-plot-column-name{font-weight:700;margin-bottom:30px;text-align:center}.main-plot-column-index-container{border:1px solid;border-radius:6px;box-shadow:0 2px 8px 0 #63636333;display:flex;padding:15px;width:100%}.main-plot-column-index{align-items:center;display:flex;justify-content:center;width:100%}.main-plot-first-category-container{display:flex;width:inherit}.main-plot-first-category-index{font-weight:600;margin-bottom:auto;margin-top:auto;transform:rotate(-180deg);white-space:nowrap;width:-webkit-fit-content;width:-moz-fit-content;width:fit-content;writing-mode:vertical-lr}.main-plot-first-category-contents-container{list-style-type:none;padding-left:10px;width:inherit}.main-plot-level-data-container{border:1px solid;border-radius:6px;box-shadow:0 2px 8px 0 #63636333;display:flex;justify-content:space-between;margin-bottom:10px;padding:15px;width:calc(100% - 1px)}.main-plot-level{line-height:40px;text-align:center;white-space:nowrap}.main-plot-data{align-items:center;cursor:pointer;display:flex;justify-content:center;width:-webkit-fit-content;width:-moz-fit-content;width:fit-content}.main-plot-second-category-container{display:flex;width:inherit}.main-plot-second-category-index{font-weight:600;margin-bottom:auto;margin-top:auto;transform:rotate(-180deg);white-space:nowrap;width:-webkit-fit-content;width:-moz-fit-content;width:fit-content;writing-mode:vertical-lr}.main-plot-second-category-contents-container{list-style-type:none;margin-top:30px;padding-left:10px;width:inherit}.main-plot-third-category-container{display:flex}.main-plot-third-category-index{font-weight:600;margin-bottom:auto;margin-top:auto;transform:rotate(-180deg);white-space:nowrap;width:-webkit-fit-content;width:-moz-fit-content;width:fit-content;writing-mode:vertical-lr}.main-plot-third-category-contents-container{list-style-type:none;margin-top:30px;padding-left:10px}.legends-container{column-gap:10px;display:flex;list-style-type:none;margin-top:90px;padding-left:0}.legends-content{align-items:center;display:flex}@media (max-width:844px){.plot-contents-container{column-gap:0}.left-main-index{font-size:14px}.main-plot-first-category-index,.main-plot-second-category-index{font-size:13px}.main-plot-column-index-container{padding:5px}.main-plot-column-index{font-size:11px}.main-plot-level-data-container{padding:5px}.main-plot-svg{height:15px;width:15px}.main-plot-level{font-size:12px;margin-right:6px}.main-plot-active{r:6}.main-plot-upgrade-a{r:6;stroke-width:.5px}.main-plot-upgrade-b{r:3}}::-webkit-scrollbar{height:8px;width:10px}::-webkit-scrollbar-track{background:#f1f1f1}::-webkit-scrollbar-thumb{background:#888;border-radius:999px}::-webkit-scrollbar-thumb:hover{background:#555}
-/*# sourceMappingURL=main.99a8c608.css.map*/
+.plot-container{padding:10px}.plot-contents-container{align-items:center;column-gap:30px;display:flex;overflow:auto;width:calc(100% - 1px)}.main-plot-container{align-items:flex-end;display:flex;flex-direction:column;width:100%}.left-main-index{font-weight:700;margin-bottom:auto;margin-top:auto;transform:rotate(-180deg);writing-mode:vertical-lr}.main-plot-column-container{list-style-type:none;width:calc(94% - 1px)}.main-plot-column-name{font-weight:700;margin-bottom:30px;text-align:center}.main-plot-column-index-container{border:1px solid;border-radius:6px;box-shadow:0 2px 8px 0 #63636333;display:flex;padding:15px;width:100%}.main-plot-column-index{align-items:center;display:flex;justify-content:center;width:100%}.main-plot-first-category-container{display:flex;width:inherit}.main-plot-first-category-index{font-weight:600;margin-bottom:auto;margin-top:auto;transform:rotate(-180deg);white-space:nowrap;width:-webkit-fit-content;width:-moz-fit-content;width:fit-content;writing-mode:vertical-lr}.main-plot-first-category-contents-container{list-style-type:none;padding-left:10px;width:inherit}.main-plot-level-data-container{border:1px solid;border-radius:6px;box-shadow:0 2px 8px 0 #63636333;display:flex;justify-content:space-between;margin-bottom:10px;padding:15px;width:calc(100% - 1px)}.main-plot-level{line-height:40px;text-align:center;white-space:nowrap}.main-plot-data{align-items:center;cursor:pointer;display:flex;justify-content:center;width:-webkit-fit-content;width:-moz-fit-content;width:fit-content}.main-plot-second-category-container{display:flex;width:inherit}.main-plot-second-category-index{font-weight:600;margin-bottom:auto;margin-top:auto;transform:rotate(-180deg);white-space:nowrap;width:-webkit-fit-content;width:-moz-fit-content;width:fit-content;writing-mode:vertical-lr}.main-plot-second-category-contents-container{list-style-type:none;margin-top:30px;padding-left:10px;width:inherit}.main-plot-third-category-container{display:flex;width:inherit}.main-plot-third-category-index{font-weight:600;margin-bottom:auto;margin-top:auto;transform:rotate(-180deg);white-space:nowrap;width:-webkit-fit-content;width:-moz-fit-content;width:fit-content;writing-mode:vertical-lr}.main-plot-third-category-contents-container{list-style-type:none;margin-top:30px;padding-left:10px;width:inherit}.legends-container{column-gap:10px;display:flex;list-style-type:none;margin-top:90px;padding-left:0}.legends-content{align-items:center;display:flex}@media (max-width:844px){.plot-contents-container{column-gap:0}.left-main-index{font-size:14px}.main-plot-first-category-index,.main-plot-second-category-index,.main-plot-third-category-index{font-size:13px}.main-plot-column-index-container{padding:5px}.main-plot-column-index{font-size:11px}.main-plot-level-data-container{padding:5px}.main-plot-svg{height:15px;width:15px}.main-plot-level{font-size:12px;margin-right:6px}.main-plot-active{r:6}.main-plot-upgrade-a{r:6;stroke-width:.5px}.main-plot-upgrade-b{r:3}}::-webkit-scrollbar{height:8px;width:10px}::-webkit-scrollbar-track{background:#f1f1f1}::-webkit-scrollbar-thumb{background:#888;border-radius:999px}::-webkit-scrollbar-thumb:hover{background:#555}
+/*# sourceMappingURL=main.80661064.css.map*/
```

### Comparing `custom-dot-plot-0.0.6/custom_dot_plot/frontend/build/static/css/main.99a8c608.css.map` & `custom-dot-plot-0.0.7/custom_dot_plot/frontend/build/static/css/main.80661064.css.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7857142857142857%*

 * *Differences: {"'file'": "'static/css/main.80661064.css'",*

 * * "'mappings'": "'AAAA,gBACI,YACJ,CAEA,yBAEI,kBAAmB,CACnB,eAAgB,CAFhB,YAAa,CAKb,aAAc,CADd,sBAGJ,CAEA,qBAII,oBAAqB,CAFrB,YAAa,CACb,qBAAsB,CAFtB,UAIJ,CAEA,iBAII,eAAgB,CAFhB,kBAAmB,CADnB,eAAgB,CAIhB,yBAA0B,CAF1B,wBAGJ,CAEA,4BACI,oBAAqB,CACrB,qBACJ,CAEA,uBAGI,eAAgB,CAFhB,kBAAmB,CACnB,iBAEJ,CAEA,kCAMI,gBAAiB,CADjB,iBAAkB,CAFlB,gCAAiD,CAFjD,YAAa,CAGb,YAAa,CAFb,UAKJ,CAEA,wBAEI,kBAAmB,CADnB,YAAa,CAEb,sBAAuB,CACvB,UAIJ,CAEA,oCACI,YAAa,CACb,aACJ,CAEA,gCAOI,eAAgB,CAHhB,kBAAm […]*

```diff
@@ -1,13 +1,13 @@
 {
-    "file": "static/css/main.99a8c608.css",
-    "mappings": "AAAA,gBACI,YACJ,CAEA,yBAEI,kBAAmB,CACnB,eAAgB,CAFhB,YAAa,CAKb,aAAc,CADd,sBAGJ,CAEA,qBAII,oBAAqB,CAFrB,YAAa,CACb,qBAAsB,CAFtB,UAIJ,CAEA,iBAII,eAAgB,CAFhB,kBAAmB,CADnB,eAAgB,CAIhB,yBAA0B,CAF1B,wBAGJ,CAEA,4BACI,oBAAqB,CACrB,qBACJ,CAEA,uBAGI,eAAgB,CAFhB,kBAAmB,CACnB,iBAEJ,CAEA,kCAMI,gBAAiB,CADjB,iBAAkB,CAFlB,gCAAiD,CAFjD,YAAa,CAGb,YAAa,CAFb,UAKJ,CAEA,wBAEI,kBAAmB,CADnB,YAAa,CAEb,sBAAuB,CACvB,UAIJ,CAEA,oCACI,YAAa,CACb,aACJ,CAEA,gCAOI,eAAgB,CAHhB,kBAAmB,CADnB,eAAgB,CADhB,yBAA0B,CAI1B,kBAAmB,CADnB,yBAAkB,CAAlB,sBAAkB,CAAlB,iBAAkB,CAJlB,wBAOJ,CAEA,6CAEI,oBAAqB,CADrB,iBAAkB,CAElB,aACJ,CAEA,gCAQI,gBAAiB,CADjB,iBAAkB,CAFlB,gCAAiD,CAHjD,YAAa,CACb,6BAA8B,CAC9B,kBAAmB,CAEnB,YAAa,CALb,sBAQJ,CAEA,iBAII,gBAAiB,CADjB,iBAAkB,CADlB,kBAGJ,CAEA,gBAGI,kBAAmB,CAEnB,cAAe,CAJf,YAAa,CACb,sBAAuB,CAEvB,yBAAkB,CAAlB,sBAAkB,CAAlB,iBAEJ,CAEA,qCACI,YAAa,CACb,aACJ,CAEA,iCAOI,eAAgB,CAHhB,kBAAmB,CADnB,eAAgB,CADhB,yBAA0B,CAI1B,kBAAmB,CADnB,yBAAkB,CAAlB,sBAAkB,CAAlB,iBAAkB,CAJlB,wBAOJ,CAEA,8CAEI,oBAAqB,CACrB,eAAgB,CAFhB,iBAAkB,CAGlB,aACJ,CAEA,oCACI,YACJ,CAEA,gCAOI,eAAgB,CAHhB,kBAAmB,CADnB,eAAgB,CADhB,yBAA0B,CAI1B,kBAAmB,CADnB,yBAAkB,CAAlB,sBAAkB,CAAlB,iBAAkB,CAJlB,wBAOJ,CAEA,6CAEI,oBAAqB,CACrB,eAAgB,CAFhB,iBAGJ,CAEA,mBAEI,eAAgB,CADhB,YAAa,CAEb,oBAAqB,CAErB,eAAgB,CADhB,cAEJ,CAEA,iBAEI,kBAAmB,CADnB,YAEJ,CAGA,yBAEI,yBACI,YACJ,CAEA,iBACI,cACJ,CAMA,iEACI,cACJ,CAEA,kCACI,WACJ,CAEA,wBACI,cACJ,CAEA,gCACI,WACJ,CAEA,eAEI,WAAY,CADZ,UAEJ,CAEA,iBACI,cAAe,CACf,gBACJ,CAEA,kBACI,GACJ,CAEA,qBACI,GAAI,CACJ,iBACJ,CAEA,qBACI,GACJ,CACJ,CAIA,oBAEI,UAAW,CADX,UAGJ,CAIA,0BACI,kBACJ,CAGA,0BACI,eAAgB,CAChB,mBACJ,CAGA,gCACI,eACJ",
+    "file": "static/css/main.80661064.css",
+    "mappings": "AAAA,gBACI,YACJ,CAEA,yBAEI,kBAAmB,CACnB,eAAgB,CAFhB,YAAa,CAKb,aAAc,CADd,sBAGJ,CAEA,qBAII,oBAAqB,CAFrB,YAAa,CACb,qBAAsB,CAFtB,UAIJ,CAEA,iBAII,eAAgB,CAFhB,kBAAmB,CADnB,eAAgB,CAIhB,yBAA0B,CAF1B,wBAGJ,CAEA,4BACI,oBAAqB,CACrB,qBACJ,CAEA,uBAGI,eAAgB,CAFhB,kBAAmB,CACnB,iBAEJ,CAEA,kCAMI,gBAAiB,CADjB,iBAAkB,CAFlB,gCAAiD,CAFjD,YAAa,CAGb,YAAa,CAFb,UAKJ,CAEA,wBAEI,kBAAmB,CADnB,YAAa,CAEb,sBAAuB,CACvB,UAIJ,CAEA,oCACI,YAAa,CACb,aACJ,CAEA,gCAOI,eAAgB,CAHhB,kBAAmB,CADnB,eAAgB,CADhB,yBAA0B,CAI1B,kBAAmB,CADnB,yBAAkB,CAAlB,sBAAkB,CAAlB,iBAAkB,CAJlB,wBAOJ,CAEA,6CAEI,oBAAqB,CADrB,iBAAkB,CAElB,aACJ,CAEA,gCAQI,gBAAiB,CADjB,iBAAkB,CAFlB,gCAAiD,CAHjD,YAAa,CACb,6BAA8B,CAC9B,kBAAmB,CAEnB,YAAa,CALb,sBAQJ,CAEA,iBAII,gBAAiB,CADjB,iBAAkB,CADlB,kBAGJ,CAEA,gBAGI,kBAAmB,CAEnB,cAAe,CAJf,YAAa,CACb,sBAAuB,CAEvB,yBAAkB,CAAlB,sBAAkB,CAAlB,iBAEJ,CAEA,qCACI,YAAa,CACb,aACJ,CAEA,iCAOI,eAAgB,CAHhB,kBAAmB,CADnB,eAAgB,CADhB,yBAA0B,CAI1B,kBAAmB,CADnB,yBAAkB,CAAlB,sBAAkB,CAAlB,iBAAkB,CAJlB,wBAOJ,CAEA,8CAEI,oBAAqB,CACrB,eAAgB,CAFhB,iBAAkB,CAGlB,aACJ,CAEA,oCACI,YAAa,CACb,aACJ,CAEA,gCAOI,eAAgB,CAHhB,kBAAmB,CADnB,eAAgB,CADhB,yBAA0B,CAI1B,kBAAmB,CADnB,yBAAkB,CAAlB,sBAAkB,CAAlB,iBAAkB,CAJlB,wBAOJ,CAEA,6CAEI,oBAAqB,CACrB,eAAgB,CAFhB,iBAAkB,CAGlB,aACJ,CAEA,mBAEI,eAAgB,CADhB,YAAa,CAEb,oBAAqB,CAErB,eAAgB,CADhB,cAEJ,CAEA,iBAEI,kBAAmB,CADnB,YAEJ,CAGA,yBAEI,yBACI,YACJ,CAEA,iBACI,cACJ,CAUA,iGACI,cACJ,CAEA,kCACI,WACJ,CAEA,wBACI,cACJ,CAEA,gCACI,WACJ,CAEA,eAEI,WAAY,CADZ,UAEJ,CAEA,iBACI,cAAe,CACf,gBACJ,CAEA,kBACI,GACJ,CAEA,qBACI,GAAI,CACJ,iBACJ,CAEA,qBACI,GACJ,CACJ,CAIA,oBAEI,UAAW,CADX,UAGJ,CAIA,0BACI,kBACJ,CAGA,0BACI,eAAgB,CAChB,mBACJ,CAGA,gCACI,eACJ",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "style.css"
     ],
     "sourcesContent": [
-        ".plot-container {\r\n    padding: 10px;\r\n}\r\n\r\n.plot-contents-container {\r\n    display: flex;\r\n    align-items: center;\r\n    column-gap: 30px;\r\n    /* width: calc(109% - 1px); */\r\n    width: calc(100% - 1px);\r\n    overflow: auto;\r\n\r\n}\r\n\r\n.main-plot-container {\r\n    width: 100%;\r\n    display: flex;\r\n    flex-direction: column;\r\n    align-items: flex-end;\r\n}\r\n\r\n.left-main-index {\r\n    margin-top: auto;\r\n    margin-bottom: auto;\r\n    writing-mode: vertical-lr;\r\n    font-weight: 700;\r\n    transform: rotate(-180deg);\r\n}\r\n\r\n.main-plot-column-container {\r\n    list-style-type: none;\r\n    width: calc(94% - 1px);\r\n}\r\n\r\n.main-plot-column-name {\r\n    margin-bottom: 30px;\r\n    text-align: center;\r\n    font-weight: 700;\r\n}\r\n\r\n.main-plot-column-index-container {\r\n    display: flex;\r\n    width: 100%;\r\n    box-shadow: rgba(99, 99, 99, 0.2) 0px 2px 8px 0px;\r\n    padding: 15px;\r\n    border-radius: 6px;\r\n    border: solid 1px;\r\n}\r\n\r\n.main-plot-column-index {\r\n    display: flex;\r\n    align-items: center;\r\n    justify-content: center;\r\n    width: 100%;\r\n    /* width: 20%; */\r\n    /* text-align: center; */\r\n    /* line-height: 40px; */\r\n}\r\n\r\n.main-plot-first-category-container {\r\n    display: flex;\r\n    width: inherit;\r\n}\r\n\r\n.main-plot-first-category-index {\r\n    writing-mode: vertical-lr;\r\n    transform: rotate(-180deg);\r\n    margin-top: auto;\r\n    margin-bottom: auto;\r\n    width: fit-content;\r\n    white-space: nowrap;\r\n    font-weight: 600;\r\n}\r\n\r\n.main-plot-first-category-contents-container {\r\n    padding-left: 10px;\r\n    list-style-type: none;\r\n    width: inherit;\r\n}\r\n\r\n.main-plot-level-data-container {\r\n    width: calc(100% - 1px);\r\n    display: flex;\r\n    justify-content: space-between;\r\n    margin-bottom: 10px;\r\n    box-shadow: rgba(99, 99, 99, 0.2) 0px 2px 8px 0px;\r\n    padding: 15px;\r\n    border-radius: 6px;\r\n    border: solid 1px;\r\n}\r\n\r\n.main-plot-level {\r\n    /* margin-right: 30px; */\r\n    white-space: nowrap;\r\n    text-align: center;\r\n    line-height: 40px;\r\n}\r\n\r\n.main-plot-data {\r\n    display: flex;\r\n    justify-content: center;\r\n    align-items: center;\r\n    width: fit-content;\r\n    cursor: pointer;\r\n}\r\n\r\n.main-plot-second-category-container {\r\n    display: flex;\r\n    width: inherit;\r\n}\r\n\r\n.main-plot-second-category-index {\r\n    writing-mode: vertical-lr;\r\n    transform: rotate(-180deg);\r\n    margin-top: auto;\r\n    margin-bottom: auto;\r\n    width: fit-content;\r\n    white-space: nowrap;\r\n    font-weight: 600;\r\n}\r\n\r\n.main-plot-second-category-contents-container {\r\n    padding-left: 10px;\r\n    list-style-type: none;\r\n    margin-top: 30px;\r\n    width: inherit;\r\n}\r\n\r\n.main-plot-third-category-container {\r\n    display: flex;\r\n}\r\n\r\n.main-plot-third-category-index {\r\n    writing-mode: vertical-lr;\r\n    transform: rotate(-180deg);\r\n    margin-top: auto;\r\n    margin-bottom: auto;\r\n    width: fit-content;\r\n    white-space: nowrap;\r\n    font-weight: 600;\r\n}\r\n\r\n.main-plot-third-category-contents-container {\r\n    padding-left: 10px;\r\n    list-style-type: none;\r\n    margin-top: 30px;\r\n}\r\n\r\n.legends-container {\r\n    display: flex;\r\n    column-gap: 10px;\r\n    list-style-type: none;\r\n    padding-left: 0px;\r\n    margin-top: 90px;\r\n}\r\n\r\n.legends-content {\r\n    display: flex;\r\n    align-items: center;\r\n}\r\n\r\n\r\n@media (max-width: 844px) {\r\n\r\n    .plot-contents-container {\r\n        column-gap: 0px;\r\n    }\r\n\r\n    .left-main-index {\r\n        font-size: 14px;\r\n    }\r\n\r\n    .main-plot-first-category-index {\r\n        font-size: 13px;\r\n    }\r\n\r\n    .main-plot-second-category-index {\r\n        font-size: 13px;\r\n    }\r\n\r\n    .main-plot-column-index-container {\r\n        padding: 5px;\r\n    }\r\n\r\n    .main-plot-column-index {\r\n        font-size: 11px;\r\n    }\r\n\r\n    .main-plot-level-data-container {\r\n        padding: 5px;\r\n    }\r\n\r\n    .main-plot-svg {\r\n        width: 15px;\r\n        height: 15px;\r\n    }\r\n\r\n    .main-plot-level {\r\n        font-size: 12px;\r\n        margin-right: 6px;\r\n    }\r\n\r\n    .main-plot-active {\r\n        r: 6;\r\n    }\r\n\r\n    .main-plot-upgrade-a {\r\n        r: 6;\r\n        stroke-width: .5px;\r\n    }\r\n\r\n    .main-plot-upgrade-b {\r\n        r: 3;\r\n    }\r\n}\r\n\r\n\r\n/* width */\r\n::-webkit-scrollbar {\r\n    width: 10px;\r\n    height: 8px;\r\n\r\n}\r\n\r\n\r\n/* Track */\r\n::-webkit-scrollbar-track {\r\n    background: #f1f1f1;\r\n}\r\n\r\n/* Handle */\r\n::-webkit-scrollbar-thumb {\r\n    background: #888;\r\n    border-radius: 999px;\r\n}\r\n\r\n/* Handle on hover */\r\n::-webkit-scrollbar-thumb:hover {\r\n    background: #555;\r\n}"
+        ".plot-container {\r\n    padding: 10px;\r\n}\r\n\r\n.plot-contents-container {\r\n    display: flex;\r\n    align-items: center;\r\n    column-gap: 30px;\r\n    /* width: calc(109% - 1px); */\r\n    width: calc(100% - 1px);\r\n    overflow: auto;\r\n\r\n}\r\n\r\n.main-plot-container {\r\n    width: 100%;\r\n    display: flex;\r\n    flex-direction: column;\r\n    align-items: flex-end;\r\n}\r\n\r\n.left-main-index {\r\n    margin-top: auto;\r\n    margin-bottom: auto;\r\n    writing-mode: vertical-lr;\r\n    font-weight: 700;\r\n    transform: rotate(-180deg);\r\n}\r\n\r\n.main-plot-column-container {\r\n    list-style-type: none;\r\n    width: calc(94% - 1px);\r\n}\r\n\r\n.main-plot-column-name {\r\n    margin-bottom: 30px;\r\n    text-align: center;\r\n    font-weight: 700;\r\n}\r\n\r\n.main-plot-column-index-container {\r\n    display: flex;\r\n    width: 100%;\r\n    box-shadow: rgba(99, 99, 99, 0.2) 0px 2px 8px 0px;\r\n    padding: 15px;\r\n    border-radius: 6px;\r\n    border: solid 1px;\r\n}\r\n\r\n.main-plot-column-index {\r\n    display: flex;\r\n    align-items: center;\r\n    justify-content: center;\r\n    width: 100%;\r\n    /* width: 20%; */\r\n    /* text-align: center; */\r\n    /* line-height: 40px; */\r\n}\r\n\r\n.main-plot-first-category-container {\r\n    display: flex;\r\n    width: inherit;\r\n}\r\n\r\n.main-plot-first-category-index {\r\n    writing-mode: vertical-lr;\r\n    transform: rotate(-180deg);\r\n    margin-top: auto;\r\n    margin-bottom: auto;\r\n    width: fit-content;\r\n    white-space: nowrap;\r\n    font-weight: 600;\r\n}\r\n\r\n.main-plot-first-category-contents-container {\r\n    padding-left: 10px;\r\n    list-style-type: none;\r\n    width: inherit;\r\n}\r\n\r\n.main-plot-level-data-container {\r\n    width: calc(100% - 1px);\r\n    display: flex;\r\n    justify-content: space-between;\r\n    margin-bottom: 10px;\r\n    box-shadow: rgba(99, 99, 99, 0.2) 0px 2px 8px 0px;\r\n    padding: 15px;\r\n    border-radius: 6px;\r\n    border: solid 1px;\r\n}\r\n\r\n.main-plot-level {\r\n    /* margin-right: 30px; */\r\n    white-space: nowrap;\r\n    text-align: center;\r\n    line-height: 40px;\r\n}\r\n\r\n.main-plot-data {\r\n    display: flex;\r\n    justify-content: center;\r\n    align-items: center;\r\n    width: fit-content;\r\n    cursor: pointer;\r\n}\r\n\r\n.main-plot-second-category-container {\r\n    display: flex;\r\n    width: inherit;\r\n}\r\n\r\n.main-plot-second-category-index {\r\n    writing-mode: vertical-lr;\r\n    transform: rotate(-180deg);\r\n    margin-top: auto;\r\n    margin-bottom: auto;\r\n    width: fit-content;\r\n    white-space: nowrap;\r\n    font-weight: 600;\r\n}\r\n\r\n.main-plot-second-category-contents-container {\r\n    padding-left: 10px;\r\n    list-style-type: none;\r\n    margin-top: 30px;\r\n    width: inherit;\r\n}\r\n\r\n.main-plot-third-category-container {\r\n    display: flex;\r\n    width: inherit;\r\n}\r\n\r\n.main-plot-third-category-index {\r\n    writing-mode: vertical-lr;\r\n    transform: rotate(-180deg);\r\n    margin-top: auto;\r\n    margin-bottom: auto;\r\n    width: fit-content;\r\n    white-space: nowrap;\r\n    font-weight: 600;\r\n}\r\n\r\n.main-plot-third-category-contents-container {\r\n    padding-left: 10px;\r\n    list-style-type: none;\r\n    margin-top: 30px;\r\n    width: inherit;\r\n}\r\n\r\n.legends-container {\r\n    display: flex;\r\n    column-gap: 10px;\r\n    list-style-type: none;\r\n    padding-left: 0px;\r\n    margin-top: 90px;\r\n}\r\n\r\n.legends-content {\r\n    display: flex;\r\n    align-items: center;\r\n}\r\n\r\n\r\n@media (max-width: 844px) {\r\n\r\n    .plot-contents-container {\r\n        column-gap: 0px;\r\n    }\r\n\r\n    .left-main-index {\r\n        font-size: 14px;\r\n    }\r\n\r\n    .main-plot-first-category-index {\r\n        font-size: 13px;\r\n    }\r\n\r\n    .main-plot-second-category-index {\r\n        font-size: 13px;\r\n    }\r\n\r\n    .main-plot-third-category-index {\r\n        font-size: 13px;\r\n    }\r\n\r\n    .main-plot-column-index-container {\r\n        padding: 5px;\r\n    }\r\n\r\n    .main-plot-column-index {\r\n        font-size: 11px;\r\n    }\r\n\r\n    .main-plot-level-data-container {\r\n        padding: 5px;\r\n    }\r\n\r\n    .main-plot-svg {\r\n        width: 15px;\r\n        height: 15px;\r\n    }\r\n\r\n    .main-plot-level {\r\n        font-size: 12px;\r\n        margin-right: 6px;\r\n    }\r\n\r\n    .main-plot-active {\r\n        r: 6;\r\n    }\r\n\r\n    .main-plot-upgrade-a {\r\n        r: 6;\r\n        stroke-width: .5px;\r\n    }\r\n\r\n    .main-plot-upgrade-b {\r\n        r: 3;\r\n    }\r\n}\r\n\r\n\r\n/* width */\r\n::-webkit-scrollbar {\r\n    width: 10px;\r\n    height: 8px;\r\n\r\n}\r\n\r\n\r\n/* Track */\r\n::-webkit-scrollbar-track {\r\n    background: #f1f1f1;\r\n}\r\n\r\n/* Handle */\r\n::-webkit-scrollbar-thumb {\r\n    background: #888;\r\n    border-radius: 999px;\r\n}\r\n\r\n/* Handle on hover */\r\n::-webkit-scrollbar-thumb:hover {\r\n    background: #555;\r\n}"
     ],
     "version": 3
 }
```

### Comparing `custom-dot-plot-0.0.6/custom_dot_plot/frontend/build/static/js/main.618d6894.js` & `custom-dot-plot-0.0.7/custom_dot_plot/frontend/build/static/js/main.618d6894.js`

 * *Files identical despite different names*

### Comparing `custom-dot-plot-0.0.6/custom_dot_plot/frontend/build/static/js/main.618d6894.js.LICENSE.txt` & `custom-dot-plot-0.0.7/custom_dot_plot/frontend/build/static/js/main.618d6894.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `custom-dot-plot-0.0.6/custom_dot_plot/frontend/build/static/js/main.618d6894.js.map` & `custom-dot-plot-0.0.7/custom_dot_plot/frontend/build/static/js/main.618d6894.js.map`

 * *Files identical despite different names*

### Comparing `custom-dot-plot-0.0.6/custom_dot_plot.egg-info/SOURCES.txt` & `custom-dot-plot-0.0.7/custom_dot_plot.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 custom_dot_plot.egg-info/dependency_links.txt
 custom_dot_plot.egg-info/requires.txt
 custom_dot_plot.egg-info/top_level.txt
 custom_dot_plot/frontend/build/asset-manifest.json
 custom_dot_plot/frontend/build/bootstrap.min.css
 custom_dot_plot/frontend/build/bootstrap.min.css.map
 custom_dot_plot/frontend/build/index.html
-custom_dot_plot/frontend/build/static/css/main.99a8c608.css
-custom_dot_plot/frontend/build/static/css/main.99a8c608.css.map
+custom_dot_plot/frontend/build/static/css/main.80661064.css
+custom_dot_plot/frontend/build/static/css/main.80661064.css.map
 custom_dot_plot/frontend/build/static/js/main.618d6894.js
 custom_dot_plot/frontend/build/static/js/main.618d6894.js.LICENSE.txt
 custom_dot_plot/frontend/build/static/js/main.618d6894.js.map
```

### Comparing `custom-dot-plot-0.0.6/setup.py` & `custom-dot-plot-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="custom-dot-plot",
-    version="0.0.6",
+    version="0.0.7",
     author="",
     author_email="", 
     # description="Streamlit component that allows you to do X",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

