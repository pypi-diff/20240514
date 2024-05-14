# Comparing `tmp/html_to_django-0.0.1.tar.gz` & `tmp/html_to_django-0.0.2.tar.gz`

## Comparing `html_to_django-0.0.1.tar` & `html_to_django-0.0.2.tar`

### file list

```diff
@@ -1,51 +1,55 @@
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 html_to_django-0.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 html_to_django-0.0.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 html_to_django-0.0.1/.github/SECURITY.md
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 html_to_django-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 html_to_django-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 html_to_django-0.0.1/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 html_to_django-0.0.1/.github/workflows/deploy.yml
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 html_to_django-0.0.1/.github/workflows/stylecheck.yml
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 html_to_django-0.0.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 html_to_django-0.0.1/docs/Attributes.md
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 html_to_django-0.0.1/html_to_django/__init__.py
--rw-r--r--   0        0        0     6946 2020-02-02 00:00:00.000000 html_to_django-0.0.1/html_to_django/converter.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 html_to_django-0.0.1/html_to_django/formatters/__init__.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 html_to_django-0.0.1/html_to_django/formatters/attr_formatter.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 html_to_django-0.0.1/html_to_django/formatters/block_formatter.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 html_to_django-0.0.1/html_to_django/formatters/command_formatter.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 html_to_django-0.0.1/html_to_django/formatters/for_formatter.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 html_to_django-0.0.1/html_to_django/formatters/for_wrap_formatter.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 html_to_django-0.0.1/html_to_django/formatters/if_formatter.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 html_to_django-0.0.1/html_to_django/formatters/include_formatter.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 html_to_django-0.0.1/html_to_django/formatters/remove_default_formatter.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 html_to_django-0.0.1/html_to_django/formatters/static_formatter.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 html_to_django-0.0.1/html_to_django/formatters/style_formatter.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 html_to_django-0.0.1/html_to_django/formatters/style_raw_formatter.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 html_to_django-0.0.1/html_to_django/formatters/unwrap_formatter.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 html_to_django-0.0.1/html_to_django/formatters/var_formatter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 html_to_django-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     8351 2020-02-02 00:00:00.000000 html_to_django-0.0.1/tests/tests_converter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 html_to_django-0.0.1/tests/formatters/__init__.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 html_to_django-0.0.1/tests/formatters/tests_attr_formatter.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 html_to_django-0.0.1/tests/formatters/tests_block_formatter.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 html_to_django-0.0.1/tests/formatters/tests_command_formatter.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 html_to_django-0.0.1/tests/formatters/tests_for_formatter.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 html_to_django-0.0.1/tests/formatters/tests_for_wrap_formatter.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 html_to_django-0.0.1/tests/formatters/tests_if_formatter.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 html_to_django-0.0.1/tests/formatters/tests_include_formatter.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 html_to_django-0.0.1/tests/formatters/tests_remove_default_formatter.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 html_to_django-0.0.1/tests/formatters/tests_static_formatter.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 html_to_django-0.0.1/tests/formatters/tests_style_formatter.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 html_to_django-0.0.1/tests/formatters/tests_style_raw_formatter.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 html_to_django-0.0.1/tests/formatters/tests_unwrap_formatter.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 html_to_django-0.0.1/tests/formatters/tests_var_formatter.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 html_to_django-0.0.1/tests/test_project/test.html
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 html_to_django-0.0.1/tests/test_project/something/other.html
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 html_to_django-0.0.1/tests/test_project_expected_result/test.html
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 html_to_django-0.0.1/tests/test_project_expected_result/something/other.html
--rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 html_to_django-0.0.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 html_to_django-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 html_to_django-0.0.1/README.md
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 html_to_django-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 html_to_django-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 html_to_django-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 html_to_django-0.0.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 html_to_django-0.0.2/.github/SECURITY.md
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 html_to_django-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 html_to_django-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 html_to_django-0.0.2/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 html_to_django-0.0.2/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 html_to_django-0.0.2/.github/workflows/stylecheck.yml
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 html_to_django-0.0.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     8571 2020-02-02 00:00:00.000000 html_to_django-0.0.2/docs/Attributes.md
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 html_to_django-0.0.2/html_to_django/__init__.py
+-rw-r--r--   0        0        0     6946 2020-02-02 00:00:00.000000 html_to_django-0.0.2/html_to_django/converter.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 html_to_django-0.0.2/html_to_django/formatters/__init__.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 html_to_django-0.0.2/html_to_django/formatters/assets_formatter.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 html_to_django-0.0.2/html_to_django/formatters/attr_formatter.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 html_to_django-0.0.2/html_to_django/formatters/block_formatter.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 html_to_django-0.0.2/html_to_django/formatters/command_formatter.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 html_to_django-0.0.2/html_to_django/formatters/for_formatter.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 html_to_django-0.0.2/html_to_django/formatters/for_wrap_formatter.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 html_to_django-0.0.2/html_to_django/formatters/if_formatter.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 html_to_django-0.0.2/html_to_django/formatters/include_formatter.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 html_to_django-0.0.2/html_to_django/formatters/remove_default_formatter.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 html_to_django-0.0.2/html_to_django/formatters/remove_formatter.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 html_to_django-0.0.2/html_to_django/formatters/static_formatter.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 html_to_django-0.0.2/html_to_django/formatters/style_formatter.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 html_to_django-0.0.2/html_to_django/formatters/style_raw_formatter.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 html_to_django-0.0.2/html_to_django/formatters/unwrap_formatter.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 html_to_django-0.0.2/html_to_django/formatters/var_formatter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 html_to_django-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     8351 2020-02-02 00:00:00.000000 html_to_django-0.0.2/tests/tests_converter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 html_to_django-0.0.2/tests/formatters/__init__.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 html_to_django-0.0.2/tests/formatters/tests_assets_formatter.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 html_to_django-0.0.2/tests/formatters/tests_attr_formatter.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 html_to_django-0.0.2/tests/formatters/tests_block_formatter.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 html_to_django-0.0.2/tests/formatters/tests_command_formatter.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 html_to_django-0.0.2/tests/formatters/tests_for_formatter.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 html_to_django-0.0.2/tests/formatters/tests_for_wrap_formatter.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 html_to_django-0.0.2/tests/formatters/tests_if_formatter.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 html_to_django-0.0.2/tests/formatters/tests_include_formatter.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 html_to_django-0.0.2/tests/formatters/tests_remove_default_formatter.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 html_to_django-0.0.2/tests/formatters/tests_remove_formatter.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 html_to_django-0.0.2/tests/formatters/tests_static_formatter.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 html_to_django-0.0.2/tests/formatters/tests_style_formatter.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 html_to_django-0.0.2/tests/formatters/tests_style_raw_formatter.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 html_to_django-0.0.2/tests/formatters/tests_unwrap_formatter.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 html_to_django-0.0.2/tests/formatters/tests_var_formatter.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 html_to_django-0.0.2/tests/test_project/test.html
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 html_to_django-0.0.2/tests/test_project/something/other.html
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 html_to_django-0.0.2/tests/test_project_expected_result/test.html
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 html_to_django-0.0.2/tests/test_project_expected_result/something/other.html
+-rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 html_to_django-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 html_to_django-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 html_to_django-0.0.2/README.md
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 html_to_django-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 html_to_django-0.0.2/PKG-INFO
```

### Comparing `html_to_django-0.0.1/CONTRIBUTING.md` & `html_to_django-0.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/.github/CODE_OF_CONDUCT.md` & `html_to_django-0.0.2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md` & `html_to_django-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/.github/workflows/deploy.yml` & `html_to_django-0.0.2/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/.github/workflows/stylecheck.yml` & `html_to_django-0.0.2/.github/workflows/stylecheck.yml`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/.github/workflows/tests.yml` & `html_to_django-0.0.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/docs/Attributes.md` & `html_to_django-0.0.2/docs/Attributes.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,479 +1,536 @@
 00000000: 2320 4174 7472 6962 7574 6573 0a0a 7c20  # Attributes..| 
-00000010: 646a 2d61 7474 7220 2020 2020 2020 207c  dj-attr        |
-00000020: 2044 796e 616d 6963 616c 6c79 2061 7373   Dynamically ass
-00000030: 6967 6e20 6174 7472 6962 7574 6573 2075  ign attributes u
-00000040: 7369 6e67 2044 6a61 6e67 6f20 7465 6d70  sing Django temp
-00000050: 6c61 7465 2076 6172 6961 626c 6573 2e20  late variables. 
-00000060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000070: 2020 2020 2020 207c 0a7c 2d2d 2d2d 2d2d         |.|------
-00000080: 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  ----------|-----
-00000090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000000a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000010: 646a 2d61 7373 6574 7320 2020 2020 207c  dj-assets      |
+00000020: 204d 6f64 6966 7920 7468 6520 2268 7265   Modify the "hre
+00000030: 6622 206f 7220 2273 7263 2220 6174 7472  f" or "src" attr
+00000040: 6962 7574 6573 206f 6620 656c 656d 656e  ibutes of elemen
+00000050: 7473 2077 6974 6820 6120 7061 7468 2070  ts with a path p
+00000060: 7265 6669 7820 616e 6420 7772 6170 2074  refix and wrap t
+00000070: 6865 6d20 696e 2061 2044 6a61 6e67 6f20  hem in a Django 
+00000080: 7374 6174 6963 2063 6f6d 6d61 6e64 2e20  static command. 
+00000090: 7c0a 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.|-------------
+000000a0: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|------------
 000000b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000000c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000000d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000000e0: 2d2d 7c0a 7c20 5379 6e74 6178 2020 2020  --|.| Syntax    
