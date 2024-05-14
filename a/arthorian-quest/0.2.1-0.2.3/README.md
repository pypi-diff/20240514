# Comparing `tmp/arthorian-quest-0.2.1.tar.gz` & `tmp/arthorian-quest-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arthorian-quest-0.2.1.tar", last modified: Mon Feb 12 18:23:02 2024, max compression
+gzip compressed data, was "arthorian-quest-0.2.3.tar", last modified: Tue May 14 11:43:31 2024, max compression
```

## Comparing `arthorian-quest-0.2.1.tar` & `arthorian-quest-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-12 18:23:02.032916 arthorian-quest-0.2.1/
--rw-r--r--   0 user       (502) staff       (20)     1069 2023-07-05 13:01:40.000000 arthorian-quest-0.2.1/LICENSE
--rw-r--r--   0 user       (502) staff       (20)     6665 2024-02-12 18:23:02.032618 arthorian-quest-0.2.1/PKG-INFO
--rw-r--r--   0 user       (502) staff       (20)     5808 2024-01-17 15:00:05.000000 arthorian-quest-0.2.1/README.md
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-12 18:23:02.022055 arthorian-quest-0.2.1/arthorian_quest/
--rw-r--r--   0 user       (502) staff       (20)      134 2024-01-17 15:00:05.000000 arthorian-quest-0.2.1/arthorian_quest/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     5125 2024-01-17 15:00:05.000000 arthorian-quest-0.2.1/arthorian_quest/arthorstein.py
--rw-r--r--   0 user       (502) staff       (20)     5299 2024-01-17 14:49:11.000000 arthorian-quest-0.2.1/arthorian_quest/create.py
--rw-r--r--   0 user       (502) staff       (20)     2166 2024-02-12 18:22:46.000000 arthorian-quest-0.2.1/arthorian_quest/ops.py
--rw-r--r--   0 user       (502) staff       (20)     2833 2023-12-08 16:54:14.000000 arthorian-quest-0.2.1/arthorian_quest/query.py
--rw-r--r--   0 user       (502) staff       (20)     2341 2023-11-16 17:06:23.000000 arthorian-quest-0.2.1/arthorian_quest/quick_place.py
--rw-r--r--   0 user       (502) staff       (20)      376 2024-01-17 14:36:46.000000 arthorian-quest-0.2.1/arthorian_quest/shorthands.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-12 18:23:02.032212 arthorian-quest-0.2.1/arthorian_quest.egg-info/
--rw-r--r--   0 user       (502) staff       (20)     6665 2024-02-12 18:23:01.000000 arthorian-quest-0.2.1/arthorian_quest.egg-info/PKG-INFO
--rw-r--r--   0 user       (502) staff       (20)      414 2024-02-12 18:23:01.000000 arthorian-quest-0.2.1/arthorian_quest.egg-info/SOURCES.txt
--rw-r--r--   0 user       (502) staff       (20)        1 2024-02-12 18:23:01.000000 arthorian-quest-0.2.1/arthorian_quest.egg-info/dependency_links.txt
--rw-r--r--   0 user       (502) staff       (20)       35 2024-02-12 18:23:01.000000 arthorian-quest-0.2.1/arthorian_quest.egg-info/requires.txt
--rw-r--r--   0 user       (502) staff       (20)       16 2024-02-12 18:23:01.000000 arthorian-quest-0.2.1/arthorian_quest.egg-info/top_level.txt
--rw-r--r--   0 user       (502) staff       (20)       38 2024-02-12 18:23:02.032954 arthorian-quest-0.2.1/setup.cfg
--rw-r--r--   0 user       (502) staff       (20)     1858 2024-02-12 18:22:46.000000 arthorian-quest-0.2.1/setup.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-14 11:43:31.521302 arthorian-quest-0.2.3/
+-rw-r--r--   0 user       (502) staff       (20)     1069 2023-07-05 13:01:40.000000 arthorian-quest-0.2.3/LICENSE
+-rw-r--r--   0 user       (502) staff       (20)     6665 2024-05-14 11:43:31.519468 arthorian-quest-0.2.3/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)     5808 2024-01-17 15:00:05.000000 arthorian-quest-0.2.3/README.md
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-14 11:43:31.484636 arthorian-quest-0.2.3/arthorian_quest/
+-rw-r--r--   0 user       (502) staff       (20)      134 2024-01-17 15:00:05.000000 arthorian-quest-0.2.3/arthorian_quest/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     5665 2024-05-08 12:25:53.000000 arthorian-quest-0.2.3/arthorian_quest/arthorstein.py
+-rw-r--r--   0 user       (502) staff       (20)     5299 2024-01-17 14:49:11.000000 arthorian-quest-0.2.3/arthorian_quest/create.py
+-rw-r--r--   0 user       (502) staff       (20)     2203 2024-05-14 11:42:15.000000 arthorian-quest-0.2.3/arthorian_quest/ops.py
+-rw-r--r--   0 user       (502) staff       (20)     2998 2024-02-13 09:51:10.000000 arthorian-quest-0.2.3/arthorian_quest/query.py
+-rw-r--r--   0 user       (502) staff       (20)     2341 2023-11-16 17:06:23.000000 arthorian-quest-0.2.3/arthorian_quest/quick_place.py
+-rw-r--r--   0 user       (502) staff       (20)      376 2024-01-17 14:36:46.000000 arthorian-quest-0.2.3/arthorian_quest/shorthands.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-14 11:43:31.517371 arthorian-quest-0.2.3/arthorian_quest.egg-info/
+-rw-r--r--   0 user       (502) staff       (20)     6665 2024-05-14 11:43:30.000000 arthorian-quest-0.2.3/arthorian_quest.egg-info/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)      414 2024-05-14 11:43:31.000000 arthorian-quest-0.2.3/arthorian_quest.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (502) staff       (20)        1 2024-05-14 11:43:30.000000 arthorian-quest-0.2.3/arthorian_quest.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (502) staff       (20)       35 2024-05-14 11:43:30.000000 arthorian-quest-0.2.3/arthorian_quest.egg-info/requires.txt
+-rw-r--r--   0 user       (502) staff       (20)       16 2024-05-14 11:43:30.000000 arthorian-quest-0.2.3/arthorian_quest.egg-info/top_level.txt
+-rw-r--r--   0 user       (502) staff       (20)       38 2024-05-14 11:43:31.521559 arthorian-quest-0.2.3/setup.cfg
+-rw-r--r--   0 user       (502) staff       (20)     1858 2024-05-14 11:43:24.000000 arthorian-quest-0.2.3/setup.py
```

### Comparing `arthorian-quest-0.2.1/LICENSE` & `arthorian-quest-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arthorian-quest-0.2.1/PKG-INFO` & `arthorian-quest-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthorian-quest
-Version: 0.2.1
+Version: 0.2.3
 Summary: using Arthor and filtering the results with Fragmenstein
 Home-page: https://github.com/matteoferla/arthorian-quest
 Author: Matteo Ferla
 Author-email: matteo.ferla@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `arthorian-quest-0.2.1/README.md` & `arthorian-quest-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `arthorian-quest-0.2.1/arthorian_quest/arthorstein.py` & `arthorian-quest-0.2.3/arthorian_quest/arthorstein.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from rdkit import Chem
 from rdkit.Chem import AllChem
 import contextlib
 import pandas as pd
 import warnings
 from .query import QueryArthor
