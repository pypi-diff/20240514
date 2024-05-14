# Comparing `tmp/django-pumaska-1.4rc12.tar.gz` & `tmp/django-pumaska-1.4rc13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pumaska-1.4rc12.tar", last modified: Mon Dec 18 12:20:48 2023, max compression
+gzip compressed data, was "django-pumaska-1.4rc13.tar", last modified: Thu Dec 28 11:34:20 2023, max compression
```

## Comparing `django-pumaska-1.4rc12.tar` & `django-pumaska-1.4rc13.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-12-18 12:20:48.736575 django-pumaska-1.4rc12/
--rw-r--r--   0 aha        (501) staff       (20)       73 2022-06-16 06:58:36.000000 django-pumaska-1.4rc12/MANIFEST.in
--rw-r--r--   0 aha        (501) staff       (20)      243 2023-12-18 12:20:48.736303 django-pumaska-1.4rc12/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)     2890 2022-06-16 06:58:36.000000 django-pumaska-1.4rc12/README.md
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-12-18 12:20:48.736079 django-pumaska-1.4rc12/django_pumaska.egg-info/
--rw-r--r--   0 aha        (501) staff       (20)      243 2023-12-18 12:20:48.000000 django-pumaska-1.4rc12/django_pumaska.egg-info/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)      617 2023-12-18 12:20:48.000000 django-pumaska-1.4rc12/django_pumaska.egg-info/SOURCES.txt
--rw-r--r--   0 aha        (501) staff       (20)        1 2023-12-18 12:20:48.000000 django-pumaska-1.4rc12/django_pumaska.egg-info/dependency_links.txt
--rw-r--r--   0 aha        (501) staff       (20)       36 2023-12-18 12:20:48.000000 django-pumaska-1.4rc12/django_pumaska.egg-info/entry_points.txt
--rw-r--r--   0 aha        (501) staff       (20)    10069 2023-12-18 12:20:48.000000 django-pumaska-1.4rc12/django_pumaska.egg-info/historia.json
--rw-r--r--   0 aha        (501) staff       (20)        1 2022-06-16 06:58:42.000000 django-pumaska-1.4rc12/django_pumaska.egg-info/not-zip-safe
--rw-r--r--   0 aha        (501) staff       (20)        8 2023-12-18 12:20:48.000000 django-pumaska-1.4rc12/django_pumaska.egg-info/top_level.txt
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-12-18 12:20:48.734711 django-pumaska-1.4rc12/pumaska/
--rw-r--r--   0 aha        (501) staff       (20)       65 2023-12-16 11:33:28.000000 django-pumaska-1.4rc12/pumaska/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)     2203 2022-06-16 06:58:36.000000 django-pumaska-1.4rc12/pumaska/koriste.py
--rw-r--r--   0 aha        (501) staff       (20)     8210 2023-12-16 11:33:28.000000 django-pumaska-1.4rc12/pumaska/lomake.py
--rw-r--r--   0 aha        (501) staff       (20)     6752 2023-12-18 12:20:00.000000 django-pumaska-1.4rc12/pumaska/nidottu.py
--rw-r--r--   0 aha        (501) staff       (20)      672 2023-12-04 08:59:17.000000 django-pumaska-1.4rc12/pumaska/piirto.py
--rw-r--r--   0 aha        (501) staff       (20)     8831 2023-12-18 12:20:00.000000 django-pumaska-1.4rc12/pumaska/sarja.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-12-18 12:20:48.730996 django-pumaska-1.4rc12/pumaska/static/
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-12-18 12:20:48.731063 django-pumaska-1.4rc12/pumaska/static/pumaska/
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-12-18 12:20:48.735009 django-pumaska-1.4rc12/pumaska/static/pumaska/js/
--rw-r--r--   0 aha        (501) staff       (20)    13023 2022-06-16 06:58:36.000000 django-pumaska-1.4rc12/pumaska/static/pumaska/js/jquery.formset.js
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-12-18 12:20:48.731239 django-pumaska-1.4rc12/pumaska/templates/
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-12-18 12:20:48.735842 django-pumaska-1.4rc12/pumaska/templates/pumaska/
--rw-r--r--   0 aha        (501) staff       (20)     2477 2023-10-06 17:43:49.000000 django-pumaska-1.4rc12/pumaska/templates/pumaska/lomakesarja.html
--rw-r--r--   0 aha        (501) staff       (20)      105 2022-06-16 06:58:36.000000 django-pumaska-1.4rc12/pumaska/templates/pumaska/lomakesarja_lomakekenttana.html
--rw-r--r--   0 aha        (501) staff       (20)       11 2022-06-16 06:58:36.000000 django-pumaska-1.4rc12/pumaska/templates/pumaska/lomakesarja_rivi.html
--rw-r--r--   0 aha        (501) staff       (20)       80 2023-08-28 11:09:41.000000 django-pumaska-1.4rc12/pyproject.toml
--rw-r--r--   0 aha        (501) staff       (20)       38 2023-12-18 12:20:48.736626 django-pumaska-1.4rc12/setup.cfg
--rw-r--r--   0 aha        (501) staff       (20)      500 2023-08-28 11:08:06.000000 django-pumaska-1.4rc12/setup.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-12-28 11:34:20.709373 django-pumaska-1.4rc13/
+-rw-r--r--   0 aha        (501) staff       (20)       73 2022-06-16 06:58:36.000000 django-pumaska-1.4rc13/MANIFEST.in
+-rw-r--r--   0 aha        (501) staff       (20)      243 2023-12-28 11:34:20.709113 django-pumaska-1.4rc13/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)     2890 2022-06-16 06:58:36.000000 django-pumaska-1.4rc13/README.md
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-12-28 11:34:20.708830 django-pumaska-1.4rc13/django_pumaska.egg-info/
+-rw-r--r--   0 aha        (501) staff       (20)      243 2023-12-28 11:34:17.000000 django-pumaska-1.4rc13/django_pumaska.egg-info/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)      617 2023-12-28 11:34:20.000000 django-pumaska-1.4rc13/django_pumaska.egg-info/SOURCES.txt
+-rw-r--r--   0 aha        (501) staff       (20)        1 2023-12-28 11:34:17.000000 django-pumaska-1.4rc13/django_pumaska.egg-info/dependency_links.txt
+-rw-r--r--   0 aha        (501) staff       (20)       36 2023-12-28 11:34:17.000000 django-pumaska-1.4rc13/django_pumaska.egg-info/entry_points.txt
+-rw-r--r--   0 aha        (501) staff       (20)    10321 2023-12-28 11:34:20.000000 django-pumaska-1.4rc13/django_pumaska.egg-info/historia.json
+-rw-r--r--   0 aha        (501) staff       (20)        1 2022-06-16 06:58:42.000000 django-pumaska-1.4rc13/django_pumaska.egg-info/not-zip-safe
+-rw-r--r--   0 aha        (501) staff       (20)        8 2023-12-28 11:34:17.000000 django-pumaska-1.4rc13/django_pumaska.egg-info/top_level.txt
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-12-28 11:34:20.707542 django-pumaska-1.4rc13/pumaska/
+-rw-r--r--   0 aha        (501) staff       (20)       65 2023-12-16 11:33:28.000000 django-pumaska-1.4rc13/pumaska/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)     2203 2022-06-16 06:58:36.000000 django-pumaska-1.4rc13/pumaska/koriste.py
+-rw-r--r--   0 aha        (501) staff       (20)     8210 2023-12-16 11:33:28.000000 django-pumaska-1.4rc13/pumaska/lomake.py
+-rw-r--r--   0 aha        (501) staff       (20)     7417 2023-12-28 11:12:25.000000 django-pumaska-1.4rc13/pumaska/nidottu.py
+-rw-r--r--   0 aha        (501) staff       (20)      672 2023-12-04 08:59:17.000000 django-pumaska-1.4rc13/pumaska/piirto.py
+-rw-r--r--   0 aha        (501) staff       (20)     9018 2023-12-28 11:06:57.000000 django-pumaska-1.4rc13/pumaska/sarja.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-12-28 11:34:20.703580 django-pumaska-1.4rc13/pumaska/static/
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-12-28 11:34:20.703669 django-pumaska-1.4rc13/pumaska/static/pumaska/
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-12-28 11:34:20.707821 django-pumaska-1.4rc13/pumaska/static/pumaska/js/
+-rw-r--r--   0 aha        (501) staff       (20)    13023 2022-06-16 06:58:36.000000 django-pumaska-1.4rc13/pumaska/static/pumaska/js/jquery.formset.js
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-12-28 11:34:20.703835 django-pumaska-1.4rc13/pumaska/templates/
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-12-28 11:34:20.708600 django-pumaska-1.4rc13/pumaska/templates/pumaska/
+-rw-r--r--   0 aha        (501) staff       (20)     2477 2023-10-06 17:43:49.000000 django-pumaska-1.4rc13/pumaska/templates/pumaska/lomakesarja.html
+-rw-r--r--   0 aha        (501) staff       (20)      105 2022-06-16 06:58:36.000000 django-pumaska-1.4rc13/pumaska/templates/pumaska/lomakesarja_lomakekenttana.html
+-rw-r--r--   0 aha        (501) staff       (20)       11 2022-06-16 06:58:36.000000 django-pumaska-1.4rc13/pumaska/templates/pumaska/lomakesarja_rivi.html
+-rw-r--r--   0 aha        (501) staff       (20)       80 2023-08-28 11:09:41.000000 django-pumaska-1.4rc13/pyproject.toml
+-rw-r--r--   0 aha        (501) staff       (20)       38 2023-12-28 11:34:20.709416 django-pumaska-1.4rc13/setup.cfg
+-rw-r--r--   0 aha        (501) staff       (20)      500 2023-08-28 11:08:06.000000 django-pumaska-1.4rc13/setup.py
```

### Comparing `django-pumaska-1.4rc12/README.md` & `django-pumaska-1.4rc13/README.md`

 * *Files identical despite different names*

### Comparing `django-pumaska-1.4rc12/django_pumaska.egg-info/SOURCES.txt` & `django-pumaska-1.4rc13/django_pumaska.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-pumaska-1.4rc12/django_pumaska.egg-info/historia.json` & `django-pumaska-1.4rc13/django_pumaska.egg-info/historia.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9821428571428571%*

 * *Differences: {'insert': "[(0, OrderedDict([('revisio', '1cd5fc301f3ab0b6121b696a575518b2716229cf'), ('versio', "*

 * *           "'1.4rc13'), ('kuvaus', 'Korjattu sisemmän lomakkeen oletus-`prefixin` asetus\\n\\n* "*

 * *           "vrt. a711974573259ac8b21d8c59b8378663944e1d7d\\n* täydennetty kommentointia')]))]"}*

