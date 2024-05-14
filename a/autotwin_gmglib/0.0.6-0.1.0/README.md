# Comparing `tmp/autotwin_gmglib-0.0.6.tar.gz` & `tmp/autotwin_gmglib-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotwin_gmglib-0.0.6.tar", max compression
+gzip compressed data, was "autotwin_gmglib-0.1.0.tar", max compression
```

## Comparing `autotwin_gmglib-0.0.6.tar` & `autotwin_gmglib-0.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    58387 2024-03-15 15:29:01.992544 autotwin_gmglib-0.0.6/autotwin_gmglib.py
--rw-r--r--   0        0        0     1518 2024-03-12 18:24:24.440595 autotwin_gmglib-0.0.6/LICENSE
--rw-r--r--   0        0        0      912 2024-03-15 16:38:18.777545 autotwin_gmglib-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      643 2024-03-12 18:24:24.440595 autotwin_gmglib-0.0.6/README.md
--rw-r--r--   0        0        0     1649 1970-01-01 00:00:00.000000 autotwin_gmglib-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    68786 2024-05-14 08:37:20.000000 autotwin_gmglib-0.1.0/autotwin_gmglib.py
+-rw-r--r--   0        0        0     1518 2024-03-12 18:24:26.000000 autotwin_gmglib-0.1.0/LICENSE
+-rw-r--r--   0        0        0      931 2024-05-14 08:57:00.000000 autotwin_gmglib-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      643 2024-03-12 18:24:26.000000 autotwin_gmglib-0.1.0/README.md
+-rw-r--r--   0        0        0     1688 1970-01-01 00:00:00.000000 autotwin_gmglib-0.1.0/PKG-INFO
```

### Comparing `autotwin_gmglib-0.0.6/autotwin_gmglib.py` & `autotwin_gmglib-0.1.0/autotwin_gmglib.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 import time
 import networkx
 import numpy
 import matplotlib.pyplot as mpyplot
 import matplotlib.colors as mcolors
 import matplotlib.patches as mpatches
 import matplotlib.backend_bases as mbackend
+import matplotlib.widgets as mwidgets
+import threading
+import warnings
+import bisect
+import scipy
+import math
 
 pandas.options.mode.copy_on_write = False
 mpyplot.rcParams["pdf.fonttype"] = 42
 mpyplot.rcParams["ps.fonttype"] = 42
 
 
 ###############################################################################
@@ -176,198 +182,257 @@
 
 
 def show_model(
     model: networkx.DiGraph,
     layout: Callable[[networkx.DiGraph], dict[str, numpy.ndarray]]
     = lambda g: networkx.nx_agraph.graphviz_layout(g, prog="circo"),
 ):