-from typing import Dict, Union, Optional
+from typing import Dict, Union, Optional, List
 
 
 def prep_for_laboratory(query_mol: Chem.Mol,
                         template_mol: Chem.Mol,
                         experiment_name:str='') \
         -> pd.DataFrame:
     """
@@ -45,15 +45,15 @@
     placements = pd.DataFrame()
     with contextlib.suppress(KeyError):
         tobeplaced = create_laboratory_df(query, template, experiment_name=experiment_name)
         placements = Laboratory(pdb_block).place(tobeplaced)
     placements['experiment'] = experiment_name
     return placements
 
-def create_laboratory_df(query_mol: Chem.Mol, template_mol: Chem.Mol, experiment_name: str= '') -> pd.DataFrame:
+def create_laboratory_df(query_mols: List[Chem.Mol], template_mols: List[Chem.Mol], experiment_name: str= '') -> pd.DataFrame:
     """
     Given a query molecule and a template molecule, return a dataframe of analogues
     by searching Arthor.
     This dataframe is ready to be passed to ``Laboratory.place``.
     It has the columns:
 
     * name: the name of the analogue
@@ -62,31 +62,39 @@
     * experiment: the name of the experiment
 
     :param query_mol:
     :param template_mol:
     :param experiment_name:
     :return:
     """
+    if isinstance(query_mols, Chem.Mol):
+        query_mols = [query_mols]
+    if isinstance(template_mols, Chem.Mol):
+        template_mols = [template_mols]
+    assert len(query_mols) == len(template_mols), 'Query and template molecules must be the same length (=paired)'
     # ## Sanitize
-    if not experiment_name and query_mol.HasProp('experiment'):
-        experiment_name = query_mol.GetProp('experiment')
-    query_mol.SetProp('experiment', experiment_name)
-    query_mol.SetProp('template', template_mol.GetProp('_Name'))
+    if not experiment_name and query_mols[0].HasProp('experiment'):
+        experiment_name = query_mols[0].GetProp('experiment')
+    for query_mol, template_mol in zip(query_mols, template_mols):
+        query_mol.SetProp('experiment', experiment_name)
+        query_mol.SetProp('template', template_mol.GetProp('_Name'))
+        query_mol.UpdatePropertyCache()
     # ## Run search
     arthor = QueryArthor()
-    df = arthor.retrieve(Chem.MolToSmarts(query_mol), ['real-database-22q1'])
-    query_mol.UpdatePropertyCache()
+    df = arthor.retrieve('.'.join([Chem.MolToSmarts(query_mol) for query_mol in query_mols]),
+                         ['real-database-22q1'])
     #AllChem.SanitizeMol(query)
     # exit early if no hits
     if len(df) == 0:
         return pd.DataFrame()
     try:
         df = df.rename(columns={'id': 'name'})
-        df['hits'] = df.smiles.apply(lambda s: [template_mol])
-        mapper = lambda smiles: {template_mol.GetProp('_Name'): get_custom_map(query_mol, template_mol, smiles)}
+        df['hits'] = df.smiles.apply(lambda s: template_mols)
+        mapper = lambda smiles: {template_mol.GetProp('_Name'): get_custom_map(query_mol, template_mol, smiles)
+                                 for query_mol, template_mol in zip(query_mols, template_mols)}
         df['custom_map'] = df.smiles.apply(mapper)
         df['experiment'] = experiment_name
         return df
     except Exception as error:
         print(error.__class__.__name__, error)
         return df
```

### Comparing `arthorian-quest-0.2.1/arthorian_quest/create.py` & `arthorian-quest-0.2.3/arthorian_quest/create.py`

 * *Files identical despite different names*

### Comparing `arthorian-quest-0.2.1/arthorian_quest/ops.py` & `arthorian-quest-0.2.3/arthorian_quest/ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from rdkit import RDLogger, Chem
 from rdkit.Chem import AllChem, Draw
 from IPython.display import display
 from IPython.display import Image as IPythonImage
 from typing import Union
 import PIL
+from PIL.Image import Image as PILImage
 import requests
 import io
 
 
 def silence_rdkit():
     """
     Silence RDKit warnings
