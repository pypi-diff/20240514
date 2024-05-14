# Comparing `tmp/mqttthreaddatalogger-1.5.1.tar.gz` & `tmp/mqttthreaddatalogger-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqttthreaddatalogger-1.5.1.tar", last modified: Sat Apr 15 19:31:37 2023, max compression
+gzip compressed data, was "mqttthreaddatalogger-1.6.0.tar", last modified: Tue May 14 07:03:20 2024, max compression
```

## Comparing `mqttthreaddatalogger-1.5.1.tar` & `mqttthreaddatalogger-1.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 19:31:37.662910 mqttthreaddatalogger-1.5.1/
--rw-rw-rw-   0        0        0     1094 2021-02-10 19:27:17.000000 mqttthreaddatalogger-1.5.1/LICENCE
--rw-rw-rw-   0        0        0     1986 2023-04-15 19:31:37.662910 mqttthreaddatalogger-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1539 2022-04-11 19:22:58.000000 mqttthreaddatalogger-1.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 19:31:37.640877 mqttthreaddatalogger-1.5.1/mqttthreaddatalogger/
--rw-rw-rw-   0        0        0       78 2021-05-20 20:55:44.000000 mqttthreaddatalogger-1.5.1/mqttthreaddatalogger/__init__.py
--rw-rw-rw-   0        0        0     5150 2023-04-15 19:30:12.000000 mqttthreaddatalogger-1.5.1/mqttthreaddatalogger/mqttthreaddatalogger.py
-drwxrwxrwx   0        0        0        0 2023-04-15 19:31:37.662910 mqttthreaddatalogger-1.5.1/mqttthreaddatalogger.egg-info/
--rw-rw-rw-   0        0        0     1986 2023-04-15 19:31:37.000000 mqttthreaddatalogger-1.5.1/mqttthreaddatalogger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-04-15 19:31:37.000000 mqttthreaddatalogger-1.5.1/mqttthreaddatalogger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 19:31:37.000000 mqttthreaddatalogger-1.5.1/mqttthreaddatalogger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-15 19:31:37.000000 mqttthreaddatalogger-1.5.1/mqttthreaddatalogger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-15 19:31:37.000000 mqttthreaddatalogger-1.5.1/mqttthreaddatalogger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 19:31:37.662910 mqttthreaddatalogger-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-04-15 19:31:01.000000 mqttthreaddatalogger-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 07:03:20.527419 mqttthreaddatalogger-1.6.0/
+-rw-rw-rw-   0        0        0     1094 2021-02-10 19:27:17.000000 mqttthreaddatalogger-1.6.0/LICENCE
+-rw-rw-rw-   0        0        0     2080 2024-05-14 07:03:20.526420 mqttthreaddatalogger-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1607 2024-05-14 07:01:22.000000 mqttthreaddatalogger-1.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 07:03:20.500017 mqttthreaddatalogger-1.6.0/mqttthreaddatalogger/
+-rw-rw-rw-   0        0        0       78 2021-05-20 20:55:44.000000 mqttthreaddatalogger-1.6.0/mqttthreaddatalogger/__init__.py
+-rw-rw-rw-   0        0        0     5151 2024-05-14 06:22:51.000000 mqttthreaddatalogger-1.6.0/mqttthreaddatalogger/mqttthreaddatalogger.py
+drwxrwxrwx   0        0        0        0 2024-05-14 07:03:20.524407 mqttthreaddatalogger-1.6.0/mqttthreaddatalogger.egg-info/
+-rw-rw-rw-   0        0        0     2080 2024-05-14 07:03:20.000000 mqttthreaddatalogger-1.6.0/mqttthreaddatalogger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-05-14 07:03:20.000000 mqttthreaddatalogger-1.6.0/mqttthreaddatalogger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 07:03:20.000000 mqttthreaddatalogger-1.6.0/mqttthreaddatalogger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-14 07:03:20.000000 mqttthreaddatalogger-1.6.0/mqttthreaddatalogger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-14 07:03:20.000000 mqttthreaddatalogger-1.6.0/mqttthreaddatalogger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 07:03:20.528419 mqttthreaddatalogger-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      811 2024-05-14 06:23:48.000000 mqttthreaddatalogger-1.6.0/setup.py
```

### Comparing `mqttthreaddatalogger-1.5.1/LICENCE` & `mqttthreaddatalogger-1.6.0/LICENCE`

 * *Files identical despite different names*

### Comparing `mqttthreaddatalogger-1.5.1/PKG-INFO` & `mqttthreaddatalogger-1.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: mqttthreaddatalogger
-Version: 1.5.1
+Version: 1.6.0
 Summary: Connexion mqtt et enregistrement des données dans un fichier csv
 Author: Didier Orlandi
 Author-email: didier.orlandi@wanadoo.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENCE
