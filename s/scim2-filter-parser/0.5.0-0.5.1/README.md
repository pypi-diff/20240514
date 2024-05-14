# Comparing `tmp/scim2_filter_parser-0.5.0.tar.gz` & `tmp/scim2_filter_parser-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scim2_filter_parser-0.5.0.tar", max compression
+gzip compressed data, was "scim2_filter_parser-0.5.1.tar", max compression
```

## Comparing `scim2_filter_parser-0.5.0.tar` & `scim2_filter_parser-0.5.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1126 2023-01-30 05:39:49.565521 scim2_filter_parser-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0    10911 2023-02-02 03:30:15.539388 scim2_filter_parser-0.5.0/README.rst
--rw-r--r--   0        0        0     1833 2023-02-03 00:20:40.706446 scim2_filter_parser-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-30 05:39:49.567866 scim2_filter_parser-0.5.0/src/scim2_filter_parser/__init__.py
--rw-r--r--   0        0        0     6356 2023-01-30 05:39:49.568031 scim2_filter_parser-0.5.0/src/scim2_filter_parser/ast.py
--rw-r--r--   0        0        0     3951 2023-01-30 05:39:49.568198 scim2_filter_parser-0.5.0/src/scim2_filter_parser/attr_paths.py
--rw-r--r--   0        0        0    12965 2023-01-30 05:39:49.568428 scim2_filter_parser-0.5.0/src/scim2_filter_parser/lexer.py
--rw-r--r--   0        0        0     9036 2023-01-30 05:39:49.568597 scim2_filter_parser-0.5.0/src/scim2_filter_parser/parser.py
--rw-r--r--   0        0        0       49 2023-01-30 05:39:49.568770 scim2_filter_parser-0.5.0/src/scim2_filter_parser/queries/__init__.py
--rw-r--r--   0        0        0     3540 2023-01-30 05:39:49.568926 scim2_filter_parser-0.5.0/src/scim2_filter_parser/queries/sql.py
--rw-r--r--   0        0        0        0 2023-01-30 05:39:49.569036 scim2_filter_parser-0.5.0/src/scim2_filter_parser/transpilers/__init__.py
--rw-r--r--   0        0        0     7094 2023-01-30 05:39:49.569246 scim2_filter_parser-0.5.0/src/scim2_filter_parser/transpilers/django_q_object.py
--rw-r--r--   0        0        0     8320 2023-01-30 05:39:49.569426 scim2_filter_parser-0.5.0/src/scim2_filter_parser/transpilers/sql.py
--rw-r--r--   0        0        0    12673 1970-01-01 00:00:00.000000 scim2_filter_parser-0.5.0/setup.py
--rw-r--r--   0        0        0    12419 1970-01-01 00:00:00.000000 scim2_filter_parser-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1126 2023-09-07 02:18:15.521678 scim2_filter_parser-0.5.1/LICENSE.txt
+-rw-r--r--   0        0        0    10911 2023-09-07 02:18:15.521841 scim2_filter_parser-0.5.1/README.rst
+-rw-r--r--   0        0        0     2782 2024-05-14 05:38:33.891967 scim2_filter_parser-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-09-07 02:18:15.523595 scim2_filter_parser-0.5.1/src/scim2_filter_parser/__init__.py
+-rw-r--r--   0        0        0     6164 2024-05-14 05:38:33.892194 scim2_filter_parser-0.5.1/src/scim2_filter_parser/ast.py
+-rw-r--r--   0        0        0     3951 2023-09-07 02:18:15.523842 scim2_filter_parser-0.5.1/src/scim2_filter_parser/attr_paths.py
+-rw-r--r--   0        0        0    12963 2024-05-14 05:38:33.892389 scim2_filter_parser-0.5.1/src/scim2_filter_parser/lexer.py
+-rw-r--r--   0        0        0     9023 2024-05-14 05:38:33.892563 scim2_filter_parser-0.5.1/src/scim2_filter_parser/parser.py
+-rw-r--r--   0        0        0       49 2023-09-07 02:18:15.524257 scim2_filter_parser-0.5.1/src/scim2_filter_parser/queries/__init__.py
+-rw-r--r--   0        0        0     3540 2023-09-07 02:18:15.524370 scim2_filter_parser-0.5.1/src/scim2_filter_parser/queries/sql.py
+-rw-r--r--   0        0        0        0 2023-09-07 02:18:15.524453 scim2_filter_parser-0.5.1/src/scim2_filter_parser/transpilers/__init__.py
+-rw-r--r--   0        0        0     7038 2024-05-14 05:38:33.892721 scim2_filter_parser-0.5.1/src/scim2_filter_parser/transpilers/django_q_object.py
+-rw-r--r--   0        0        0     8320 2023-09-07 02:18:15.524742 scim2_filter_parser-0.5.1/src/scim2_filter_parser/transpilers/sql.py
+-rw-r--r--   0        0        0    12268 1970-01-01 00:00:00.000000 scim2_filter_parser-0.5.1/PKG-INFO
```

### Comparing `scim2_filter_parser-0.5.0/LICENSE.txt` & `scim2_filter_parser-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scim2_filter_parser-0.5.0/README.rst` & `scim2_filter_parser-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `scim2_filter_parser-0.5.0/src/scim2_filter_parser/ast.py` & `scim2_filter_parser-0.5.1/src/scim2_filter_parser/ast.py`

 * *Files 13% similar despite different names*