-    """Show a graph model in a figure window.
+    """Show a graph model in interactive figures.
 
     Args:
         model: Graph model.
         layout: Layout function.
     """
     name = model.graph["name"]
     version = model.graph["version"]
-    title = name + " " + version if version else name
 
     stations = list(model.nodes.keys())
     station_flows = dict()
     for station in stations:
         operation = model.nodes[station]["operation"]
         formulas = model.nodes[station]["formulas"]
         if operation in {"ORDINARY", "DETACH"}:
-            flow = []
+            flow = list()
             for formula in formulas:
                 type_ = next(iter(formula["input"].keys()))
                 major = type_.split("_")[0]
                 if major not in flow:
                     flow.append(major)
             flow.sort()
             flow = "|".join(flow)
         elif operation == "ATTACH":
-            flow = []
+            flow = list()
             for formula in formulas:
                 type_ = next(iter(formula["output"].keys()))
                 major = type_.split("_")[0]
                 if major not in flow:
                     flow.append(major)
             flow.sort()
             flow = "|".join(flow)
         else:
             flow = None
         station_flows[station] = flow
 
     connections = list(model.edges.keys())
     connection_flows = dict()
     for connection in connections:
-        flow = []
-        transfer_times = model.edges[connection]["transfer_times"]
-        for type_ in transfer_times.keys():
+        flow = list()
+        routing_probabilities = model.edges[connection]["routing_probabilities"]
+        for type_ in routing_probabilities.keys():
             major = type_.split("_")[0]
             if major not in flow:
                 flow.append(major)
         flow.sort()
         flow = "|".join(flow)
         connection_flows[connection] = flow
 
-    flows = []
+    flows = list()
     for flow in station_flows.values():
         if flow not in flows:
             flows.append(flow)
     for flow in connection_flows.values():
         if flow not in flows:
             flows.append(flow)
     if None in flows:
         flows.remove(None)
     flows.sort()
 
-    mpyplot.title(title, fontsize=10)
+    figure, axes = mpyplot.subplots()
+    window_title = "Graph Model"
+    figure.canvas.manager.set_window_title(window_title)
+    axes_title = name + " (" + version + ")" if version else name
+    axes.set_title(axes_title, fontsize=10.0)
     pos = layout(model)
     cmap = mpyplot.get_cmap("gist_rainbow")
     white = mcolors.to_rgba_array("white")
     black = mcolors.to_rgba_array("black")
     colors = cmap(numpy.linspace(0.0, 1.0, len(flows)))
     flow_colors = dict()
     for x in range(len(flows)):
         flow_colors[flows[x]] = colors[x].reshape(1, -1)
 
-    paths = []
+    paths = list()
     for station in stations:
         flow = station_flows[station]
         if flow is None:
             color = white
         else:
             color = flow_colors[flow]
         path = networkx.draw_networkx_nodes(
             model, pos, nodelist=[station], node_color=color, edgecolors=black
         )
         paths.append(path)
 
-    patches = []
+    patches = list()
     for connection in connections:
         flow = connection_flows[connection]
         if flow is None:
             color = white
         else:
             color = flow_colors[flow]
         patch = networkx.draw_networkx_edges(
             model, pos, edgelist=[connection], edge_color=color, arrowsize=20
         )
         patch[0].set_edgecolor(black)
         patches.append(patch[0])
 
-    networkx.draw_networkx_labels(model, pos, font_size=8)
+    networkx.draw_networkx_labels(model, pos, font_size=8.0)
 
-    handles = []
-    labels = []
+    handles = list()
+    labels = list()
     for flow in flows:
         color = flow_colors[flow]
-        handles.append(mpatches.Rectangle((0, 0), 0, 0, color=color))
+        handles.append(mpatches.Rectangle((0.0, 0.0), 0.0, 0.0, color=color))
         labels.append(flow)
-    mpyplot.legend(handles, labels, fontsize=8, title="Flow", title_fontsize=8)
+    axes.legend(handles, labels, fontsize=8, title="Flow", title_fontsize=8)
 
-    annotation = mpyplot.annotate(
+    focus = None
+    lock = threading.Lock()
+    annotation = axes.annotate(
         "",
         xy=(0.0, 0.0),
         xytext=(0.0, 0.0),
         textcoords="offset points",
-        arrowprops={"arrowstyle": "-"},
+        arrowprops={"arrowstyle": "-", "linestyle": "--"},
+        bbox={"boxstyle": "round", "edgecolor": "lightgray", "facecolor": "white"},
+        fontsize=8.0,
         multialignment="left",
-        bbox={"boxstyle": "round", "facecolor": "white"},
-        fontsize=8,
         visible=False,
-        zorder=6,
+        zorder=6.0,
     )
+    cdf_figure_num = 0
+    cdf_focus = None
+    cdf_index = 0
 
     def handle_mouse_motion(event: mbackend.MouseEvent):
-        """Handle a mouse motion in a figure window.
+        """Handle a mouse motion in the main figure.
 
         Args:
             event: Mouse motion event.
         """
+        nonlocal focus
+        nonlocal cdf_figure_num
+        nonlocal cdf_focus
+        nonlocal cdf_index
         is_inside = False
         text = ""
         for x_ in range(len(paths)):
             if is_inside:
                 break
             is_inside, _ = paths[x_].contains(event)
             if is_inside:
                 station_ = stations[x_]
+                with lock:
+                    if focus == station_:
+                        return
+                    focus = station_
                 attributes = model.nodes[station_]
                 annotation.xy = pos[station_]
                 text += "Station: " + str(station_) + "\n"
                 text += "Operation: "
                 text += get_display_text(attributes["operation"], 1) + "\n"
                 text += "Formulas: "
                 text += get_display_text(attributes["formulas"], 1) + "\n"
                 text += "Buffer Capacities: "
                 text += get_display_text(attributes["buffer_capacities"], 1) + "\n"
                 text += "Machine Capacity: "
                 text += get_display_text(attributes["machine_capacity"], 1) + "\n"
                 text += "Processing Times: "
                 text += get_display_text(attributes["processing_times"], 1)
