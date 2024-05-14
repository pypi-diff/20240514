# Comparing `tmp/royalspells-3.2.tar.gz` & `tmp/royalspells-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/royalspells-3.2.tar", last modified: Mon Mar 25 11:36:55 2019, max compression
+gzip compressed data, was "royalspells-4.0.0.tar", last modified: Tue May 14 01:55:38 2024, max compression
```

## Comparing `royalspells-3.2.tar` & `royalspells-4.0.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 steffo    (1001) steffo    (1001)        0 2019-03-25 11:36:55.000000 royalspells-3.2/
--rw-r--r--   0 steffo    (1001) steffo    (1001)      620 2019-03-25 11:36:55.000000 royalspells-3.2/PKG-INFO
--rw-r--r--   0 steffo    (1001) steffo    (1001)       68 2019-03-25 10:44:39.000000 royalspells-3.2/README.md
-drwxr-xr-x   0 steffo    (1001) steffo    (1001)        0 2019-03-25 11:36:55.000000 royalspells-3.2/royalspells/
--rw-r--r--   0 steffo    (1001) steffo    (1001)      225 2019-03-25 10:40:55.000000 royalspells-3.2/royalspells/__init__.py
--rw-r--r--   0 steffo    (1001) steffo    (1001)     7158 2019-03-25 10:54:39.000000 royalspells-3.2/royalspells/main.py
-drwxr-xr-x   0 steffo    (1001) steffo    (1001)        0 2019-03-25 11:36:55.000000 royalspells-3.2/royalspells.egg-info/
--rw-r--r--   0 steffo    (1001) steffo    (1001)      620 2019-03-25 11:36:54.000000 royalspells-3.2/royalspells.egg-info/PKG-INFO
--rw-r--r--   0 steffo    (1001) steffo    (1001)      202 2019-03-25 11:36:54.000000 royalspells-3.2/royalspells.egg-info/SOURCES.txt
--rw-r--r--   0 steffo    (1001) steffo    (1001)        1 2019-03-25 11:36:54.000000 royalspells-3.2/royalspells.egg-info/dependency_links.txt
--rw-r--r--   0 steffo    (1001) steffo    (1001)       12 2019-03-25 11:36:54.000000 royalspells-3.2/royalspells.egg-info/top_level.txt
--rw-r--r--   0 steffo    (1001) steffo    (1001)       38 2019-03-25 11:36:55.000000 royalspells-3.2/setup.cfg
--rw-r--r--   0 steffo    (1001) steffo    (1001)      739 2019-03-25 11:23:56.000000 royalspells-3.2/setup.py
+drwxr-xr-x   0 steffo    (2000) steffo    (2000)        0 2024-05-14 01:55:38.464401 royalspells-4.0.0/
+-rw-r--r--   0 steffo    (2000) steffo    (2000)     1072 2024-05-14 01:38:04.000000 royalspells-4.0.0/LICENSE.txt
+-rw-r--r--   0 steffo    (2000) steffo    (2000)      718 2024-05-14 01:55:38.463401 royalspells-4.0.0/PKG-INFO
+-rw-r--r--   0 steffo    (2000) steffo    (2000)      227 2024-05-14 01:42:41.000000 royalspells-4.0.0/README.md
+drwxr-xr-x   0 steffo    (2000) steffo    (2000)        0 2024-05-14 01:55:38.462401 royalspells-4.0.0/royalspells/
+-rw-r--r--   0 steffo    (2000) steffo    (2000)      225 2024-05-14 01:38:04.000000 royalspells-4.0.0/royalspells/__init__.py
+-rw-r--r--   0 steffo    (2000) steffo    (2000)     7662 2024-05-14 01:52:24.000000 royalspells-4.0.0/royalspells/main.py
+drwxr-xr-x   0 steffo    (2000) steffo    (2000)        0 2024-05-14 01:55:38.463401 royalspells-4.0.0/royalspells.egg-info/
+-rw-r--r--   0 steffo    (2000) steffo    (2000)      718 2024-05-14 01:55:38.000000 royalspells-4.0.0/royalspells.egg-info/PKG-INFO
+-rw-r--r--   0 steffo    (2000) steffo    (2000)      214 2024-05-14 01:55:38.000000 royalspells-4.0.0/royalspells.egg-info/SOURCES.txt
+-rw-r--r--   0 steffo    (2000) steffo    (2000)        1 2024-05-14 01:55:38.000000 royalspells-4.0.0/royalspells.egg-info/dependency_links.txt
+-rw-r--r--   0 steffo    (2000) steffo    (2000)       12 2024-05-14 01:55:38.000000 royalspells-4.0.0/royalspells.egg-info/top_level.txt
+-rw-r--r--   0 steffo    (2000) steffo    (2000)       38 2024-05-14 01:55:38.464401 royalspells-4.0.0/setup.cfg
+-rw-r--r--   0 steffo    (2000) steffo    (2000)      724 2024-05-14 01:54:22.000000 royalspells-4.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `royalspells-3.2/royalspells/main.py` & `royalspells-4.0.0/royalspells/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -80,20 +80,25 @@
 
 class StatsComponent:
     all_stats = ["Attacco", "Difesa", "Velocità", "Elusione", "Tenacia", "Rubavita",
                  "Vampirismo", "Forza", "Destrezza", "Costituzione", "Intelligenza",
                  "Saggezza", "Carisma", "Attacco Speciale", "Difesa Speciale",
                  "Eccellenza", "Immaginazione", "Cromosomi", "Timidezza", "Sonno",
                  "Elasticità", "Peso", "Sanità", "Appetito", "Fortuna", "Percezione",
-                 "Determinazione"]
-
-    change_distribution = (["--"] * 1) + \
-                          (["-"] * 2) + \
-                          (["+"] * 2) + \
-                          (["++"] * 1)
+                 "Determinazione", "Chips", "Mult", "Nucleare", "Psiche", "Psicologia",
+                 "Garasauto", "Tifoseria", "Gioia", "Visione", "Visibilità", "Fuffa",
+                 "Morbidezza", "Magia", "Spettacolo", "Appeal", "Infezione", "Infestazione"
+                 "Genere"]
+
+    change_distribution = (["--"] * 16) + \
+                          (["-"] * 32) + \
+                          (["+"] * 32) + \
+                          (["++"] * 16) + \
+                          (["×2"] * 2) + \
+                          (["×3"] * 1)
 
     multistat_distribution = ([1] * 16) + \
                              ([2] * 8) + \
                              ([3] * 4) + \
                              ([5] * 2) + \
                              ([8] * 1)
 
@@ -113,19 +118,21 @@
 
 
 class StatusEffectComponent:
     all_status_effects = ["Bruciatura", "Sanguinamento", "Paralisi", "Veleno",
                           "Congelamento", "Iperveleno", "Sonno", "Stordimento",
                           "Rallentamento", "Radicamento", "Rigenerazione", "Morte",
                           "Affaticamento", "Glitch", "Accecamento", "Silenzio",
-                          "Esilio", "Invisibilità", "Rapidità", "Splendore"]
+                          "Esilio", "Invisibilità", "Rapidità", "Splendore",
+                          "Visione notturna", "Resistenza al fuoco", "Respirazione subacqua",
+                          "Debolezza", "Slimed", "Jarate"]
 
     def __init__(self):
         # ENSURE THE SEED IS ALREADY SET WHEN CREATING THIS COMPONENT!!!
-        self.chance = random.randrange(1, 101)
+        self.chance = random.randrange(1, 103)
         self.effect = random.sample(self.all_status_effects, 1)[0]
 
     def __repr__(self):
         return f"<StatusEffectComponent>"
 
 
 class Spell:
```

### Comparing `royalspells-3.2/setup.py` & `royalspells-4.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="royalspells",
-    version="3.2",
+    version="4.0.0",
     author="Stefano Pigozzi",
-    author_email="ste.pigozzi@gmail.com",
-    description="A package to procedurally generate useless spells!",
+    author_email="me@steffo.eu",
+    description="Meaningless fantasy spell stats generator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Steffo99/royalspells",
     packages=setuptools.find_packages(),
     install_requires=[],
-    python_requires="~=3.6",
+    python_requires=">=3.6",
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 6 - Mature",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.6",
     ]
 )
```

