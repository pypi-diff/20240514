# Comparing `tmp/combogenius-0.2.2.tar.gz` & `tmp/combogenius-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "combogenius-0.2.2.tar", last modified: Mon May 13 17:39:00 2024, max compression
+gzip compressed data, was "combogenius-0.2.3.tar", last modified: Mon May 13 18:19:19 2024, max compression
```

## Comparing `combogenius-0.2.2.tar` & `combogenius-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 17:39:00.253302 combogenius-0.2.2/
--rw-rw-rw-   0        0        0     1086 2024-04-28 15:40:17.000000 combogenius-0.2.2/LICENSE
--rw-rw-rw-   0        0        0       36 2024-04-28 15:40:17.000000 combogenius-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5490 2024-05-13 17:39:00.251183 combogenius-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     4710 2024-05-12 20:09:46.000000 combogenius-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 17:39:00.251183 combogenius-0.2.2/combogenius.egg-info/
--rw-rw-rw-   0        0        0     5490 2024-05-13 17:39:00.000000 combogenius-0.2.2/combogenius.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2024-05-13 17:39:00.000000 combogenius-0.2.2/combogenius.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 17:39:00.000000 combogenius-0.2.2/combogenius.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 17:39:00.000000 combogenius-0.2.2/combogenius.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 17:39:00.253302 combogenius-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1073 2024-05-13 17:35:57.000000 combogenius-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:19:19.114638 combogenius-0.2.3/
+-rw-rw-rw-   0        0        0     1086 2024-04-28 15:40:17.000000 combogenius-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0       36 2024-04-28 15:40:17.000000 combogenius-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     5514 2024-05-13 18:19:19.114638 combogenius-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4710 2024-05-12 20:09:46.000000 combogenius-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 18:19:19.109208 combogenius-0.2.3/combogenius.egg-info/
+-rw-rw-rw-   0        0        0     5514 2024-05-13 18:19:18.000000 combogenius-0.2.3/combogenius.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-05-13 18:19:19.000000 combogenius-0.2.3/combogenius.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 18:19:18.000000 combogenius-0.2.3/combogenius.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-13 18:19:18.000000 combogenius-0.2.3/combogenius.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 18:19:19.114638 combogenius-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1065 2024-05-13 18:13:50.000000 combogenius-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:19:19.114638 combogenius-0.2.3/tests/
+-rw-rw-rw-   0        0        0      118 2024-05-10 17:32:30.000000 combogenius-0.2.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      472 2024-05-10 17:29:35.000000 combogenius-0.2.3/tests/test_api.py
+-rw-rw-rw-   0        0        0     1447 2024-05-10 17:31:41.000000 combogenius-0.2.3/tests/test_database.py
+-rw-rw-rw-   0        0        0     1748 2024-05-10 17:31:40.000000 combogenius-0.2.3/tests/test_make_combos.py
```

### Comparing `combogenius-0.2.2/LICENSE` & `combogenius-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `combogenius-0.2.2/PKG-INFO` & `combogenius-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: combogenius
-Version: 0.2.2
+Version: 0.2.3
 Summary: A package designed to efficiently generate new product combinations using check information, and deliver combo suggestions to business partners via email.
 Author: Anna Movsisyan, Lusine Aghinyan, Ararat Kazarian, Hovhannes Hovhannisyan, Eduard Petrosyan
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ComboGenius 
 ## Problem
 
 Many restaurants and food courts face challenges when it comes to expanding their corporate lunch service market through B2B websites. Despite offering great value and quality products, these businesses struggle with visibility among potential clients. The main issue lies in the lack of effective engagement strategies, making it difficult to showcase their benefits and attract new customers.
```

### Comparing `combogenius-0.2.2/README.md` & `combogenius-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `combogenius-0.2.2/combogenius.egg-info/PKG-INFO` & `combogenius-0.2.3/combogenius.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: combogenius
-Version: 0.2.2
+Version: 0.2.3
 Summary: A package designed to efficiently generate new product combinations using check information, and deliver combo suggestions to business partners via email.
 Author: Anna Movsisyan, Lusine Aghinyan, Ararat Kazarian, Hovhannes Hovhannisyan, Eduard Petrosyan
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ComboGenius 
 ## Problem
 
 Many restaurants and food courts face challenges when it comes to expanding their corporate lunch service market through B2B websites. Despite offering great value and quality products, these businesses struggle with visibility among potential clients. The main issue lies in the lack of effective engagement strategies, making it difficult to showcase their benefits and attract new customers.
```

### Comparing `combogenius-0.2.2/setup.py` & `combogenius-0.2.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 this_directory=Path(__file__).parent
 long_description=(this_directory / "README.md").read_text()
 
 setup(
     author='Anna Movsisyan, Lusine Aghinyan, Ararat Kazarian, Hovhannes Hovhannisyan, Eduard Petrosyan',
     name='combogenius',
     description='A package designed to efficiently generate new product combinations using check information, and deliver combo suggestions to business partners via email.',
-    version='0.2.2',
+    version='0.2.3',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    packages=find_packages(include=['combogenius','combogenius.*']),
+    packages=find_packages(),
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',]
+        'Programming Language :: Python :: 3.8',],
+    python_requires='>=3.6',
 )
```