```diff
@@ -71,49 +71,49 @@
 # ----------------------------------------------------------------------
 
 # Abstract AST nodes.  These are not instantiated directly, but other
 # classes inherit from them.
 
 
 class Filter(AST):
-    expr      : AST  # noqa: E203
-    negated   : bool  # noqa: E203
-    namespace : AST  # noqa: E203
+    expr      : AST
+    negated   : bool
+    namespace : AST
 
 
 class LogExpr(AST):
-    op    : str  # noqa: E203
-    expr1 : Filter  # noqa: E203
-    expr2 : Filter  # noqa: E203
+    op    : str
+    expr1 : Filter
+    expr2 : Filter
 
 
 class SubAttr(AST):
-    value : str  # noqa: E203
+    value : str
 
 
 class AttrPath(AST):
-    attr_name : str  # noqa: E203
-    sub_attr  : (SubAttr, type(None))  # noqa: E203
-    uri       : (str, type(None))  # noqa: E203
+    attr_name : str
+    sub_attr  : (SubAttr, type(None))
+    uri       : (str, type(None))
 
     @property
     def case_insensitive(self):
         # userName is always case-insensitive
         # https://datatracker.ietf.org/doc/html/rfc7643#section-4.1.1
         return self.attr_name == 'userName'
 
 
 class CompValue(AST):
-    value : str  # noqa: E203
+    value : str
 
 
 class AttrExpr(AST):
-    value : str  # noqa: E203
-    attr_path  : AttrPath  # noqa: E203
-    comp_value : CompValue  # noqa: E203
+    value : str
+    attr_path  : AttrPath
+    comp_value : CompValue
 
     @property
     def case_insensitive(self):
         return self.attr_path.case_insensitive
 
 
 # The following classes for visiting and rewriting the AST are taken
@@ -172,26 +172,26 @@
 
     def generic_visit(self, node):
         '''
         Method executed if no applicable `visit_` method can be found.
         This examines the node to see if it has `_fields`, is a list,
         or can be further traversed.
         '''
-        for field in getattr(node, '_fields'):
+        for field in node._fields:
             value = getattr(node, field, None)
             self.visit(value)
 
     @classmethod
     def __init_subclass__(cls):
         '''
         Sanity check. Make sure that visitor classes use the right names.
         '''
         for key in vars(cls):
             if key.startswith('visit_'):
-                assert key[6:] in AST._nodes, f"{key} doesn't match any AST node"
+                assert key[6:] in AST._nodes, f"{key} doesn't match any AST node"  # noqa: SLF001
 
 
 def flatten(top):
     '''
     Flatten the entire parse tree into a list for the purposes of
     debugging and testing.  This returns a list of tuples of the
     form (depth, node) where depth is an integer representing the
```

### Comparing `scim2_filter_parser-0.5.0/src/scim2_filter_parser/attr_paths.py` & `scim2_filter_parser-0.5.1/src/scim2_filter_parser/attr_paths.py`

 * *Files identical despite different names*

### Comparing `scim2_filter_parser-0.5.0/src/scim2_filter_parser/lexer.py` & `scim2_filter_parser-0.5.1/src/scim2_filter_parser/lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
    |          |             | expressions MAY be used.  See examples   |
    |          |             | below.                                   |
    +----------+-------------+------------------------------------------+
 
                         Table 5: Grouping Operators
 
 """
-# flake8: noqa: F821
+# ruff: noqa: F821
 from sly import Lexer
 
 
 class SCIMLexer(Lexer):
     tokens = {
         # Attribute Operators
         EQ, NE,
```

### Comparing `scim2_filter_parser-0.5.0/src/scim2_filter_parser/parser.py` & `scim2_filter_parser-0.5.1/src/scim2_filter_parser/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         ('left', OR, AND),  # noqa F821
         ('right', NOT), # noqa F821
     )
 
     # FILTER    = attrExp / logExp / valuePath / *1"not" "(" FILTER ")"
     #                                           ; 0 or 1 "not"s
     @_('attr_exp')  # noqa F821
-    def filter(self, p):  # noqa F811
+    def filter(self, p):
         return ast.Filter(p.attr_exp, False, None)
 
     @_('log_exp')  # noqa F821
     def filter(self, p):  # noqa F811
         return ast.Filter(p.log_exp, False, None)
 
     @_('value_path')  # noqa F821
```

### Comparing `scim2_filter_parser-0.5.0/src/scim2_filter_parser/queries/sql.py` & `scim2_filter_parser-0.5.1/src/scim2_filter_parser/queries/sql.py`

 * *Files identical despite different names*

### Comparing `scim2_filter_parser-0.5.0/src/scim2_filter_parser/transpilers/django_q_object.py` & `scim2_filter_parser-0.5.1/src/scim2_filter_parser/transpilers/django_q_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 The logic in this module builds a Django Q object from an SCIM filter.
 """
 import ast
 from typing import Mapping
 
