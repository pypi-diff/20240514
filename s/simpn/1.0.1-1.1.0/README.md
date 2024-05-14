# Comparing `tmp/simpn-1.0.1.tar.gz` & `tmp/simpn-1.1.0.tar.gz`

## Comparing `simpn-1.0.1.tar` & `simpn-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 simpn-1.0.1/CHANGELOG.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simpn-1.0.1/simpn/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 simpn-1.0.1/simpn/immutabletypes.py
--rw-r--r--   0        0        0     7210 2020-02-02 00:00:00.000000 simpn-1.0.1/simpn/prototypes.py
--rw-r--r--   0        0        0    13403 2020-02-02 00:00:00.000000 simpn-1.0.1/simpn/reporters.py
--rw-r--r--   0        0        0    31964 2020-02-02 00:00:00.000000 simpn-1.0.1/simpn/simulator.py
--rw-r--r--   0        0        0    16480 2020-02-02 00:00:00.000000 simpn-1.0.1/simpn/visualisation.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 simpn-1.0.1/.gitignore
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 simpn-1.0.1/LICENSE
--rw-r--r--   0        0        0     8892 2020-02-02 00:00:00.000000 simpn-1.0.1/README.rst
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 simpn-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    10576 2020-02-02 00:00:00.000000 simpn-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 simpn-1.1.0/CHANGELOG.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simpn-1.1.0/simpn/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 simpn-1.1.0/simpn/immutabletypes.py
+-rw-r--r--   0        0        0    13797 2020-02-02 00:00:00.000000 simpn-1.1.0/simpn/prototypes.py
+-rw-r--r--   0        0        0    13403 2020-02-02 00:00:00.000000 simpn-1.1.0/simpn/reporters.py
+-rw-r--r--   0        0        0    32992 2020-02-02 00:00:00.000000 simpn-1.1.0/simpn/simulator.py
+-rw-r--r--   0        0        0    18097 2020-02-02 00:00:00.000000 simpn-1.1.0/simpn/visualisation.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 simpn-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 simpn-1.1.0/LICENSE
+-rw-r--r--   0        0        0     8892 2020-02-02 00:00:00.000000 simpn-1.1.0/README.rst
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 simpn-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    10576 2020-02-02 00:00:00.000000 simpn-1.1.0/PKG-INFO
```

### Comparing `simpn-1.0.1/simpn/reporters.py` & `simpn-1.1.0/simpn/reporters.py`

 * *Files identical despite different names*

### Comparing `simpn-1.0.1/simpn/simulator.py` & `simpn-1.1.0/simpn/simulator.py`

 * *Files 8% similar despite different names*

```diff
@@ -282,14 +282,15 @@
     it can happen on any of these values.
 
     :param debugging: if set to True, produces more information for debugging purposes (defaults to True).
     """
     def __init__(self, debugging=True):
         self.places = []
         self.events = []
+        self.prototypes = []
         self.id2node = dict()
         self.clock = 0
         self._debugging = debugging
         self.clock_checkpoints = dict()
 
     def __str__(self):
         result = ""
@@ -456,14 +457,27 @@
         # Generate and add SimEvent
         result = SimEvent(t_name, guard=guard, behavior=behavior, incoming=inflow, outgoing=outflow)
         self.events.append(result)
         self.id2node[t_name] = result
 
         return result
 
+    def add_prototype(self, prototype):
+        if len(prototype.places) == 0 and len(prototype.events) == 0:
+            raise TypeError("Prototype " + prototype.name + ": does not have any variables or events. That should not be possible, please notify the developer.")
+        for place in prototype.places:
+            if place not in self.places:
+                raise TypeError("Prototype " + prototype.name + ": did not add all its places to the model. That should not be possible, please notify the developer.")
+        for event in prototype.events:
+            if event not in self.events:
+                raise TypeError("Prototype " + prototype.name + ": did not add all its events to the model. That should not be possible, please notify the developer.")
+        if prototype.get_id() in self.id2node:
+            raise TypeError("Prototype " + prototype.name + ": node with the same name already exists. Names must be unique.")
+        self.prototypes.append(prototype)
+
     @staticmethod
     def tokens_combinations(event):
         """
         Creates a list of token combinations that are available to the specified event.
         These are combinations of tokens that are on the incoming SimVar of the event.
         For example, if a event has incoming SimVar a and b with tokens 1@0 on a and 2@0, 3@0 on b,
         the possible combinations are [(a, 1@0), (b, 2@0)] and [(a, 1@0), (b, 3@0)]
```

### Comparing `simpn-1.0.1/simpn/visualisation.py` & `simpn-1.1.0/simpn/visualisation.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 TUE_RED = (200, 25, 25)
 TUE_LIGHTRED = (249, 204, 204)
 TUE_BLUE = (16, 16, 115)
 TUE_LIGHTBLUE = (188, 188, 246)
 TUE_GREY = (242, 242, 242)
 WHITE = (255, 255, 255)
 # sizes
