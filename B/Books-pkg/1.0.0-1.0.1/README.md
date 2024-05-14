# Comparing `tmp/books_pkg-1.0.0.tar.gz` & `tmp/books_pkg-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "books_pkg-1.0.0.tar", last modified: Tue May 14 02:27:23 2024, max compression
+gzip compressed data, was "books_pkg-1.0.1.tar", last modified: Tue May 14 02:38:05 2024, max compression
```

## Comparing `books_pkg-1.0.0.tar` & `books_pkg-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 02:27:23.381001 books_pkg-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-05-14 02:27:23.192259 books_pkg-1.0.0/Books_pkg/
--rw-rw-rw-   0        0        0       37 2024-05-14 02:18:23.000000 books_pkg-1.0.0/Books_pkg/__init__.py
--rw-rw-rw-   0        0        0    12151 2015-08-14 13:17:32.000000 books_pkg-1.0.0/Books_pkg/books.csv
--rw-rw-rw-   0        0        0     1566 2024-05-14 02:24:18.000000 books_pkg-1.0.0/Books_pkg/random_books.py
-drwxrwxrwx   0        0        0        0 2024-05-14 02:27:23.372218 books_pkg-1.0.0/Books_pkg.egg-info/
--rw-rw-rw-   0        0        0      334 2024-05-14 02:27:22.000000 books_pkg-1.0.0/Books_pkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-14 02:27:22.000000 books_pkg-1.0.0/Books_pkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 02:27:22.000000 books_pkg-1.0.0/Books_pkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-14 02:27:22.000000 books_pkg-1.0.0/Books_pkg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-14 02:27:22.000000 books_pkg-1.0.0/Books_pkg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      334 2024-05-14 02:27:23.377099 books_pkg-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      860 2024-05-14 02:27:18.000000 books_pkg-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-14 02:27:23.381976 books_pkg-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      536 2024-05-14 02:27:18.000000 books_pkg-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 02:38:05.097663 books_pkg-1.0.1/
+drwxrwxrwx   0        0        0        0 2024-05-14 02:38:04.838605 books_pkg-1.0.1/Books_pkg/
+-rw-rw-rw-   0        0        0       37 2024-05-14 02:18:23.000000 books_pkg-1.0.1/Books_pkg/__init__.py
+-rw-rw-rw-   0        0        0    12151 2015-08-14 13:17:32.000000 books_pkg-1.0.1/Books_pkg/books.csv
+-rw-rw-rw-   0        0        0     1572 2024-05-14 02:35:48.000000 books_pkg-1.0.1/Books_pkg/random_books.py
+drwxrwxrwx   0        0        0        0 2024-05-14 02:38:05.058609 books_pkg-1.0.1/Books_pkg.egg-info/
+-rw-rw-rw-   0        0        0      334 2024-05-14 02:38:02.000000 books_pkg-1.0.1/Books_pkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-14 02:38:02.000000 books_pkg-1.0.1/Books_pkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 02:38:02.000000 books_pkg-1.0.1/Books_pkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-14 02:38:02.000000 books_pkg-1.0.1/Books_pkg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-14 02:38:02.000000 books_pkg-1.0.1/Books_pkg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      334 2024-05-14 02:38:05.094733 books_pkg-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      860 2024-05-14 02:27:18.000000 books_pkg-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-14 02:38:05.098637 books_pkg-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      535 2024-05-14 02:37:28.000000 books_pkg-1.0.1/setup.py
```

### Comparing `books_pkg-1.0.0/Books_pkg/books.csv` & `books_pkg-1.0.1/Books_pkg/books.csv`

 * *Files identical despite different names*

### Comparing `books_pkg-1.0.0/Books_pkg/random_books.py` & `books_pkg-1.0.1/Books_pkg/random_books.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,27 +17,27 @@
         self._books = self._file.sample()
         self._title = self._books["Title"].values[0]
         self._author = self._books["Author"].values[0]
         self._genre = self._books["Genre"].values[0]
         self._height = self._books["Height"].values[0]
         self._publisher = self._books["Publisher"].values[0]
 
-    def buscar_title(self):
+    def buscar_title(title):
         file = "books.csv"
         datos = pd.read_csv(file)
-        buscar = datos[datos["Title"] == self]
+        buscar = datos[datos["Title"] == title]
         if buscar.size == 0:
             return buscar
         else:
             return "No se encontro el Titulo: "
 
-    def buscar_author(self):
+    def buscar_author(author):
         file = "books.csv"
         datos = pd.read_csv(file)
-        buscar = datos[datos["Author"] == self]
+        buscar = datos[datos["Author"] == author]
         if buscar.size == 0:
             return buscar
         else:
             return "No se encontro el Titulo: "
 
     def getTitle(self):
         return self._title
```

### Comparing `books_pkg-1.0.0/README.md` & `books_pkg-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `books_pkg-1.0.0/setup.py` & `books_pkg-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
 
    name='Books_pkg',
-   version='1.0.0',
-   author= 'Milton Alejandro Angel Cardenas ',
+   version='1.0.1',
+   author='Milton Alejandro Angel Cardenas ',
    author_email='milton_ac@tesch.edu.mx',
    description='Es una libreria en la cual podremos encontrar el autor y el libro, de pende el que se escriba',
    packages= ['Books_pkg'],
    package_data={'Books_pkg': ['books.csv']},
    install_requires=['pandas',
                      'twine',
                      'wheel' ,
```