-000000f0: 2020 2020 207c 2060 3c65 6c65 6d65 6e74       | `<element
-00000100: 2064 6a2d 6174 7472 3d22 6174 7472 6962   dj-attr="attrib
-00000110: 7574 6531 3b76 616c 7565 317e 6174 7472  ute1;value1~attr
-00000120: 6962 7574 6532 3b76 616c 7565 327e 6174  ibute2;value2~at
-00000130: 7472 6962 7574 6533 3b76 616c 7565 3322  tribute3;value3"
-00000140: 3e3c 2f65 6c65 6d65 6e74 3e60 207c 0a7c  ></element>` |.|
-00000150: 2045 7861 6d70 6c65 2049 6e70 7574 2020   Example Input  
-00000160: 7c20 603c 6469 7620 646a 2d61 7474 723d  | `<div dj-attr=
-00000170: 2263 6c61 7373 3b6d 792d 636c 6173 737e  "class;my-class~
-00000180: 6964 3b6d 792d 6964 223e 3c2f 6469 763e  id;my-id"></div>
-00000190: 6020 2020 2020 2020 2020 2020 2020 2020  `               
-000001a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000001b0: 2020 2020 2020 2020 7c0a 7c20 4578 616d          |.| Exam
-000001c0: 706c 6520 4f75 7470 7574 207c 2060 3c64  ple Output | `<d
-000001d0: 6976 2063 6c61 7373 3d22 7b7b 206d 792d  iv class="{{ my-
-000001e0: 636c 6173 7320 7d7d 2220 6964 3d22 7b7b  class }}" id="{{
-000001f0: 206d 792d 6964 207d 7d22 3e3c 2f64 6976   my-id }}"></div
-00000200: 3e60 2020 2020 2020 2020 2020 2020 2020  >`              
-00000210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000220: 2020 207c 0a0a 7c20 646a 2d62 6c6f 636b     |..| dj-block
-00000230: 2020 2020 2020 207c 2052 6570 6c61 6365         | Replace
-00000240: 2074 6865 2065 6c65 6d65 6e74 2077 6974   the element wit
-00000250: 6820 446a 616e 676f 2062 6c6f 636b 2074  h Django block t
-00000260: 6167 732e 2020 2020 2020 2020 207c 0a7c  ags.         |.|
-00000270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000280: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
-00000290: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000002a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000002b0: 2d2d 2d2d 2d2d 7c0a 7c20 5379 6e74 6178  ------|.| Syntax
-000002c0: 2020 2020 2020 2020 207c 2060 3c65 6c65           | `<ele
-000002d0: 6d65 6e74 2064 6a2d 626c 6f63 6b3d 2262  ment dj-block="b
-000002e0: 6c6f 636b 6e61 6d65 223e 436f 6e74 656e  lockname">Conten
-000002f0: 743c 2f65 6c65 6d65 6e74 3e60 2020 207c  t</element>`   |
-00000300: 0a7c 2045 7861 6d70 6c65 2049 6e70 7574  .| Example Input
-00000310: 2020 7c20 603c 6469 7620 646a 2d62 6c6f    | `<div dj-blo
-00000320: 636b 3d22 636f 6e74 656e 7422 3e43 6f6e  ck="content">Con
-00000330: 7465 6e74 3c2f 6469 763e 6020 2020 2020  tent</div>`     
-00000340: 2020 2020 2020 2020 7c0a 7c20 4578 616d          |.| Exam
-00000350: 706c 6520 4f75 7470 7574 207c 2060 7b25  ple Output | `{%
-00000360: 2062 6c6f 636b 2063 6f6e 7465 6e74 2025   block content %
-00000370: 7d43 6f6e 7465 6e74 7b25 2065 6e64 626c  }Content{% endbl
-00000380: 6f63 6b20 257d 6020 2020 2020 2020 2020  ock %}`         
-00000390: 207c 0a0a 7c20 646a 2d63 6f6d 6d61 6e64   |..| dj-command
-000003a0: 2020 2020 207c 2052 6570 6c61 6365 2074       | Replace t
-000003b0: 6865 2065 6c65 6d65 6e74 2077 6974 6820  he element with 
-000003c0: 6120 446a 616e 676f 2074 656d 706c 6174  a Django templat
-000003d0: 6520 636f 6d6d 616e 642e 2020 2020 2020  e command.      
-000003e0: 2020 207c 0a7c 2d2d 2d2d 2d2d 2d2d 2d2d     |.|----------
-000003f0: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
-00000400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000430: 2d2d 2d2d 7c0a 7c20 5379 6e74 6178 2020  ----|.| Syntax  
-00000440: 2020 2020 2020 207c 2060 3c65 6c65 6d65         | `<eleme
-00000450: 6e74 2064 6a2d 636f 6d6d 616e 643d 2263  nt dj-command="c
-00000460: 6f6d 6d61 6e64 223e 3c2f 656c 656d 656e  ommand"></elemen
-00000470: 743e 6020 2020 2020 2020 2020 2020 2020  t>`             
-00000480: 2020 2020 207c 0a7c 2045 7861 6d70 6c65       |.| Example
-00000490: 2049 6e70 7574 2020 7c20 603c 6469 7620   Input  | `<div 
-000004a0: 646a 2d63 6f6d 6d61 6e64 3d22 7572 6c20  dj-command="url 
-000004b0: 2769 6e64 6578 2722 3e3c 2f64 6976 3e60  'index'"></div>`
-000004c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000004d0: 2020 2020 2020 7c0a 7c20 4578 616d 706c        |.| Exampl
-000004e0: 6520 4f75 7470 7574 207c 2060 7b25 2075  e Output | `{% u
-000004f0: 726c 2027 696e 6465 7827 2025 7d60 2020  rl 'index' %}`  
-00000500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000520: 2020 2020 2020 207c 0a0a 7c20 646a 2d66         |..| dj-f
-00000530: 6f72 2020 2020 2020 2020 207c 2052 6570  or         | Rep
-00000540: 6c61 6365 2074 6865 2065 6c65 6d65 6e74  lace the element
-00000550: 2077 6974 6820 6120 446a 616e 676f 2074   with a Django t
-00000560: 656d 706c 6174 6520 666f 7220 6c6f 6f70  emplate for loop
-00000570: 2e20 2020 2020 2020 2020 7c0a 7c2d 2d2d  .         |.|---
-00000580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  -------------|--
-00000590: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000005a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000005b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000005c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 7c20  ------------|.| 
-000005d0: 5379 6e74 6178 2020 2020 2020 2020 207c  Syntax         |
-000005e0: 2060 3c65 6c65 6d65 6e74 2064 6a2d 666f   `<element dj-fo
-000005f0: 723d 2269 7465 6d20 696e 206c 6973 7422  r="item in list"
-00000600: 3e43 6f6e 7465 6e74 3c2f 656c 656d 656e  >Content</elemen
-00000610: 743e 6020 2020 2020 2020 2020 2020 7c0a  t>`           |.
-00000620: 7c20 4578 616d 706c 6520 496e 7075 7420  | Example Input 
-00000630: 207c 2060 3c64 6976 2064 6a2d 666f 723d   | `<div dj-for=
-00000640: 2269 7465 6d20 696e 206c 6973 7422 3e3c  "item in list"><
-00000650: 703e 4865 6c6c 6f3c 2f70 3e3c 2f64 6976  p>Hello</p></div
-00000660: 3e60 2020 2020 2020 2020 2020 2020 2020  >`              
-00000670: 7c0a 7c20 4578 616d 706c 6520 4f75 7470  |.| Example Outp
-00000680: 7574 207c 2060 7b25 2066 6f72 2069 7465  ut | `{% for ite
-00000690: 6d20 696e 206c 6973 7420 257d 3c70 3e48  m in list %}<p>H
-000006a0: 656c 6c6f 3c2f 703e 7b25 2065 6e64 666f  ello</p>{% endfo
-000006b0: 7220 257d 6020 2020 2020 2020 2020 2020  r %}`           
-000006c0: 2020 7c0a 0a7c 2064 6a2d 666f 722d 7772    |..| dj-for-wr
-000006d0: 6170 2020 2020 7c20 5772 6170 2074 6865  ap    | Wrap the
-000006e0: 2065 6c65 6d65 6e74 2077 6974 6869 6e20   element within 
-000006f0: 6120 446a 616e 676f 2074 656d 706c 6174  a Django templat
-00000700: 6520 666f 7220 6c6f 6f70 2e20 2020 2020  e for loop.     
-00000710: 2020 2020 7c0a 7c2d 2d2d 2d2d 2d2d 2d2d      |.|---------
-00000720: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
-00000730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000760: 2d2d 2d2d 2d7c 0a7c 2053 796e 7461 7820  -----|.| Syntax 
-00000770: 2020 2020 2020 2020 7c20 603c 656c 656d          | `<elem
-00000780: 656e 7420 646a 2d66 6f72 2d77 7261 703d  ent dj-for-wrap=
-00000790: 2269 7465 6d20 696e 206c 6973 7422 3e43  "item in list">C
-000007a0: 6f6e 7465 6e74 3c2f 656c 656d 656e 743e  ontent</element>
-000007b0: 6020 2020 2020 7c0a 7c20 4578 616d 706c  `     |.| Exampl
-000007c0: 6520 496e 7075 7420 207c 2060 3c64 6976  e Input  | `<div
-000007d0: 2064 6a2d 666f 722d 7772 6170 3d22 6974   dj-for-wrap="it
-000007e0: 656d 2069 6e20 6c69 7374 223e 436f 6e74  em in list">Cont
-000007f0: 656e 743c 2f64 6976 3e60 2020 2020 2020  ent</div>`      
-00000800: 2020 2020 2020 207c 0a7c 2045 7861 6d70         |.| Examp
-00000810: 6c65 204f 7574 7075 7420 7c20 607b 2520  le Output | `{% 
-00000820: 666f 7220 6974 656d 2069 6e20 6c69 7374  for item in list
-00000830: 2025 7d3c 6469 763e 436f 6e74 656e 743c   %}<div>Content<
-00000840: 2f64 6976 3e7b 2520 656e 6466 6f72 2025  /div>{% endfor %
-00000850: 7d60 2020 2020 2020 7c0a 0a7c 2064 6a2d  }`      |..| dj-
-00000860: 6966 2c20 646a 2d65 6c69 662c 2064 6a2d  if, dj-elif, dj-
-00000870: 656c 7365 207c 2052 6570 6c61 6365 2074  else | Replace t
-00000880: 6865 2065 6c65 6d65 6e74 7320 7769 7468  he elements with
-00000890: 2061 2044 6a61 6e67 6f20 7465 6d70 6c61   a Django templa
-000008a0: 7465 2069 662d 656c 6966 2d65 6c73 6520  te if-elif-else 
-000008b0: 7374 7275 6374 7572 652e 2020 2020 2020  structure.      
-000008c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000910: 7c0a 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.|-------------
-00000920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d  ------------|---
-00000930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000009a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000009b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000009c0: 2d2d 2d2d 2d2d 2d7c 0a7c 2053 796e 7461  -------|.| Synta
-000009d0: 7820 2020 2020 2020 2020 2020 2020 2020  x               
-000009e0: 2020 207c 2060 3c65 6c65 6d65 6e74 2064     | `<element d
-000009f0: 6a2d 6966 3d22 636f 6e64 6974 696f 6e22  j-if="condition"
-00000a00: 3e43 6f6e 7465 6e74 3c2f 656c 656d 656e  >Content</elemen
-00000a10: 743e 603c 6272 2f3e 603c 656c 656d 656e  t>`<br/>`<elemen
-00000a20: 7420 646a 2d65 6c69 663d 2263 6f6e 6469  t dj-elif="condi
-00000a30: 7469 6f6e 223e 436f 6e74 656e 743c 2f65  tion">Content</e
-00000a40: 6c65 6d65 6e74 3e60 3c62 722f 3e60 3c65  lement>`<br/>`<e
-00000a50: 6c65 6d65 6e74 2064 6a2d 656c 7365 3d22  lement dj-else="
-00000a60: 636f 6e64 6974 696f 6e22 3e43 6f6e 7465  condition">Conte
-00000a70: 6e74 3c2f 656c 656d 656e 743e 6020 7c0a  nt</element>` |.
-00000a80: 7c20 4e6f 7465 2020 2020 2020 2020 2020  | Note          
-00000a90: 2020 2020 2020 2020 2020 7c20 5468 6520            | The 
-00000aa0: 6064 6a2d 656c 6966 6020 616e 6420 6064  `dj-elif` and `d
-00000ab0: 6a2d 656c 7365 6020 6174 7472 6962 7574  j-else` attribut
-00000ac0: 6573 2061 7265 206f 7074 696f 6e61 6c2e  es are optional.
-00000ad0: 204d 756c 7469 706c 6520 6064 6a2d 656c   Multiple `dj-el
-00000ae0: 6966 6020 6174 7472 6962 7574 6573 2061  if` attributes a
-00000af0: 7265 2061 6c6c 6f77 6564 2e20 2020 2020  re allowed.     
-00000b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b30: 2020 2020 207c 0a7c 2045 7861 6d70 6c65       |.| Example
-00000b40: 2049 6e70 7574 2020 2020 2020 2020 2020   Input          
-00000b50: 207c 2060 3c64 6976 2064 6a2d 6966 3d22   | `<div dj-if="
-00000b60: 636f 6e64 6974 696f 6e31 223e 5465 7374  condition1">Test
-00000b70: 3c2f 6469 763e 3c64 6976 2064 6a2d 656c  </div><div dj-el
-00000b80: 6966 3d22 636f 6e64 6974 696f 6e32 223e  if="condition2">
-00000b90: 5465 7374 323c 2f64 6976 3e3c 6469 7620  Test2</div><div 
-00000ba0: 646a 2d65 6c73 653e 5465 7374 333c 2f64  dj-else>Test3</d
-00000bb0: 6976 3e60 2020 2020 2020 2020 2020 2020  iv>`            
-00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000be0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-00000bf0: 4578 616d 706c 6520 4f75 7470 7574 2020  Example Output  
-00000c00: 2020 2020 2020 2020 7c20 607b 2520 6966          | `{% if
-00000c10: 2063 6f6e 6469 7469 6f6e 3120 257d 5465   condition1 %}Te
-00000c20: 7374 7b25 2065 6c69 6620 636f 6e64 6974  st{% elif condit
-00000c30: 696f 6e32 2025 7d54 6573 7432 7b25 2065  ion2 %}Test2{% e
-00000c40: 6c73 6520 257d 5465 7374 337b 2520 656e  lse %}Test3{% en
-00000c50: 6469 6620 257d 6020 2020 2020 2020 2020  dif %}`         
-00000c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ca0: 2020 207c 0a0a 7c20 646a 2d69 6e63 6c75     |..| dj-inclu
-00000cb0: 6465 2020 2020 207c 2052 6570 6c61 6365  de     | Replace
-00000cc0: 2074 6865 2063 6f6e 7465 6e74 206f 6620   the content of 
-00000cd0: 7468 6520 656c 656d 656e 7420 7769 7468  the element with
-00000ce0: 2061 2044 6a61 6e67 6f20 7465 6d70 6c61   a Django templa
-00000cf0: 7465 2069 6e63 6c75 6465 2063 6f6d 6d61  te include comma
-00000d00: 6e64 2e20 7c0a 7c2d 2d2d 2d2d 2d2d 2d2d  nd. |.|---------
-00000d10: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
-00000d20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000d30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000d40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000d50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000d60: 2d2d 2d2d 7c0a 7c20 5379 6e74 6178 2020  ----|.| Syntax  
-00000d70: 2020 2020 2020 207c 2060 3c65 6c65 6d65         | `<eleme
-00000d80: 6e74 2064 6a2d 696e 636c 7564 653d 2274  nt dj-include="t
-00000d90: 656d 706c 6174 655f 6e61 6d65 223e 3c2f  emplate_name"></
-00000da0: 656c 656d 656e 743e 6020 2020 2020 2020  element>`       
+000000e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000000f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000100: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000110: 2d2d 2d2d 7c0a 7c20 5379 6e74 6178 2020  ----|.| Syntax  
+00000120: 2020 2020 2020 207c 2060 3c68 746d 6c20         | `<html 
+00000130: 646a 2d61 7373 6574 733d 2261 7373 6574  dj-assets="asset
+00000140: 5f69 6465 6e74 6966 6965 723b 6173 7365  _identifier;asse
+00000150: 745f 7072 6566 6978 223e 2e2e 2e3c 2f68  t_prefix">...</h
+00000160: 746d 6c3e 6020 2020 2020 2020 2020 2020  tml>`           
+00000170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000190: 2020 2020 2020 2020 7c0a 7c20 4578 616d          |.| Exam
+000001a0: 706c 6520 496e 7075 7420 207c 2060 3c68  ple Input  | `<h
+000001b0: 746d 6c20 646a 2d61 7373 6574 733d 2261  tml dj-assets="a
+000001c0: 7373 6574 733b 6d6f 6475 6c65 223e 3c69  ssets;module"><i
+000001d0: 6d67 2073 7263 3d22 6173 7365 7473 2f69  mg src="assets/i
+000001e0: 6d61 6765 2e70 6e67 223e 3c2f 6874 6d6c  mage.png"></html
+000001f0: 3e60 2020 2020 2020 2020 2020 2020 2020  >`              
+00000200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000210: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00000220: 4578 616d 706c 6520 4f75 7470 7574 207c  Example Output |
+00000230: 2060 3c68 746d 6c3e 3c69 6d67 2073 7263   `<html><img src
+00000240: 3d22 7b25 2073 7461 7469 6320 276d 6f64  ="{% static 'mod
+00000250: 756c 652f 6173 7365 7473 2f69 6d61 6765  ule/assets/image
+00000260: 2e70 6e67 2720 257d 222f 3e3c 2f68 746d  .png' %}"/></htm
+00000270: 6c3e 6020 2020 2020 2020 2020 2020 2020  l>`             
+00000280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000002a0: 7c0a 0a7c 2064 6a2d 6174 7472 2020 2020  |..| dj-attr    
+000002b0: 2020 2020 7c20 4479 6e61 6d69 6361 6c6c      | Dynamicall
+000002c0: 7920 6173 7369 676e 2061 7474 7269 6275  y assign attribu
+000002d0: 7465 7320 7573 696e 6720 446a 616e 676f  tes using Django
+000002e0: 2074 656d 706c 6174 6520 7661 7269 6162   template variab
+000002f0: 6c65 732e 2020 2020 2020 2020 2020 2020  les.            
+00000300: 2020 2020 2020 2020 2020 2020 7c0a 7c2d              |.|-
+00000310: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
+00000320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000340: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000350: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000370: 2d2d 2d2d 2d2d 2d7c 0a7c 2053 796e 7461  -------|.| Synta
+00000380: 7820 2020 2020 2020 2020 7c20 603c 656c  x         | `<el
+00000390: 656d 656e 7420 646a 2d61 7474 723d 2261  ement dj-attr="a
+000003a0: 7474 7269 6275 7465 313b 7661 6c75 6531  ttribute1;value1
+000003b0: 7e61 7474 7269 6275 7465 323b 7661 6c75  ~attribute2;valu
+000003c0: 6532 7e61 7474 7269 6275 7465 333b 7661  e2~attribute3;va
+000003d0: 6c75 6533 223e 3c2f 656c 656d 656e 743e  lue3"></element>
+000003e0: 6020 7c0a 7c20 4578 616d 706c 6520 496e  ` |.| Example In
+000003f0: 7075 7420 207c 2060 3c64 6976 2064 6a2d  put  | `<div dj-
+00000400: 6174 7472 3d22 636c 6173 733b 6d79 2d63  attr="class;my-c
+00000410: 6c61 7373 7e69 643b 6d79 2d69 6422 3e3c  lass~id;my-id"><
+00000420: 2f64 6976 3e60 2020 2020 2020 2020 2020  /div>`          
+00000430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000440: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00000450: 2045 7861 6d70 6c65 204f 7574 7075 7420   Example Output 
+00000460: 7c20 603c 6469 7620 636c 6173 733d 227b  | `<div class="{
+00000470: 7b20 6d79 2d63 6c61 7373 207d 7d22 2069  { my-class }}" i
+00000480: 643d 227b 7b20 6d79 2d69 6420 7d7d 223e  d="{{ my-id }}">
+00000490: 3c2f 6469 763e 6020 2020 2020 2020 2020  </div>`         
+000004a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000004b0: 2020 2020 2020 2020 7c0a 0a7c 2064 6a2d          |..| dj-
+000004c0: 626c 6f63 6b20 2020 2020 2020 7c20 5265  block       | Re
+000004d0: 706c 6163 6520 7468 6520 656c 656d 656e  place the elemen
+000004e0: 7420 7769 7468 2044 6a61 6e67 6f20 626c  t with Django bl
+000004f0: 6f63 6b20 7461 6773 2e20 2020 2020 2020  ock tags.       
+00000500: 2020 7c0a 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d    |.|-----------
+00000510: 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d  -----|----------
+00000520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000530: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000540: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 2053  -----------|.| S
+00000550: 796e 7461 7820 2020 2020 2020 2020 7c20  yntax         | 
+00000560: 603c 656c 656d 656e 7420 646a 2d62 6c6f  `<element dj-blo
+00000570: 636b 3d22 626c 6f63 6b6e 616d 6522 3e43  ck="blockname">C
+00000580: 6f6e 7465 6e74 3c2f 656c 656d 656e 743e  ontent</element>
+00000590: 6020 2020 7c0a 7c20 4578 616d 706c 6520  `   |.| Example 
+000005a0: 496e 7075 7420 207c 2060 3c64 6976 2064  Input  | `<div d
+000005b0: 6a2d 626c 6f63 6b3d 2263 6f6e 7465 6e74  j-block="content
+000005c0: 223e 436f 6e74 656e 743c 2f64 6976 3e60  ">Content</div>`
+000005d0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+000005e0: 2045 7861 6d70 6c65 204f 7574 7075 7420   Example Output 
+000005f0: 7c20 607b 2520 626c 6f63 6b20 636f 6e74  | `{% block cont
+00000600: 656e 7420 257d 436f 6e74 656e 747b 2520  ent %}Content{% 
+00000610: 656e 6462 6c6f 636b 2025 7d60 2020 2020  endblock %}`    
+00000620: 2020 2020 2020 7c0a 0a7c 2064 6a2d 636f        |..| dj-co
+00000630: 6d6d 616e 6420 2020 2020 7c20 5265 706c  mmand     | Repl
+00000640: 6163 6520 7468 6520 656c 656d 656e 7420  ace the element 
+00000650: 7769 7468 2061 2044 6a61 6e67 6f20 7465  with a Django te
+00000660: 6d70 6c61 7465 2063 6f6d 6d61 6e64 2e20  mplate command. 
+00000670: 2020 2020 2020 2020 7c0a 7c2d 2d2d 2d2d          |.|-----
+00000680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  -----------|----
+00000690: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000006a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000006b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000006c0: 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 2053 796e  ---------|.| Syn
+000006d0: 7461 7820 2020 2020 2020 2020 7c20 603c  tax         | `<
+000006e0: 656c 656d 656e 7420 646a 2d63 6f6d 6d61  element dj-comma
+000006f0: 6e64 3d22 636f 6d6d 616e 6422 3e3c 2f65  nd="command"></e
+00000700: 6c65 6d65 6e74 3e60 2020 2020 2020 2020  lement>`        
+00000710: 2020 2020 2020 2020 2020 7c0a 7c20 4578            |.| Ex
+00000720: 616d 706c 6520 496e 7075 7420 207c 2060  ample Input  | `
+00000730: 3c64 6976 2064 6a2d 636f 6d6d 616e 643d  <div dj-command=
+00000740: 2275 726c 2027 696e 6465 7827 223e 3c2f  "url 'index'"></
+00000750: 6469 763e 6020 2020 2020 2020 2020 2020  div>`           
+00000760: 2020 2020 2020 2020 2020 207c 0a7c 2045             |.| E
+00000770: 7861 6d70 6c65 204f 7574 7075 7420 7c20  xample Output | 
+00000780: 607b 2520 7572 6c20 2769 6e64 6578 2720  `{% url 'index' 
+00000790: 257d 6020 2020 2020 2020 2020 2020 2020  %}`             
+000007a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007b0: 2020 2020 2020 2020 2020 2020 7c0a 0a7c              |..|
+000007c0: 2064 6a2d 666f 7220 2020 2020 2020 2020   dj-for         
+000007d0: 7c20 5265 706c 6163 6520 7468 6520 656c  | Replace the el
+000007e0: 656d 656e 7420 7769 7468 2061 2044 6a61  ement with a Dja
+000007f0: 6e67 6f20 7465 6d70 6c61 7465 2066 6f72  ngo template for
+00000800: 206c 6f6f 702e 2020 2020 2020 2020 207c   loop.         |
+00000810: 0a7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .|--------------
+00000820: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --|-------------
+00000830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000850: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000860: 2d7c 0a7c 2053 796e 7461 7820 2020 2020  -|.| Syntax     
+00000870: 2020 2020 7c20 603c 656c 656d 656e 7420      | `<element 
+00000880: 646a 2d66 6f72 3d22 6974 656d 2069 6e20  dj-for="item in 
+00000890: 6c69 7374 223e 436f 6e74 656e 743c 2f65  list">Content</e
+000008a0: 6c65 6d65 6e74 3e60 2020 2020 2020 2020  lement>`        
+000008b0: 2020 207c 0a7c 2045 7861 6d70 6c65 2049     |.| Example I
+000008c0: 6e70 7574 2020 7c20 603c 6469 7620 646a  nput  | `<div dj
+000008d0: 2d66 6f72 3d22 6974 656d 2069 6e20 6c69  -for="item in li
+000008e0: 7374 223e 3c70 3e48 656c 6c6f 3c2f 703e  st"><p>Hello</p>
+000008f0: 3c2f 6469 763e 6020 2020 2020 2020 2020  </div>`         
+00000900: 2020 2020 207c 0a7c 2045 7861 6d70 6c65       |.| Example
+00000910: 204f 7574 7075 7420 7c20 607b 2520 666f   Output | `{% fo
+00000920: 7220 6974 656d 2069 6e20 6c69 7374 2025  r item in list %
+00000930: 7d3c 703e 4865 6c6c 6f3c 2f70 3e7b 2520  }<p>Hello</p>{% 
+00000940: 656e 6466 6f72 2025 7d60 2020 2020 2020  endfor %}`      
+00000950: 2020 2020 2020 207c 0a0a 7c20 646a 2d66         |..| dj-f
+00000960: 6f72 2d77 7261 7020 2020 207c 2057 7261  or-wrap    | Wra
+00000970: 7020 7468 6520 656c 656d 656e 7420 7769  p the element wi
+00000980: 7468 696e 2061 2044 6a61 6e67 6f20 7465  thin a Django te
+00000990: 6d70 6c61 7465 2066 6f72 206c 6f6f 702e  mplate for loop.
+000009a0: 2020 2020 2020 2020 207c 0a7c 2d2d 2d2d           |.|----
+000009b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d  ------------|---
+000009c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000009d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000009e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000009f0: 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 7c20 5379  ----------|.| Sy
+00000a00: 6e74 6178 2020 2020 2020 2020 207c 2060  ntax         | `
+00000a10: 3c65 6c65 6d65 6e74 2064 6a2d 666f 722d  <element dj-for-
+00000a20: 7772 6170 3d22 6974 656d 2069 6e20 6c69  wrap="item in li
+00000a30: 7374 223e 436f 6e74 656e 743c 2f65 6c65  st">Content</ele
+00000a40: 6d65 6e74 3e60 2020 2020 207c 0a7c 2045  ment>`     |.| E
+00000a50: 7861 6d70 6c65 2049 6e70 7574 2020 7c20  xample Input  | 
+00000a60: 603c 6469 7620 646a 2d66 6f72 2d77 7261  `<div dj-for-wra
+00000a70: 703d 2269 7465 6d20 696e 206c 6973 7422  p="item in list"
+00000a80: 3e43 6f6e 7465 6e74 3c2f 6469 763e 6020  >Content</div>` 
+00000a90: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00000aa0: 4578 616d 706c 6520 4f75 7470 7574 207c  Example Output |
+00000ab0: 2060 7b25 2066 6f72 2069 7465 6d20 696e   `{% for item in
+00000ac0: 206c 6973 7420 257d 3c64 6976 3e43 6f6e   list %}<div>Con
+00000ad0: 7465 6e74 3c2f 6469 763e 7b25 2065 6e64  tent</div>{% end
+00000ae0: 666f 7220 257d 6020 2020 2020 207c 0a0a  for %}`      |..
+00000af0: 7c20 646a 2d69 662c 2064 6a2d 656c 6966  | dj-if, dj-elif
+00000b00: 2c20 646a 2d65 6c73 6520 7c20 5265 706c  , dj-else | Repl
+00000b10: 6163 6520 7468 6520 656c 656d 656e 7473  ace the elements
+00000b20: 2077 6974 6820 6120 446a 616e 676f 2074   with a Django t
+00000b30: 656d 706c 6174 6520 6966 2d65 6c69 662d  emplate if-elif-
+00000b40: 656c 7365 2073 7472 7563 7475 7265 2e20  else structure. 
+00000b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ba0: 2020 2020 207c 0a7c 2d2d 2d2d 2d2d 2d2d       |.|--------
+00000bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000bc0: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|--------------
+00000bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000be0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000bf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000c00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000c10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000c20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000c30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 7c20  ------------|.| 
+00000c60: 5379 6e74 6178 2020 2020 2020 2020 2020  Syntax          
+00000c70: 2020 2020 2020 2020 7c20 603c 656c 656d          | `<elem
+00000c80: 656e 7420 646a 2d69 663d 2263 6f6e 6469  ent dj-if="condi
+00000c90: 7469 6f6e 223e 436f 6e74 656e 743c 2f65  tion">Content</e
+00000ca0: 6c65 6d65 6e74 3e60 3c62 722f 3e60 3c65  lement>`<br/>`<e
+00000cb0: 6c65 6d65 6e74 2064 6a2d 656c 6966 3d22  lement dj-elif="
+00000cc0: 636f 6e64 6974 696f 6e22 3e43 6f6e 7465  condition">Conte
+00000cd0: 6e74 3c2f 656c 656d 656e 743e 603c 6272  nt</element>`<br
+00000ce0: 2f3e 603c 656c 656d 656e 7420 646a 2d65  />`<element dj-e
+00000cf0: 6c73 653d 2263 6f6e 6469 7469 6f6e 223e  lse="condition">
+00000d00: 436f 6e74 656e 743c 2f65 6c65 6d65 6e74  Content</element
+00000d10: 3e60 207c 0a7c 204e 6f74 6520 2020 2020  >` |.| Note     
+00000d20: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00000d30: 2054 6865 2060 646a 2d65 6c69 6660 2061   The `dj-elif` a
+00000d40: 6e64 2060 646a 2d65 6c73 6560 2061 7474  nd `dj-else` att
+00000d50: 7269 6275 7465 7320 6172 6520 6f70 7469  ributes are opti
+00000d60: 6f6e 616c 2e20 4d75 6c74 6970 6c65 2060  onal. Multiple `
+00000d70: 646a 2d65 6c69 6660 2061 7474 7269 6275  dj-elif` attribu
+00000d80: 7465 7320 6172 6520 616c 6c6f 7765 642e  tes are allowed.
+00000d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000dc0: 2020 2020 7c0a 7c20 4578 616d 706c 6520      |.| Example 
-00000dd0: 496e 7075 7420 207c 2060 3c64 6976 2064  Input  | `<div d
-00000de0: 6a2d 696e 636c 7564 653d 2274 656d 706c  j-include="templ
-00000df0: 6174 655f 6e61 6d65 2e68 746d 6c22 3e3c  ate_name.html"><
-00000e00: 2f64 6976 3e60 2020 2020 2020 2020 2020  /div>`          
-00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e20: 2020 2020 7c0a 7c20 4578 616d 706c 6520      |.| Example 
-00000e30: 4f75 7470 7574 207c 2060 7b25 2069 6e63  Output | `{% inc
-00000e40: 6c75 6465 2022 7465 6d70 6c61 7465 5f6e  lude "template_n
-00000e50: 616d 652e 6874 6d6c 2220 257d 6020 2020  ame.html" %}`   
+00000dc0: 2020 2020 2020 2020 2020 7c0a 7c20 4578            |.| Ex
+00000dd0: 616d 706c 6520 496e 7075 7420 2020 2020  ample Input     
+00000de0: 2020 2020 2020 7c20 603c 6469 7620 646a        | `<div dj
+00000df0: 2d69 663d 2263 6f6e 6469 7469 6f6e 3122  -if="condition1"
+00000e00: 3e54 6573 743c 2f64 6976 3e3c 6469 7620  >Test</div><div 
+00000e10: 646a 2d65 6c69 663d 2263 6f6e 6469 7469  dj-elif="conditi
+00000e20: 6f6e 3222 3e54 6573 7432 3c2f 6469 763e  on2">Test2</div>
+00000e30: 3c64 6976 2064 6a2d 656c 7365 3e54 6573  <div dj-else>Tes
+00000e40: 7433 3c2f 6469 763e 6020 2020 2020 2020  t3</div>`       
+00000e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e80: 2020 2020 7c0a 0a7c 2064 6a2d 7265 6d6f      |..| dj-remo
-00000e90: 7665 2d64 6566 6175 6c74 207c 2052 656d  ve-default | Rem
-00000ea0: 6f76 696e 6720 7468 6520 446f 6374 7970  oving the Doctyp
-00000eb0: 652c 2022 6865 6164 2220 656c 656d 656e  e, "head" elemen
-00000ec0: 742c 2061 6e64 2022 7363 7269 7074 2220  t, and "script" 
-00000ed0: 656c 656d 656e 7420 7769 7468 696e 2074  element within t
-00000ee0: 6865 2022 626f 6479 2220 656c 656d 656e  he "body" elemen
-00000ef0: 742e 2049 7420 616c 736f 2075 6e77 7261  t. It also unwra
-00000f00: 7073 2074 6865 2022 626f 6479 2220 616e  ps the "body" an
-00000f10: 6420 2268 746d 6c22 2065 6c65 6d65 6e74  d "html" element
-00000f20: 732c 206c 6561 7669 6e67 206f 6e6c 7920  s, leaving only 
-00000f30: 7468 6520 7265 6d61 696e 696e 6720 636f  the remaining co
-00000f40: 6e74 656e 7420 6f66 2074 6865 2022 626f  ntent of the "bo
-00000f50: 6479 2220 656c 656d 656e 742e 207c 0a7c  dy" element. |.|
-00000f60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f70: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|------------
-00000f80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000fa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e80: 207c 0a7c 2045 7861 6d70 6c65 204f 7574   |.| Example Out
+00000e90: 7075 7420 2020 2020 2020 2020 207c 2060  put          | `
+00000ea0: 7b25 2069 6620 636f 6e64 6974 696f 6e31  {% if condition1
+00000eb0: 2025 7d54 6573 747b 2520 656c 6966 2063   %}Test{% elif c
+00000ec0: 6f6e 6469 7469 6f6e 3220 257d 5465 7374  ondition2 %}Test
+00000ed0: 327b 2520 656c 7365 2025 7d54 6573 7433  2{% else %}Test3
+00000ee0: 7b25 2065 6e64 6966 2025 7d60 2020 2020  {% endif %}`    
+00000ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f30: 2020 2020 2020 2020 7c0a 0a7c 2064 6a2d          |..| dj-
+00000f40: 696e 636c 7564 6520 2020 2020 7c20 5265  include     | Re
+00000f50: 706c 6163 6520 7468 6520 636f 6e74 656e  place the conten
+00000f60: 7420 6f66 2074 6865 2065 6c65 6d65 6e74  t of the element
+00000f70: 2077 6974 6820 6120 446a 616e 676f 2074   with a Django t
+00000f80: 656d 706c 6174 6520 696e 636c 7564 6520  emplate include 
+00000f90: 636f 6d6d 616e 642e 207c 0a7c 2d2d 2d2d  command. |.|----
+00000fa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d  ------------|---
 00000fb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000fc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000fd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000fe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000ff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001030: 2d2d 2d2d 2d7c 0a7c 2053 796e 7461 7820  -----|.| Syntax 