-NODE_WIDTH, NODE_HEIGHT = 50, 50
+STANDARD_NODE_WIDTH, STANDARD_NODE_HEIGHT = 50, 50
 NODE_SPACING = 100
 GRID_SPACING = 50
 LINE_WIDTH = 2
 ARROW_WIDTH, ARROW_HEIGHT = 12, 10
 TEXT_SIZE = 16
 
 
@@ -44,28 +44,30 @@
     #   by using (x_new if x_new >= 0 else x, y_new if y_new >= 0 else y)
     def __init__(self, start, end):
         self._start = start
         self._end = end
 
     def draw(self, screen):
         start_node_xy = self.get_start_node().get_pos()
+        start_node_width, start_node_height = self.get_start_node()._width, self.get_start_node()._height
         end_node_xy = self.get_end_node().get_pos()
-        if start_node_xy[1] - NODE_HEIGHT/2 > end_node_xy[1] + NODE_HEIGHT/2:
+        end_node_width, end_node_height = self.get_end_node()._width, self.get_end_node()._height
+        if start_node_xy[1] - start_node_height/2 > end_node_xy[1] + end_node_height/2:
             self.set_start_hook(Hook.TOP)
-        elif start_node_xy[1] + NODE_HEIGHT/2 < end_node_xy[1] - NODE_HEIGHT/2:
+        elif start_node_xy[1] + start_node_height/2 < end_node_xy[1] - end_node_height/2:
             self.set_start_hook(Hook.BOTTOM)
-        elif start_node_xy[0] - NODE_WIDTH/2 > end_node_xy[0] + NODE_WIDTH/2:
+        elif start_node_xy[0] - start_node_width/2 > end_node_xy[0] + end_node_width/2:
             self.set_start_hook(Hook.LEFT)
         else:
             self.set_start_hook(Hook.RIGHT)
-        if end_node_xy[1] - NODE_HEIGHT/2 > start_node_xy[1] + NODE_HEIGHT/2:
+        if end_node_xy[1] - end_node_height/2 > start_node_xy[1] + start_node_height/2:
             self.set_end_hook(Hook.TOP)
-        elif end_node_xy[1] + NODE_HEIGHT/2 < start_node_xy[1] - NODE_HEIGHT/2:
+        elif end_node_xy[1] + end_node_height/2 < start_node_xy[1] - start_node_height/2:
             self.set_end_hook(Hook.BOTTOM)
-        elif end_node_xy[0] - NODE_WIDTH/2 > start_node_xy[0] + NODE_WIDTH/2:
+        elif end_node_xy[0] - end_node_width/2 > start_node_xy[0] + start_node_width/2:
             self.set_end_hook(Hook.LEFT)
         else:
             self.set_end_hook(Hook.RIGHT)
         start = pygame.Vector2(self._start[0].hook(self._start[1]))
         end = pygame.Vector2(self._end[0].hook(self._end[1]))
         arrow = start - end
         angle = arrow.angle_to(pygame.Vector2(0, -1))
@@ -119,19 +121,18 @@
         self._end = (self._end[0], hook)
 
 
 class Node:
     def __init__(self, model_node):
         self._model_node = model_node
         self._pos = (0, 0)  # the center of the node
-        self._half_height = NODE_HEIGHT / 2
-        self._half_width = NODE_WIDTH / 2
-        self._width = NODE_WIDTH
-        self._height = NODE_HEIGHT
-        self._size = MAX_SIZE
+        self._width = STANDARD_NODE_WIDTH
+        self._height = STANDARD_NODE_HEIGHT
+        self._half_width =  self._width / 2
+        self._half_height = self._height / 2
             
     def draw(self, screen):
         raise Exception("Node.raise must be implemented at subclass level.")
 
     def hook(self, hook_pos):
         if hook_pos == Hook.LEFT:
             return self._pos[0] - self._half_width, self._pos[1]
@@ -145,24 +146,24 @@
     def set_pos(self, pos):
         self._pos = pos
     
     def get_pos(self):
         return self._pos
     
     def get_id(self):
-        raise Exception("Node.get_id must be implemented at subclass level.")
+        return self._model_node.get_id()
         
 
 class PlaceViz(Node):
     def __init__(self, model_node):
         super().__init__(model_node)
     
     def draw(self, screen):
