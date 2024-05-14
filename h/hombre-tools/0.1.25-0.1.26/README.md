# Comparing `tmp/hombre_tools-0.1.25.tar.gz` & `tmp/hombre_tools-0.1.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hombre_tools-0.1.25.tar", last modified: Mon May 13 12:27:24 2024, max compression
+gzip compressed data, was "hombre_tools-0.1.26.tar", last modified: Tue May 14 08:41:03 2024, max compression
```

## Comparing `hombre_tools-0.1.25.tar` & `hombre_tools-0.1.26.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 12:27:24.416851 hombre_tools-0.1.25/
--rw-rw-rw-   0        0        0     1088 2024-05-13 11:48:41.000000 hombre_tools-0.1.25/LICENSE.txt
--rw-rw-rw-   0        0        0      139 2024-05-13 11:48:41.000000 hombre_tools-0.1.25/MANIFEST.in
--rw-rw-rw-   0        0        0      759 2024-05-13 12:27:24.413860 hombre_tools-0.1.25/PKG-INFO
--rw-rw-rw-   0        0        0      385 2024-05-13 11:48:41.000000 hombre_tools-0.1.25/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 12:27:24.224642 hombre_tools-0.1.25/hombre_tools/
--rw-rw-rw-   0        0        0        0 2024-05-13 11:48:42.000000 hombre_tools-0.1.25/hombre_tools/__init__.py
--rw-rw-rw-   0        0        0     2088 2024-05-13 12:26:56.000000 hombre_tools-0.1.25/hombre_tools/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 12:27:24.265560 hombre_tools-0.1.25/hombre_tools/db/
--rw-rw-rw-   0        0        0        0 2024-05-13 11:48:42.000000 hombre_tools-0.1.25/hombre_tools/db/__init__.py
--rw-rw-rw-   0        0        0     1356 2024-05-13 11:48:42.000000 hombre_tools-0.1.25/hombre_tools/db/db.py
--rw-rw-rw-   0        0        0     1184 2024-05-13 11:48:42.000000 hombre_tools-0.1.25/hombre_tools/db/db_jde.py
--rw-rw-rw-   0        0        0      969 2024-05-13 11:48:42.000000 hombre_tools-0.1.25/hombre_tools/pswd.py
-drwxrwxrwx   0        0        0        0 2024-05-13 12:27:24.288499 hombre_tools-0.1.25/hombre_tools/tools/
--rw-rw-rw-   0        0        0        0 2024-05-13 11:48:42.000000 hombre_tools-0.1.25/hombre_tools/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 12:27:24.305673 hombre_tools-0.1.25/hombre_tools/tools/catalog/
--rw-rw-rw-   0        0        0        0 2024-05-13 11:48:42.000000 hombre_tools-0.1.25/hombre_tools/tools/catalog/__init__.py
--rw-rw-rw-   0        0        0     2345 2024-05-13 11:48:42.000000 hombre_tools-0.1.25/hombre_tools/tools/catalog/catalog.py
--rw-rw-rw-   0        0        0 34124902 2024-05-13 12:03:22.000000 hombre_tools-0.1.25/hombre_tools/tools/catalog/catalog_new.h5
--rw-rw-rw-   0        0        0      577 2024-05-13 11:48:42.000000 hombre_tools-0.1.25/hombre_tools/tools/data_profiling.py
--rw-rw-rw-   0        0        0     2162 2024-05-13 12:03:10.000000 hombre_tools-0.1.25/hombre_tools/tools/jde_sql_decorate.py
--rw-rw-rw-   0        0        0     1167 2024-05-13 11:48:43.000000 hombre_tools-0.1.25/hombre_tools/tools/metadata.py
-drwxrwxrwx   0        0        0        0 2024-05-13 12:27:24.405883 hombre_tools-0.1.25/hombre_tools/utils/
--rw-rw-rw-   0        0        0        0 2024-05-13 11:48:43.000000 hombre_tools-0.1.25/hombre_tools/utils/__init__.py
--rw-rw-rw-   0        0        0     3476 2024-05-13 11:48:43.000000 hombre_tools-0.1.25/hombre_tools/utils/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-13 12:27:24.410868 hombre_tools-0.1.25/hombre_tools.egg-info/
--rw-rw-rw-   0        0        0      759 2024-05-13 12:27:24.000000 hombre_tools-0.1.25/hombre_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      684 2024-05-13 12:27:24.000000 hombre_tools-0.1.25/hombre_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 12:27:24.000000 hombre_tools-0.1.25/hombre_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      198 2024-05-13 12:27:24.000000 hombre_tools-0.1.25/hombre_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-13 12:27:24.000000 hombre_tools-0.1.25/hombre_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 12:27:24.417850 hombre_tools-0.1.25/setup.cfg
--rw-rw-rw-   0        0        0     1421 2024-05-13 12:25:32.000000 hombre_tools-0.1.25/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:41:03.753617 hombre_tools-0.1.26/
+-rw-rw-rw-   0        0        0     1088 2024-05-13 11:48:41.000000 hombre_tools-0.1.26/LICENSE.txt
+-rw-rw-rw-   0        0        0      139 2024-05-13 11:48:41.000000 hombre_tools-0.1.26/MANIFEST.in
+-rw-rw-rw-   0        0        0      759 2024-05-14 08:41:03.750623 hombre_tools-0.1.26/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2024-05-13 11:48:41.000000 hombre_tools-0.1.26/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 08:41:03.540328 hombre_tools-0.1.26/hombre_tools/
+-rw-rw-rw-   0        0        0        0 2024-05-13 11:48:42.000000 hombre_tools-0.1.26/hombre_tools/__init__.py
+-rw-rw-rw-   0        0        0     2026 2024-05-14 08:29:55.000000 hombre_tools-0.1.26/hombre_tools/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:41:03.621966 hombre_tools-0.1.26/hombre_tools/db/
+-rw-rw-rw-   0        0        0        0 2024-05-13 11:48:42.000000 hombre_tools-0.1.26/hombre_tools/db/__init__.py
+-rw-rw-rw-   0        0        0     1356 2024-05-13 11:48:42.000000 hombre_tools-0.1.26/hombre_tools/db/db.py
+-rw-rw-rw-   0        0        0     1184 2024-05-13 11:48:42.000000 hombre_tools-0.1.26/hombre_tools/db/db_jde.py
+-rw-rw-rw-   0        0        0      969 2024-05-13 11:48:42.000000 hombre_tools-0.1.26/hombre_tools/pswd.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:41:03.638921 hombre_tools-0.1.26/hombre_tools/tools/
+-rw-rw-rw-   0        0        0        0 2024-05-13 11:48:42.000000 hombre_tools-0.1.26/hombre_tools/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:41:03.650889 hombre_tools-0.1.26/hombre_tools/tools/catalog/
+-rw-rw-rw-   0        0        0        0 2024-05-13 11:48:42.000000 hombre_tools-0.1.26/hombre_tools/tools/catalog/__init__.py
+-rw-rw-rw-   0        0        0     2345 2024-05-13 11:48:42.000000 hombre_tools-0.1.26/hombre_tools/tools/catalog/catalog.py
+-rw-rw-rw-   0        0        0 34124902 2024-05-14 08:32:29.000000 hombre_tools-0.1.26/hombre_tools/tools/catalog/catalog_new.h5
+-rw-rw-rw-   0        0        0      577 2024-05-13 11:48:42.000000 hombre_tools-0.1.26/hombre_tools/tools/data_profiling.py
+-rw-rw-rw-   0        0        0     2880 2024-05-14 08:32:17.000000 hombre_tools-0.1.26/hombre_tools/tools/jde_sql_decorate.py
+-rw-rw-rw-   0        0        0     1167 2024-05-13 11:48:43.000000 hombre_tools-0.1.26/hombre_tools/tools/metadata.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:41:03.740649 hombre_tools-0.1.26/hombre_tools/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-13 11:48:43.000000 hombre_tools-0.1.26/hombre_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0     3476 2024-05-13 11:48:43.000000 hombre_tools-0.1.26/hombre_tools/utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:41:03.745636 hombre_tools-0.1.26/hombre_tools.egg-info/
+-rw-rw-rw-   0        0        0      759 2024-05-14 08:41:03.000000 hombre_tools-0.1.26/hombre_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      684 2024-05-14 08:41:03.000000 hombre_tools-0.1.26/hombre_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 08:41:03.000000 hombre_tools-0.1.26/hombre_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      198 2024-05-14 08:41:03.000000 hombre_tools-0.1.26/hombre_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-14 08:41:03.000000 hombre_tools-0.1.26/hombre_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 08:41:03.753617 hombre_tools-0.1.26/setup.cfg
+-rw-rw-rw-   0        0        0     1421 2024-05-14 08:40:38.000000 hombre_tools-0.1.26/setup.py
```

### Comparing `hombre_tools-0.1.25/LICENSE.txt` & `hombre_tools-0.1.26/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hombre_tools-0.1.25/PKG-INFO` & `hombre_tools-0.1.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hombre_tools
-Version: 0.1.25
+Version: 0.1.26
 Summary: tools for daily usage
 Home-page: https://github.com/hombre66/hombre_tools
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyOpenSSL
 Requires-Dist: pyperclip
 Requires-Dist: python-dateutil
 Requires-Dist: python-settings