-00001040: 2020 2020 2020 2020 2020 207c 2060 3c68             | `<h
-00001050: 746d 6c20 646a 2d72 656d 6f76 652d 6465  tml dj-remove-de
-00001060: 6661 756c 743e 2e2e 2e3c 2f68 746d 6c3e  fault>...</html>
-00001070: 6020 2020 2020 2020 2020 2020 2020 2020  `               
-00001080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ff0: 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 2053 796e  ---------|.| Syn
+00001000: 7461 7820 2020 2020 2020 2020 7c20 603c  tax         | `<
+00001010: 656c 656d 656e 7420 646a 2d69 6e63 6c75  element dj-inclu
+00001020: 6465 3d22 7465 6d70 6c61 7465 5f6e 616d  de="template_nam
+00001030: 6522 3e3c 2f65 6c65 6d65 6e74 3e60 2020  e"></element>`  
+00001040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001050: 2020 2020 2020 2020 207c 0a7c 2045 7861           |.| Exa
+00001060: 6d70 6c65 2049 6e70 7574 2020 7c20 603c  mple Input  | `<
+00001070: 6469 7620 646a 2d69 6e63 6c75 6465 3d22  div dj-include="
+00001080: 7465 6d70 6c61 7465 5f6e 616d 652e 6874  template_name.ht
+00001090: 6d6c 223e 3c2f 6469 763e 6020 2020 2020  ml"></div>`     
 000010a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001100: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-00001110: 204e 6f74 6520 2020 2020 2020 2020 2020   Note           