```diff
@@ -1,9 +1,14 @@
 [
     {
+        "kuvaus": "Korjattu sisemm\u00e4n lomakkeen oletus-`prefixin` asetus\n\n* vrt. a711974573259ac8b21d8c59b8378663944e1d7d\n* t\u00e4ydennetty kommentointia",
+        "revisio": "1cd5fc301f3ab0b6121b696a575518b2716229cf",
+        "versio": "1.4rc13"
+    },
+    {
         "kuvaus": "Korjattu `testaa_html`-testi: tarvittavat `render`-toteutukset",
         "revisio": "4d18ef79e2b6f6e0bbd58e6acf9b00a73b9bf1bf",
         "versio": "1.4rc12"
     },
     {
         "kuvaus": "Muutettu testit tox-pohjaisiksi",
         "revisio": "e9fd2dad347d69f4c2e6d6c818cf87b4cd1acaf6",
```

### Comparing `django-pumaska-1.4rc12/pumaska/koriste.py` & `django-pumaska-1.4rc13/pumaska/koriste.py`

 * *Files identical despite different names*

### Comparing `django-pumaska-1.4rc12/pumaska/lomake.py` & `django-pumaska-1.4rc13/pumaska/lomake.py`

 * *Files identical despite different names*

### Comparing `django-pumaska-1.4rc12/pumaska/nidottu.py` & `django-pumaska-1.4rc13/pumaska/nidottu.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,54 +39,65 @@
         try:
           ajonaikainen_kwargs[param] = kwargs[param]
         except KeyError:
           pass
 
       super().__init__(*args, prefix=prefix, **kwargs)
 
