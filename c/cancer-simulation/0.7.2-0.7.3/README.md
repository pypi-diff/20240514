# Comparing `tmp/cancer_simulation-0.7.2.tar.gz` & `tmp/cancer_simulation-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cancer_simulation-0.7.2.tar", last modified: Mon May 13 05:55:04 2024, max compression
+gzip compressed data, was "cancer_simulation-0.7.3.tar", last modified: Tue May 14 04:17:51 2024, max compression
```

## Comparing `cancer_simulation-0.7.2.tar` & `cancer_simulation-0.7.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-13 05:55:04.554490 cancer_simulation-0.7.2/
--rw-r--r--   0 zhukowych  (1000) zhukowych  (1000)      546 2024-05-13 05:55:04.554490 cancer_simulation-0.7.2/PKG-INFO
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     9885 2024-05-12 12:44:46.000000 cancer_simulation-0.7.2/README.md
-drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-13 05:55:04.554490 cancer_simulation-0.7.2/cancer_simulation.egg-info/
--rw-r--r--   0 zhukowych  (1000) zhukowych  (1000)      546 2024-05-13 05:55:04.000000 cancer_simulation-0.7.2/cancer_simulation.egg-info/PKG-INFO
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      390 2024-05-13 05:55:04.000000 cancer_simulation-0.7.2/cancer_simulation.egg-info/SOURCES.txt
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)        1 2024-05-13 05:55:04.000000 cancer_simulation-0.7.2/cancer_simulation.egg-info/dependency_links.txt
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       34 2024-05-13 05:55:04.000000 cancer_simulation-0.7.2/cancer_simulation.egg-info/entry_points.txt
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       62 2024-05-13 05:55:04.000000 cancer_simulation-0.7.2/cancer_simulation.egg-info/requires.txt
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)        4 2024-05-13 05:55:04.000000 cancer_simulation-0.7.2/cancer_simulation.egg-info/top_level.txt
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       38 2024-05-13 05:55:04.554490 cancer_simulation-0.7.2/setup.cfg
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      828 2024-05-13 05:54:35.000000 cancer_simulation-0.7.2/setup.py
-drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-13 05:55:04.550490 cancer_simulation-0.7.2/src/
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       30 2024-05-12 18:56:52.000000 cancer_simulation-0.7.2/src/__init__.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     2986 2024-05-12 19:00:27.000000 cancer_simulation-0.7.2/src/automaton.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     1625 2024-05-12 17:43:44.000000 cancer_simulation-0.7.2/src/cell.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      274 2024-05-11 21:25:41.000000 cancer_simulation-0.7.2/src/constants.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)    12362 2024-05-12 18:59:45.000000 cancer_simulation-0.7.2/src/csimulation.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     8346 2024-05-12 19:00:17.000000 cancer_simulation-0.7.2/src/entity.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     2924 2024-05-12 19:00:03.000000 cancer_simulation-0.7.2/src/grid.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     4286 2024-05-12 11:57:53.000000 cancer_simulation-0.7.2/src/variables.py
+drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-14 04:17:51.428361 cancer_simulation-0.7.3/
+-rw-r--r--   0 zhukowych  (1000) zhukowych  (1000)      599 2024-05-14 04:17:51.428361 cancer_simulation-0.7.3/PKG-INFO
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)    11757 2024-05-14 04:13:21.000000 cancer_simulation-0.7.3/README.md
+drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-14 04:17:51.424361 cancer_simulation-0.7.3/cancer_simulation.egg-info/
+-rw-r--r--   0 zhukowych  (1000) zhukowych  (1000)      599 2024-05-14 04:17:51.000000 cancer_simulation-0.7.3/cancer_simulation.egg-info/PKG-INFO
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      390 2024-05-14 04:17:51.000000 cancer_simulation-0.7.3/cancer_simulation.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)        1 2024-05-14 04:17:51.000000 cancer_simulation-0.7.3/cancer_simulation.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       34 2024-05-14 04:17:51.000000 cancer_simulation-0.7.3/cancer_simulation.egg-info/entry_points.txt
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       62 2024-05-14 04:17:51.000000 cancer_simulation-0.7.3/cancer_simulation.egg-info/requires.txt
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)        4 2024-05-14 04:17:51.000000 cancer_simulation-0.7.3/cancer_simulation.egg-info/top_level.txt
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       38 2024-05-14 04:17:51.428361 cancer_simulation-0.7.3/setup.cfg
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      822 2024-05-14 04:17:44.000000 cancer_simulation-0.7.3/setup.py
+drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-14 04:17:51.424361 cancer_simulation-0.7.3/src/
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       30 2024-05-12 18:56:52.000000 cancer_simulation-0.7.3/src/__init__.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     3168 2024-05-13 20:56:21.000000 cancer_simulation-0.7.3/src/automaton.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     1625 2024-05-12 17:43:44.000000 cancer_simulation-0.7.3/src/cell.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      274 2024-05-14 04:13:21.000000 cancer_simulation-0.7.3/src/constants.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)    12399 2024-05-13 13:03:22.000000 cancer_simulation-0.7.3/src/csimulation.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     8368 2024-05-13 20:53:28.000000 cancer_simulation-0.7.3/src/entity.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     2924 2024-05-12 19:00:03.000000 cancer_simulation-0.7.3/src/grid.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     5155 2024-05-14 04:14:52.000000 cancer_simulation-0.7.3/src/variables.py
```

### Comparing `cancer_simulation-0.7.2/PKG-INFO` & `cancer_simulation-0.7.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: cancer_simulation
-Version: 0.7.2
+Version: 0.7.3
+Summary: A simple cancer and chemotherapy simulation
 Home-page: https://github.com/Zhukowych/CancerSimulation
 Requires-Dist: pygame==2.5.2
 Requires-Dist: pygame-chart==1.0.0
 Requires-Dist: numpy==1.26.3
 Requires-Dist: PyYAML==6.0.1
 
 We implemented cancer development and chemotherapy impact simulation using