-try:  # noqa: I003
+try:
     from django.db.models import Q
 except ImportError:
     import warnings
     warnings.warn('Django not installed but Django Q Transpiler in use. Please install Django.')
 
     class Q:
         def __init__(self, *args, **kwargs):
@@ -19,17 +19,17 @@
 
         def __and__(self, other):
             return self
 
         def __invert__(self):
             return self
 
-from scim2_filter_parser import ast as scim2ast  # noqa: I001
-from scim2_filter_parser.lexer import SCIMLexer  # noqa: I001
-from scim2_filter_parser.parser import SCIMParser  # noqa: I001
+from scim2_filter_parser import ast as scim2ast
+from scim2_filter_parser.lexer import SCIMLexer
+from scim2_filter_parser.parser import SCIMParser
 
 
 def get_query(scim_query: str, attr_map: Mapping):
     token_stream = SCIMLexer().tokenize(scim_query)
     tree = SCIMParser().parse(token_stream)
     return Transpiler(attr_map).transpile(tree)
```

### Comparing `scim2_filter_parser-0.5.0/src/scim2_filter_parser/transpilers/sql.py` & `scim2_filter_parser-0.5.1/src/scim2_filter_parser/transpilers/sql.py`

 * *Files identical despite different names*

### Comparing `scim2_filter_parser-0.5.0/setup.py` & `scim2_filter_parser-0.5.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,322 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: scim2-filter-parser
+Version: 0.5.1
+Summary: A customizable parser/transpiler for SCIM2.0 filters.
+Home-page: https://pypi.org/project/scim2-filter-parser/
+License: MIT
+Keywords: scim,scim2,2.0,filter
+Author: Paul Logston
+Author-email: paul@15five.com
+Maintainer: Paul Logston
+Maintainer-email: paul.logston@gmail.com
+Requires-Python: >=3.8
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: django-query
+Requires-Dist: django (>=3.2) ; extra == "django-query"
+Requires-Dist: sly (==0.5)
+Project-URL: Documentation, https://scim2-filter-parser.readthedocs.io/en/stable/
+Project-URL: Repository, https://github.com/15five/scim2-filter-parser
+Description-Content-Type: text/x-rst
 
-package_dir = \
-{'': 'src'}
+SCIM 2.0 Filter Parser
+======================
 