-      # Käytetään A-lomakkeen vedostajaa oletuksena
-      # myös B-lomakkeella.
-      # Huomaa, että Django vaatii, että `renderer` periytyy
-      # lomakeluokan mahdollisesta `default_renderer`-luokasta.
+      # Käytetään A-lomakkeen vedostajaa oletuksena myös B-lomakkeella.
+      # Huomaa:
+      # - Django vaatii, että `renderer` periytyy lomakeluokan
+      #   mahdollisesta `default_renderer`-luokasta;
+      # - lomake ei ota (Django 4.2) vastaan parametriä `renderer`,
+      #   tämä täytyy asettaa jälkeenpäin määreenä.
       if not 'renderer' in ajonaikainen_kwargs:
         class PiirtoB(Piirto, LomakeB=liitos): pass
         # Lomakesarja ei ota `renderer`-parametriä vastaan.
         # Asetetaan tämä alustuksen jälkeen määreenä.
         if issubclass(liitos, forms.BaseFormSet):
           asetettavat_maareet['renderer'] = PiirtoB(self)
         else:
           ajonaikainen_kwargs['renderer'] = PiirtoB(self)
         # if not 'renderer' in ajonaikainen_kwargs
 
-      # Asetetaan liitoksen oletus-`prefix`.
-      ajonaikainen_kwargs.setdefault(
-        'prefix', f'{self.prefix}-{tunnus}' if self.prefix else tunnus
-      )
-
+      # Annetaan sisemmän lomakkeen alustuksessa oletuksena:
+      # - data ja files, mikäli ulompi lomake on lähetetty,
+      # - initial: `<tunnus>-`-alkuiset, epätyhjät avaimet ulomman
+      #   lomakkeen initial-datassa
+      # - prefix: `<ulompi prefix>-<tunnus>`
+      # Huomaa, että `liitos_kwargs()` ja `ajonaikainen_kwargs` (tässä
+      # järjestyksessä) ylikirjoittavat nämä oletusarvot.
       _liitos = liitos(**{
         **({
           'data': self.data,
           'files': self.files,
         } if self.is_bound else {}),
         'initial': {
           avain.replace(tunnus + '-', '', 1): arvo
           for avain, arvo in self.initial.items()
           if avain.startswith(tunnus + '-') and avain != tunnus + '-'
         },
+        'prefix': f'{self.prefix}-{tunnus}' if self.prefix else tunnus,
         **liitos_kwargs(self),
         **ajonaikainen_kwargs,
       })