+                if not mpyplot.fignum_exists(cdf_figure_num):
+                    cdf_figure_num = create_cdf_figure()
+                cdf_axes = mpyplot.figure(num=cdf_figure_num).axes[0]
+                if len(cdf_axes.lines) > 2:
+                    cdf_axes.lines[2].remove()
+                cdf_axes_title = (
+                    "Processing Time CDF of Formula 1 at Station " + station_
+                )
+                cdf_axes.set_title(cdf_axes_title, fontsize=10.0)
+                cdf = attributes["processing_times"][0]["cdf"]
+                warnings.simplefilter("ignore", category=UserWarning)
+                cdf_axes.set_xlim(left=cdf[0][0], right=cdf[-1][0])
+                warnings.simplefilter("default", category=UserWarning)
+                cdf_axes.set_ylim(bottom=0.0, top=1.2)
+                cdf_axes.step(*zip(*cdf), where="post", color="tab:blue", linewidth=1.0)
+                cdf_focus = station_
+                cdf_index = 0
         for x_ in range(len(patches)):
             if is_inside:
                 break
-            is_inside, _ = patches[x_].contains(event, radius=5)
+            is_inside, _ = patches[x_].contains(event, radius=5.0)
             if is_inside:
                 connection_ = connections[x_]
+                with lock:
+                    if focus == connection_:
+                        return
+                    focus = connection_
                 attributes = model.edges[connection_]
                 origin_xy = pos[connection_[0]]
                 destination_xy = pos[connection_[1]]
                 annotation.xy = (
                     (origin_xy[0] + destination_xy[0]) / 2,
                     (origin_xy[1] + destination_xy[1]) / 2,
                 )
                 text += "Origin Station: " + str(connection_[0]) + "\n"
                 text += "Destination Station: " + str(connection_[1]) + "\n"
                 text += "Routing Probabilities: "
                 text += get_display_text(attributes["routing_probabilities"], 1) + "\n"
                 text += "Transfer Times: "
                 text += get_display_text(attributes["transfer_times"], 1)
+                if not mpyplot.fignum_exists(cdf_figure_num):
+                    cdf_figure_num = create_cdf_figure()
+                cdf_axes = mpyplot.figure(num=cdf_figure_num).axes[0]
+                if len(cdf_axes.lines) > 2:
+                    cdf_axes.lines[2].remove()
+                types = list(attributes["transfer_times"].keys())
+                cdf_axes_title = (
+                    "Transfer Time CDF of Type " + types[0] + " on Connection ("
+                    + connection_[0] + ", " + connection_[1] + ")"
+                )
+                cdf_axes.set_title(cdf_axes_title, fontsize=10.0)
+                cdf = attributes["transfer_times"][types[0]]["cdf"]
+                warnings.simplefilter("ignore", category=UserWarning)
+                cdf_axes.set_xlim(left=cdf[0][0], right=cdf[-1][0])
+                warnings.simplefilter("default", category=UserWarning)
+                cdf_axes.set_ylim(bottom=0.0, top=1.2)
+                cdf_axes.step(*zip(*cdf), where="post", color="tab:blue", linewidth=1.0)
+                cdf_focus = connection_
+                cdf_index = 0
         if is_inside:
-            point_xy = mpyplot.gca().transData.transform(annotation.xy)
-            center_xy = mpyplot.gcf().transFigure.transform((0.5, 0.5))
+            point_xy = axes.transData.transform(annotation.xy)
+            center_xy = figure.transFigure.transform((0.5, 0.5))
             if point_xy[0] <= center_xy[0]:
                 annotation.set(horizontalalignment="left")
             else:
                 annotation.set(horizontalalignment="right")
             if point_xy[1] <= center_xy[1] - 30.0:
                 annotation.xyann = (0.0, 30.0)
                 annotation.set(verticalalignment="bottom")
             else:
                 annotation.xyann = (0.0, -30.0)
                 annotation.set(verticalalignment="top")
             annotation.set_text(text)
             annotation.set_visible(True)
         else:
+            with lock:
+                focus = None
             if annotation.get_visible():
                 annotation.set_visible(False)
 
+    ignored_keys = {"cdf"}
     display_names = {
         "input": "Input",
         "output": "Output",
         "mean": "Mean",
         "std": "Standard Deviation",
     }
 