-00001120: 2020 207c 2054 6869 7320 6973 206d 6561     | This is mea
-00001130: 6e74 2074 6f20 7265 6d6f 7665 2061 6c6c  nt to remove all
-00001140: 2074 6865 2064 6566 6175 6c74 2068 746d   the default htm
-00001150: 6c20 7772 6170 7065 7220 636f 6465 206d  l wrapper code m
-00001160: 6f73 7420 7374 6174 6963 2068 746d 6c20  ost static html 
-00001170: 6765 6e65 7261 746f 7273 2070 726f 6475  generators produ
-00001180: 6365 2e20 2020 2020 2020 2020 2020 2020  ce.             
-00001190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011e0: 2020 2020 207c 0a7c 2045 7861 6d70 6c65       |.| Example
-000011f0: 2049 6e70 7574 2020 2020 207c 2060 3c21   Input     | `<!
-00001200: 444f 4354 5950 4520 6874 6d6c 3e3c 6874  DOCTYPE html><ht
-00001210: 6d6c 2064 6a2d 7265 6d6f 7665 2d64 6566  ml dj-remove-def
-00001220: 6175 6c74 3e3c 6865 6164 3e2e 2e2e 3c2f  ault><head>...</
-00001230: 6865 6164 3e3c 626f 6479 3e43 6f6e 7465  head><body>Conte
-00001240: 6e74 3c73 6372 6970 743e 2e2e 2e3c 2f73  nt<script>...</s
-00001250: 6372 6970 743e 3c2f 626f 6479 3e3c 2f68  cript></body></h
-00001260: 746d 6c3e 6020 2020 2020 2020 2020 2020  tml>`           
-00001270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012b0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-000012c0: 2045 7861 6d70 6c65 204f 7574 7075 7420   Example Output 
-000012d0: 2020 207c 2060 436f 6e74 656e 7460 2020     | `Content`  
-000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010b0: 2020 2020 2020 2020 207c 0a7c 2045 7861           |.| Exa
+000010c0: 6d70 6c65 204f 7574 7075 7420 7c20 607b  mple Output | `{
+000010d0: 2520 696e 636c 7564 6520 2274 656d 706c  % include "templ
+000010e0: 6174 655f 6e61 6d65 2e68 746d 6c22 2025  ate_name.html" %
+000010f0: 7d60 2020 2020 2020 2020 2020 2020 2020  }`              
+00001100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001110: 2020 2020 2020 2020 207c 0a0a 7c20 646a           |..| dj
+00001120: 2d72 656d 6f76 652d 6465 6661 756c 7420  -remove-default 
+00001130: 7c20 5265 6d6f 7665 2074 6865 2044 6f63  | Remove the Doc
+00001140: 7479 7065 2c20 2268 6561 6422 2065 6c65  type, "head" ele
+00001150: 6d65 6e74 2c20 616e 6420 2273 6372 6970  ment, and "scrip
+00001160: 7422 2065 6c65 6d65 6e74 2077 6974 6869  t" element withi
+00001170: 6e20 7468 6520 2262 6f64 7922 2065 6c65  n the "body" ele
+00001180: 6d65 6e74 2e20 4974 2061 6c73 6f20 756e  ment. It also un
+00001190: 7772 6170 7320 7468 6520 2262 6f64 7922  wraps the "body"
+000011a0: 2061 6e64 2022 6874 6d6c 2220 656c 656d   and "html" elem
+000011b0: 656e 7473 2c20 6c65 6176 696e 6720 6f6e  ents, leaving on
+000011c0: 6c79 2074 6865 2072 656d 6169 6e69 6e67  ly the remaining
+000011d0: 2063 6f6e 7465 6e74 206f 6620 7468 6520   content of the 
+000011e0: 2262 6f64 7922 2065 6c65 6d65 6e74 2e20  "body" element. 
+000011f0: 7c0a 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.|-------------
+00001200: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
+00001210: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001230: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001290: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000012a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000012b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000012c0: 2d2d 2d2d 2d2d 7c0a 7c20 5379 6e74 6178  ------|.| Syntax
+000012d0: 2020 2020 2020 2020 2020 2020 7c20 603c              | `<
+000012e0: 6874 6d6c 2064 6a2d 7265 6d6f 7665 2d64  html dj-remove-d
+000012f0: 6566 6175 6c74 3e2e 2e2e 3c2f 6874 6d6c  efault>...</html
+00001300: 3e60 2020 2020 2020 2020 2020 2020 2020  >`              
 00001310: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001320: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001330: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001340: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001350: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001360: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001370: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001390: 2020 2020 207c 0a0a 7c20 646a 2d73 7461       |..| dj-sta