-packages = \
-['scim2_filter_parser',
- 'scim2_filter_parser.queries',
- 'scim2_filter_parser.transpilers']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['sly==0.5']
-
-extras_require = \
-{'django-query': ['django>=3.2']}
-
-entry_points = \
-{'console_scripts': ['sfp-lexer = scim2_filter_parser.lexer:main',
-                     'sfp-parser = scim2_filter_parser.parser:main',
-                     'sfp-query = scim2_filter_parser.queries.sql:main',
-                     'sfp-transpiler = '
-                     'scim2_filter_parser.transpilers.sql:main']}
-
-setup_kwargs = {
-    'name': 'scim2-filter-parser',
-    'version': '0.5.0',
-    'description': 'A customizable parser/transpiler for SCIM2.0 filters.',
-    'long_description': 'SCIM 2.0 Filter Parser\n======================\n\n|github| |codecov| |docs|\n\n.. |codecov| image:: https://codecov.io/gh/15five/scim2-filter-parser/branch/master/graph/badge.svg\n  :target: https://codecov.io/gh/15five/scim2-filter-parser\n\n.. |docs| image:: https://readthedocs.org/projects/scim2-filter-parser/badge/?version=latest\n  :target: https://scim2-filter-parser.readthedocs.io/en/latest/?badge=latest\n  :alt: Documentation Status\n\n.. |github| image:: https://github.com/15five/scim2-filter-parser/workflows/CI%2FCD/badge.svg\n  :target: https://github.com/15five/scim2-filter-parser/actions?workflow=CI%2FCD\n  :alt: CI/CD Status\n\nDescription\n-----------\n\nSCIM 2.0 defines queries that look like this::\n\n    \'emails[type eq "work" and value co "@example.com"] or ims[type eq "xmpp" and value co "@foo.com"]\'\n\nThese can be hard to work with and covert into SQL to run against a database.\n\nThat\'s where SCIM 2.0 Filter Parser (SFP) can help.\n\nSFP is broken up into four modules, each handling a different part of\ntranslating a SCIM call into a SQL query.\n\nThe first step is tokenization or lexical analysis where the filter query\nis broken down into many tokens that make it up.\n\n::\n\n    sfp-lexer \'emails[type eq "work" and value co "@example.com"] or ims[type eq "xmpp" and value co "@foo.com"]\'\n\n    Token(type=\'ATTRNAME\', value=\'emails\', lineno=1, index=0)\n    Token(type=\'LBRACKET\', value=\'[\', lineno=1, index=6)\n    Token(type=\'ATTRNAME\', value=\'type\', lineno=1, index=7)\n    Token(type=\'EQ\', value=\'eq\', lineno=1, index=12)\n    Token(type=\'COMP_VALUE\', value=\'work\', lineno=1, index=15)\n    Token(type=\'AND\', value=\'and\', lineno=1, index=22)\n    Token(type=\'ATTRNAME\', value=\'value\', lineno=1, index=26)\n    Token(type=\'CO\', value=\'co\', lineno=1, index=32)\n    Token(type=\'COMP_VALUE\', value=\'@example.com\', lineno=1, index=35)\n    Token(type=\'RBRACKET\', value=\']\', lineno=1, index=49)\n    Token(type=\'OR\', value=\'or\', lineno=1, index=51)\n    Token(type=\'ATTRNAME\', value=\'ims\', lineno=1, index=54)\n    Token(type=\'LBRACKET\', value=\'[\', lineno=1, index=57)\n    Token(type=\'ATTRNAME\', value=\'type\', lineno=1, index=58)\n    Token(type=\'EQ\', value=\'eq\', lineno=1, index=63)\n    Token(type=\'COMP_VALUE\', value=\'xmpp\', lineno=1, index=66)\n    Token(type=\'AND\', value=\'and\', lineno=1, index=73)\n    Token(type=\'ATTRNAME\', value=\'value\', lineno=1, index=77)\n    Token(type=\'CO\', value=\'co\', lineno=1, index=83)\n    Token(type=\'COMP_VALUE\', value=\'@foo.com\', lineno=1, index=86)\n    Token(type=\'RBRACKET\', value=\']\', lineno=1, index=96)\n\n\nThe second step is to convert that series of tokens into a abstract syntax tree.\n\n::\n\n    sfp-parser \'emails[type eq "work" and value co "@example.com"] or ims[type eq "xmpp" and value co "@foo.com"]\'\n\n    Filter(expr=LogExpr, negated=False, namespace=None)\n        LogExpr(op=\'or\', expr1=Filter, expr2=Filter)\n            Filter(expr=Filter, negated=False, namespace=None)\n                Filter(expr=Filter, negated=False, namespace=AttrPath)\n                    Filter(expr=LogExpr, negated=False, namespace=None)\n                        LogExpr(op=\'and\', expr1=Filter, expr2=Filter)\n                            Filter(expr=AttrExpr, negated=False, namespace=None)\n                                AttrExpr(value=\'eq\', attr_path=AttrPath, comp_value=CompValue)\n                                    AttrPath(attr_name=\'type\', sub_attr=None, uri=None)\n                                    CompValue(value=\'work\')\n                            Filter(expr=AttrExpr, negated=False, namespace=None)\n                                AttrExpr(value=\'co\', attr_path=AttrPath, comp_value=CompValue)\n                                    AttrPath(attr_name=\'value\', sub_attr=None, uri=None)\n                                    CompValue(value=\'@example.com\')\n                    AttrPath(attr_name=\'emails\', sub_attr=None, uri=None)\n            Filter(expr=Filter, negated=False, namespace=None)\n                Filter(expr=Filter, negated=False, namespace=AttrPath)\n                    Filter(expr=LogExpr, negated=False, namespace=None)\n                        LogExpr(op=\'and\', expr1=Filter, expr2=Filter)\n                            Filter(expr=AttrExpr, negated=False, namespace=None)\n                                AttrExpr(value=\'eq\', attr_path=AttrPath, comp_value=CompValue)\n                                    AttrPath(attr_name=\'type\', sub_attr=None, uri=None)\n                                    CompValue(value=\'xmpp\')\n                            Filter(expr=AttrExpr, negated=False, namespace=None)\n                                AttrExpr(value=\'co\', attr_path=AttrPath, comp_value=CompValue)\n                                    AttrPath(attr_name=\'value\', sub_attr=None, uri=None)\n                                    CompValue(value=\'@foo.com\')\n                    AttrPath(attr_name=\'ims\', sub_attr=None, uri=None)\n\nThe third step is to transpile this AST into a language of our choice.\nThe above query is transpiled to SQL below.\n\n::\n\n    sfp-transpiler \'emails[type eq "work" and value co "@example.com"] or ims[type eq "xmpp" and value co "@foo.com"]\'\n\n    ((emails.type = {0}) AND (emails.value LIKE {1})) OR ((ims.type = {2}) AND (ims.value LIKE {3}))\n    {0: \'work\', 1: \'%@example.com%\', 2: \'xmpp\', 3: \'%@foo.com%\'}\n\nThe fourth step is to take what is a segment of a SQL WHERE clause and complete\nthe rest of the SQL query.\n\n::\n\n    sfp-query \'emails[type eq "work" and value co "@example.com"] or ims[type eq "xmpp" and value co "@foo.com"]\'\n\n    >>> DO NOT USE THIS OUTPUT DIRECTLY\n    >>> SQL INJECTION ATTACK RISK\n    >>> SQL PREVIEW:\n        SELECT DISTINCT users.*\n        FROM users\n        LEFT JOIN emails ON emails.user_id = users.id\n        LEFT JOIN schemas ON schemas.user_id = users.id\n        WHERE ((emails.type = work) AND (emails.value LIKE %@example.com%)) OR ((ims.type = xmpp) AND (ims.value LIKE %@foo.com%));\n\nPlease note that SFP does not build SQL queries with parameters pre-injected.\nThat would create a SQL injection attack vulnerability. Instead a ``SQLQuery``\nobject is created and can be forced to display itself as seen above\nby ``print`` ing the query object.\n\nInstallation\n------------\n::\n\n    pip install scim2-filter-parser\n\n    # Or ...\n\n    pip install scim2-filter-parser[django-query]\n\nUse\n---\n\nAlthough command line shims are provided, the library is intended to be used\nprogrammatically. Users of the library should instantiate the\n``scim2_filter_parser.queries.SQLQuery`` class with an attribute map and optionally\nany joins necessary to make all required fields accessible in the query.\n\nFor example, if user information is stored in the ``users`` table and email\ninformation is stored in a different table ``emails``, then the attribute map\nand the joins might be defined as so::\n\n    from scim2_filter_parser.queries import SQLQuery\n\n    attr_map = {\n        (\'userName\', None, None): \'users.username\',\n        (\'name\', \'familyName\', None): \'users.family_name\',\n        (\'meta\', \'lastModified\', None): \'users.update_ts\',\n        (\'emails\', None, None): \'emails.address\',\n        (\'emails\', \'value\', None): \'emails.address\',\n    }\n\n    joins = (\n        \'LEFT JOIN emails ON emails.user_id = users.id\',\n    )\n\n    filter_ = \'name.familyName co "Simpson" or emails.value eq "lisa@example.com"\'\n\n    q = SQLQuery(filter_, \'users\', attr_map, joins)\n\n    q.sql # Will be...\n\n    SELECT DISTINCT users.*\n    FROM users\n    LEFT JOIN emails ON emails.user_id = users.id\n    WHERE (users.family_name LIKE %s) OR (emails.address = %s);\n\n    q.params # Will be...\n\n    [\'%Simpson%\', \'lisa@example.com\']\n\nThe attribute_map (``attr_map``) is a mapping of SCIM attribute, subattribute,\nand schema uri to a table field. You will need to customize this to your\nparticular database schema.\n\nThe ``SQLQuery.sql`` method returns SQL that can be used as the first\nargument in a call to ``cursor.execute()`` with your favorite DB engine.\nIf you are using a database that requires a replacement character other than \'%s\',\nthen you can subclass the ``SQLQuery`` class and override the ``placeholder`` class\nlevel variable. See the query module and unit tests for an example of this subclassing\nwith SQLite.\n\nThe ``SQLQuery.params`` method returns a list of items that can be used as the\nsecond argument in a call to ``cursor.execute()``.\n\nDjango\n------\n\nIf you would like to produce a `Django Q`_ object instead of a raw SQL query, you can pass\na SCIM filter query and attribute map to the ``get_query`` function from the module\n``scim2_filter_parser.transpilers.django_q_object``. For example::\n\n    get_query(scim_query: str, attr_map: Mapping)\n\nThis Q object can then be passed to a Django filter query like so::\n\n    query = get_query(scim_query, attr_map)\n    User.objects.filter(query)\n\nPlease note that you will need to install the Django Query extra like for this feature to be available::\n\n    pip install scim2-filter-parser[django-query]\n\n.. _`Django Q`: https://docs.djangoproject.com/en/3.1/topics/db/queries/#complex-lookups-with-q-objects\n\nSpeed\n-----\n\nSFP is pretty fast. Check out the speed_test.py script for details on the long and short\nfilter queries tested. SFP transpiled a short filter query into SQL in under 54 microseconds.\nFor a longer query, SFP only took 273 microseconds.\n\n::\n\n    ➜  scim2-filter-parser git:(master) ✗ python -m timeit -s "import speed_test" "speed_test.short()"\n    10000 loops, best of 3: 53.8 usec per loop\n    ➜  scim2-filter-parser git:(master) ✗ python -m timeit -s "import speed_test" "speed_test.long()"\n    1000 loops, best of 3: 273 usec per loop\n\nDevelopment Speed\n-----------------\n\nSince this project is relatively stable, time is only dedicated to it on\nFridays. Thus if you issue a PR, bug, etc, please note that it may take a week\nbefore we get back to you. Thanks you for your patience.\n\nDevelopment\n-----------\n\nThis project uses Poetry to manage dependencies, etc. Thus to install the\nnecessary tools when developing, run:\n\n::\n\n    poetry install -v --extras "django-query"\n\nTests\n-----\n\n.. |tests| image:: https://github.com/15five/scim2-filter-parser/workflows/CI%2FCD/badge.svg\n    :target: https://github.com/15five/scim2-filter-parser/actions\n\nhttps://github.com/15five/scim2-filter-parser/actions\n\nTests are typically run locally with `tox` (https://tox.wiki/). Tox will test\nall supported versions of Python.\n\n```\ntox\n```\n\nTo run the test suite with a single version of Python (the version you created\nthe virtualenv with), run:\n\n::\n\n    poetry run pytest tests/\n\nCoverage\n--------\n\n.. |coverage| image:: https://codecov.io/gh/15five/scim2-filter-parser/graph/badge.svg\n    :target: https://codecov.io/gh/15five/scim2-filter-parser\n\nhttps://codecov.io/gh/15five/scim2-filter-parser\n\n::\n\n    tox -e coverage\n\n\nDeployment\n----------\n\nhttps://pypi.org/project/scim2-filter-parser/\n\nTo deploy this package to PyPI, run:\n\n::\n\n    poetry build\n    poetry publish\n',
-    'author': 'Paul Logston',
-    'author_email': 'paul@15five.com',
-    'maintainer': 'Paul Logston',
-    'maintainer_email': 'paul.logston@gmail.com',
-    'url': 'https://pypi.org/project/scim2-filter-parser/',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8',
-}
+|github| |codecov| |docs|
 
