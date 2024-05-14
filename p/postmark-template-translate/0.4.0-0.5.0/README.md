# Comparing `tmp/postmark_template_translate-0.4.0.tar.gz` & `tmp/postmark_template_translate-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postmark_template_translate-0.4.0.tar", last modified: Tue May 14 12:57:12 2024, max compression
+gzip compressed data, was "postmark_template_translate-0.5.0.tar", last modified: Tue May 14 13:07:16 2024, max compression
```

## Comparing `postmark_template_translate-0.4.0.tar` & `postmark_template_translate-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 12:57:12.596992 postmark_template_translate-0.4.0/
--rw-rw-rw-   0        0        0      793 2024-05-14 12:57:12.595992 postmark_template_translate-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      167 2024-05-14 05:58:54.000000 postmark_template_translate-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 12:57:12.594997 postmark_template_translate-0.4.0/postmark_template_translate.egg-info/
--rw-rw-rw-   0        0        0      793 2024-05-14 12:57:12.000000 postmark_template_translate-0.4.0/postmark_template_translate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-05-14 12:57:12.000000 postmark_template_translate-0.4.0/postmark_template_translate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 12:57:12.000000 postmark_template_translate-0.4.0/postmark_template_translate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-14 12:57:12.000000 postmark_template_translate-0.4.0/postmark_template_translate.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 12:57:12.000000 postmark_template_translate-0.4.0/postmark_template_translate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 12:57:12.596992 postmark_template_translate-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      916 2024-05-14 12:56:56.000000 postmark_template_translate-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:07:16.244017 postmark_template_translate-0.5.0/
+-rw-rw-rw-   0        0        0      793 2024-05-14 13:07:16.243018 postmark_template_translate-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2024-05-14 05:58:54.000000 postmark_template_translate-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 13:07:16.242016 postmark_template_translate-0.5.0/postmark_template_translate.egg-info/
+-rw-rw-rw-   0        0        0      793 2024-05-14 13:07:16.000000 postmark_template_translate-0.5.0/postmark_template_translate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-05-14 13:07:16.000000 postmark_template_translate-0.5.0/postmark_template_translate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 13:07:16.000000 postmark_template_translate-0.5.0/postmark_template_translate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-14 13:07:16.000000 postmark_template_translate-0.5.0/postmark_template_translate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 13:07:16.000000 postmark_template_translate-0.5.0/postmark_template_translate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 13:07:16.244017 postmark_template_translate-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      936 2024-05-14 13:07:13.000000 postmark_template_translate-0.5.0/setup.py
```

### Comparing `postmark_template_translate-0.4.0/PKG-INFO` & `postmark_template_translate-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postmark-template-translate
-Version: 0.4.0
+Version: 0.5.0
 Summary: A library to send Postmark templates with translated content
 Home-page: https://github.com/DanielDls-exe/postmark_template_translate
 Author: Daniel Alvarado
 Author-email: dani.alvarado@kirbic.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `postmark_template_translate-0.4.0/postmark_template_translate.egg-info/PKG-INFO` & `postmark_template_translate-0.5.0/postmark_template_translate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postmark-template-translate
-Version: 0.4.0
+Version: 0.5.0
 Summary: A library to send Postmark templates with translated content
 Home-page: https://github.com/DanielDls-exe/postmark_template_translate
 Author: Daniel Alvarado
 Author-email: dani.alvarado@kirbic.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `postmark_template_translate-0.4.0/setup.py` & `postmark_template_translate-0.5.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from setuptools import setup, find_packages
 
 setup(
     name='postmark-template-translate',
-    version='0.4.0',  
-    packages=find_packages(),
+    version='0.5.0',  
+    packages=find_packages(include=['app', 'app.*']),  
     install_requires=[
         'postmarker',
         'beautifulsoup4',
         'googletrans==4.0.0-rc1',
         'python-dotenv'
     ],
     entry_points={
         'console_scripts': [
-            
+        
         ],
     },
     author='Daniel Alvarado',
     author_email='dani.alvarado@kirbic.com',
     description='A library to send Postmark templates with translated content',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url='https://github.com/DanielDls-exe/postmark_template_translate',  
+    url='https://github.com/DanielDls-exe/postmark_template_translate',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
 )
```

