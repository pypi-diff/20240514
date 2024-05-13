# Comparing `tmp/journeylib-2.0.2.tar.gz` & `tmp/journeylib-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "journeylib-2.0.2.tar", last modified: Mon May 13 18:00:17 2024, max compression
+gzip compressed data, was "journeylib-2.0.3.tar", last modified: Mon May 13 23:21:07 2024, max compression
```

## Comparing `journeylib-2.0.2.tar` & `journeylib-2.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-13 18:00:17.795108 journeylib-2.0.2/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1471 2024-05-13 18:00:17.788402 journeylib-2.0.2/PKG-INFO
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1147 2024-05-06 08:54:27.000000 journeylib-2.0.2/README.md
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-13 18:00:17.603423 journeylib-2.0.2/journeylib/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       24 2024-04-25 11:14:41.000000 journeylib-2.0.2/journeylib/__init__.py
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1489 2024-05-13 17:58:31.000000 journeylib-2.0.2/journeylib/funciones.py
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2772 2024-05-13 17:14:25.000000 journeylib-2.0.2/journeylib/tests.py
-drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-13 18:00:17.760513 journeylib-2.0.2/journeylib.egg-info/
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1471 2024-05-13 18:00:17.000000 journeylib-2.0.2/journeylib.egg-info/PKG-INFO
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)      254 2024-05-13 18:00:17.000000 journeylib-2.0.2/journeylib.egg-info/SOURCES.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)        1 2024-05-13 18:00:17.000000 journeylib-2.0.2/journeylib.egg-info/dependency_links.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       17 2024-05-13 18:00:17.000000 journeylib-2.0.2/journeylib.egg-info/requires.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       11 2024-05-13 18:00:17.000000 journeylib-2.0.2/journeylib.egg-info/top_level.txt
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)       38 2024-05-13 18:00:17.799623 journeylib-2.0.2/setup.cfg
--rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1361 2024-05-13 17:58:55.000000 journeylib-2.0.2/setup.py
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-13 23:21:07.250957 journeylib-2.0.3/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1471 2024-05-13 23:21:07.242589 journeylib-2.0.3/PKG-INFO
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1147 2024-05-06 08:54:27.000000 journeylib-2.0.3/README.md
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-13 23:21:07.086379 journeylib-2.0.3/journeylib/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       24 2024-04-25 11:14:41.000000 journeylib-2.0.3/journeylib/__init__.py
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1485 2024-05-13 23:20:56.000000 journeylib-2.0.3/journeylib/funciones.py
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     2772 2024-05-13 17:14:25.000000 journeylib-2.0.3/journeylib/tests.py
+drwxrwxrwx   0 pancho    (1000) pancho    (1000)        0 2024-05-13 23:21:07.210646 journeylib-2.0.3/journeylib.egg-info/
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1471 2024-05-13 23:21:06.000000 journeylib-2.0.3/journeylib.egg-info/PKG-INFO
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)      254 2024-05-13 23:21:06.000000 journeylib-2.0.3/journeylib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)        1 2024-05-13 23:21:06.000000 journeylib-2.0.3/journeylib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       17 2024-05-13 23:21:06.000000 journeylib-2.0.3/journeylib.egg-info/requires.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       11 2024-05-13 23:21:06.000000 journeylib-2.0.3/journeylib.egg-info/top_level.txt
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)       38 2024-05-13 23:21:07.253853 journeylib-2.0.3/setup.cfg
+-rwxrwxrwx   0 pancho    (1000) pancho    (1000)     1361 2024-05-13 23:21:02.000000 journeylib-2.0.3/setup.py
```

### Comparing `journeylib-2.0.2/PKG-INFO` & `journeylib-2.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: journeylib
-Version: 2.0.2
+Version: 2.0.3
 Summary: Libreria para gestionar datos del historico del proyecto GPTravel
 Home-page: https://ismigit.fi.upm.es/gptravel-2024/ai-squad/journeygenai
 Author: Equipo JourneyGen UPM
 Author-email: f.gonzalez.lopez@alumnos.upm.es
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `journeylib-2.0.2/README.md` & `journeylib-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `journeylib-2.0.2/journeylib/funciones.py` & `journeylib-2.0.3/journeylib/funciones.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,18 +30,18 @@
 def get_historico_falso(usr, url='http://farlier.org:5000/chat/obtener'):
 
     datos_post = {
         'usr': usr
     }
     response = requests.post(url, json=datos_post)
 
-    return {'respuesta': response.json(), 'codigo': response.status_code}
+    return {'respuesta': response.text, 'codigo': response.status_code}
 
 def ins_historico_falso(usr, msgs, url='http://farlier.org:5000/chat/insertar'):
 
     datos_post = {
         'usr': usr,
         'msgs': msgs
     }
     response = requests.post(url, json=datos_post)
 
-    return {'respuesta': response.json(), 'codigo': response.status_code}
+    return {'respuesta': response.text, 'codigo': response.status_code}
```

### Comparing `journeylib-2.0.2/journeylib/tests.py` & `journeylib-2.0.3/journeylib/tests.py`

 * *Files identical despite different names*

### Comparing `journeylib-2.0.2/journeylib.egg-info/PKG-INFO` & `journeylib-2.0.3/journeylib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: journeylib
-Version: 2.0.2
+Version: 2.0.3
 Summary: Libreria para gestionar datos del historico del proyecto GPTravel
 Home-page: https://ismigit.fi.upm.es/gptravel-2024/ai-squad/journeygenai
 Author: Equipo JourneyGen UPM
 Author-email: f.gonzalez.lopez@alumnos.upm.es
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `journeylib-2.0.2/setup.py` & `journeylib-2.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '2.0.2' #Numero de version que decidamos, cambiarlo al añadir nuevas funcionalidades o cambios
+VERSION = '2.0.3' #Numero de version que decidamos, cambiarlo al añadir nuevas funcionalidades o cambios
 PACKAGE_NAME = 'journeylib' #Nombre de la libreria
 AUTHOR = 'Equipo JourneyGen UPM' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'f.gonzalez.lopez@alumnos.upm.es' #Modificar con vuestros datos
 URL = 'https://ismigit.fi.upm.es/gptravel-2024/ai-squad/journeygenai' #Modificar con vuestros datos
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = 'Libreria para gestionar datos del historico del proyecto GPTravel' #Descripción corta
```