```

### Comparing `cancer_simulation-0.7.2/README.md` & `cancer_simulation-0.7.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,60 @@
 
 # Cancer simulation
 We implemented cancer development and chemotherapy impact simulation using **stochastic cellular automaton** with Python. The main feature of implemented app is capability of simulating different treatment strategies under same-type cancer behavior.
 
 ![Alt text](img/first_screen.png?raw=true "Optional Title")
 
 ## Contents
-- [Instalation](#instalation)
-- [Usage](#usage)
-- [Simulation model](#simulation-model)
+- [Cancer simulation](#cancer-simulation)
+  - [Contents](#contents)
+  - [Instalation](#instalation)
+  - [Usage](#usage)
+  - [Simulation model](#simulation-model)
     - [States](#states)
     - [Initial parameters](#initial-parameters)
     - [Transition rules](#transition-rules)
         - [Growth rules](#growth-rules)
         - [Therapy impact](#therapy-impact)
 - [Implementation & architecture](#implementation--architecture)
     - [Model architecture](#model-architecture)
     - [GUI](#gui)
     - [Config file](#config-file)
+  - [Simulation demonstrations](#simulation-demonstrations)
+  - [Team](#team)
 
 
 ## Instalation
 To use app you must clone it from git repo and install requirements. Preferrable version Python3.12
+
 ```
 git clone https://github.com/Zhukowych/CancerSimulation.git
 cd CancerSimulation
 pip install -r requirements
 ```
 
+or 
+
+```
+$ pip install cancer-simulation
+```
+if you use pip to install app, check warnings on installation. On Linux-based OS
+pip installs scripts to ~/.local/bin/, so this folder should be in the PATH variable
+
 ## Usage
 
 To run app you must use the following bash command
 ```
-python csimulation.py config.yaml
+$ python csimulation.py config.yaml
+```
+or, if you installed from pip
+```bash
+$ csim config.yaml
 ```
-providing config.yaml file, which structure will be discussed further in the part [Config file](#config-file)
+providing config.yaml file, which structure will be discussed further in the part [Config file](#config-file). TO start simulation press "s" key.
 
 ## Simulation model
 In this project we implemented models proposed in the following articles. First focus on main principles of cancer growth, while second introduces main principles of chemotherapy treatment simulation.
 - [Cellular-automaton model for tumor growth dynamics: Virtualization of different scenarios](https://www.sciencedirect.com/science/article/pii/S0010482522011891?ref=pdf_download&fr=RR-2&rr=8800d112bd3635b1)
 - [A cellular automata model of chemotherapy effects on tumour growth: targeting cancer and immune cells](https://www.tandfonline.com/doi/full/10.1080/13873954.2019.1571515)
 
 
@@ -110,15 +127,15 @@
 - Drug is evenly distributed among all cells
 - We can affect tumor growth via reducing probability of proliferation, increasing probability of cell death and decreasing $K_c$
 
 Drug can kill RTC, QC, IC with different probabilities:
 
 $$F_i(g) = l_i\times PK\times e^{-c_i(t - n_d\tau)}$$
 
-$$l_i=\frac{l_i\times g}{y'_i\times n_d+1}$$
+$$l_i=\frac{k_i\times g}{y'_i\times n_d+1}$$
 
 $$y'_i = \theta\times y_i$$ 
 
 $$ 0< \theta \leq1$$
 
 where i can be (RTC, QC, IC) and $g$ is the drug concentration at each cell. Also therapy affects proliferation potential
 
@@ -141,15 +158,30 @@
  - **Entity** - is a class to define behavior of each state via overriding next_state method. So, in our implementation classes derived from **Entity** work as states. We have implemented the following **Entity**es: BiologicalCell CancerCell, StemCell, QuiescentCell, NecroticCell, ImmuneCell. Each class has redefined next_state method 
  - **FiniteAutomaton** - main class of model that takes care of calling next_state() methods of each active entity, recruiting new ICs and controlling therapy injections.
  - **Variables** - class that holds all initial parameters as well as other dynamic variables that are needed in runtime
 
  All, in all this this architecture decisions made development of model very flexible what allowed us to make more experiments on the system
 
 ### GUI
+PyGame framework was used for GUI development. Upon initialization each simulation's grid size is calculated according to indentation size, which itself is calculated with respect to window size, that can be set in [constants.py](./constants.py). The following formulas are used:
+$$GCL=\min\left(\left\lfloor  \frac{\left\lfloor\frac{SW}{2} \right\rfloor - 3IX}{2} \right \rfloor ,\left\lfloor  \frac{SH - 3IY}{2} \right \rfloor  \right)
+\newline$$
+$$IX = \left\lfloor\frac{SW}{190}\right\rfloor$$
+$$IY = \left\lfloor\frac{SH}{50}\right\rfloor \text{where}$$
+$$GCL - \text{grid side length}$$
+$$IX - \text{indentation with respect to x axis}$$
+$$IY - \text{indentation with respect to y axis}$$
+$$SW - \text{screen width}$$
+$$SH - \text{screen height}$$
+
+Simulations' outlines and dashboard are rendered with the help of "prepare_board" function. Also few functions were implemented for handiness of working with text, such as: render_fps, render_sim_status, render_text.
+
+Simulation, class stores counter, coordiantes of left corner of simulation, name and queue. Queue is a shared memory between simulation and paralleled process where steps are calculated. Draw method of Simulation blanks it's area on each tick and draws only pixels that contaion cells.
 
+Each simulation's step is calculated in a respective parallel process with function "calculate_step". Than, on each tick whole board is rerendered.
 ### Config file
 
 [Initial parameters](#initial-parameters) have default values in our implementation, but to compare different therapy strategies or various drugs we must vary these parameters, so user must pass a yaml file with settings for each simulation:
 
 ```yaml
 global:
   yI: 1
@@ -164,8 +196,8 @@
 ## Simulation demonstrations
 
 
 ## Team
  - [Anton Valihurskyi](https://github.com/BlueSkyAndSomeCurses) - Research, GUI development, computation paralelization
  - [Oleksandra Sherhina](https://github.com/shshrg) - Current state chart creation, simulation video export
  - [Viktoriia Lushpak](https://github.com/linyvez) - Current state chart creation, simulation video export
- - [Maksym Zhuk](https://github.com/Zhukowych) - Research, cellular automaton implementation
+ - [Maksym Zhuk](https://github.com/Zhukowych) - Research, cellular automaton implementation
```

### Comparing `cancer_simulation-0.7.2/cancer_simulation.egg-info/PKG-INFO` & `cancer_simulation-0.7.3/cancer_simulation.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: cancer_simulation
-Version: 0.7.2
+Version: 0.7.3
+Summary: A simple cancer and chemotherapy simulation
 Home-page: https://github.com/Zhukowych/CancerSimulation
 Requires-Dist: pygame==2.5.2
 Requires-Dist: pygame-chart==1.0.0
 Requires-Dist: numpy==1.26.3
 Requires-Dist: PyYAML==6.0.1
 
 We implemented cancer development and chemotherapy impact simulation using
```

### Comparing `cancer_simulation-0.7.2/setup.py` & `cancer_simulation-0.7.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="cancer_simulation",
-    version='0.7.2',
+    version='0.7.3',
     packages=find_packages(),
-    short_description="A simple cancer and chemotherapy simulation",
+    description="A simple cancer and chemotherapy simulation",
     long_description="""We implemented cancer development and chemotherapy impact simulation using
                    stochastic cellular automaton with Python. The main feature of implemented 
                    app is capability of simulating different treatment strategies under same-
                    type cancer behavior.""",
     url = "https://github.com/Zhukowych/CancerSimulation",
     install_requires = [
         'pygame==2.5.2',
```

### Comparing `cancer_simulation-0.7.2/src/automaton.py` & `cancer_simulation-0.7.3/src/automaton.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,37 +65,43 @@
             else:
                 entity.energy_level = 0
 
             if entity.free_neighbors:
                 edge_cells.append(cell)
 
             self.counter.immune_cell += 1 if isinstance(entity, ImmuneCell) else 0
-            self.counter.tumor_cell += 1 if isinstance(entity, CancerCell) else 0
+            self.counter.proliferating_cell += 1 if isinstance(entity, (TrueStemCell, CancerCell)) else 0
+            self.counter.tumor_cell += 1 if isinstance(entity, (CancerCell, QuiescentCell, NecroticCell)) else 0
             self.counter.stem_cell += 1 if isinstance(entity, TrueStemCell) else 0
 
-            entity.next_state(self.variables, *random_variables[i])
+            entity.next_state(*random_variables[i])
 
             entity.cell = None
             entity.neighbors = None
             entity.free_neighbors = None
 
         self.edge_cells = edge_cells
 
+        self.variables.time_step()
         self.process_chemotherapy()
         self.spawn_immune_cells()
 
     def process_chemotherapy(self):
         """Process effect of chemotherapy on cell"""
         if self.variables.is_injection_start:
             self.variables.injection_number += 1
 
     def spawn_immune_cells(self):
         """Spawn immune cells on the grid"""
-        recrutient = (
-            2 * self.counter.immune_cell * self.counter.tumor_cell / (10**3 + self.counter.tumor_cell)
-        )
-        if self.counter.immune_cell >= self.variables.max_immune_cell_count:
+        if not self.variables.immune_response:
+            return
+
+        needed_immune_cells = self.variables.ics * self.counter.tumor_cell
+
+        recrutient = needed_immune_cells - self.counter.immune_cell
+
+        if recrutient < 0:
             return
 
         for _ in range(int(recrutient)):
             free_cell = self.grid.get_random_free_cell()
             free_cell.entity = ImmuneCell()
```

### Comparing `cancer_simulation-0.7.2/src/cell.py` & `cancer_simulation-0.7.3/src/cell.py`

 * *Files identical despite different names*

### Comparing `cancer_simulation-0.7.2/src/csimulation.py` & `cancer_simulation-0.7.3/src/csimulation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Super pygame visualisation with multiprocessing backed up with rust, C and C++ at the same time.
 """
 
-import sys
-from multiprocessing import Process, Queue, Value
+from multiprocessing import Process, Queue, Value, Event
 import pygame
 import pygame_chart as pyc
 
 import pygame
 import argparse
 from .automaton import FiniteAutomaton
 from .grid import Grid
@@ -130,25 +129,26 @@
             else [
                 self.sim.counter.immune_cell,
                 self.sim.counter.tumor_cell,
                 self.sim.counter.proliferating_cell,
                 self.sim.counter.stem_cell,
             ]
         )
+        colors = ['#1b9e77', '#a9f971', '#fdaa48','#6890F0']
         self.figure.set_ylim((0, 10000))
         self.figure.set_xlim((0, 8))
         self.figure.add_title(f"Simulation {self.index + 1}")
         self.figure.add_legend()
         self.figure.add_gridlines()
 
         self.figure.bar(
             "Immune, Tumor, Proliferating and Stem cells",
             [1, 3, 5, 7],
             data,
-            color=(168, 168, 168),
+            color=colors[0],
         )
         self.figure.draw()
 
 
 def prepare_board():
     """
     renders board
@@ -326,23 +326,18 @@
 
     screen.blit(
         text_font.render(f"FPS: {fps_num}", False, (0, 0, 0)),
         (x, y),
     )
 
 
-def render_sim_status(x: int, y: int):
+def render_sim_status():
     """
     render function for printing sim status
     """
-    # pygame.draw.rect(
-    #     screen,
-    #     (174, 198, 207),
-    #     pygame.Rect(x, y, 300, 400),
-    # )
 
     if running_sim.value:
         render_text(
             "Status: Running",
             DASHBOARD_X_Y[0] + 120,
             DASHBOARD_X_Y[1] + 5,
             20,
@@ -364,17 +359,19 @@
     """
     Calculates a steps for each process. Creates an automaton and calculates one step at a time.
     Puts in queue: list of [coordinates of active cells with their respective color, days elapsed,
     CellCunter(for graphs)]
     """
 
     automaton = FiniteAutomaton(Grid(GRID_SIZE[1], GRID_SIZE[0]), variables)
-    automaton.grid.place_entity(TrueStemCell(), start_x, start_y)
-    automaton.grid.place_entity(ImmuneCell(), 1, 1)
+    automaton.grid.place_entity(TrueStemCell(proliferation_potential=variables.max_proliferation_potential), start_x, start_y)
+    if variables.immune_response:
+        automaton.grid.place_entity(ImmuneCell(), 1, 1)
     while True:
+
         if queue.empty() and active.value:
             automaton.next()
             automaton.variables.time_step()
             queue.put(
                 (
                     automaton.grid.coloured_cells,
                     automaton.variables.days_elapsed,
@@ -441,36 +438,35 @@
             args=(simulation_variables[i],
                   simulation.queue,
                   running_sim,
                   GRID_SIZE[0] // 2,
                   GRID_SIZE[1] // 2),
         )
         new_process.start()
+        processes.append(new_process)
 
     prepare_board()
 
     pygame.display.set_caption("Cancer simulation")
+    run = True
 
-    while True:
-
+    while run:
 
         if all(simulation.has_frames for simulation in simulations):
             for chart in charts:
                 chart.draw()
 
             for simulation in simulations:
                 simulation.draw()
 
         for event in pygame.event.get():
             if event.type == pygame.QUIT:
-                for simulation in processes:
-                    simulation.kill()
-                pygame.quit()
-                sys.exit()
 
+                run = False
+                break 
             if event.type == pygame.KEYDOWN and event.key == pygame.K_s:
                 running_sim.value = (running_sim.value + 1) % 2
 
             if event.type == pygame.VIDEORESIZE or event.type == pygame.VIDEOEXPOSE:
                 prepare_board()
 
         pygame.display.update()
@@ -480,15 +476,15 @@
             DASHBOARD_X_Y[0] + 10,
             DASHBOARD_X_Y[1] + 5,
             20,
             (174, 198, 207),
             (0, 0, 0),
         )
 
-        render_sim_status(40, DASHBOARD_X_Y[1])
+        render_sim_status()
 
         render_text(
             "Days elapsed: " + str(simulations[0].days),
             DASHBOARD_X_Y[0] + 320,
             DASHBOARD_X_Y[1] + 5,
             20,
             (174, 198, 207),
@@ -498,8 +494,13 @@
         render_text(
             "Config filename: " + str(args.config_file),
             DASHBOARD_X_Y[0] + 540,
             DASHBOARD_X_Y[1] + 5,
             20,
             (174, 198, 207),
             (0, 0, 0),
-        )
+        )
+
+    for process in processes:
+        process.kill()
+
+    pygame.quit()
```

### Comparing `cancer_simulation-0.7.2/src/entity.py` & `cancer_simulation-0.7.3/src/entity.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,35 @@
 """Entities"""
 import math
 import numpy as np
 from random import random, choice
-from .variables import Variables
+from .variables import Variables, LOW_PROLIFERATION_COLOR, MAX_PROLIFERATION_COLOR
 from .cell import Cell
 
 
-MAX_PROLIFERATION_POTENTIAL = 30
-MAX_PROLIFERATION_COLOR = np.array([250,0,0])
-LOW_PROLIFERATION_COLOR = np.array([0, 0, 0])
-
-DELTA = ( MAX_PROLIFERATION_COLOR - LOW_PROLIFERATION_COLOR ) / MAX_PROLIFERATION_POTENTIAL
-
 
 def get_chemo_death_probability(theta, k, y, variables: Variables) -> float:
     """Return probability of cell's death due to chemotherapy"""
     l = k * variables.drug_concentration / (theta * y * variables.injection_number + 1)
-    return l * variables.PK * math.e ** ( -variables.ci * (variables.days_elapsed - \
-            variables.injection_number * variables.time_constant))
+    return l * variables.PK * math.e ** ( -variables.ci * variables.days_from_injection)
 
 
 class Entity:
     """Entity"""
 
     __dict__ = ["cell", "neighbors", "free_neighbors", "variables"]
 
     def __init__(self) -> None:
         """Initialize entity"""
         self.cell = None
         self.neighbors = None
         self.free_neighbors = None
         self.variables = None
 
-    def next_state(self) -> None:
+    def next_state(self, *args, **kwargs) -> None:
         """Mutate cell or neighbors to represent the next state"""
 
     def move_to(self, next_cell: Cell) -> None:
         """Move from current cell to next"""
         self.cell.entity = None
         next_cell.entity = self
 
@@ -57,16 +50,15 @@
 class BiologicalCell(Entity):
     """Biological cell"""
 
     ID = 1
 
     __dict__ = ["ID", "proliferation_potential", "cell", "neighbors", "free_neighbors", "variables"]
 
-    def __init__(self, proliferation_potential=MAX_PROLIFERATION_POTENTIAL,
-                 *args, **kwargs) -> None:
+    def __init__(self, *args, proliferation_potential=None, **kwargs) -> None:
         """Initialize Biological cell"""
         super().__init__(*args, **kwargs)
 
         self.proliferation_potential = proliferation_potential
         self.energy_level = 0
 
     @property
@@ -75,23 +67,32 @@
         return self.variables.pA
 
     @property
     def proliferation_probability(self) -> float:
         """Return probability of proliferation"""
         return self.variables.p0 * (1 - (self.cell.distance / (self.variables.Rmax - self.variables.Kc) ))
 
+    def process_chemotherapy(self, theta: float, death: float) -> None:
+        """Process the effect of the chemotherapy"""
+        if not self.variables.is_treatment:
+            return
+
+        chemo_death_probability = self.get_chemo_death_probability(theta=theta)
+        if death <= chemo_death_probability:
+            self.apotose()
+
+    def get_chemo_death_probability(self, theta) -> float:
+        """Return the probability of death due to chemotherapy"""
+        return 0
+
     @property
     def migration_probability(self) -> float:
         """Return probability of migration"""
         return self.variables.mu
 
-    def next_state(self, *random_values) -> None:
-        """Next state implementation to BiologicalCell"""
-        pass
-
     def proliferate(self) -> None:
         """Proliferate"""
         free_neighbors = self.free_neighbors
         if not free_neighbors:
             return
 
         free_cell = choice(free_neighbors)
@@ -100,15 +101,15 @@
             self.apotose()
             return
 
         free_cell.entity = self.replicate()
 
     def replicate(self) -> Entity:
         """Return daughter cell"""
-        daughter =  BiologicalCell(self.proliferation_potential - 1)
+        daughter =  BiologicalCell(proliferation_potential=self.proliferation_potential - 1)
         self.proliferation_potential -= 1
         return daughter
 
     def apotose(self) -> None:
         """Cell death"""
         self.cell.entity = None
 
@@ -117,162 +118,158 @@
         r, g, b =  LOW_PROLIFERATION_COLOR + self.proliferation_potential * DELTA
         return int(r), int(g), int(b)
 
 
 class CancerCell(BiologicalCell):
     """Cancer cell"""
 
-    def __init__(self, proliferation_potential=MAX_PROLIFERATION_POTENTIAL,
-                 *args, **kwargs) -> None:
-        super().__init__(proliferation_potential, *args, **kwargs)
-
-    def next_state(self, variables: Variables, *random_variables) -> None:
-        apotosis, proliferation, migration, theta, death = random_variables
+    def next_state(self, *random_variables) -> None:
+        apotosis, proliferation, migration, theta, death, *_ = random_variables
 
         if apotosis <= self.apotisis_probability:
             self.apotose()
             return
 
         if proliferation <= self.proliferation_probability:
             self.proliferate()
 
         if migration <= self.migration_probability:
             self.move_to_random()
 
-        self.process_chemotherapy(variables=variables, theta=theta, death=death)
+        self.process_chemotherapy(theta=theta, death=death)
 
-        if self.energy_level >= variables.quiescent_distance:
+        if self.energy_level >= self.variables.quiescent_distance:
             self.cell.entity = QuiescentCell(self)
 
-        if self.energy_level >= variables.necrotic_distance:
+        if self.energy_level >= self.variables.necrotic_distance:
             self.cell.entity = NecroticCell()
 
 
-    def process_chemotherapy(self, variables: Variables, theta: float, death: float) -> None:
-        """Process the effect of the chemotherapy"""
-
-        if not variables.is_treatment:
-            return
-
-        chemo_death_probability = self.get_chemo_death_probability(theta=theta, variables=variables)
-
-        if death <= chemo_death_probability:
-            self.apotose()
-
-    def get_chemo_death_probability(self, variables, theta) -> float:
+    def get_chemo_death_probability(self, theta) -> float:
         """Return the probability of death due to chemotherapy"""
-        return   get_chemo_death_probability(theta=theta,
-                                             k=variables.kPC,
-                                             y=variables.yPC,
-                                             variables=variables)
+        return  get_chemo_death_probability(theta=theta,
+                                             k=self.variables.kPC,
+                                             y=self.variables.yPC,
+                                             variables=self.variables)
 
     def replicate(self) -> Entity:
         """Return daughter cell"""
-        daughter =  CancerCell(self.proliferation_potential - 1)
+        daughter =  CancerCell(proliferation_potential=self.proliferation_potential - 1)
         self.proliferation_potential -= 1
         return daughter
 
     @property
     def color(self) -> tuple[int, int, int]:
-        r, g, b =  LOW_PROLIFERATION_COLOR + self.proliferation_potential * DELTA
+        if not self.variables:
+            r, g, b = MAX_PROLIFERATION_COLOR
+        else:
+            r, g, b =  LOW_PROLIFERATION_COLOR + self.proliferation_potential * self.variables.color_delta
         return int(r), int(g), int(b)
 
 
-class QuiescentCell(BiologicalCell):
+class QuiescentCell(CancerCell):
     """Quiescent cell"""
 
     def __init__(self, previous_entity, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.previous_entity = previous_entity
 
-    def next_state(self, variables: Variables, *random_variables) -> None:
+    def next_state(self, *_) -> None:
         if self.energy_level < self.variables.quiescent_distance:
             self.cell.entity = self.previous_entity
 
+        if self.energy_level > self.variables.necrotic_distance:
+            self.cell.entity = NecroticCell()
+
     @property
     def color(self):
         return self.previous_entity
 
 
-class NecroticCell(BiologicalCell):
+class NecroticCell(CancerCell):
     """Necrotic cell"""
 
-    def next_state(self, variables: Variables, *random_variables) -> None:
-        pass
+    def next_state(self, *args, **kwargs) -> None:
+        """Necrotic cell cannot do anything"""
 
     @property
     def color(self):
         return (133, 21, 21)
 
 
 class TrueStemCell(CancerCell):
     """
     True Stem cell.
     Cell that is immortal and can give birth to either
     RTC or other True stem cell
-    """
+    """     
 
     ID = 3
 
     @property
     def apotisis_probability(self) -> float:
         """Return probability of spontaneous death"""
         return 0
 
     def replicate(self) -> Entity:
         """Return daughter cell"""
         new_stem_chance = random()
         if new_stem_chance <= self.variables.pS:
-            daughter = TrueStemCell(self.proliferation_potential)
+            daughter = TrueStemCell(proliferation_potential=self.proliferation_potential)
         else:
-            daughter =  CancerCell(self.proliferation_potential)
+            daughter =  CancerCell(proliferation_potential=self.proliferation_potential)
         return daughter
 
-    def get_chemo_death_probability(self, variables, theta) -> float:
+    def get_chemo_death_probability(self, theta) -> float:
         return 0
 
     @property
     def color(self):
         return 255, 238, 0
 
 
 class ImmuneCell(BiologicalCell):
     """Immune cell"""
 
-    def next_state(self, variables: Variables, *random_values) -> None:
-        *_, cancer_cell_death_probability, immune_cell_death_probability = random_values
+    def next_state(self, *random_values) -> None:
+        *_, theta , death, cancer_cell_death_probability, immune_cell_death_probability = random_values
 
         self.move_to_random(immune_cell_death_probability)
 
         for neighbor in self.neighbors:
             if neighbor.empty:
                 continue
 
             if isinstance(neighbor.entity, CancerCell):
-                if cancer_cell_death_probability <= variables.pdT:
+                if cancer_cell_death_probability <= self.variables.pdT:
                     neighbor.entity = None
 
-                if immune_cell_death_probability <= variables.pdI:
+                if immune_cell_death_probability <= self.variables.pdI:
                     self.apotose()
 
                 break
 
+        self.process_chemotherapy(death=death, theta=theta)
+
+
+    def get_chemo_death_probability(self, theta) -> float:
+        """Return the probability of death due to chemotherapy"""
+        return  get_chemo_death_probability(theta=theta,
+                                             k=self.variables.kI,
+                                             y=self.variables.yI,
+                                             variables=self.variables)
+
     def move_to_random(self, direction_probability) -> None:
         """Move to random free neighbor"""
 
-        if direction_probability <= self.variables.ics:
-            free_neighbor = sorted(self.free_neighbors, key=lambda c: c.distance)[:3]
-        else:
-            free_neighbor = sorted(self.free_neighbors, key=lambda c: c.distance)
-
         if not self.cell.entity: # cell has died
             return
 
-        if not free_neighbor:
+        if not self.free_neighbors:
             return
 
-        cell = choice(free_neighbor)
-        self.move_to(cell)
+        cell = choice(self.free_neighbors)
+        self.move_to(cell)   
 
     @property
     def color(self):
         return 245, 91, 209
```

### Comparing `cancer_simulation-0.7.2/src/grid.py` & `cancer_simulation-0.7.3/src/grid.py`

 * *Files identical despite different names*

### Comparing `cancer_simulation-0.7.2/src/variables.py` & `cancer_simulation-0.7.3/src/variables.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,52 @@
 """Variables"""
 import yaml
+import numpy as np
+
+
+MAX_PROLIFERATION_COLOR = np.array([250,0,0])
+LOW_PROLIFERATION_COLOR = np.array([0, 0, 0])
+
 
 class Variables:
     """Variables"""
 
     def __init__(self,
                  name=None,
                  p0=0.7, pA=0, pS=0.1, ap=0.42, bn=0.53,
                  Kc=10, Rmax=100, pdT=0.5, pdI=0.5,
                  yPC=0.55, yQ=0.4, yI=0.7, kPC=0.8, mu=0.4, ics=0.4,
-                 max_immune_cell_count=2000,
+                 max_immune_cell_count=2000, immune_response=True,
+                 treatment=True,
                  kQ=0.4, kI=0.6, ci=0.5, PK=1, max_energy_level=30,
                  necrotic_distance=30, quiescent_distance=30,
                  treatment_start_time=10, injection_interval=10,
-                 time_constant=3, drug_concentration=0.1
+                 time_constant=3, drug_concentration=0.1,
+                 max_proliferation_potential=20,
                  ) -> None:
         self.name = name
 
         # Static variables
         self.p0 = p0
         self.pA = pA
         self.pS = pS
         self.mu = mu
 
+        self.immune_response = immune_response
         self.ics = ics
         self.max_immune_cell_count = max_immune_cell_count
+        self.max_proliferation_potential = max_proliferation_potential
 
         self.ap = ap
         self.bn = bn
 
         self.Kc = Kc
         self.Rmax = Rmax
 
+        self.treatment = treatment
         self.pdT = pdT
         self.pdI = pdI
 
         self.yPC = yPC
         self.yQ = yQ
         self.yI = yI
         self.kPC = kPC
@@ -51,18 +62,21 @@
         self.treatment_start_time = treatment_start_time
         self.injection_interval = injection_interval
         self.time_constant = time_constant
         self.drug_concentration = drug_concentration
 
         # Dynamic variables
         self.Rt = 0
+        self.tumor_center = (0, 0)
         self.injection_number = 0
         self.time_delta = 5
         self.time = 0
 
+        self.color_delta = ( MAX_PROLIFERATION_COLOR - LOW_PROLIFERATION_COLOR ) / self.max_proliferation_potential
+
     @property
     def Wp(self) -> float:
         return self.ap * self.Rt ** (2/3)
 
     @property
     def Rn(self) -> float:
         return self.Rt - self.bn * self.Rt ** (2/3)
@@ -74,14 +88,16 @@
     def time_step(self):
         self.time += self.time_delta
 
     @property
     def is_treatment(self) -> bool:
         """Return true if chemotherapy injection is in process"""
 
+        if not self.treatment:
+            return False
         # Treatment has not started yet
         if self.days_elapsed < self.treatment_start_time:
             return False
 
         days_from_start = self.days_elapsed - self.treatment_start_time
 
         # No drug in blood
@@ -99,14 +115,22 @@
 
         days_from_start = self.days_elapsed - self.treatment_start_time
 
         if days_from_start % self.injection_interval == 0 and self.time % 24 == 0:
             return True
         return False
 
+    @property
+    def days_from_injection(self) -> int:
+        """Return number of days from last injection""" 
+        if self.is_injection_start:
+            return 0
+        return self.days_elapsed - self.treatment_start_time - (self.injection_number - 1) * self.injection_interval
+
+
 
 class ConfigFileException(Exception):
     """Exception for incorrect config file"""
 
 
 def read_variables(filepath: str) -> list[Variables]:
     """
```