@@ -377,36 +442,151 @@
         Args:
             value: Attribute value.
             level: Indent level.
 
         Returns:
             Display text.
         """
+        text = ""
         if isinstance(value, list):
-            text = ""
             for x_ in range(len(value)):
                 x_ += 1
                 y_ = value[x_ - 1]
                 text += "\n" + "     " * level
                 text += str(x_) + ": " + get_display_text(y_, level + 1)
         elif isinstance(value, dict):
-            text = ""
             for x_, y_ in value.items():
+                if x_ in ignored_keys:
+                    continue
                 if x_ in display_names.keys():
                     x_ = display_names[x_]
                 text += "\n" + "     " * level
                 text += str(x_) + ": " + get_display_text(y_, level + 1)
         elif isinstance(value, float) or isinstance(value, numpy.floating):
-            text = f"{value:.2f}"
+            text += f"{value:.2f}"
         else:
-            text = str(value)
+            text += str(value)
         return text
 
+    def create_cdf_figure():
+        """Create a new CDF figure.
+
+        Returns:
+            int: Number of the CDF figure.
+        """
+        cdf_figure, cdf_axes = mpyplot.subplots()
+        cdf_window_title = "Processing/Transfer Time CDF"
+        cdf_figure.canvas.manager.set_window_title(cdf_window_title)
+        cdf_axes.axhline(color="black", linestyle="--", linewidth=1.0, visible=False)
+        cdf_axes.axvline(color="black", linestyle="--", linewidth=1.0, visible=False)
+        cdf_axes.text(
+            0.02,
+            0.975,
+            "",
+            bbox={"boxstyle": "round", "edgecolor": "lightgray", "facecolor": "white"},
+            fontsize=8.0,
+            verticalalignment="top",
+            transform=cdf_axes.transAxes,
+        )
+        cdf_figure.canvas.mpl_connect("motion_notify_event", handle_cdf_mouse_motion)
+        previous_axes = cdf_axes.inset_axes([0.76, 0.9, 0.1, 0.075])
+        previous_axes.button = mwidgets.Button(previous_axes, "Previous")
+        previous_axes.button.label.set_fontsize(8.0)
+        previous_axes.button.on_clicked(handle_cdf_button_click)
+        next_axes = cdf_axes.inset_axes([0.88, 0.9, 0.1, 0.075])
+        next_axes.button = mwidgets.Button(next_axes, "Next")
+        next_axes.button.label.set_fontsize(8)
+        next_axes.button.on_clicked(handle_cdf_button_click)
+        return cdf_figure.number
+
+    def handle_cdf_mouse_motion(event):
+        """Handle a mouse motion in the CDF figure.
+
+        Args:
+            event (mbases.MouseEvent): Mouse motion event.
+        """
+        cdf_axes = mpyplot.figure(num=cdf_figure_num).axes[0]
+        if event.inaxes:
+            cdf_xdata, cdf_ydata = cdf_axes.lines[2].get_data()
+            if event.xdata <= cdf_xdata[0]:
+                x_ = 0
+            else:
+                x_ = bisect.bisect_right(cdf_xdata, event.xdata)
+                x_ = min(x_, len(cdf_xdata) - 1)
+            cdf_axes.lines[0].set_ydata([cdf_ydata[x_]])
+            cdf_axes.lines[1].set_xdata([cdf_xdata[x_]])
+            cdf_axes.lines[0].set_visible(True)
+            cdf_axes.lines[1].set_visible(True)
+            text = ""
+            text += f"Quantile: {cdf_xdata[x_]:.2f}\n"
+            text += f"Probability: {cdf_ydata[x_]:.2f}"
+            cdf_axes.texts[0].set_text(text)
+            cdf_axes.texts[0].set_visible(True)
+        else:
+            if cdf_axes.lines[0].get_visible():
+                cdf_axes.lines[0].set_visible(False)
+            if cdf_axes.lines[1].get_visible():
+                cdf_axes.lines[1].set_visible(False)
+            if cdf_axes.texts[0].get_visible():
+                cdf_axes.texts[0].set_visible(False)
+
+    def handle_cdf_button_click(event):
+        """Handle a button click on the CDF figure.
+
+        Args:
+            event (mbases.MouseEvent): Button click event.
+        """
+        nonlocal cdf_index
+        button = event.inaxes.button
+        if cdf_focus in stations:
+            processing_times = model.nodes[cdf_focus]["processing_times"]
+            if button.label.get_text() == "Previous":
+                if cdf_index <= 0:
+                    return
+                cdf_index -= 1
+            else:
+                if cdf_index >= len(processing_times) - 1:
+                    return
+                cdf_index += 1
+            cdf_axes = mpyplot.figure(num=cdf_figure_num).axes[0]
+            if len(cdf_axes.lines) > 2:
+                cdf_axes.lines[2].remove()
+            cdf = processing_times[cdf_index]["cdf"]
+            cdf_axes_title = (
+                "Processing Time CDF of Formula " + str(cdf_index + 1)
+                + " at Station " + cdf_focus
+            )
+        else:
+            transfer_times = model.edges[cdf_focus[0], cdf_focus[1]]["transfer_times"]
+            types = list(transfer_times.keys())
+            if button.label.get_text() == "Previous":
+                if cdf_index <= 0:
+                    return
+                cdf_index -= 1
+            else:
+                if cdf_index >= len(types) - 1:
+                    return
+                cdf_index += 1
+            cdf_axes = mpyplot.figure(num=cdf_figure_num).axes[0]
+            if len(cdf_axes.lines) > 2:
+                cdf_axes.lines[2].remove()
+            cdf = transfer_times[types[cdf_index]]["cdf"]
+            cdf_axes_title = (
+                "Transfer Time CDF of Type " + types[cdf_index]
+                + " on Connection (" + cdf_focus[0] + ", " + cdf_focus[1] + ")"
+            )
+        cdf_axes.set_title(cdf_axes_title, fontsize=10.0)
+        warnings.simplefilter("ignore", category=UserWarning)
+        cdf_axes.set_xlim(left=cdf[0][0], right=cdf[-1][0])
+        warnings.simplefilter("default", category=UserWarning)
+        cdf_axes.set_ylim(bottom=0.0, top=1.2)
+        cdf_axes.step(*zip(*cdf), where="post", color="tab:blue", linewidth=1.0)
+
+    figure.canvas.mpl_connect("motion_notify_event", handle_mouse_motion)
     mpyplot.ion()
-    mpyplot.connect("motion_notify_event", handle_mouse_motion)
     mpyplot.show(block=True)
 
 
 ###############################################################################
 # Private functions                                                           #
 ###############################################################################
 
@@ -595,15 +775,21 @@
         formulas = attributes["formulas"]
         processing_times = attributes["processing_times"]
         for x in range(len(formulas)):
             formula_id = transaction.run(
                 f"""
                 CREATE (fm:Entity:Resource:Station:Formula)
                 SET fm.processingTimeMean = {processing_times[x]['mean']},