+Requires-Dist: paho-mqtt
 
 #mqttdatalogger
 
 Enregistrement des données issues d'un serveur MQTT dans un fichier csv.<br />
 
 Exemple d'utilisation : <br />
 
@@ -31,16 +32,16 @@
 # crée le thread transport tcp ou websockets <br />
 m = MQTT.mqttthreaddatalogger("url_mqtt",portmqtt,auth["username"],auth["password"],"tcp")   <br /> 
 # topics auquel on s'abonne<br />
 m.selectTopic(["node_iot2020/arduino/out/"])  <br />
 # selection des clés des données voulues , les données seront dans m.data[0], m.data[1],... <br />
 m.selectKey(["['ecl']","['temps']"])<br />
 # ou pour Lorawan, après le # se trouve le nom du champ qui sera utilisé dans le fichier csv,... <br />
-m.selectKey(["['uplink_message']['decoded_payload']['analog_in_1']#température","['uplink_message']['rx_metadata'][0]['gateway_ids']['gateway_id']#gateway_id","['end_device_ids']['device_id']#device_id"])
-<br />
+m.selectKey(["['uplink_message']['decoded_payload']['temperature']#temp","['uplink_message']['rx_metadata'][0]['gateway_ids']['gateway_id']#Id_gateway","['end_device_ids']['device_id']#ID_device"])
+<br />Après le # on rajoute le nom de la 1ère ligne du fichier de données</br>>
  
 m.selectNomFichier("testdonnees.csv")<br />
 # pour afficher ou non les info sur la console <br />
 m.affichage_console(True) <br />
 # démarre le thread, (exécution indépendante du programme principal)<br />
 m.start()   <br />               
 time.sleep(1)<br />
```

### Comparing `mqttthreaddatalogger-1.5.1/README.md` & `mqttthreaddatalogger-1.6.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 # crée le thread transport tcp ou websockets <br />
 m = MQTT.mqttthreaddatalogger("url_mqtt",portmqtt,auth["username"],auth["password"],"tcp")   <br /> 
 # topics auquel on s'abonne<br />
 m.selectTopic(["node_iot2020/arduino/out/"])  <br />
 # selection des clés des données voulues , les données seront dans m.data[0], m.data[1],... <br />
 m.selectKey(["['ecl']","['temps']"])<br />
 # ou pour Lorawan, après le # se trouve le nom du champ qui sera utilisé dans le fichier csv,... <br />
-m.selectKey(["['uplink_message']['decoded_payload']['analog_in_1']#température","['uplink_message']['rx_metadata'][0]['gateway_ids']['gateway_id']#gateway_id","['end_device_ids']['device_id']#device_id"])
-<br />
+m.selectKey(["['uplink_message']['decoded_payload']['temperature']#temp","['uplink_message']['rx_metadata'][0]['gateway_ids']['gateway_id']#Id_gateway","['end_device_ids']['device_id']#ID_device"])
+<br />Après le # on rajoute le nom de la 1ère ligne du fichier de données</br>>
  
 m.selectNomFichier("testdonnees.csv")<br />
 # pour afficher ou non les info sur la console <br />
 m.affichage_console(True) <br />
 # démarre le thread, (exécution indépendante du programme principal)<br />
 m.start()   <br />               
 time.sleep(1)<br />
