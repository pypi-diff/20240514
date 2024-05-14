# Comparing `tmp/pynapse-1.0.0.tar.gz` & `tmp/pynapse-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynapse-1.0.0.tar", last modified: Sat May 11 07:18:55 2024, max compression
+gzip compressed data, was "pynapse-1.1.0.tar", last modified: Tue May 14 07:12:59 2024, max compression
```

## Comparing `pynapse-1.0.0.tar` & `pynapse-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 07:18:55.211813 pynapse-1.0.0/
--rw-rw-rw-   0        0        0     2770 2024-05-11 07:18:55.207822 pynapse-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-11 07:18:55.166337 pynapse-1.0.0/Pynapse/
--rw-rw-rw-   0        0        0      180 2024-05-11 04:02:14.000000 pynapse-1.0.0/Pynapse/__init__.py
--rw-rw-rw-   0        0        0     2743 2024-05-11 03:54:04.000000 pynapse-1.0.0/Pynapse/main.py
-drwxrwxrwx   0        0        0        0 2024-05-11 07:18:55.205828 pynapse-1.0.0/Pynapse.egg-info/
--rw-rw-rw-   0        0        0     2770 2024-05-11 07:18:54.000000 pynapse-1.0.0/Pynapse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2024-05-11 07:18:55.000000 pynapse-1.0.0/Pynapse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 07:18:54.000000 pynapse-1.0.0/Pynapse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-11 07:18:54.000000 pynapse-1.0.0/Pynapse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-11 07:18:54.000000 pynapse-1.0.0/Pynapse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2649 2024-05-11 07:18:48.000000 pynapse-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-11 07:18:55.212814 pynapse-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      316 2024-05-11 07:18:18.000000 pynapse-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 07:12:59.856742 pynapse-1.1.0/
+-rw-rw-rw-   0        0        0     2800 2024-05-14 07:12:59.841120 pynapse-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-14 07:12:59.825499 pynapse-1.1.0/Pynapse/
+-rw-rw-rw-   0        0        0      180 2024-05-11 04:02:14.000000 pynapse-1.1.0/Pynapse/__init__.py
+-rw-rw-rw-   0        0        0     3419 2024-05-14 07:06:57.000000 pynapse-1.1.0/Pynapse/main.py
+drwxrwxrwx   0        0        0        0 2024-05-14 07:12:59.841120 pynapse-1.1.0/Pynapse.egg-info/
+-rw-rw-rw-   0        0        0     2800 2024-05-14 07:12:59.000000 pynapse-1.1.0/Pynapse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2024-05-14 07:12:59.000000 pynapse-1.1.0/Pynapse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 07:12:59.000000 pynapse-1.1.0/Pynapse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-14 07:12:59.000000 pynapse-1.1.0/Pynapse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-14 07:12:59.000000 pynapse-1.1.0/Pynapse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2679 2024-05-14 07:09:24.000000 pynapse-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-14 07:12:59.856742 pynapse-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      316 2024-05-14 07:12:22.000000 pynapse-1.1.0/setup.py
```

### Comparing `pynapse-1.0.0/PKG-INFO` & `pynapse-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pynapse
-Version: 1.0.0
+Version: 1.1.0
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 
 # VERSION
 
 *MAJOR.MINOR.PATCH*
 
@@ -66,10 +66,13 @@
 
 Net_Save.load('model.json', layers)                 # Load the network from a json file
 
 prediction = net.forward(np.array([[1,0]]))[0][0]   # You can remove brackets in a variable like this
 print(prediction)                                   # Print the prediction
 ```
 
+# CHANGES
+- added verbose
+
 
 # WHY NAMED "Pynapse"
 #### This module has been named "Pynapse" meaning Python and Synapse
```

### Comparing `pynapse-1.0.0/Pynapse/main.py` & `pynapse-1.1.0/Pynapse/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,25 +39,38 @@
             if isinstance(layer, Activation_Sigmoid):
                 dvalues *= layer.output * (1 - layer.output)  # Sigmoid derivative
             if hasattr(layer, 'backward'):
                 layer.backward(dvalues)
                 dvalues = layer.dinputs
 
 
-    def train(self, X, y, epochs, lr=0.1):
-        for epoch in range(epochs):
-            output = self.forward(X)
-            loss = output - y
-            self.backward(loss)
+    def train(self, X, y, epochs, lr=0.1, v=True):
+        if v == True: # made like this so we are not checking if v = true to print many times (to hopefully be faster than constantly checking)
+            for epoch in range(epochs):
+                output = self.forward(X)
+                loss = output - y
+                self.backward(loss)
 
-            #update weights and biases
-            for layer in self.layers:
-                if hasattr(layer, 'weights'):
-                    layer.weights -= lr * layer.dweights
-                    layer.biases -= lr * layer.dbiases
+                #update weights and biases
+                for layer in self.layers:
+                    if hasattr(layer, 'weights'):
+                        layer.weights -= lr * layer.dweights
+                        layer.biases -= lr * layer.dbiases
+                print(f"Epoch: {epoch} Loss: {loss}")
+        else:
+            for epoch in range(epochs):
+                output = self.forward(X)
+                loss = output - y
+                self.backward(loss)
+
+                #update weights and biases
+                for layer in self.layers:
+                    if hasattr(layer, 'weights'):
+                        layer.weights -= lr * layer.dweights
+                        layer.biases -= lr * layer.dbiases
 
 class Bin_Round:
     def Bin_Round(X):
         if X >= 0.5:
             return 1
         elif X < 0.5:
             return 0
```

### Comparing `pynapse-1.0.0/Pynapse.egg-info/PKG-INFO` & `pynapse-1.1.0/Pynapse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pynapse
-Version: 1.0.0
+Version: 1.1.0
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 
 # VERSION
 
 *MAJOR.MINOR.PATCH*
 
@@ -66,10 +66,13 @@
 
 Net_Save.load('model.json', layers)                 # Load the network from a json file
 
 prediction = net.forward(np.array([[1,0]]))[0][0]   # You can remove brackets in a variable like this
 print(prediction)                                   # Print the prediction
 ```
 
+# CHANGES
+- added verbose
+
 
 # WHY NAMED "Pynapse"
 #### This module has been named "Pynapse" meaning Python and Synapse
```

### Comparing `pynapse-1.0.0/README.md` & `pynapse-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,10 +60,13 @@
 
 Net_Save.load('model.json', layers)                 # Load the network from a json file
 
 prediction = net.forward(np.array([[1,0]]))[0][0]   # You can remove brackets in a variable like this
 print(prediction)                                   # Print the prediction
 ```
 
+# CHANGES
+- added verbose
+
 
 # WHY NAMED "Pynapse"
 #### This module has been named "Pynapse" meaning Python and Synapse
```