-                    fm.processingTimeStd = {processing_times[x]['std']}
+                    fm.processingTimeStd = {processing_times[x]['std']},
+                    fm.processingTimeCdfX = {
+                        [point[0] for point in processing_times[x]['cdf']]
+                    },
+                    fm.processingTimeCdfY = {
+                        [point[1] for point in processing_times[x]['cdf']]
+                    }
                 RETURN elementId(fm) AS eid
                 """
             ).data()[0]["eid"]
 
             for type_, cardinality in formulas[x]["input"].items():
                 transaction.run(
                     f"""
@@ -654,15 +840,21 @@
         transfer_times = attributes["transfer_times"]
         for type_ in routing_probabilities.keys():
             route_id = transaction.run(
                 f"""
                 CREATE (rt:Entity:Resource:Connection:Route)
                 SET rt.probability = {routing_probabilities[type_]},
                     rt.transferTimeMean = {transfer_times[type_]['mean']},
-                    rt.transferTimeStd = {transfer_times[type_]['std']}
+                    rt.transferTimeStd = {transfer_times[type_]['std']},
+                    rt.transferTimeCdfX = {
+                        [point[0] for point in transfer_times[type_]['cdf']]
+                    },
+                    rt.transferTimeCdfY = {
+                        [point[1] for point in transfer_times[type_]['cdf']]
+                    }
                 RETURN elementId(rt) AS eid
                 """
             ).data()[0]["eid"]
             transaction.run(
                 f"""
                 MATCH (ent:EntityType) WHERE elementId(ent) = '{type_ids[type_]}'
                 MATCH (rt:Route) WHERE elementId(rt) = '{route_id}'
@@ -796,18 +988,18 @@
     for connection in connections:
         model.add_edge(*connection)
 
     for station in stations:
         model.nodes[station]["is_source"] = model.in_degree(station) <= 0
         model.nodes[station]["is_sink"] = model.out_degree(station) <= 0
         model.nodes[station]["operation"] = "ORDINARY"
-        model.nodes[station]["formulas"] = []
+        model.nodes[station]["formulas"] = list()
         model.nodes[station]["buffer_capacities"] = dict()
         model.nodes[station]["machine_capacity"] = 0
-        model.nodes[station]["processing_times"] = []
+        model.nodes[station]["processing_times"] = list()
 
     for connection in connections:
         model.edges[connection]["routing_probabilities"] = dict()
         model.edges[connection]["transfer_times"] = dict()
 
 
 def _identify_operations(
@@ -968,15 +1160,15 @@
                 elif activity == "ENTER_BP":
                     event["output"].update(output)
                     output.clear()
 
     for station, sublog in station_sublogs.items():
         operation = model.nodes[station]["operation"]
         formulas = model.nodes[station]["formulas"]
-        frequencies = []
+        frequencies = list()
         formula = None
         for j in range(len(sublog)):
             event = sublog.iloc[j]
             type_ = event["type"]
             activity = event["activity"]
             input_ = event["input"]
             output = event["output"]
@@ -1172,32 +1364,40 @@
     """Mine buffer and machine capacities at each station.
 
     Args:
         model: Graph model.
         log: Event log.
         window: Definite window.
     """
-    ceiling_state = _create_state(model)
+    event = log.loc[window[0]]
+    state = event["state"]
+    max_buffer_loads = dict()
+    max_machine_loads = dict()
+    for station in state.keys():
+        max_buffer_loads[station] = dict()
+        for type_ in state[station]["B"].keys():
+            max_buffer_loads[station][type_] = state[station]["B"][type_]
+        max_machine_loads[station] = sum(state[station]["M"].values())
     for i in range(window[0], window[1]):
         state = log.at[i, "state"]
         for station in state.keys():
-            for location in state[station].keys():
-                for type_ in state[station][location].keys():
-                    ceiling_state[station][location][type_] = max(
-                        state[station][location][type_],
-                        ceiling_state[station][location][type_],
-                    )
+            for type_ in state[station]["B"].keys():
+                max_buffer_loads[station][type_] = max(
+                    state[station]["B"][type_], max_buffer_loads[station][type_]
+                )
+            max_machine_loads[station] = max(
+                sum(state[station]["M"].values()), max_machine_loads[station]
+            )
 
     for station in model.nodes.keys():
         buffer_capacities = model.nodes[station]["buffer_capacities"]
-        for type_, load in ceiling_state[station]["B"].items():
-            buffer_capacities[type_] = load
+        buffer_capacities.update(max_buffer_loads[station])
         operation = model.nodes[station]["operation"]
         if operation == "ORDINARY":
-            machine_capacity = max(ceiling_state[station]["M"].values())
+            machine_capacity = max_machine_loads[station]
         else:
             machine_capacity = 1
         model.nodes[station]["machine_capacity"] = machine_capacity
 
 
 def _mine_processing_times(
     model: networkx.DiGraph,
@@ -1216,17 +1416,15 @@
         log: Event log.
         window: Definite window.
         config: Configuration.
     """
     for station, station_sublog in station_sublogs.items():
         formulas = model.nodes[station]["formulas"]
         operation = model.nodes[station]["operation"]
-        counts = [0 for _ in range(len(formulas))]
-        means = [0.0 for _ in range(len(formulas))]
-        tses = [0.0 for _ in range(len(formulas))]
+        samples = [list() for _ in range(len(formulas))]
         for j in range(0, len(station_sublog)):
             i = station_sublog.index[j]
             if i <= window[0] or i >= window[1]:
                 continue
 
             enter_event = None
             enter_index = -1
@@ -1286,19 +1484,19 @@
                 next_event = part_sublog.iloc[j + 1]
                 next_station = next_event["station"]
                 buffer_load = exit_event["state"][next_station]["B"][exit_type]
                 buffer_capacity = (
                     model.nodes[next_station]["buffer_capacities"][exit_type]
                 )
                 if buffer_load >= buffer_capacity:
-                    release_delay = config["model"]["delays"]["release"]
+                    max_delay = config["model"]["delays"]["release"]
                     event = exit_event
                     while (
                         i > window[0]
-                        and exit_event["time"] - event["time"] <= release_delay
+                        and exit_event["time"] - event["time"] <= max_delay
                     ):
                         i -= 1
                         event = log.loc[i]
                         buffer_load = event["state"][next_station]["B"][exit_type]
                         if buffer_load >= buffer_capacity:
                             is_blocked = True
                             break
@@ -1307,28 +1505,32 @@
                 input_ = exit_event["input"]
                 output = enter_event["output"]
                 for x in range(len(formulas)):
                     if (
                         formulas[x]["input"].keys() == input_.keys()
                         and formulas[x]["output"].keys() == output.keys()
                     ):
-                        counts[x] += 1
-                        last_mean = means[x]
-                        means[x] = means[x] + (sample - means[x]) / counts[x]
-                        tses[x] = tses[x] + (sample - last_mean) * (sample - means[x])
+                        samples[x].append(sample)
                         break
 
         processing_times = model.nodes[station]["processing_times"]
         for x in range(len(formulas)):
             processing_times.append(dict())
-            processing_times[x]["mean"] = means[x]
-            if counts[x] <= 1:
+            if len(samples[x]) <= 0:
+                processing_times[x]["mean"] = 0.0
+                processing_times[x]["std"] = 0.0
+                processing_times[x]["cdf"] = [[0.0, 1.0]]
+            elif len(samples[x]) == 1:
+                processing_times[x]["mean"] = samples[x][0]
                 processing_times[x]["std"] = 0.0
+                processing_times[x]["cdf"] = [[samples[x][0], 1.0]]
             else:
-                processing_times[x]["std"] = (tses[x] / (counts[x] - 1)) ** 0.5
+                processing_times[x]["mean"] = scipy.stats.tmean(samples[x])
+                processing_times[x]["std"] = scipy.stats.tstd(samples[x])
+                processing_times[x]["cdf"] = _compute_empirical_cdf(samples[x], config)
 
 
 def _mine_transfer_times(
     model: networkx.DiGraph,
     station_sublogs: dict[str, pandas.DataFrame],
     part_sublogs: dict[str, pandas.DataFrame],
     log: pandas.DataFrame,
@@ -1342,17 +1544,15 @@
         station_sublogs: Station sublogs.
         part_sublogs: Part sublogs.
         log: Event log.
         window: Definite window.
         config: Configuration.
     """
     connections = model.edges.keys()
-    counts = {connection: dict() for connection in connections}
-    means = {connection: dict() for connection in connections}
-    tses = {connection: dict() for connection in connections}
+    samples = {connection: dict() for connection in connections}
     for part_sublog in part_sublogs.values():
         for j in range(0, len(part_sublog)):
             i = part_sublog.index[j]
             if i <= window[0] or i >= window[1]:
                 continue
 
             enter_event = None
@@ -1376,36 +1576,32 @@
             ):
                 continue
 
             enter_station = enter_event["station"]
             exit_station = exit_event["station"]
             connection = (exit_station, enter_station)
             type_ = event["type"]
-            if type_ not in counts[connection].keys():
-                counts[connection][type_] = 0
-            if type_ not in means[connection].keys():
-                means[connection][type_] = 0.0
-            if type_ not in tses[connection].keys():
-                tses[connection][type_] = 0.0
+            if type_ not in samples[connection].keys():
+                samples[connection][type_] = list()
 
             sample = enter_event["time"] - exit_event["time"]
             is_queued = False
             operation = model.nodes[enter_station]["operation"]
-            seize_delay = config["model"]["delays"]["seize"]
+            max_delay = config["model"]["delays"]["seize"]
             if operation == "ORDINARY":
                 machine_load = enter_event["state"][enter_station]["M"][type_]
                 machine_capacity = (
                     model.nodes[enter_station]["machine_capacity"]
                 )
                 if machine_load >= machine_capacity:
                     i_ = i
                     event = enter_event
                     while (
                         i_ > window[0]
-                        and enter_event["time"] - event["time"] <= seize_delay
+                        and enter_event["time"] - event["time"] <= max_delay
                     ):
                         i_ -= 1
                         event = log.loc[i_]
                         machine_load = event["state"][enter_station]["M"][type_]
                         if machine_load >= machine_capacity:
                             is_queued = True
                             break
@@ -1413,48 +1609,88 @@
                 station_sublog = station_sublogs[enter_station]
                 j_ = station_sublog.index.get_loc(i)
                 i_ = i
                 event = enter_event
                 while (
                     j_ > 0
                     and i_ > window[0]
-                    and enter_event["time"] - event["time"] <= seize_delay
+                    and enter_event["time"] - event["time"] <= max_delay
                 ):
                     j_ -= 1
                     i_ = station_sublog.index[j_]
                     event = station_sublog.iloc[j_]
                     if event["activity"].startswith("EXIT"):
                         is_queued = True
                         break
 
             if not is_queued:
-                counts[connection][type_] += 1
-                last_mean = means[connection][type_]
-                means[connection][type_] = (
-                    means[connection][type_]
-                    + (sample - means[connection][type_])
-                    / counts[connection][type_]
-                )
-                tses[connection][type_] = (
-                    tses[connection][type_]
-                    + (sample - last_mean)
-                    * (sample - means[connection][type_])
-                )
+                samples[connection][type_].append(sample)
 
     for connection in connections:
         transfer_times = model.edges[connection]["transfer_times"]
-        for type_ in counts[connection].keys():
+        for type_ in samples[connection].keys():
             transfer_times[type_] = dict()
-            transfer_times[type_]["mean"] = means[connection][type_]
-            if counts[connection][type_] <= 1:
+            if len(samples[connection][type_]) <= 0:
+                transfer_times[type_]["mean"] = 0.0
+                transfer_times[type_]["std"] = 0.0
+                transfer_times[type_]["cdf"] = [[0.0, 1.0]]
+            elif len(samples[connection][type_]) == 1:
+                transfer_times[type_]["mean"] = samples[connection][type_][0]
                 transfer_times[type_]["std"] = 0.0
+                transfer_times[type_]["cdf"] = [[samples[connection][type_][0], 1.0]]
+            else:
+                transfer_times[type_]["mean"] = scipy.stats.tmean(
+                    samples[connection][type_]
+                )
+                transfer_times[type_]["std"] = scipy.stats.tstd(
+                    samples[connection][type_]
+                )
+                transfer_times[type_]["cdf"] = _compute_empirical_cdf(
+                    samples[connection][type_], config
+                )
+
+
+def _compute_empirical_cdf(samples, config):
+    """Compute the empirical CDF of multiple samples.
+
+    Args:
+        samples (list[float]): Input samples.
+        config (dict[str, Any]): Configuration.
+
+    Returns:
+        list[list[float]]: Empirical CDF
+    """
+    cdf = scipy.stats.ecdf(samples).cdf
+    max_points = config["model"]["cdf"]["points"]
+    if max_points < 0 or len(cdf.quantiles) <= max_points:
+        quantiles = cdf.quantiles
+        probabilities = cdf.probabilities
+    else:
+        bin_size = math.ceil(len(cdf.quantiles) / max_points)
+        num_bins = math.ceil(len(cdf.quantiles) / bin_size)
+        quantiles = [0.0 for _ in range(num_bins)]
+        probabilities = [0.0 for _ in range(num_bins)]
+        quantile = 0.0
+        max_delta = 0.0
+        for x in range(len(cdf.quantiles)):
+            if x <= 0:
+                delta = cdf.probabilities[x]
             else:
-                transfer_times[type_]["std"] = (
-                    tses[connection][type_] / (counts[connection][type_] - 1)
-                ) ** 0.5
+                delta = cdf.probabilities[x] - cdf.probabilities[x - 1]
+            if delta > max_delta:
+                max_delta = delta
+                quantile = cdf.quantiles[x]
+            if x % bin_size >= bin_size - 1 or x >= len(cdf.quantiles) - 1:
+                y = x // bin_size
+                quantiles[y] = quantile
+                probabilities[y] = cdf.probabilities[x]
+                quantile = 0.0
+                max_delta = 0.0
+    cdf = [[quantiles[x], probabilities[x]] for x in range(len(quantiles))]
+    return cdf
 
 
 def _mine_routing_probabilities(
     model: networkx.DiGraph,
     part_sublogs: dict[str, pandas.DataFrame],
     window: list[int],
 ):
```

### Comparing `autotwin_gmglib-0.0.6/LICENSE` & `autotwin_gmglib-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autotwin_gmglib-0.0.6/pyproject.toml` & `autotwin_gmglib-0.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autotwin_gmglib"
-version = "0.0.6"
+version = "0.1.0"
 description = "Graph Model Generation Library for Auto-Twin"
 license = "BSD-3-Clause"
 authors = [
     "Lulai Zhu <lulai.zhu@gmail.com>"
 ]
 readme = "README.md"
 homepage = "https://github.com/AutotwinEU/graph-model-gen"
@@ -20,14 +20,15 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 neo4j = "^5.17.0"
 pandas = "^2.2.1"
 networkx = "^3.2.1"
 pygraphviz = "^1.12"
 matplotlib = "^3.8.3"
+scipy = "^1.13.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 flake8 = "^7.0.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `autotwin_gmglib-0.0.6/README.md` & `autotwin_gmglib-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `autotwin_gmglib-0.0.6/PKG-INFO` & `autotwin_gmglib-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotwin_gmglib
-Version: 0.0.6
+Version: 0.1.0
 Summary: Graph Model Generation Library for Auto-Twin
 Home-page: https://github.com/AutotwinEU/graph-model-gen
 License: BSD-3-Clause
 Keywords: auto-twin,system discovery,graph model
 Author: Lulai Zhu
 Author-email: lulai.zhu@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: neo4j (>=5.17.0,<6.0.0)
 Requires-Dist: networkx (>=3.2.1,<4.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: pygraphviz (>=1.12,<2.0)
+Requires-Dist: scipy (>=1.13.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 [![PyPI - License](https://img.shields.io/pypi/l/autotwin_gmglib)](https://github.com/AutotwinEU/graph-model-gen/blob/main/LICENSE)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/autotwin_gmglib)](https://www.python.org/downloads/)
 [![PyPI - Version](https://img.shields.io/pypi/v/autotwin_gmglib)](https://pypi.org/project/autotwin_gmglib/)
 
 # Graph Model Generation Library for Auto-Twin
```