```

### Comparing `mqttthreaddatalogger-1.5.1/mqttthreaddatalogger/mqttthreaddatalogger.py` & `mqttthreaddatalogger-1.6.0/mqttthreaddatalogger/mqttthreaddatalogger.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,32 +90,32 @@
     # The callback for when a PUBLISH message is received from the server.
     def on_message(self, client, userdata, msg):
         data = msg.payload.decode("utf-8").strip('\r\n') # decode et enlève les \r \n
         #print("message reçu")
         tab = []
         try:
             y = json.loads(data)
+            if self.verbose :
+                print("json", y)
             for i in range(0,len(self.Key)):
-                #txt = self.Key[i].split("#")# split pour le nom des champs
-                txt = self.Key[i]
-                value = y[txt]
-                #value = eval('y'+txt[0])# la valeur string est évaluée
+                txt = self.Key[i].split("#")# split pour le nom des champs
+                value = eval('y'+str(txt[0]))# la valeur string est évaluée
                 try: 
                     value = float(value)# essaye de convertir en float
                 except:
                     pass  # rien à faire
                 tab.append(value)
             #print("ma key ", tab)
         except:
             if self.verbose :
                 print("problème de lecture JSON ",data)
         else:# si pas d'erreur
             if self.verbose :
-                print(data)
-                #print("réception : ", tab)
+                #print(data)
+                print("réception : ", tab)
             enregistreFichier(self.nomFichier,self.Key,tab)
             #for i in range(len(tab)): 
             #    self.data[i].append(tab[i])
             #print(self.data[0])
             
     def selectTopic(self,top):
         self.topic = top
```

### Comparing `mqttthreaddatalogger-1.5.1/mqttthreaddatalogger.egg-info/PKG-INFO` & `mqttthreaddatalogger-1.6.0/mqttthreaddatalogger.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: mqttthreaddatalogger
-Version: 1.5.1
+Version: 1.6.0
 Summary: Connexion mqtt et enregistrement des données dans un fichier csv
 Author: Didier Orlandi
 Author-email: didier.orlandi@wanadoo.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENCE
+Requires-Dist: paho-mqtt
 
 #mqttdatalogger
 
 Enregistrement des données issues d'un serveur MQTT dans un fichier csv.<br />
 
 Exemple d'utilisation : <br />
 
@@ -31,16 +32,16 @@
 # crée le thread transport tcp ou websockets <br />
 m = MQTT.mqttthreaddatalogger("url_mqtt",portmqtt,auth["username"],auth["password"],"tcp")   <br /> 
 # topics auquel on s'abonne<br />
 m.selectTopic(["node_iot2020/arduino/out/"])  <br />
 # selection des clés des données voulues , les données seront dans m.data[0], m.data[1],... <br />
 m.selectKey(["['ecl']","['temps']"])<br />
 # ou pour Lorawan, après le # se trouve le nom du champ qui sera utilisé dans le fichier csv,... <br />
-m.selectKey(["['uplink_message']['decoded_payload']['analog_in_1']#température","['uplink_message']['rx_metadata'][0]['gateway_ids']['gateway_id']#gateway_id","['end_device_ids']['device_id']#device_id"])
-<br />
+m.selectKey(["['uplink_message']['decoded_payload']['temperature']#temp","['uplink_message']['rx_metadata'][0]['gateway_ids']['gateway_id']#Id_gateway","['end_device_ids']['device_id']#ID_device"])
+<br />Après le # on rajoute le nom de la 1ère ligne du fichier de données</br>>
  
 m.selectNomFichier("testdonnees.csv")<br />
 # pour afficher ou non les info sur la console <br />
 m.affichage_console(True) <br />
 # démarre le thread, (exécution indépendante du programme principal)<br />
 m.start()   <br />               
 time.sleep(1)<br />
```

### Comparing `mqttthreaddatalogger-1.5.1/setup.py` & `mqttthreaddatalogger-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mqttthreaddatalogger", # Replace with your own username
-    version="1.5.1",
+    version="1.6.0",
     author="Didier Orlandi",
     author_email="didier.orlandi@wanadoo.fr",
     description="Connexion mqtt et enregistrement des données dans un fichier csv",
     long_description=long_description,
     long_description_content_type="text/markdown",
     #url="https://github.com/",
     packages=setuptools.find_packages(),
```