-        pygame.draw.circle(screen, TUE_LIGHTBLUE, (self._pos[0], self._pos[1]), NODE_WIDTH/2)
-        pygame.draw.circle(screen, TUE_BLUE, (self._pos[0], self._pos[1]), NODE_WIDTH/2, LINE_WIDTH)    
+        pygame.draw.circle(screen, TUE_LIGHTBLUE, (self._pos[0], self._pos[1]), self._half_height)
+        pygame.draw.circle(screen, TUE_BLUE, (self._pos[0], self._pos[1]), self._half_height, LINE_WIDTH)    
         font = pygame.font.SysFont('Calibri', TEXT_SIZE)
         bold_font = pygame.font.SysFont('Calibri', TEXT_SIZE, bold=True)
 
         # draw label
         label = font.render(self._model_node.get_id(), True, TUE_BLUE)
         text_x_pos = self._pos[0] - int(label.get_width()/2)
         text_y_pos = self._pos[1] + self._half_height + LINE_WIDTH
@@ -173,41 +174,35 @@
         ti = 0
         for token in self._model_node.marking:
             mstr += str(token.value) + "@" + str(round(token.time, 2))
             if ti < len(self._model_node.marking) - 1:
                 mstr += ", "
             ti += 1
         mstr += "]"
-        label = label = bold_font.render(mstr, True, TUE_RED)
+        label = bold_font.render(mstr, True, TUE_RED)
         text_x_pos = self._pos[0] - int(label.get_width()/2)
         text_y_pos = self._pos[1] + self._half_height + LINE_WIDTH + int(label.get_height())
-        screen.blit(label, (text_x_pos, text_y_pos))
-
-    def get_id(self):
-        return self._model_node.get_id()
+        screen.blit(label, (text_x_pos, text_y_pos))        
 
 
 class TransitionViz(Node):
     def __init__(self, model_node):
         super().__init__(model_node)
     
     def draw(self, screen):
-        pygame.draw.rect(screen, TUE_LIGHTBLUE, pygame.Rect(self._pos[0]-self._half_width, self._pos[1]-self._half_height, NODE_WIDTH, NODE_HEIGHT))
-        pygame.draw.rect(screen, TUE_BLUE, pygame.Rect(self._pos[0]-self._half_width, self._pos[1]-self._half_height, NODE_WIDTH, NODE_HEIGHT), LINE_WIDTH)
+        pygame.draw.rect(screen, TUE_LIGHTBLUE, pygame.Rect(self._pos[0]-self._half_width, self._pos[1]-self._half_height, self._width, self._height))
+        pygame.draw.rect(screen, TUE_BLUE, pygame.Rect(self._pos[0]-self._half_width, self._pos[1]-self._half_height, self._width, self._height), LINE_WIDTH)
         font = pygame.font.SysFont('Calibri', TEXT_SIZE)
 
         # draw label
         label = font.render(self._model_node.get_id(), True, TUE_BLUE)
         text_x_pos = self._pos[0] - int(label.get_width()/2)
         text_y_pos = self._pos[1] + self._half_height + LINE_WIDTH
         screen.blit(label, (text_x_pos, text_y_pos))
 
-    def get_id(self):
-        return self._model_node.get_id()
-
 
 class Button(pygame.sprite.Sprite):
     def __init__(self):
         super().__init__()
         self.image = pygame.Surface((31, 31), pygame.SRCALPHA, 32)
         self.image = self.image.convert_alpha()
         self.image.set_alpha(128)
@@ -239,30 +234,54 @@
         pygame.display.set_caption('Petri Net Visualisation')
         
         self.__running = False
         self._problem = sim_problem
         self._nodes = dict()
         self._edges = []
         self._selected_nodes = None        
-        
+
+        # Add visualizations for prototypes, places, and transitions,
+        # but not for places and transitions that are part of prototypes.
+        element_to_prototype = dict()  # mapping of prototype element ids to prototype ids
+        viznodes_with_edges = []
+        for prototype in self._problem.prototypes:
+            prototype_viznode = prototype.get_visualisation()
+            self._nodes[prototype.get_id()] = prototype_viznode
+            viznodes_with_edges.append(prototype_viznode)
+            for event in prototype.events:
+                element_to_prototype[event.get_id()] = prototype.get_id()
+            for place in prototype.places:
+                element_to_prototype[place.get_id()] = prototype.get_id()
         for var in self._problem.places:
-            self._nodes[var.get_id()] = PlaceViz(var)
+            if var.get_id() not in element_to_prototype:
+                self._nodes[var.get_id()] = PlaceViz(var)
         for event in self._problem.events:
-            event_shape = TransitionViz(event)
-            self._nodes[event.get_id()] = event_shape
-            for incoming in event.incoming:
+            if event.get_id() not in element_to_prototype:
+                event_viznode = TransitionViz(event)
+                self._nodes[event.get_id()] = event_viznode
+                viznodes_with_edges.append(event_viznode)                
+        # Add visualization for edges.
+        # If an edge is from or to a prototype element, it must be from or to the prototype itself.
+        for viznode in viznodes_with_edges:
+            for incoming in viznode._model_node.incoming:
                 node_id = incoming.get_id()
                 if node_id.endswith(".queue"):
                     node_id = node_id[:-len(".queue")]