```

### Comparing `hombre_tools-0.1.25/hombre_tools/__main__.py` & `hombre_tools-0.1.26/hombre_tools/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """Main module for comand line usege of hombre_tools"""
 from os import scandir
 import logging
 import sqlparse
 from hombre_tools.utils.utils import argument_parser
 
+
+
 def jde_comment():
     """ adds comment to JDE source queries"""
     from hombre_tools.tools.jde_sql_decorate import comment as _comment, OPTIONS
     print(ARGS.path)
-    OPTIONS['strip_comments'] = ARGS.strip_comments
+    OPTIONS['strip_comments'] = True
     header = ARGS.header
     _copyright = f'Copyright Edwards Lifesciences {ARGS.year}, All rights reserved.'
     author = ARGS.author
     path = ARGS.path
 
     files = [entry for entry in scandir(path) if entry.is_file()]
 
     for file in files:
         with open(file.path) as in_file:
             print(file.path)
             new_name = file.path.split('.')[0] + '.sql'
-            script = sqlparse.format(in_file.read(), **OPTIONS)
-            _header = [f'/*\n{_copyright}',
-                       f'AUTHOR:{author}',
-                       f'file_name: {file.name.split(".")[0] +".sql"}',
-                       '*/\n']
-            
-            header = '\n'.join(_header)
-            script = header + _comment(script)
+            _header = [f'/*{_copyright}*/',
+                       f'/*AUTHOR:{author}*/',
+                       f'/*file_name: {file.name.split(".")[0] +".sql"}*/\n\n']
+
+            script = _comment(sqlparse.format(in_file.read(), **OPTIONS))
+            script = '\n'.join(_header) +  '\n'*2 + script
             new_name = file.path.split('.')[0] + '.sql'
             with open(new_name, 'w') as out_file:
                 out_file.write(script)
 
 def profile():
     """wrapper for data profile module"""
     from hombre_tools.db.db import sqlalchemy_engine, db_read_sql, ora_url