+.. |codecov| image:: https://codecov.io/gh/15five/scim2-filter-parser/branch/master/graph/badge.svg
+  :target: https://codecov.io/gh/15five/scim2-filter-parser
+
+.. |docs| image:: https://readthedocs.org/projects/scim2-filter-parser/badge/?version=latest
+  :target: https://scim2-filter-parser.readthedocs.io/en/latest/?badge=latest
+  :alt: Documentation Status
+
+.. |github| image:: https://github.com/15five/scim2-filter-parser/workflows/CI%2FCD/badge.svg
+  :target: https://github.com/15five/scim2-filter-parser/actions?workflow=CI%2FCD
+  :alt: CI/CD Status
+
+Description
+-----------
+
+SCIM 2.0 defines queries that look like this::
+
+    'emails[type eq "work" and value co "@example.com"] or ims[type eq "xmpp" and value co "@foo.com"]'
+
+These can be hard to work with and covert into SQL to run against a database.
+
+That's where SCIM 2.0 Filter Parser (SFP) can help.
+
+SFP is broken up into four modules, each handling a different part of
+translating a SCIM call into a SQL query.
+
+The first step is tokenization or lexical analysis where the filter query
+is broken down into many tokens that make it up.
+
+::
+
+    sfp-lexer 'emails[type eq "work" and value co "@example.com"] or ims[type eq "xmpp" and value co "@foo.com"]'
+
+    Token(type='ATTRNAME', value='emails', lineno=1, index=0)
+    Token(type='LBRACKET', value='[', lineno=1, index=6)
+    Token(type='ATTRNAME', value='type', lineno=1, index=7)
+    Token(type='EQ', value='eq', lineno=1, index=12)
+    Token(type='COMP_VALUE', value='work', lineno=1, index=15)
+    Token(type='AND', value='and', lineno=1, index=22)
+    Token(type='ATTRNAME', value='value', lineno=1, index=26)
+    Token(type='CO', value='co', lineno=1, index=32)
+    Token(type='COMP_VALUE', value='@example.com', lineno=1, index=35)
+    Token(type='RBRACKET', value=']', lineno=1, index=49)
+    Token(type='OR', value='or', lineno=1, index=51)
+    Token(type='ATTRNAME', value='ims', lineno=1, index=54)
+    Token(type='LBRACKET', value='[', lineno=1, index=57)
+    Token(type='ATTRNAME', value='type', lineno=1, index=58)
+    Token(type='EQ', value='eq', lineno=1, index=63)
+    Token(type='COMP_VALUE', value='xmpp', lineno=1, index=66)
+    Token(type='AND', value='and', lineno=1, index=73)
+    Token(type='ATTRNAME', value='value', lineno=1, index=77)
+    Token(type='CO', value='co', lineno=1, index=83)
+    Token(type='COMP_VALUE', value='@foo.com', lineno=1, index=86)
+    Token(type='RBRACKET', value=']', lineno=1, index=96)
+
+
+The second step is to convert that series of tokens into a abstract syntax tree.
+
+::
+
+    sfp-parser 'emails[type eq "work" and value co "@example.com"] or ims[type eq "xmpp" and value co "@foo.com"]'
+
+    Filter(expr=LogExpr, negated=False, namespace=None)
+        LogExpr(op='or', expr1=Filter, expr2=Filter)
+            Filter(expr=Filter, negated=False, namespace=None)
+                Filter(expr=Filter, negated=False, namespace=AttrPath)
+                    Filter(expr=LogExpr, negated=False, namespace=None)
+                        LogExpr(op='and', expr1=Filter, expr2=Filter)
+                            Filter(expr=AttrExpr, negated=False, namespace=None)
+                                AttrExpr(value='eq', attr_path=AttrPath, comp_value=CompValue)
+                                    AttrPath(attr_name='type', sub_attr=None, uri=None)
+                                    CompValue(value='work')
+                            Filter(expr=AttrExpr, negated=False, namespace=None)
+                                AttrExpr(value='co', attr_path=AttrPath, comp_value=CompValue)
+                                    AttrPath(attr_name='value', sub_attr=None, uri=None)
+                                    CompValue(value='@example.com')
+                    AttrPath(attr_name='emails', sub_attr=None, uri=None)
+            Filter(expr=Filter, negated=False, namespace=None)
+                Filter(expr=Filter, negated=False, namespace=AttrPath)
+                    Filter(expr=LogExpr, negated=False, namespace=None)
+                        LogExpr(op='and', expr1=Filter, expr2=Filter)
+                            Filter(expr=AttrExpr, negated=False, namespace=None)
+                                AttrExpr(value='eq', attr_path=AttrPath, comp_value=CompValue)
+                                    AttrPath(attr_name='type', sub_attr=None, uri=None)
+                                    CompValue(value='xmpp')
+                            Filter(expr=AttrExpr, negated=False, namespace=None)
+                                AttrExpr(value='co', attr_path=AttrPath, comp_value=CompValue)
+                                    AttrPath(attr_name='value', sub_attr=None, uri=None)
+                                    CompValue(value='@foo.com')
+                    AttrPath(attr_name='ims', sub_attr=None, uri=None)
+
+The third step is to transpile this AST into a language of our choice.
+The above query is transpiled to SQL below.
+
+::
+
+    sfp-transpiler 'emails[type eq "work" and value co "@example.com"] or ims[type eq "xmpp" and value co "@foo.com"]'
+
+    ((emails.type = {0}) AND (emails.value LIKE {1})) OR ((ims.type = {2}) AND (ims.value LIKE {3}))
+    {0: 'work', 1: '%@example.com%', 2: 'xmpp', 3: '%@foo.com%'}
+
+The fourth step is to take what is a segment of a SQL WHERE clause and complete
+the rest of the SQL query.
+
+::
+
+    sfp-query 'emails[type eq "work" and value co "@example.com"] or ims[type eq "xmpp" and value co "@foo.com"]'
+
+    >>> DO NOT USE THIS OUTPUT DIRECTLY
+    >>> SQL INJECTION ATTACK RISK
+    >>> SQL PREVIEW:
+        SELECT DISTINCT users.*
+        FROM users
+        LEFT JOIN emails ON emails.user_id = users.id
+        LEFT JOIN schemas ON schemas.user_id = users.id
+        WHERE ((emails.type = work) AND (emails.value LIKE %@example.com%)) OR ((ims.type = xmpp) AND (ims.value LIKE %@foo.com%));
+
+Please note that SFP does not build SQL queries with parameters pre-injected.
+That would create a SQL injection attack vulnerability. Instead a ``SQLQuery``
+object is created and can be forced to display itself as seen above
+by ``print`` ing the query object.
+
+Installation
+------------
+::
+
+    pip install scim2-filter-parser
+
+    # Or ...
+
+    pip install scim2-filter-parser[django-query]
+
+Use
+---
+
+Although command line shims are provided, the library is intended to be used
+programmatically. Users of the library should instantiate the
+``scim2_filter_parser.queries.SQLQuery`` class with an attribute map and optionally
+any joins necessary to make all required fields accessible in the query.
+
+For example, if user information is stored in the ``users`` table and email
+information is stored in a different table ``emails``, then the attribute map
+and the joins might be defined as so::
+
+    from scim2_filter_parser.queries import SQLQuery
+
+    attr_map = {
+        ('userName', None, None): 'users.username',
+        ('name', 'familyName', None): 'users.family_name',
+        ('meta', 'lastModified', None): 'users.update_ts',
+        ('emails', None, None): 'emails.address',
+        ('emails', 'value', None): 'emails.address',
+    }
+
+    joins = (
+        'LEFT JOIN emails ON emails.user_id = users.id',
+    )
+
+    filter_ = 'name.familyName co "Simpson" or emails.value eq "lisa@example.com"'
+
+    q = SQLQuery(filter_, 'users', attr_map, joins)
+
+    q.sql # Will be...
+
+    SELECT DISTINCT users.*
+    FROM users
+    LEFT JOIN emails ON emails.user_id = users.id
+    WHERE (users.family_name LIKE %s) OR (emails.address = %s);
+
+    q.params # Will be...
+
+    ['%Simpson%', 'lisa@example.com']
+
+The attribute_map (``attr_map``) is a mapping of SCIM attribute, subattribute,
+and schema uri to a table field. You will need to customize this to your
+particular database schema.
+
+The ``SQLQuery.sql`` method returns SQL that can be used as the first
+argument in a call to ``cursor.execute()`` with your favorite DB engine.
+If you are using a database that requires a replacement character other than '%s',
+then you can subclass the ``SQLQuery`` class and override the ``placeholder`` class
+level variable. See the query module and unit tests for an example of this subclassing
+with SQLite.
+
+The ``SQLQuery.params`` method returns a list of items that can be used as the
+second argument in a call to ``cursor.execute()``.
+
+Django
+------
+
+If you would like to produce a `Django Q`_ object instead of a raw SQL query, you can pass
+a SCIM filter query and attribute map to the ``get_query`` function from the module
+``scim2_filter_parser.transpilers.django_q_object``. For example::
+
+    get_query(scim_query: str, attr_map: Mapping)
+
+This Q object can then be passed to a Django filter query like so::
+
+    query = get_query(scim_query, attr_map)
+    User.objects.filter(query)
+
+Please note that you will need to install the Django Query extra like for this feature to be available::
+
+    pip install scim2-filter-parser[django-query]
+
+.. _`Django Q`: https://docs.djangoproject.com/en/3.1/topics/db/queries/#complex-lookups-with-q-objects
+
+Speed
+-----
+
+SFP is pretty fast. Check out the speed_test.py script for details on the long and short
+filter queries tested. SFP transpiled a short filter query into SQL in under 54 microseconds.
+For a longer query, SFP only took 273 microseconds.
+
+::
+
+    ➜  scim2-filter-parser git:(master) ✗ python -m timeit -s "import speed_test" "speed_test.short()"
+    10000 loops, best of 3: 53.8 usec per loop
+    ➜  scim2-filter-parser git:(master) ✗ python -m timeit -s "import speed_test" "speed_test.long()"
+    1000 loops, best of 3: 273 usec per loop
+
+Development Speed
+-----------------
+
+Since this project is relatively stable, time is only dedicated to it on
+Fridays. Thus if you issue a PR, bug, etc, please note that it may take a week
+before we get back to you. Thanks you for your patience.
+
+Development
+-----------
+
+This project uses Poetry to manage dependencies, etc. Thus to install the
+necessary tools when developing, run:
+
+::
+
+    poetry install -v --extras "django-query"
+
+Tests
+-----
+
+.. |tests| image:: https://github.com/15five/scim2-filter-parser/workflows/CI%2FCD/badge.svg
+    :target: https://github.com/15five/scim2-filter-parser/actions
+
+https://github.com/15five/scim2-filter-parser/actions
+
+Tests are typically run locally with `tox` (https://tox.wiki/). Tox will test
+all supported versions of Python.
+
+```
+tox
+```
+
+To run the test suite with a single version of Python (the version you created
+the virtualenv with), run:
+
+::
+
+    poetry run pytest tests/
+
+Coverage
+--------
+
+.. |coverage| image:: https://codecov.io/gh/15five/scim2-filter-parser/graph/badge.svg
+    :target: https://codecov.io/gh/15five/scim2-filter-parser
+
+https://codecov.io/gh/15five/scim2-filter-parser
+
+::
+
+    tox -e coverage
+
+
+Deployment
+----------
+
+https://pypi.org/project/scim2-filter-parser/
+
+To deploy this package to PyPI, run:
+
+::
+
+    poetry build
+    poetry publish
 
-setup(**setup_kwargs)
```