-                self._edges.append(Edge(start=(self._nodes[node_id], Hook.RIGHT), end=(event_shape, Hook.LEFT)))
-            for outgoing in event.outgoing:
+                if node_id in element_to_prototype:
+                    node_id = element_to_prototype[node_id]
+                other_viznode = self._nodes[node_id]
+                self._edges.append(Edge(start=(other_viznode, Hook.RIGHT), end=(viznode, Hook.LEFT)))
+            for outgoing in viznode._model_node.outgoing:
                 node_id = outgoing.get_id()
                 if node_id.endswith(".queue"):
                     node_id = node_id[:-len(".queue")]
-                self._edges.append(Edge(start=(event_shape, Hook.RIGHT), end=(self._nodes[node_id], Hook.LEFT)))
+                if node_id in element_to_prototype:
+                    node_id = element_to_prototype[node_id]
+                other_viznode = self._nodes[node_id]
+                self._edges.append(Edge(start=(viznode, Hook.RIGHT), end=(other_viznode, Hook.LEFT)))
         layout_loaded = False
         if layout_file is not None:
             try:
                 self.__load_layout(layout_file)
                 layout_loaded = True
             except FileNotFoundError as e:
                 print("WARNING: could not load the layout because of the exception below.\nauto-layout will be used.\n", e)
@@ -312,17 +331,17 @@
         for node in self._nodes.values():
             graph.add_vertex(node.get_id())
         for edge in self._edges:            
             graph.add_edge(edge.get_start_node().get_id(), edge.get_end_node().get_id())
         layout = graph.layout_sugiyama()
         layout.rotate(-90)
         layout.scale(NODE_SPACING)
-        boundaries = layout.boundaries(border=NODE_WIDTH)
+        boundaries = layout.boundaries(border=STANDARD_NODE_WIDTH)
         layout.translate(-boundaries[0][0], -boundaries[0][1])
-        canvas_size = layout.boundaries(border=NODE_WIDTH)[1]
+        canvas_size = layout.boundaries(border=STANDARD_NODE_WIDTH)[1]
         self._size = (min(MAX_SIZE[0], canvas_size[0]), min(MAX_SIZE[1], canvas_size[1]))
         i = 0
         for v in graph.vs:
             xy = layout[i]
             xy  = (round(xy[0]/GRID_SPACING)*GRID_SPACING, round(xy[1]/GRID_SPACING)*GRID_SPACING)
             self._nodes[v["name"]].set_pos(xy)
             i += 1
@@ -346,15 +365,15 @@
             self._size = tuple(map(int, f.readline().strip().split(",")))
             for line in f:
                 id, x, y = line.strip().split(",")
                 self._nodes[id].set_pos((int(x), int(y)))
 
     def __get_node_at(self, pos):
         for node in self._nodes.values():
-            if node.get_pos()[0] - NODE_WIDTH/2 <= pos[0] <= node.get_pos()[0] + NODE_WIDTH/2 and node.get_pos()[1] - NODE_HEIGHT/2 <= pos[1] <= node.get_pos()[1] + NODE_HEIGHT/2:
+            if node.get_pos()[0] - node._width/2 <= pos[0] <= node.get_pos()[0] + node._width/2 and node.get_pos()[1] - node._height/2 <= pos[1] <= node.get_pos()[1] + node._height/2:
                 return node
         return None
 
     def __drag(self, snap=False):
         nodes = self._selected_nodes[0]
         org_pos = self._selected_nodes[1]
         new_pos = pygame.mouse.get_pos()
```

### Comparing `simpn-1.0.1/.gitignore` & `simpn-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `simpn-1.0.1/LICENSE` & `simpn-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simpn-1.0.1/README.rst` & `simpn-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `simpn-1.0.1/pyproject.toml` & `simpn-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "simpn"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
   { name="Remco Dijkman", email="r.m.dijkman@tue.nl" },
 ]
 description = "A package for Discrete Event Simulation, using the theory of Petri Nets."
 readme = "README.rst"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
```

### Comparing `simpn-1.0.1/PKG-INFO` & `simpn-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: simpn
-Version: 1.0.1
+Version: 1.1.0
 Summary: A package for Discrete Event Simulation, using the theory of Petri Nets.
 Project-URL: Homepage, https://github.com/bpogroup/simpn
 Project-URL: Documentation, https://bpogroup.github.io/simpn/
 Author-email: Remco Dijkman <r.m.dijkman@tue.nl>
 License: Copyright (c) 2023 Remco Dijkman (Eindhoven University of Technology)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