```

### Comparing `hombre_tools-0.1.25/hombre_tools/db/db.py` & `hombre_tools-0.1.26/hombre_tools/db/db.py`

 * *Files identical despite different names*

### Comparing `hombre_tools-0.1.25/hombre_tools/db/db_jde.py` & `hombre_tools-0.1.26/hombre_tools/db/db_jde.py`

 * *Files identical despite different names*

### Comparing `hombre_tools-0.1.25/hombre_tools/pswd.py` & `hombre_tools-0.1.26/hombre_tools/pswd.py`

 * *Files identical despite different names*

### Comparing `hombre_tools-0.1.25/hombre_tools/tools/catalog/catalog.py` & `hombre_tools-0.1.26/hombre_tools/tools/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `hombre_tools-0.1.25/hombre_tools/tools/catalog/catalog_new.h5` & `hombre_tools-0.1.26/hombre_tools/tools/catalog/catalog_new.h5`

 * *Files identical despite different names*

### Comparing `hombre_tools-0.1.25/hombre_tools/tools/data_profiling.py` & `hombre_tools-0.1.26/hombre_tools/tools/data_profiling.py`

 * *Files identical despite different names*

### Comparing `hombre_tools-0.1.25/hombre_tools/tools/jde_sql_decorate.py` & `hombre_tools-0.1.26/hombre_tools/tools/jde_sql_decorate.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,65 +14,81 @@
     TABLES = store.get('tables')
     COLUMNS = store.get('columns')
 
 CATALOG = ((TABLES, 'Table'),
            (COLUMNS, 'Field'))
 
 OPTIONS = {'keyword_case':'upper',
-           'reindent':True,
+           'identifier_case':'upper',
+           'reindent_aligned':True,
            'indent_width':4}
 
 P = re.compile(r'(\w*)')
 