@@ -33,29 +34,29 @@
     display(query)
     if save:
         Draw.MolToFile(query, f'{experiment_name}.png')
     return None
 
 
 
-def retrieve_smartsplus(smarts: Union[str, Chem.Mol], PIL_image=True, **options) -> Union[IPythonImage, PIL.Image]:
+def retrieve_smartsplus(smarts: Union[str, Chem.Mol], PIL_image=True, **options) -> Union[IPythonImage, PILImage]:
     """
     Given a SMARTS query, retrieve the image from https://smarts.plus.
     The returned object is an IPython.display.Image not a PIL.Image.
     If using this image remember to cite it as
     "SMARTSviewer smartsview.zbh.uni-hamburg.de, ZBH Center for Bioinformatics, University of Hamburg"
 
     :param smarts: SMARTS query or Chem.Mol
     :param PIL_image: return PIL.Image instead of IPython.display.Image
     :param options: See https://smarts.plus/rest
     :return:
     """
     if isinstance(smarts, Chem.Mol):
         q = smarts
-        smarts: str = Chem.MolFromSmarts(q)
+        smarts: str = Chem.MolToSmarts(q)
     # retrieve from smarts.plus
     response: requests.Response = requests.get('https://smarts.plus/smartsview/download_rest', # noqa to sensitive data in options
                                                {'smarts': smarts, **options}
                                               )
     png_binary: bytes = response.content
     if PIL_image:
         return PIL.Image.open(io.BytesIO(png_binary))
```

### Comparing `arthorian-quest-0.2.1/arthorian_quest/query.py` & `arthorian-quest-0.2.3/arthorian_quest/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,17 @@
         if isinstance(query, Chem.Mol):
             query = Chem.MolToSmarts(query)
         response: requests.Response = requests.get(self.base_url + f'/dt/{dbname}/search',
                                                    dict(query=query,
                                                         type=search_type,
                                                         length=length)
                                                    )
+        if response.status_code == 503:
+            raise ConnectionError('Arthor unavailable. cf. https://arthor.docking.org/')
+        response.raise_for_status()
         data: dict = response.json()
         if data.get("message", '') == "SMARTS query is always false!":
             warnings.warn(f"SMARTS query {query} is always false")
             return pd.DataFrame()
         if data.get('warning',''):
             warnings.warn(data['warning'])
         if not data.get('recordsTotal', False):
```

### Comparing `arthorian-quest-0.2.1/arthorian_quest/quick_place.py` & `arthorian-quest-0.2.3/arthorian_quest/quick_place.py`

 * *Files identical despite different names*

### Comparing `arthorian-quest-0.2.1/arthorian_quest.egg-info/PKG-INFO` & `arthorian-quest-0.2.3/arthorian_quest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthorian-quest
-Version: 0.2.1
+Version: 0.2.3
 Summary: using Arthor and filtering the results with Fragmenstein
 Home-page: https://github.com/matteoferla/arthorian-quest
 Author: Matteo Ferla
 Author-email: matteo.ferla@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `arthorian-quest-0.2.1/setup.py` & `arthorian-quest-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         requirements = [line.split('#')[0].strip() for line in f.readlines()]
         requirements = [line for line in requirements if line]
 else:
     requirements = []
 
 setup(
     name='arthorian-quest',
-    version='0.2.1',
+    version='0.2.3',
     description='using Arthor and filtering the results with Fragmenstein',
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.7',
     packages=find_packages(),
     include_package_data=True,
     install_requires=requirements,
```