+
+      # Asetetaan tarvittavat määreet (renderer).
       for avain, arvo in asetettavat_maareet.items():
         setattr(_liitos, avain, arvo)
+
+      # Asetetaan viittaus ulommasta lomakkeesta sisempään.
       setattr(self, tunnus, _liitos)
-      # Jos B-viittaus saa olla tyhjä, asetetaan kaikki B-lomakkeen
-      # kentät valinnaisiksi GET-pyynnöllä.
-      # – Huomaa, että tämä koskee myös mahdollisten sisäkkäisten
-      # lomakkeiden (C) kenttiä.
-      # Lisäksi ohitetaan vimpainten `required`-määreen tulostus.
+
+      # Jos B-viittaus saa olla tyhjä:
+      # - asetetaan kaikki B-lomakkeen kentät valinnaisiksi GET-pyynnöllä;
+      # – huomaa, että tämä koskee myös mahdollisten sisäkkäisten
+      #   lomakkeiden (C) kenttiä; ks. `__iter__`-toteutus alla;
+      # - ohitetaan vimpainten `required`-määreen tulostus;
+      # - huomaa, että tämä ei tee mitään sisemmälle lomakesarjalle.
       if not pakollinen:
         for kentta in _liitos:
           if hasattr(kentta, 'field'):
             if not self.data:
               kentta.field.required = False
             kentta.field.widget.use_required_attribute = lambda initial: False
       # def __init__
```

### Comparing `django-pumaska-1.4rc12/pumaska/piirto.py` & `django-pumaska-1.4rc13/pumaska/piirto.py`

 * *Files identical despite different names*

### Comparing `django-pumaska-1.4rc12/pumaska/sarja.py` & `django-pumaska-1.4rc13/pumaska/sarja.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,14 +117,20 @@
   if tunnus in LomakeA.base_fields:
     raise RuntimeError(
       f'Lomakesarjaa ei voida nitoa samalla nimellä'
       f' kuin olemassaoleva lomakekenttä: {tunnus}'
     )
 
   def liitos_kwargs(self: LomakeA):
+    '''
+    Korvataan oletusarvoinen, ulommasta initial-datasta poimittu
+    `initial` luetteloksi käärityllä versiolla.
+
+    Asetetaan ulompi olio lomakesarjan `instanceksi`.
+    '''
     initial = {
       avain.replace(tunnus + '-', '', 1): arvo
       for avain, arvo in self.initial.items()
       if avain.startswith(tunnus + '-') and avain != tunnus + '-'
     }
     assert isinstance(self.instance, self.Meta.model), (
       f'Kohde A ei voi olla tyyppiä {type(self.instance)} != {self.Meta.model}!'
```

### Comparing `django-pumaska-1.4rc12/pumaska/static/pumaska/js/jquery.formset.js` & `django-pumaska-1.4rc13/pumaska/static/pumaska/js/jquery.formset.js`

 * *Files identical despite different names*

### Comparing `django-pumaska-1.4rc12/pumaska/templates/pumaska/lomakesarja.html` & `django-pumaska-1.4rc13/pumaska/templates/pumaska/lomakesarja.html`

 * *Files identical despite different names*