-STOP_WORD = {'', 'select', 'from', 'as', 'where', 'group', 'by',
-             'left', 'join', 'is', 'not', 'null', 'inner',
-             'outer', 'case', 'when', 'else', 'then', 'end',
-             'union', 'nolock', 'in', 'order'}
 
 #creating index to speed _find
 TABLES.reset_index()
 TABLES.set_index('Table', inplace=True)
 COLUMNS.reset_index()
 COLUMNS.set_index('Field', inplace=True)
 
-def _find(catalog, word):
-    """
-    finds description by df index
-    """
-    descr = None
-    if word.lower() in STOP_WORD:
-        return None
-
-    try:
-       _desc = catalog.loc[word]
-    except:
-       return None
-    else:
-       if isinstance(_desc, DataFrame):
-           descr = _desc.Description.values[0]
-       else:
-            descr = _desc.Description
+STOP_WORD = {'', 'SELECT', 'FROM', 'AS', 'WHERE', 'GROUP', 'BY',
+             'LEFT', 'JOIN', 'IS', 'NOT', 'NULL', 'INNER',
+             'OUTER', 'CASE', 'WHEN', 'ELSE', 'THEN', 'END',
+             'UNION', 'NOLOCK', 'IN', 'ORDER', 'CREATE', 'OR', 'AND', 'NOT',
+             'REPLACE', 'VIEW', 'TO', 'GRANT'}
 
-    return descr
+MEME= {}
 
 def comment(script):
     """
     For each line with JDE table or
     column adds comment with JDE object description
     """
+    global STOP_WORD, MEME
+
+    def _find():
+        """
+        finds description by df index
+        """
+        descr = None
+        try:
+            desc = catalog.loc[word].Description
+            result =   desc if isinstance(desc, str) else desc.values[0]
+            MEME[word]=result
+        except KeyError:
+           MEME[word] = None
+    def meme():
+        if MEME.get(word):
+            descr = MEME.get(word)
+            if descr:
+                _comment.append(f'{word}:{descr}')
+                return True
+            return False
+
     sqls = []
     for sql in script.split(';'):
         lines = []
         for line in sql.splitlines():
+            _comment = []
             if '*/' in line:
+                lines.append(line)
                 continue
-            _comment = []
             for word in P.findall(line):
-                for _catalog, _ in CATALOG:
-                    descr = _find(_catalog, word)
-                    if descr:
-                        _comment.append(f'{word}:{descr}')
+                exists = False
+                word = word.upper()
+                if word not in STOP_WORD:
+                    if meme():
+                        continue
+                    else:
+                        for catalog, _ in CATALOG:
+                            _find()
+                            if meme():
+                                exists = True
+                                break
+                        if not exists:
+                            STOP_WORD = set(list(STOP_WORD) + [word])                                  
             if _comment:
                 line += f" /* {', '.join(_comment)} */"
             lines.append(line)
         sqls.append('\n'.join(lines[:]))
     return ';\n'.join(sqls)
```

### Comparing `hombre_tools-0.1.25/hombre_tools/tools/metadata.py` & `hombre_tools-0.1.26/hombre_tools/tools/metadata.py`

 * *Files identical despite different names*

### Comparing `hombre_tools-0.1.25/hombre_tools/utils/utils.py` & `hombre_tools-0.1.26/hombre_tools/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hombre_tools-0.1.25/hombre_tools.egg-info/PKG-INFO` & `hombre_tools-0.1.26/hombre_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hombre_tools
-Version: 0.1.25
+Version: 0.1.26
 Summary: tools for daily usage
 Home-page: https://github.com/hombre66/hombre_tools
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyOpenSSL
 Requires-Dist: pyperclip
 Requires-Dist: python-dateutil
 Requires-Dist: python-settings
```

### Comparing `hombre_tools-0.1.25/hombre_tools.egg-info/SOURCES.txt` & `hombre_tools-0.1.26/hombre_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hombre_tools-0.1.25/setup.py` & `hombre_tools-0.1.26/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name='hombre_tools',  # Required
 
-    version='0.1.25',  # Required
+    version='0.1.26',  # Required
     description='tools for daily usage',  # Optional
     url='https://github.com/hombre66/hombre_tools',  # Optional
 
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),  # Required
     include_package_data=True,
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     install_requires=['numpy',
                       'pandas',
                       'pyOpenSSL',
                       'pyperclip',
                       'python-dateutil',
                       'python-settings',
                       'pywin32',
```