-000013a0: 7469 6320 2020 2020 207c 2052 6570 6c61  tic      | Repla
-000013b0: 6365 2074 6865 2076 616c 7565 206f 6620  ce the value of 
-000013c0: 7468 6520 7370 6563 6966 6965 6420 7461  the specified ta
-000013d0: 6720 7769 7468 2061 2044 6a61 6e67 6f20  g with a Django 
-000013e0: 7465 6d70 6c61 7465 2073 7461 7469 6320  template static 
-000013f0: 636f 6d6d 616e 642c 2075 7369 6e67 2074  command, using t
-00001400: 6865 2073 7065 6369 6669 6564 2073 7461  he specified sta
-00001410: 7469 6320 6669 6c65 2070 6174 682e 207c  tic file path. |
-00001420: 0a7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .|--------------
-00001430: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --|-------------
-00001440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001450: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000014a0: 2d2d 2d2d 2d2d 2d2d 7c0a 7c20 5379 6e74  --------|.| Synt
-000014b0: 6178 2020 2020 2020 2020 207c 2060 3c65  ax         | `<e
-000014c0: 6c65 6d65 6e74 2064 6a2d 7374 6174 6963  lement dj-static
-000014d0: 3d22 7461 673b 7374 6174 6963 5f66 696c  ="tag;static_fil
-000014e0: 655f 7061 7468 223e 3c2f 656c 656d 656e  e_path"></elemen
-000014f0: 743e 6020 2020 2020 2020 2020 2020 2020  t>`             
+00001390: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+000013a0: 4e6f 7465 2020 2020 2020 2020 2020 2020  Note            
+000013b0: 2020 7c20 5468 6973 2069 7320 6d65 616e    | This is mean
+000013c0: 7420 746f 2072 656d 6f76 6520 616c 6c20  t to remove all 
+000013d0: 7468 6520 6465 6661 756c 7420 6874 6d6c  the default html
+000013e0: 2077 7261 7070 6572 2063 6f64 6520 6d6f   wrapper code mo
+000013f0: 7374 2073 7461 7469 6320 6874 6d6c 2067  st static html g
+00001400: 656e 6572 6174 6f72 7320 7072 6f64 7563  enerators produc
+00001410: 652e 2020 2020 2020 2020 2020 2020 2020  e.              
+00001420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001470: 2020 7c0a 7c20 4578 616d 706c 6520 496e    |.| Example In
+00001480: 7075 7420 2020 2020 7c20 603c 2144 4f43  put     | `<!DOC
+00001490: 5459 5045 2068 746d 6c3e 3c68 746d 6c20  TYPE html><html 
+000014a0: 646a 2d72 656d 6f76 652d 6465 6661 756c  dj-remove-defaul
+000014b0: 743e 3c68 6561 643e 2e2e 2e3c 2f68 6561  t><head>...</hea
+000014c0: 643e 3c62 6f64 793e 436f 6e74 656e 743c  d><body>Content<
+000014d0: 7363 7269 7074 3e2e 2e2e 3c2f 7363 7269  script>...</scri
+000014e0: 7074 3e3c 2f62 6f64 793e 3c2f 6874 6d6c  pt></body></html
+000014f0: 3e60 2020 2020 2020 2020 2020 2020 2020  >`              
 00001500: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001510: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001530: 207c 0a7c 2045 7861 6d70 6c65 2049 6e70   |.| Example Inp
-00001540: 7574 2020 7c20 603c 696d 6720 646a 2d73  ut  | `<img dj-s
-00001550: 7461 7469 633d 2273 7263 3b69 6d61 6765  tatic="src;image
-00001560: 732f 7069 632e 6a70 6722 3e60 2020 2020  s/pic.jpg">`    
+00001530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001540: 2020 2020 2020 2020 7c0a 7c20 4578 616d          |.| Exam
+00001550: 706c 6520 4f75 7470 7574 2020 2020 7c20  ple Output    | 
+00001560: 6043 6f6e 7465 6e74 6020 2020 2020 2020  `Content`       
 00001570: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001580: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001590: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000015a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015b0: 2020 2020 2020 2020 2020 7c0a 7c20 4578            |.| Ex
-000015c0: 616d 706c 6520 4f75 7470 7574 207c 2060  ample Output | `
-000015d0: 3c69 6d67 2073 7263 3d22 7b25 2073 7461  <img src="{% sta
-000015e0: 7469 6320 2769 6d61 6765 732f 7069 632e  tic 'images/pic.
-000015f0: 6a70 6727 2025 7d22 3e60 2020 2020 2020  jpg' %}">`      
+000015b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001640: 2020 207c 0a0a 7c20 646a 2d73 7479 6c65     |..| dj-style
-00001650: 2020 2020 2020 207c 204d 6f64 6966 7920         | Modify 
-00001660: 7468 6520 7374 796c 6520 6174 7472 6962  the style attrib
-00001670: 7574 6520 6f66 2061 2065 6c65 6d65 6e74  ute of a element
-00001680: 2077 6974 6820 646a 616e 676f 2076 6172   with django var
-00001690: 6961 626c 6573 2e20 2020 2020 2020 2020  iables.         
-000016a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016b0: 2020 2020 7c0a 7c2d 2d2d 2d2d 2d2d 2d2d      |.|---------
-000016c0: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
-000016d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000016e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000016f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001720: 2d2d 2d2d 7c0a 7c20 5379 6e74 6178 2020  ----|.| Syntax  
-00001730: 2020 2020 2020 207c 2060 3c65 6c65 6d65         | `<eleme
-00001740: 6e74 2064 6a2d 7374 796c 653d 2270 726f  nt dj-style="pro
-00001750: 7065 7274 7931 3b76 616c 7565 313b 7661  perty1;value1;va
-00001760: 6c75 655f 7479 7065 317e 7072 6f70 6572  lue_type1~proper
-00001770: 7479 323b 7661 6c75 6532 3b76 616c 7565  ty2;value2;value
-00001780: 5f74 7970 6532 223e 3c2f 656c 656d 656e  _type2"></elemen
-00001790: 743e 6020 7c0a 7c20 4e6f 7465 2020 2020  t>` |.| Note    
-000017a0: 2020 2020 2020 207c 2054 6865 2060 7661         | The `va
-000017b0: 6c75 655f 7479 7065 6020 6973 206f 7074  lue_type` is opt
-000017c0: 696f 6e61 6c2e 2049 6620 6e6f 7420 696e  ional. If not in
-000017d0: 636c 7564 6564 2073 7469 6c6c 2061 6464  cluded still add
-000017e0: 2074 6865 2060 3b60 2061 6674 6572 2074   the `;` after t
-000017f0: 6865 2076 616c 7565 2e20 2020 2020 2020  he value.       
-00001800: 2020 2020 7c0a 7c20 4578 616d 706c 6520      |.| Example 
-00001810: 496e 7075 7420 207c 2060 3c64 6976 2073  Input  | `<div s
-00001820: 7479 6c65 3d22 636f 6c6f 723a 7265 6422  tyle="color:red"
-00001830: 2064 6a2d 7374 796c 653d 2262 6163 6b67   dj-style="backg
-00001840: 726f 756e 642d 636f 6c6f 723b 636f 6c6f  round-color;colo
-00001850: 723b 7e70 6164 6469 6e67 3b70 6164 6469  r;~padding;paddi
-00001860: 6e67 3b70 7822 3e60 2020 2020 2020 2020  ng;px">`        
-00001870: 2020 2020 7c0a 7c20 4578 616d 706c 6520      |.| Example 
-00001880: 4f75 7470 7574 207c 2060 3c64 6976 2073  Output | `<div s
-00001890: 7479 6c65 3d22 636f 6c6f 723a 7265 643b  tyle="color:red;
-000018a0: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
-000018b0: 3a7b 7b20 636f 6c6f 7220 7d7d 3b70 6164  :{{ color }};pad
-000018c0: 6469 6e67 3a7b 7b20 7061 6464 696e 6720  ding:{{ padding 
-000018d0: 7d7d 7078 223e 6020 2020 2020 2020 2020  }}px">`         
-000018e0: 2020 2020 7c0a 0a7c 2064 6a2d 7374 796c      |..| dj-styl
-000018f0: 652d 7261 7720 2020 7c20 4d6f 6469 6679  e-raw   | Modify
-00001900: 2074 6865 2073 7479 6c65 2061 7474 7269   the style attri
-00001910: 6275 7465 206f 6620 6120 656c 656d 656e  bute of a elemen
-00001920: 742e 2054 6865 2076 616c 7565 2077 696c  t. The value wil
-00001930: 6c20 6265 2069 6e73 6572 7465 6420 6173  l be inserted as
-00001940: 2069 732e 2020 2020 2020 207c 0a7c 2d2d   is.       |.|--
-00001950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d  --------------|-
-00001960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000019a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000019b0: 2d7c 0a7c 2053 796e 7461 7820 2020 2020  -|.| Syntax     
-000019c0: 2020 2020 7c20 603c 656c 656d 656e 7420      | `<element 
-000019d0: 646a 2d73 7479 6c65 2d72 6177 3d22 7072  dj-style-raw="pr
-000019e0: 6f70 6572 7479 313b 7661 6c75 6531 7e70  operty1;value1~p
-000019f0: 726f 7065 7274 7932 3b76 616c 7565 3222  roperty2;value2"
-00001a00: 3e3c 2f65 6c65 6d65 6e74 3e60 2020 2020  ></element>`    
-00001a10: 2020 2020 2020 207c 0a7c 2045 7861 6d70         |.| Examp
-00001a20: 6c65 2049 6e70 7574 2020 7c20 603c 6469  le Input  | `<di
-00001a30: 7620 7374 796c 653d 2263 6f6c 6f72 3a72  v style="color:r
-00001a40: 6564 2220 646a 2d73 7479 6c65 2d72 6177  ed" dj-style-raw
-00001a50: 3d22 6261 636b 6772 6f75 6e64 2d63 6f6c  ="background-col
-00001a60: 6f72 3b62 6c75 657e 636f 6c6f 723a 7b7b  or;blue~color:{{
-00001a70: 2063 6f6c 6f72 207d 7d22 3e60 207c 0a7c   color }}">` |.|
-00001a80: 2045 7861 6d70 6c65 204f 7574 7075 7420   Example Output 
-00001a90: 7c20 603c 6469 7620 7374 796c 653d 2263  | `<div style="c
-00001aa0: 6f6c 6f72 3a7b 7b20 636f 6c6f 7220 7d7d  olor:{{ color }}
-00001ab0: 3b62 6163 6b67 726f 756e 642d 636f 6c6f  ;background-colo
-00001ac0: 723a 626c 7565 223e 6020 2020 2020 2020  r:blue">`       
-00001ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ae0: 2020 207c 0a0a 7c20 646a 2d75 6e77 7261     |..| dj-unwra
-00001af0: 7020 2020 2020 207c 2052 656d 6f76 6520  p      | Remove 
-00001b00: 7468 6520 656c 656d 656e 7427 7320 7461  the element's ta
-00001b10: 6773 2062 7574 206b 6565 7073 2069 7473  gs but keeps its
-00001b20: 2063 6f6e 7465 6e74 2e20 7c0a 7c2d 2d2d   content. |.|---
-00001b30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  -------------|--
-00001b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001b70: 7c0a 7c20 5379 6e74 6178 2020 2020 2020  |.| Syntax      
-00001b80: 2020 207c 2060 3c65 6c65 6d65 6e74 2064     | `<element d
-00001b90: 6a2d 756e 7772 6170 3e43 6f6e 7465 6e74  j-unwrap>Content
-00001ba0: 3c2f 656c 656d 656e 743e 6020 2020 2020  </element>`     
-00001bb0: 2020 2020 2020 7c0a 7c20 4578 616d 706c        |.| Exampl
-00001bc0: 6520 496e 7075 7420 207c 2060 3c64 6976  e Input  | `<div
-00001bd0: 2064 6a2d 756e 7772 6170 3e3c 703e 4865   dj-unwrap><p>He
-00001be0: 6c6c 6f2c 2077 6f72 6c64 213c 2f70 3e3c  llo, world!</p><
-00001bf0: 2f64 6976 3e60 2020 2020 2020 7c0a 7c20  /div>`      |.| 
-00001c00: 4578 616d 706c 6520 4f75 7470 7574 207c  Example Output |
-00001c10: 2060 3c70 3e48 656c 6c6f 2c20 776f 726c   `<p>Hello, worl
-00001c20: 6421 3c2f 703e 6020 2020 2020 2020 2020  d!</p>`         
-00001c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c40: 2020 7c0a 0a7c 2064 6a2d 7661 7220 2020    |..| dj-var   
-00001c50: 2020 2020 2020 7c20 5265 706c 6163 6520        | Replace 
-00001c60: 7468 6520 656c 656d 656e 7427 7320 636f  the element's co
-00001c70: 6e74 656e 7420 7769 7468 2061 2044 6a61  ntent with a Dja
-00001c80: 6e67 6f20 7465 6d70 6c61 7465 2076 6172  ngo template var
-00001c90: 6961 626c 652e 207c 0a7c 2d2d 2d2d 2d2d  iable. |.|------
-00001ca0: 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  ----------|-----
-00001cb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001cd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 2053  -----------|.| S
-00001cf0: 796e 7461 7820 2020 2020 2020 2020 7c20  yntax         | 
-00001d00: 603c 656c 656d 656e 7420 646a 2d76 6172  `<element dj-var
-00001d10: 3d22 7661 7269 6162 6c65 5f6e 616d 6522  ="variable_name"
-00001d20: 3e43 6f6e 7465 6e74 3c2f 656c 656d 656e  >Content</elemen
-00001d30: 743e 6020 2020 2020 2020 2020 2020 207c  t>`            |
-00001d40: 0a7c 2045 7861 6d70 6c65 2049 6e70 7574  .| Example Input
-00001d50: 2020 7c20 603c 7020 646a 2d76 6172 3d22    | `<p dj-var="
-00001d60: 6772 6565 7469 6e67 223e 4865 6c6c 6f2c  greeting">Hello,
-00001d70: 2077 6f72 6c64 213c 2f70 3e60 2020 2020   world!</p>`    
-00001d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d90: 2020 207c 0a7c 2045 7861 6d70 6c65 204f     |.| Example O
-00001da0: 7574 7075 7420 7c20 603c 703e 7b7b 2067  utput | `<p>{{ g
-00001db0: 7265 6574 696e 6720 7d7d 3c2f 703e 6020  reeting }}</p>` 
-00001dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001de0: 2020 2020 2020 207c                             |
+00001610: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00001620: 0a7c 2064 6a2d 7265 6d6f 7665 2020 2020  .| dj-remove    
+00001630: 2020 7c20 5265 6d6f 7665 2074 6865 2065    | Remove the e
+00001640: 6c65 6d65 6e74 2e20 2020 2020 2020 2020  lement.         
+00001650: 2020 2020 7c0a 7c2d 2d2d 2d2d 2d2d 2d2d      |.|---------
+00001660: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
+00001670: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001680: 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 2053 796e  ---------|.| Syn
+00001690: 7461 7820 2020 2020 2020 2020 7c20 603c  tax         | `<
+000016a0: 656c 656d 656e 7420 646a 2d72 656d 6f76  element dj-remov
+000016b0: 653e 3c2f 656c 656d 656e 743e 6020 7c0a  e></element>` |.
+000016c0: 7c20 4578 616d 706c 6520 496e 7075 7420  | Example Input 
+000016d0: 207c 2060 3c64 6976 3e3c 7020 646a 2d72   | `<div><p dj-r
+000016e0: 656d 6f76 653e 3c2f 703e 3c2f 6469 763e  emove></p></div>
+000016f0: 6020 207c 0a7c 2045 7861 6d70 6c65 204f  `  |.| Example O
+00001700: 7574 7075 7420 7c20 6020 6020 2020 2020  utput | ` `     
+00001710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001720: 2020 2020 2020 2020 7c0a 0a7c 2064 6a2d          |..| dj-
+00001730: 7374 6174 6963 2020 2020 2020 7c20 5265  static      | Re
+00001740: 706c 6163 6520 7468 6520 7661 6c75 6520  place the value 
+00001750: 6f66 2074 6865 2073 7065 6369 6669 6564  of the specified
+00001760: 2074 6167 2077 6974 6820 6120 446a 616e   tag with a Djan
+00001770: 676f 2074 656d 706c 6174 6520 7374 6174  go template stat
+00001780: 6963 2063 6f6d 6d61 6e64 2c20 7573 696e  ic command, usin
+00001790: 6720 7468 6520 7370 6563 6966 6965 6420  g the specified 
+000017a0: 7374 6174 6963 2066 696c 6520 7061 7468  static file path
+000017b0: 2e20 7c0a 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  . |.|-----------
+000017c0: 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d  -----|----------
+000017d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000017e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000017f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 2053  -----------|.| S
+00001840: 796e 7461 7820 2020 2020 2020 2020 7c20  yntax         | 
+00001850: 603c 656c 656d 656e 7420 646a 2d73 7461  `<element dj-sta
+00001860: 7469 633d 2274 6167 3b73 7461 7469 635f  tic="tag;static_
+00001870: 6669 6c65 5f70 6174 6822 3e3c 2f65 6c65  file_path"></ele
+00001880: 6d65 6e74 3e60 2020 2020 2020 2020 2020  ment>`          
+00001890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018c0: 2020 2020 7c0a 7c20 4578 616d 706c 6520      |.| Example 
+000018d0: 496e 7075 7420 207c 2060 3c69 6d67 2064  Input  | `<img d
+000018e0: 6a2d 7374 6174 6963 3d22 7372 633b 696d  j-static="src;im
+000018f0: 6167 6573 2f70 6963 2e6a 7067 223e 6020  ages/pic.jpg">` 
+00001900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001940: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00001950: 2045 7861 6d70 6c65 204f 7574 7075 7420   Example Output 
+00001960: 7c20 603c 696d 6720 7372 633d 227b 2520  | `<img src="{% 
+00001970: 7374 6174 6963 2027 696d 6167 6573 2f70  static 'images/p
+00001980: 6963 2e6a 7067 2720 257d 222f 3e60 2020  ic.jpg' %}"/>`  
+00001990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019d0: 2020 2020 2020 7c0a 0a7c 2064 6a2d 7374        |..| dj-st
+000019e0: 796c 6520 2020 2020 2020 7c20 4d6f 6469  yle       | Modi
+000019f0: 6679 2074 6865 2073 7479 6c65 2061 7474  fy the style att
+00001a00: 7269 6275 7465 206f 6620 6120 656c 656d  ribute of a elem
+00001a10: 656e 7420 7769 7468 2064 6a61 6e67 6f20  ent with django 
+00001a20: 7661 7269 6162 6c65 732e 2020 2020 2020  variables.      
+00001a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a40: 2020 2020 2020 207c 0a7c 2d2d 2d2d 2d2d         |.|------
+00001a50: 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  ----------|-----
+00001a60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001a70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001ab0: 2d2d 2d2d 2d2d 2d7c 0a7c 2053 796e 7461  -------|.| Synta
+00001ac0: 7820 2020 2020 2020 2020 7c20 603c 656c  x         | `<el
+00001ad0: 656d 656e 7420 646a 2d73 7479 6c65 3d22  ement dj-style="
+00001ae0: 7072 6f70 6572 7479 313b 7661 6c75 6531  property1;value1
+00001af0: 3b76 616c 7565 5f74 7970 6531 7e70 726f  ;value_type1~pro
+00001b00: 7065 7274 7932 3b76 616c 7565 323b 7661  perty2;value2;va
+00001b10: 6c75 655f 7479 7065 3222 3e3c 2f65 6c65  lue_type2"></ele
+00001b20: 6d65 6e74 3e60 207c 0a7c 204e 6f74 6520  ment>` |.| Note 
+00001b30: 2020 2020 2020 2020 2020 7c20 5468 6520            | The 
+00001b40: 6076 616c 7565 5f74 7970 6560 2069 7320  `value_type` is 
+00001b50: 6f70 7469 6f6e 616c 2e20 4966 206e 6f74  optional. If not
+00001b60: 2069 6e63 6c75 6465 6420 7374 696c 6c20   included still 
+00001b70: 6164 6420 7468 6520 603b 6020 6166 7465  add the `;` afte
+00001b80: 7220 7468 6520 7661 6c75 652e 2020 2020  r the value.    
+00001b90: 2020 2020 2020 207c 0a7c 2045 7861 6d70         |.| Examp
+00001ba0: 6c65 2049 6e70 7574 2020 7c20 603c 6469  le Input  | `<di
+00001bb0: 7620 7374 796c 653d 2263 6f6c 6f72 3a72  v style="color:r
+00001bc0: 6564 2220 646a 2d73 7479 6c65 3d22 6261  ed" dj-style="ba
+00001bd0: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3b63  ckground-color;c
+00001be0: 6f6c 6f72 3b7e 7061 6464 696e 673b 7061  olor;~padding;pa
+00001bf0: 6464 696e 673b 7078 223e 6020 2020 2020  dding;px">`     
+00001c00: 2020 2020 2020 207c 0a7c 2045 7861 6d70         |.| Examp
+00001c10: 6c65 204f 7574 7075 7420 7c20 603c 6469  le Output | `<di
+00001c20: 7620 7374 796c 653d 2263 6f6c 6f72 3a72  v style="color:r
+00001c30: 6564 3b62 6163 6b67 726f 756e 642d 636f  ed;background-co
+00001c40: 6c6f 723a 7b7b 2063 6f6c 6f72 207d 7d3b  lor:{{ color }};
+00001c50: 7061 6464 696e 673a 7b7b 2070 6164 6469  padding:{{ paddi
+00001c60: 6e67 207d 7d70 7822 3e60 2020 2020 2020  ng }}px">`      
+00001c70: 2020 2020 2020 207c 0a0a 7c20 646a 2d73         |..| dj-s
+00001c80: 7479 6c65 2d72 6177 2020 207c 204d 6f64  tyle-raw   | Mod
+00001c90: 6966 7920 7468 6520 7374 796c 6520 6174  ify the style at
+00001ca0: 7472 6962 7574 6520 6f66 2061 2065 6c65  tribute of a ele
+00001cb0: 6d65 6e74 2e20 5468 6520 7661 6c75 6520  ment. The value 
+00001cc0: 7769 6c6c 2062 6520 696e 7365 7274 6564  will be inserted
+00001cd0: 2061 7320 6973 2e20 2020 2020 2020 7c0a   as is.       |.
+00001ce0: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
+00001cf0: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|--------------
+00001d00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d40: 2d2d 2d2d 7c0a 7c20 5379 6e74 6178 2020  ----|.| Syntax  
+00001d50: 2020 2020 2020 207c 2060 3c65 6c65 6d65         | `<eleme
+00001d60: 6e74 2064 6a2d 7374 796c 652d 7261 773d  nt dj-style-raw=
+00001d70: 2270 726f 7065 7274 7931 3b76 616c 7565  "property1;value
+00001d80: 317e 7072 6f70 6572 7479 323b 7661 6c75  1~property2;valu
+00001d90: 6532 223e 3c2f 656c 656d 656e 743e 6020  e2"></element>` 
+00001da0: 2020 2020 2020 2020 2020 7c0a 7c20 4578            |.| Ex
+00001db0: 616d 706c 6520 496e 7075 7420 207c 2060  ample Input  | `
+00001dc0: 3c64 6976 2073 7479 6c65 3d22 636f 6c6f  <div style="colo
+00001dd0: 723a 7265 6422 2064 6a2d 7374 796c 652d  r:red" dj-style-
+00001de0: 7261 773d 2262 6163 6b67 726f 756e 642d  raw="background-
+00001df0: 636f 6c6f 723b 626c 7565 7e63 6f6c 6f72  color;blue~color
+00001e00: 3a7b 7b20 636f 6c6f 7220 7d7d 223e 6020  :{{ color }}">` 
+00001e10: 7c0a 7c20 4578 616d 706c 6520 4f75 7470  |.| Example Outp
+00001e20: 7574 207c 2060 3c64 6976 2073 7479 6c65  ut | `<div style
+00001e30: 3d22 636f 6c6f 723a 7b7b 2063 6f6c 6f72  ="color:{{ color
+00001e40: 207d 7d3b 6261 636b 6772 6f75 6e64 2d63   }};background-c
+00001e50: 6f6c 6f72 3a62 6c75 6522 3e60 2020 2020  olor:blue">`    
+00001e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e70: 2020 2020 2020 7c0a 0a7c 2064 6a2d 756e        |..| dj-un
+00001e80: 7772 6170 2020 2020 2020 7c20 5265 6d6f  wrap      | Remo
+00001e90: 7665 2074 6865 2065 6c65 6d65 6e74 2773  ve the element's
+00001ea0: 2074 6167 7320 6275 7420 6b65 6570 7320   tags but keeps 
+00001eb0: 6974 7320 636f 6e74 656e 742e 207c 0a7c  its content. |.|
+00001ec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001ed0: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
+00001ee0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001ef0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001f00: 2d2d 2d7c 0a7c 2053 796e 7461 7820 2020  ---|.| Syntax   
+00001f10: 2020 2020 2020 7c20 603c 656c 656d 656e        | `<elemen
+00001f20: 7420 646a 2d75 6e77 7261 703e 436f 6e74  t dj-unwrap>Cont
+00001f30: 656e 743c 2f65 6c65 6d65 6e74 3e60 2020  ent</element>`  
+00001f40: 2020 2020 2020 2020 207c 0a7c 2045 7861           |.| Exa
+00001f50: 6d70 6c65 2049 6e70 7574 2020 7c20 603c  mple Input  | `<
+00001f60: 6469 7620 646a 2d75 6e77 7261 703e 3c70  div dj-unwrap><p
+00001f70: 3e48 656c 6c6f 2c20 776f 726c 6421 3c2f  >Hello, world!</
+00001f80: 703e 3c2f 6469 763e 6020 2020 2020 207c  p></div>`      |
+00001f90: 0a7c 2045 7861 6d70 6c65 204f 7574 7075  .| Example Outpu
+00001fa0: 7420 7c20 603c 703e 4865 6c6c 6f2c 2077  t | `<p>Hello, w
+00001fb0: 6f72 6c64 213c 2f70 3e60 2020 2020 2020  orld!</p>`      
+00001fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fd0: 2020 2020 207c 0a0a 7c20 646a 2d76 6172       |..| dj-var
+00001fe0: 2020 2020 2020 2020 207c 2052 6570 6c61           | Repla
+00001ff0: 6365 2074 6865 2065 6c65 6d65 6e74 2773  ce the element's
+00002000: 2063 6f6e 7465 6e74 2077 6974 6820 6120   content with a 
+00002010: 446a 616e 676f 2074 656d 706c 6174 6520  Django template 
+00002020: 7661 7269 6162 6c65 2e20 7c0a 7c2d 2d2d  variable. |.|---
+00002030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  -------------|--
+00002040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002060: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002070: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a  --------------|.
+00002080: 7c20 5379 6e74 6178 2020 2020 2020 2020  | Syntax        
+00002090: 207c 2060 3c65 6c65 6d65 6e74 2064 6a2d   | `<element dj-
+000020a0: 7661 723d 2276 6172 6961 626c 655f 6e61  var="variable_na
+000020b0: 6d65 223e 436f 6e74 656e 743c 2f65 6c65  me">Content</ele
+000020c0: 6d65 6e74 3e60 2020 2020 2020 2020 2020  ment>`          
+000020d0: 2020 7c0a 7c20 4578 616d 706c 6520 496e    |.| Example In
+000020e0: 7075 7420 207c 2060 3c70 2064 6a2d 7661  put  | `<p dj-va
+000020f0: 723d 2267 7265 6574 696e 6722 3e48 656c  r="greeting">Hel
+00002100: 6c6f 2c20 776f 726c 6421 3c2f 703e 6020  lo, world!</p>` 
+00002110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002120: 2020 2020 2020 7c0a 7c20 4578 616d 706c        |.| Exampl
+00002130: 6520 4f75 7470 7574 207c 2060 3c70 3e7b  e Output | `<p>{
+00002140: 7b20 6772 6565 7469 6e67 207d 7d3c 2f70  { greeting }}</p
+00002150: 3e60 2020 2020 2020 2020 2020 2020 2020  >`              
+00002160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002170: 2020 2020 2020 2020 2020 7c                        |
```

### Comparing `html_to_django-0.0.1/html_to_django/__init__.py` & `html_to_django-0.0.2/html_to_django/__init__.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/html_to_django/converter.py` & `html_to_django-0.0.2/html_to_django/converter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/html_to_django/formatters/__init__.py` & `html_to_django-0.0.2/html_to_django/formatters/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 This package contains modules that define various formatters for modifying a BeautifulSoup object in place.
 
 Each formatter module contains a `format` function that performs a specific modification on the BeautifulSoup object.
 
 The `formatters` list in this package contains all the formatter modules for easy access and usage.
 """
 from . import (for_formatter, if_formatter, var_formatter, block_formatter, static_formatter, attr_formatter,
-               for_wrap_formatter, unwrap_formatter, include_formatter, remove_default_formatter, command_formatter,
-               style_formatter, style_raw_formatter)
+               for_wrap_formatter, unwrap_formatter, remove_formatter, include_formatter, assets_formatter,
+               remove_default_formatter, command_formatter, style_formatter, style_raw_formatter)
 
 
 formatters = [for_formatter, if_formatter, var_formatter, block_formatter, static_formatter, attr_formatter,
-              for_wrap_formatter, unwrap_formatter, include_formatter, remove_default_formatter, command_formatter,
-              style_formatter, style_raw_formatter]
+              for_wrap_formatter, unwrap_formatter, remove_formatter, include_formatter, assets_formatter,
+              remove_default_formatter, command_formatter, style_formatter, style_raw_formatter]
```

### Comparing `html_to_django-0.0.1/html_to_django/formatters/attr_formatter.py` & `html_to_django-0.0.2/html_to_django/formatters/attr_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/html_to_django/formatters/block_formatter.py` & `html_to_django-0.0.2/html_to_django/formatters/block_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/html_to_django/formatters/command_formatter.py` & `html_to_django-0.0.2/html_to_django/formatters/command_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/html_to_django/formatters/for_formatter.py` & `html_to_django-0.0.2/html_to_django/formatters/for_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/html_to_django/formatters/for_wrap_formatter.py` & `html_to_django-0.0.2/html_to_django/formatters/for_wrap_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/html_to_django/formatters/if_formatter.py` & `html_to_django-0.0.2/html_to_django/formatters/if_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/html_to_django/formatters/include_formatter.py` & `html_to_django-0.0.2/html_to_django/formatters/include_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/html_to_django/formatters/remove_default_formatter.py` & `html_to_django-0.0.2/html_to_django/formatters/remove_default_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/html_to_django/formatters/static_formatter.py` & `html_to_django-0.0.2/html_to_django/formatters/static_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/html_to_django/formatters/style_formatter.py` & `html_to_django-0.0.2/html_to_django/formatters/style_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/html_to_django/formatters/style_raw_formatter.py` & `html_to_django-0.0.2/html_to_django/formatters/style_raw_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/html_to_django/formatters/unwrap_formatter.py` & `html_to_django-0.0.2/html_to_django/formatters/unwrap_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/html_to_django/formatters/var_formatter.py` & `html_to_django-0.0.2/html_to_django/formatters/var_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/tests/tests_converter.py` & `html_to_django-0.0.2/tests/tests_converter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/tests/formatters/tests_attr_formatter.py` & `html_to_django-0.0.2/tests/formatters/tests_attr_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/tests/formatters/tests_block_formatter.py` & `html_to_django-0.0.2/tests/formatters/tests_block_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/tests/formatters/tests_command_formatter.py` & `html_to_django-0.0.2/tests/formatters/tests_command_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/tests/formatters/tests_for_formatter.py` & `html_to_django-0.0.2/tests/formatters/tests_for_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/tests/formatters/tests_for_wrap_formatter.py` & `html_to_django-0.0.2/tests/formatters/tests_for_wrap_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/tests/formatters/tests_if_formatter.py` & `html_to_django-0.0.2/tests/formatters/tests_if_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/tests/formatters/tests_include_formatter.py` & `html_to_django-0.0.2/tests/formatters/tests_include_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/tests/formatters/tests_remove_default_formatter.py` & `html_to_django-0.0.2/tests/formatters/tests_remove_default_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/tests/formatters/tests_static_formatter.py` & `html_to_django-0.0.2/tests/formatters/tests_static_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/tests/formatters/tests_style_formatter.py` & `html_to_django-0.0.2/tests/formatters/tests_style_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/tests/formatters/tests_style_raw_formatter.py` & `html_to_django-0.0.2/tests/formatters/tests_style_raw_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/tests/formatters/tests_unwrap_formatter.py` & `html_to_django-0.0.2/tests/formatters/tests_unwrap_formatter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from unittest import TestCase
 from bs4 import BeautifulSoup
 from html_to_django.formatters import unwrap_formatter
 
 
 class UnwrapTests(TestCase):
     def test_basic(self) -> None:
-        soup = BeautifulSoup('<div dj-unwrap="true"><div>Test</div></div>', "html.parser")
+        soup = BeautifulSoup('<div dj-unwrap><div>Test</div></div>', "html.parser")
         unwrap_formatter.format(soup)
         expected_result = "<div>Test</div>"
         self.assertEqual(expected_result, str(soup))
 
     def test_empty(self) -> None:
-        soup = BeautifulSoup('<div dj-unwrap="true"></div>', "html.parser")
+        soup = BeautifulSoup('<div dj-unwrap></div>', "html.parser")
         unwrap_formatter.format(soup)
         expected_result = ""
         self.assertEqual(expected_result, str(soup))
 
     def test_with_unwrap_inside(self) -> None:
-        soup = BeautifulSoup('<div dj-unwrap="true"><div dj-unwrap="true">Inner Test</div></div>', "html.parser")
+        soup = BeautifulSoup('<div dj-unwrap><div dj-unwrap>Inner Test</div></div>', "html.parser")
         unwrap_formatter.format(soup)
         expected_result = "Inner Test"
         self.assertEqual(expected_result, str(soup))
```

### Comparing `html_to_django-0.0.1/tests/formatters/tests_var_formatter.py` & `html_to_django-0.0.2/tests/formatters/tests_var_formatter.py`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/.gitignore` & `html_to_django-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/LICENSE.txt` & `html_to_django-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `html_to_django-0.0.1/README.md` & `html_to_django-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 ![tests workflow](https://github.com/truePhilipp/html_to_django/actions/workflows/tests.yml/badge.svg)
 ![stylecheck workflow](https://github.com/truePhilipp/html_to_django/actions/workflows/stylecheck.yml/badge.svg)
 
 Converts HTML files with special attributes to Django templates.
 
 
 # Installation
-TODO: pip install instructions
+```bash
+pip install html-to-django
+```
 
 
 # Usage
 ```bash
 html_to_django [-h] [-r] path
 ```
 `path` can either be a path to a file or a folder. When a file is passed only the file itself will be converted. When a folder is passed, all files ending in .html will be replaced. This searches through the folder recursivley.
```

### Comparing `html_to_django-0.0.1/pyproject.toml` & `html_to_django-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 dynamic = ["version"]
 authors = [
   { name="Philipp Mayr", email="philipp@mayr.software" },
 ]
 description = "HTML to Django Converter"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE.txt"}
-keywords = ["html", "django"]
+keywords = ["html", "converter", "django", "tool", "web development", "static html"]
 requires-python = ">= 3.12"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: MIT License"
 ]
```

### Comparing `html_to_django-0.0.1/PKG-INFO` & `html_to_django-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: html_to_django
-Version: 0.0.1
+Version: 0.0.2
 Summary: HTML to Django Converter
 Project-URL: Homepage, https://github.com/truePhilipp/html_to_django
 Project-URL: Issues, https://github.com/truePhilipp/html_to_django/issues
 Author-email: Philipp Mayr <philipp@mayr.software>
 License: MIT License
         
         Copyright (c) 2024 Philipp Mayr
@@ -23,15 +23,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE.txt
-Keywords: django,html
+Keywords: converter,django,html,static html,tool,web development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12
 Requires-Dist: beautifulsoup4==4.12.3
 Provides-Extra: dev
@@ -47,15 +47,17 @@
 ![tests workflow](https://github.com/truePhilipp/html_to_django/actions/workflows/tests.yml/badge.svg)
 ![stylecheck workflow](https://github.com/truePhilipp/html_to_django/actions/workflows/stylecheck.yml/badge.svg)
 
 Converts HTML files with special attributes to Django templates.
 
 
 # Installation
-TODO: pip install instructions
+```bash
+pip install html-to-django
+```
 
 
 # Usage
 ```bash
 html_to_django [-h] [-r] path
 ```
 `path` can either be a path to a file or a folder. When a file is passed only the file itself will be converted. When a folder is passed, all files ending in .html will be replaced. This searches through the folder recursivley.
```

